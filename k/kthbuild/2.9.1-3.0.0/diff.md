# Comparing `tmp/kthbuild-2.9.1.tar.gz` & `tmp/kthbuild-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthbuild-2.9.1.tar", last modified: Fri May 26 14:15:03 2023, max compression
+gzip compressed data, was "kthbuild-3.0.0.tar", last modified: Fri Jun 16 10:40:42 2023, max compression
```

## Comparing `kthbuild-2.9.1.tar` & `kthbuild-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:15:03.422568 kthbuild-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-26 14:14:32.000000 kthbuild-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-26 14:15:03.422568 kthbuild-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-26 14:14:32.000000 kthbuild-2.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:15:03.422568 kthbuild-2.9.1/kthbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-26 14:15:03.000000 kthbuild-2.9.1/kthbuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    44530 2023-05-26 14:14:32.000000 kthbuild-2.9.1/kthbuild.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 14:15:03.422568 kthbuild-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4872 2023-05-26 14:14:32.000000 kthbuild-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:40:42.519691 kthbuild-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-16 10:40:17.000000 kthbuild-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-06-16 10:40:42.519691 kthbuild-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-16 10:40:17.000000 kthbuild-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 10:40:42.519691 kthbuild-3.0.0/kthbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-16 10:40:42.000000 kthbuild-3.0.0/kthbuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    45558 2023-06-16 10:40:17.000000 kthbuild-3.0.0/kthbuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 10:40:42.519691 kthbuild-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-06-16 10:40:17.000000 kthbuild-3.0.0/setup.py
```

### Comparing `kthbuild-2.9.1/LICENSE` & `kthbuild-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthbuild-2.9.1/PKG-INFO` & `kthbuild-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 2.9.1
+Version: 3.0.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-2.9.1/kthbuild.egg-info/PKG-INFO` & `kthbuild-3.0.0/kthbuild.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthbuild
-Version: 2.9.1
+Version: 3.0.0
 Summary: Knuth node build tools
 Home-page: https://github.com/k-nuth/kthbuild
 Author: Fernando Pelliccioni
 Author-email: fpelliccioni@gmail.com
 License: MIT
 Keywords: knuth kth crypto bitcoin btc bch cash build tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kthbuild-2.9.1/kthbuild.py` & `kthbuild-3.0.0/kthbuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -479,15 +479,16 @@
     # While redundant, this moves upload remote to position 0.
     # remotes = [get_conan_upload_for_remote(org_name),
     #           'https://knuth.jfrog.io/artifactory/api/conan/knuth',
     #           'https://taocpp.jfrog.io/artifactory/api/conan/tao',]
 
     remotes = ['https://center.conan.io',
                get_conan_upload_for_remote(org_name),
-               'https://taocpp.jfrog.io/artifactory/api/conan/tao']
+            #    'https://taocpp.jfrog.io/artifactory/api/conan/tao'
+               ]
 
     # # Add bincrafters repository for other users, e.g. if the package would
     # # require other packages from the bincrafters repo.
     # bincrafters_user = "bincrafters"
     # if username != bincrafters_user:
     #     remotes.append(get_conan_upload(bincrafters_user))
     return remotes
@@ -953,64 +954,80 @@
         if self.info.options.get_safe("march_strategy") is not None:
             self.info.options.march_strategy = "ANY"
 
     def _cmake_database(self, tc):
         if self.options.get_safe("db") is None:
             return
 
-        if self.options.db == "legacy":
+        if self.options.db == "dynamic":
+            tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(False)
+            tc.variables["DB_SPENDS"] = option_on_off(False)
+            tc.variables["DB_HISTORY"] = option_on_off(False)
+            tc.variables["DB_STEALTH"] = option_on_off(False)
+            tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(False)
+            tc.variables["DB_LEGACY"] = option_on_off(False)
+            tc.variables["DB_NEW"] = option_on_off(False)
+            tc.variables["DB_NEW_BLOCKS"] = option_on_off(False)
+            tc.variables["DB_NEW_FULL"] = option_on_off(False)
+            tc.variables["DB_DYNAMIC"] = option_on_off(True)
+        elif self.options.db == "legacy":
             tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(False)
             tc.variables["DB_SPENDS"] = option_on_off(False)
             tc.variables["DB_HISTORY"] = option_on_off(False)
             tc.variables["DB_STEALTH"] = option_on_off(False)
             tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(True)
             tc.variables["DB_LEGACY"] = option_on_off(True)
             tc.variables["DB_NEW"] = option_on_off(False)
             tc.variables["DB_NEW_BLOCKS"] = option_on_off(False)
             tc.variables["DB_NEW_FULL"] = option_on_off(False)
