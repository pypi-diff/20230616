# Comparing `tmp/rqsdk-1.5.0.tar.gz` & `tmp/rqsdk-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rqsdk-1.5.0.tar", last modified: Mon Jun  5 02:40:19 2023, max compression
+gzip compressed data, was "dist/rqsdk-1.5.1.tar", last modified: Fri Jun 16 08:17:43 2023, max compression
```

## Comparing `rqsdk-1.5.0.tar` & `rqsdk-1.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 02:40:19.009682 rqsdk-1.5.0/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2023-06-05 02:40:04.000000 rqsdk-1.5.0/HISTORY.md
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2023-06-05 02:40:04.000000 rqsdk-1.5.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-05 02:40:19.009682 rqsdk-1.5.0/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2023-06-05 02:40:04.000000 rqsdk-1.5.0/README.md
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 02:40:19.011682 rqsdk-1.5.0/rqsdk/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/__main__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2023-06-05 02:40:19.011682 rqsdk-1.5.0/rqsdk/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    12905 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/cmds.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1738 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/const.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/license_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/proxy_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/script_update.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2023-06-05 02:40:04.000000 rqsdk-1.5.0/rqsdk/testing.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-05 02:40:19.008682 rqsdk-1.5.0/rqsdk.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3363 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2023-06-05 02:40:18.000000 rqsdk-1.5.0/rqsdk.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2023-06-05 02:40:19.010682 rqsdk-1.5.0/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3129 2023-06-05 02:40:04.000000 rqsdk-1.5.0/setup.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79815 2023-06-05 02:40:04.000000 rqsdk-1.5.0/versioneer.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-16 08:17:43.561169 rqsdk-1.5.1/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2023-06-16 08:17:37.000000 rqsdk-1.5.1/HISTORY.md
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2023-06-16 08:17:37.000000 rqsdk-1.5.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-16 08:17:43.561169 rqsdk-1.5.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2023-06-16 08:17:37.000000 rqsdk-1.5.1/README.md
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-16 08:17:43.570169 rqsdk-1.5.1/rqsdk/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/__main__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2023-06-16 08:17:43.570169 rqsdk-1.5.1/rqsdk/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    13017 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/cmds.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1738 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/const.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/license_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/proxy_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/script_update.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2023-06-16 08:17:37.000000 rqsdk-1.5.1/rqsdk/testing.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-16 08:17:43.561169 rqsdk-1.5.1/rqsdk.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      760 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3363 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2023-06-16 08:17:43.000000 rqsdk-1.5.1/rqsdk.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2023-06-16 08:17:43.562169 rqsdk-1.5.1/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3129 2023-06-16 08:17:37.000000 rqsdk-1.5.1/setup.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79860 2023-06-16 08:17:37.000000 rqsdk-1.5.1/versioneer.py
```

### Comparing `rqsdk-1.5.0/PKG-INFO` & `rqsdk-1.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.5.0
+Version: 1.5.1
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.5.0/README.md` & `rqsdk-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.0/rqsdk/__init__.py` & `rqsdk-1.5.1/rqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.0/rqsdk/__main__.py` & `rqsdk-1.5.1/rqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.0/rqsdk/cmds.py` & `rqsdk-1.5.1/rqsdk/cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,18 +162,21 @@
     * rqdatac - 金融数据API（默认已安装）
     * rqalpha_plus - 多资产回测引擎
     * rqoptimizer - 股票优化器
     * rqfactor - 因子投研和检验
     * rqpattr - 绩效归因计算
     """
     if product != "":
-        if product not in PRODUCTS:
+        if product == "rqsdk":
+            full_name = product
+        elif product in PRODUCTS:
+            full_name = "rqsdk[{}]".format(product)
+        else:
             click.echo("PRODUCT可选为:{}\n,当前为{}。".format(PRODUCTS, product))
             return
-        key = [product]
     else:
         key = ["rqdatac"]
         try:
             import rqalpha_plus
             key.append("rqalpha_plus")
         except ImportError:
             try:
@@ -187,16 +190,15 @@
             except ImportError:
                 pass
             try:
                 import rqpattr
                 key.append('rqpattr')
             except ImportError:
                 pass
-
-    full_name = "rqsdk[{}]".format(",".join(key))
+        full_name = "rqsdk rqsdk[{}]".format(",".join(key))
     click.echo("开始更新 {} 请稍后...".format(full_name))
     return pip_install(full_name, index_url)
 
 
 @cli.command()
 @click.argument('product', default="", nargs=1)
 @click.option('-i', '--index-url', default="https://pypi.douban.com/simple/", help="指定默认源", hidden=True)
```

### Comparing `rqsdk-1.5.0/rqsdk/const.py` & `rqsdk-1.5.1/rqsdk/const.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.0/rqsdk/license_helper.py` & `rqsdk-1.5.1/rqsdk/license_helper.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.0/rqsdk/script_update.py` & `rqsdk-1.5.1/rqsdk/script_update.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.0/rqsdk/testing.py` & `rqsdk-1.5.1/rqsdk/testing.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.0/rqsdk.egg-info/PKG-INFO` & `rqsdk-1.5.1/rqsdk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.5.0
+Version: 1.5.1
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.5.0/rqsdk.egg-info/requires.txt` & `rqsdk-1.5.1/rqsdk.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-rqdatac>=2.9.44
-pyjwt==1.7.1
-pandas>=0.24.2
+wcwidth
 tabulate
-requests
+rqdatac>=2.9.44
 click>=7.0
+rqdatac_fund==1.0.*,>=1.0.18
 patsy>=0.5.1
+requests
+pyjwt==1.7.1
 statsmodels>=0.12.1
-rqdatac_fund==1.0.*,>=1.0.18
-wcwidth
+pandas>=0.24.2
 
 [:python_version <= "3.6"]
-cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
+cryptography==2.9.2
 
 [:python_version <= "3.7"]
 scipy<=1.7.3
 
 [:python_version == "3.7"]
 numpy>=1.20.0
 
 [:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [:python_version >= "3.8"]
-numpy>=1.23.0
 scipy>=1.8.0
+numpy>=1.23.0
 
 [rqalpha_plus]
-rqdatac>=2.9.44
-rqalpha-mod-fund==0.0.12
-rqalpha-mod-incremental==0.0.8
-rqrisk==1.0.7
-rqalpha-mod-rqfactor==1.0.10
+rqalpha-mod-ricequant-data==2.4.0
 tabulate
-click>=7.0
-rqalpha==5.0.0
+rqdatac>=2.9.44
+rqalpha==5.1.0
 ta-lib>=0.4.20
-hdf5plugin
-rqalpha-mod-ricequant-data==2.4.0
 rqalpha-mod-convertible==1.2.15
-wcwidth
-rqalpha-mod-optimizer2==1.0.8
-pandas>=0.24.2
-pyjwt==1.7.1
-rqalpha-mod-option==1.1.23
+rqalpha-mod-rqfactor==1.0.10
 matplotlib>=3.1.0
-rqalpha-plus==4.2.4
+h5py>=3.0.0
+rqdatac_fund==1.0.*,>=1.0.18
 requests
+pandas>=0.24.2
+rqalpha-mod-optimizer2==1.0.8
+rqalpha-mod-fund==0.0.12
+rqrisk==1.0.7
+rqalpha-mod-incremental==0.0.8
+wcwidth
+rqalpha-mod-option==1.1.23
+click>=7.0
 patsy>=0.5.1
+rqalpha-mod-spot==1.0.9
+pyjwt==1.7.1
 statsmodels>=0.12.1
-rqdatac_fund==1.0.*,>=1.0.18
+rqalpha-plus==4.2.4
+hdf5plugin
 rqfactor==1.3.*,>=1.3.1
-rqalpha-mod-spot==1.0.9
-h5py>=3.0.0
 
 [rqalpha_plus:python_version <= "3.6"]
-python-rapidjson<=1.5
 cryptography==2.9.2
 numpy>=1.19.5
+python-rapidjson<=1.5
 
 [rqalpha_plus:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqalpha_plus:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqalpha_plus:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqalpha_plus:python_version >= "3.8"]
-numpy>=1.23.0
 scipy>=1.8.0
+numpy>=1.23.0
 
 [rqdatac]
-rqdatac>=2.9.44
-pyjwt==1.7.1
-pandas>=0.24.2
+wcwidth
 tabulate
-requests
+rqdatac>=2.9.44
 click>=7.0
+rqdatac_fund==1.0.*,>=1.0.18
 patsy>=0.5.1
+requests
+pyjwt==1.7.1
 statsmodels>=0.12.1
-rqdatac_fund==1.0.*,>=1.0.18
-wcwidth
+pandas>=0.24.2
 
 [rqdatac:python_version <= "3.6"]
-cryptography==2.9.2
 python-rapidjson<=1.5
 numpy>=1.19.5
+cryptography==2.9.2
 
 [rqdatac:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqdatac:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqdatac:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqdatac:python_version >= "3.8"]
-numpy>=1.23.0
 scipy>=1.8.0
+numpy>=1.23.0
 
 [rqfactor]
-rqdatac>=2.9.44
 tabulate
-click>=7.0
+rqdatac>=2.9.44
 ta-lib>=0.4.20
-wcwidth
-pandas>=0.24.2
-pyjwt==1.7.1
+rqdatac_fund==1.0.*,>=1.0.18
 requests
+pandas>=0.24.2
+wcwidth
+click>=7.0
 patsy>=0.5.1
+pyjwt==1.7.1
 statsmodels>=0.12.1
-rqdatac_fund==1.0.*,>=1.0.18
 rqfactor==1.3.*,>=1.3.1
 
 [rqfactor:python_version <= "3.6"]
-python-rapidjson<=1.5
 cryptography==2.9.2
 numpy>=1.19.5
+python-rapidjson<=1.5
 
 [rqfactor:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqfactor:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqfactor:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqfactor:python_version >= "3.8"]
-numpy>=1.23.0
 scipy>=1.8.0
+numpy>=1.23.0
 
 [rqoptimizer]
-rqdatac>=2.9.44
-osqp==0.6.2.post5
+rqoptimizer2==1.2.*,>=1.2.17
 tabulate
-click>=7.0
-rqoptimizer==1.2.*,>=1.2.17
+rqdatac>=2.9.44
+scs==2.1.4
+rqdatac_fund==1.0.*,>=1.0.18
+requests
+pandas>=0.24.2
 ecos==2.0.10
-rqoptimizer2==1.2.*,>=1.2.17
+osqp==0.6.2.post5
 wcwidth
-pandas>=0.24.2
-pyjwt==1.7.1
-requests
+click>=7.0
 patsy>=0.5.1
+pyjwt==1.7.1
 statsmodels>=0.12.1
-rqdatac_fund==1.0.*,>=1.0.18
-scs==2.1.4
+rqoptimizer==1.2.*,>=1.2.17
 
 [rqoptimizer:python_version <= "3.6"]
-python-rapidjson<=1.5
 cryptography==2.9.2
 numpy>=1.19.5
+python-rapidjson<=1.5
 
 [rqoptimizer:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqoptimizer:python_version == "3.6"]
 cvxpy==1.1.18
 
@@ -169,40 +169,40 @@
 [rqoptimizer:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqoptimizer:python_version >= "3.7"]
 cvxpy==1.2.0
 
 [rqoptimizer:python_version >= "3.8"]
-numpy>=1.23.0
 scipy>=1.8.0
+numpy>=1.23.0
 
 [rqpattr]
-rqdatac>=2.9.44
 tabulate
-click>=7.0
-wcwidth
-rqpattr>=0.0.2
-pandas>=0.24.2
-pyjwt==1.7.1
+rqdatac>=2.9.44
+rqdatac_fund==1.0.*,>=1.0.18
 requests
+pandas>=0.24.2
+rqpattr>=0.0.2
+wcwidth
+click>=7.0
 patsy>=0.5.1
+pyjwt==1.7.1
 statsmodels>=0.12.1
-rqdatac_fund==1.0.*,>=1.0.18
 
 [rqpattr:python_version <= "3.6"]
-python-rapidjson<=1.5
 cryptography==2.9.2
 numpy>=1.19.5
+python-rapidjson<=1.5
 
 [rqpattr:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqpattr:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqpattr:python_version > "3.7"]
 pyopenssl>22.0.0
 
 [rqpattr:python_version >= "3.8"]
-numpy>=1.23.0
 scipy>=1.8.0
+numpy>=1.23.0
```

### Comparing `rqsdk-1.5.0/setup.py` & `rqsdk-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "cvxpy==1.1.18 ; python_version == '3.6'",
     "cvxpy==1.2.0 ; python_version >= '3.7'",
     "osqp==0.6.2.post5",
     "rqoptimizer==1.2.*,>=1.2.17",
     "rqoptimizer2==1.2.*,>=1.2.17",
 }
 version_map["rqalpha_plus"] = version_map["rqfactor"] | {
-    "rqalpha==5.0.0",
+    "rqalpha==5.1.0",
     "rqalpha-mod-option==1.1.23",
     "rqalpha-mod-optimizer2==1.0.8",
     "rqalpha-mod-convertible==1.2.15",
     "rqalpha-mod-ricequant-data==2.4.0",
     "rqalpha-mod-rqfactor==1.0.10",
     "rqalpha-mod-spot==1.0.9",
     "rqalpha-mod-fund==0.0.12",
```

### Comparing `rqsdk-1.5.0/versioneer.py` & `rqsdk-1.5.1/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1423,15 +1423,15 @@
             rendered += ".dirty"
 
     tracking_branch = git_tracking_branch()
     # # 如果是dev和master分支或者hotfix分支来的，或者是一个tag，那就用pep440的版本号，否则带上git commit id
     if tracking_branch in ["origin/develop", "origin/master"] or tracking_branch.startswith("origin/hotfix/") or pieces[
         "distance"] == 0:
         return rendered
-
+    rendered += "+{}".format(pieces["short"])
     return rendered
 
 
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
```

