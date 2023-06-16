# Comparing `tmp/arch_github_package-0.0.1.tar.gz` & `tmp/arch_github_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_github_package-0.0.1.tar", last modified: Fri Jun 16 04:55:32 2023, max compression
+gzip compressed data, was "arch_github_package-0.0.2.tar", max compression
```

## Comparing `arch_github_package-0.0.1.tar` & `arch_github_package-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,9 @@
-drwxr-xr-x   0 jin       (1000) jin       (1000)        0 2023-06-16 04:55:32.627082 arch_github_package-0.0.1/
--rw-r--r--   0 jin       (1000) jin       (1000)    11357 2023-06-15 13:00:10.000000 arch_github_package-0.0.1/LICENSE
--rw-r--r--   0 jin       (1000) jin       (1000)     2688 2023-06-16 04:55:32.627082 arch_github_package-0.0.1/PKG-INFO
--rw-r--r--   0 jin       (1000) jin       (1000)     2078 2023-06-16 04:47:01.000000 arch_github_package-0.0.1/README.md
-drwxr-xr-x   0 jin       (1000) jin       (1000)        0 2023-06-16 04:55:32.627082 arch_github_package-0.0.1/arch_github_package/
--rw-r--r--   0 jin       (1000) jin       (1000)        0 2023-06-16 03:36:07.000000 arch_github_package-0.0.1/arch_github_package/__init__.py
--rw-r--r--   0 jin       (1000) jin       (1000)     1452 2023-06-16 03:02:23.000000 arch_github_package-0.0.1/arch_github_package/gh.py
--rw-r--r--   0 jin       (1000) jin       (1000)     3340 2023-06-16 03:38:45.000000 arch_github_package-0.0.1/arch_github_package/main.py
--rw-r--r--   0 jin       (1000) jin       (1000)     3327 2023-06-16 04:40:18.000000 arch_github_package-0.0.1/arch_github_package/pm.py
--rw-r--r--   0 jin       (1000) jin       (1000)     2055 2023-06-16 02:59:54.000000 arch_github_package-0.0.1/arch_github_package/state.py
-drwxr-xr-x   0 jin       (1000) jin       (1000)        0 2023-06-16 04:55:32.627082 arch_github_package-0.0.1/arch_github_package.egg-info/
--rw-r--r--   0 jin       (1000) jin       (1000)     2688 2023-06-16 04:55:32.000000 arch_github_package-0.0.1/arch_github_package.egg-info/PKG-INFO
--rw-r--r--   0 jin       (1000) jin       (1000)      433 2023-06-16 04:55:32.000000 arch_github_package-0.0.1/arch_github_package.egg-info/SOURCES.txt
--rw-r--r--   0 jin       (1000) jin       (1000)        1 2023-06-16 04:55:32.000000 arch_github_package-0.0.1/arch_github_package.egg-info/dependency_links.txt
--rw-r--r--   0 jin       (1000) jin       (1000)       53 2023-06-16 04:55:32.000000 arch_github_package-0.0.1/arch_github_package.egg-info/entry_points.txt
--rw-r--r--   0 jin       (1000) jin       (1000)      740 2023-06-16 04:55:32.000000 arch_github_package-0.0.1/arch_github_package.egg-info/requires.txt
--rw-r--r--   0 jin       (1000) jin       (1000)       20 2023-06-16 04:55:32.000000 arch_github_package-0.0.1/arch_github_package.egg-info/top_level.txt
--rw-r--r--   0 jin       (1000) jin       (1000)     1862 2023-06-16 03:46:09.000000 arch_github_package-0.0.1/pyproject.toml
--rw-r--r--   0 jin       (1000) jin       (1000)       38 2023-06-16 04:55:32.627082 arch_github_package-0.0.1/setup.cfg
+-rw-r--r--   0        0        0    11357 2023-06-15 13:00:10.223792 arch_github_package-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2079 2023-06-16 05:17:40.073206 arch_github_package-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 03:36:07.034151 arch_github_package-0.0.2/arch_github_package/__init__.py
+-rw-r--r--   0        0        0     1452 2023-06-16 03:02:23.248227 arch_github_package-0.0.2/arch_github_package/gh.py
+-rw-r--r--   0        0        0     3340 2023-06-16 03:38:45.508865 arch_github_package-0.0.2/arch_github_package/main.py
+-rw-r--r--   0        0        0     3327 2023-06-16 04:40:18.833283 arch_github_package-0.0.2/arch_github_package/pm.py
+-rw-r--r--   0        0        0     2055 2023-06-16 02:59:54.253016 arch_github_package-0.0.2/arch_github_package/state.py
+-rw-r--r--   0        0        0      953 2023-06-16 05:25:51.295143 arch_github_package-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 arch_github_package-0.0.2/PKG-INFO
```

### Comparing `arch_github_package-0.0.1/LICENSE` & `arch_github_package-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.1/PKG-INFO` & `arch_github_package-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
-Name: arch_github_package
-Version: 0.0.1
-Author-email: Jin Liu <m.liu.jin@gmail.com>
-Project-URL: Homepage, https://github.com/jinliu/arch-github-package
-Project-URL: Bug Tracker, https://github.com/jinliu/arch-github-package/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
+Name: arch-github-package
+Version: 0.0.2
+Summary: Convert GitHub project releases to Archlinux package, with autoupdate.
+Author: Jin Liu
+Author-email: m.liu.jin@gmail.com
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: System
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyGithub (>=1.58.2,<2.0.0)
+Requires-Dist: filetype (>=1.2.0,<2.0.0)
+Requires-Dist: tabulate-expwidth (>=0.9.0.1.3.8,<0.10.0.0.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # arch-github-package
 
-Convert GitHub project releases to Archlinux package, with autoupdate
+Convert GitHub project releases to Archlinux package, with autoupdate.
 
 ## Why
 
 A lot of packages in Archlinux's AUR are just a single PKGBUILD file that downloads the
 latest release from GitHub, and many of them are human-maintained, which means that they
 are not updated as soon as a new release is published.
 
@@ -98,7 +101,8 @@
 So remember to use `agp uninstall` to remove it.
 
 ## Internals
 
 ### Package metadata
 
 Metadata is stored under `~/.local/share/arch-github-package`.
+
```

### Comparing `arch_github_package-0.0.1/README.md` & `arch_github_package-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # arch-github-package
 
-Convert GitHub project releases to Archlinux package, with autoupdate
+Convert GitHub project releases to Archlinux package, with autoupdate.
 
 ## Why
 
 A lot of packages in Archlinux's AUR are just a single PKGBUILD file that downloads the
 latest release from GitHub, and many of them are human-maintained, which means that they
 are not updated as soon as a new release is published.
```

### Comparing `arch_github_package-0.0.1/arch_github_package/gh.py` & `arch_github_package-0.0.2/arch_github_package/gh.py`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.1/arch_github_package/main.py` & `arch_github_package-0.0.2/arch_github_package/main.py`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.1/arch_github_package/pm.py` & `arch_github_package-0.0.2/arch_github_package/pm.py`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.1/arch_github_package/state.py` & `arch_github_package-0.0.2/arch_github_package/state.py`

 * *Files identical despite different names*