+            tc.variables["DB_DYNAMIC"] = option_on_off(False)
         elif self.options.db == "legacy_full":
             tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(True)
             tc.variables["DB_SPENDS"] = option_on_off(True)
             tc.variables["DB_HISTORY"] = option_on_off(True)
             tc.variables["DB_STEALTH"] = option_on_off(True)
             tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(True)
             tc.variables["DB_LEGACY"] = option_on_off(True)
             tc.variables["DB_NEW"] = option_on_off(False)
             tc.variables["DB_NEW_BLOCKS"] = option_on_off(False)
             tc.variables["DB_NEW_FULL"] = option_on_off(False)
+            tc.variables["DB_DYNAMIC"] = option_on_off(False)
         elif self.options.db == "pruned":
             tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(False)
             tc.variables["DB_SPENDS"] = option_on_off(False)
             tc.variables["DB_HISTORY"] = option_on_off(False)
             tc.variables["DB_STEALTH"] = option_on_off(False)
             tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(False)
             tc.variables["DB_LEGACY"] = option_on_off(False)
             tc.variables["DB_NEW"] = option_on_off(True)
             tc.variables["DB_NEW_BLOCKS"] = option_on_off(False)
             tc.variables["DB_NEW_FULL"] = option_on_off(False)
+            tc.variables["DB_DYNAMIC"] = option_on_off(False)
         elif self.options.db == "default":
             tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(False)
             tc.variables["DB_SPENDS"] = option_on_off(False)
             tc.variables["DB_HISTORY"] = option_on_off(False)
             tc.variables["DB_STEALTH"] = option_on_off(False)
             tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(False)
             tc.variables["DB_LEGACY"] = option_on_off(False)
             tc.variables["DB_NEW"] = option_on_off(True)
             tc.variables["DB_NEW_BLOCKS"] = option_on_off(True)
             tc.variables["DB_NEW_FULL"] = option_on_off(False)
+            tc.variables["DB_DYNAMIC"] = option_on_off(False)
         elif self.options.db == "full":
             tc.variables["DB_TRANSACTION_UNCONFIRMED"] = option_on_off(False)
             tc.variables["DB_SPENDS"] = option_on_off(False)
             tc.variables["DB_HISTORY"] = option_on_off(False)
             tc.variables["DB_STEALTH"] = option_on_off(False)
             tc.variables["DB_UNSPENT_LEGACY"] = option_on_off(False)
             tc.variables["DB_LEGACY"] = option_on_off(False)
             tc.variables["DB_NEW"] = option_on_off(True)
             tc.variables["DB_NEW_BLOCKS"] = option_on_off(False)
             tc.variables["DB_NEW_FULL"] = option_on_off(True)
+            tc.variables["DB_DYNAMIC"] = option_on_off(False)
 
     def cmake_toolchain_basis(self, pure_c=False):
         tc = CMakeToolchain(self)
         tc.variables["USE_CONAN"] = option_on_off(True)
         tc.variables["NO_CONAN_AT_ALL"] = option_on_off(False)
         # cmake.verbose = self.options.verbose
         tc.variables["ENABLE_SHARED"] = option_on_off(self.is_shared)
```

### Comparing `kthbuild-2.9.1/setup.py` & `kthbuild-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import subprocess
 import os
 import platform
 
 __title__ = "kthbuild"
 __summary__ = "Knuth node build tools"
 __uri__ = "https://github.com/k-nuth/kthbuild"
-__version__ = "2.9.1"
+__version__ = "3.0.0"
 __author__ = "Fernando Pelliccioni"
 __email__ = "fpelliccioni@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2019-2023 Knuth Project"
 
 
 install_requires = [
@@ -42,15 +42,15 @@
     """Override Install
     """
     def run(self):
         install.run(self)
         if not running_in_cpt_context():
             self.__setup_conan_remote("kth",     'https://packages.kth.cash/api/')
             # self.__setup_conan_remote("kthbuild_tao_temp_",    'https://taocpp.jfrog.io/artifactory/api/conan/tao')
-            self.__setup_conan_remote("tao",                    'https://taocpp.jfrog.io/artifactory/api/conan/tao')
+            # self.__setup_conan_remote("tao",                    'https://taocpp.jfrog.io/artifactory/api/conan/tao')
 
     def __setup_conan_remote(self, remote_alias, remote_url):
         try:
             params = ["conan", "remote", "add", remote_alias, remote_url]
             res = subprocess.Popen(params, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             output, _ = res.communicate()
             if output:
```

