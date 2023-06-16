# Comparing `tmp/acore_db_ssh_tunnel-0.1.1.tar.gz` & `tmp/acore_db_ssh_tunnel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_db_ssh_tunnel-0.1.1.tar", last modified: Fri Jun 16 04:39:13 2023, max compression
+gzip compressed data, was "acore_db_ssh_tunnel-0.1.2.tar", last modified: Fri Jun 16 15:41:39 2023, max compression
```

## Comparing `acore_db_ssh_tunnel-0.1.1.tar` & `acore_db_ssh_tunnel-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 04:39:13.214134 acore_db_ssh_tunnel-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-16 04:39:13.213968 acore_db_ssh_tunnel-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4527 2023-06-16 04:35:58.000000 acore_db_ssh_tunnel-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 04:39:13.212267 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/
--rw-r--r--   0 sanhehu    (501) staff       (20)      436 2023-06-16 04:36:53.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1938 2023-06-16 04:24:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/acore_ssh_tunnel.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-16 04:25:38.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 04:39:13.212984 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      354 2023-06-16 03:06:37.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/mysql_engine.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7304 2023-06-16 04:21:21.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/ssh_tunnel.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 04:39:13.213353 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 04:39:13.213628 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 04:39:13.212867 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-16 04:39:13.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      844 2023-06-16 04:39:13.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 04:39:13.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-06-16 04:39:13.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-16 04:39:13.000000 acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      797 2023-06-16 04:38:08.000000 acore_db_ssh_tunnel-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       77 2023-06-16 04:31:11.000000 acore_db_ssh_tunnel-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 04:39:13.214184 acore_db_ssh_tunnel-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 04:39:13.213761 acore_db_ssh_tunnel-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      414 2023-06-16 04:26:05.000000 acore_db_ssh_tunnel-0.1.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.387557 acore_db_ssh_tunnel-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-16 15:41:39.387421 acore_db_ssh_tunnel-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4527 2023-06-16 04:35:58.000000 acore_db_ssh_tunnel-0.1.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.385612 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      436 2023-06-16 04:36:53.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 15:39:32.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1938 2023-06-16 04:24:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/acore_ssh_tunnel.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-16 04:25:38.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386424 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      354 2023-06-16 03:06:37.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/mysql_engine.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7930 2023-06-16 15:39:03.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/ssh_tunnel.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386716 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386986 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.386269 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5692 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      844 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      186 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-16 15:41:39.000000 acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1113 2023-06-16 15:40:46.000000 acore_db_ssh_tunnel-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       77 2023-06-16 04:31:11.000000 acore_db_ssh_tunnel-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 15:41:39.387592 acore_db_ssh_tunnel-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-16 02:38:39.000000 acore_db_ssh_tunnel-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 15:41:39.387128 acore_db_ssh_tunnel-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      414 2023-06-16 04:26:05.000000 acore_db_ssh_tunnel-0.1.2/tests/test_api.py
```

### Comparing `acore_db_ssh_tunnel-0.1.1/AUTHORS.rst` & `acore_db_ssh_tunnel-0.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/LICENSE.txt` & `acore_db_ssh_tunnel-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/PKG-INFO` & `acore_db_ssh_tunnel-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_db_ssh_tunnel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create Database SSH Tunnel for Azerothcore World of Warcraft MySQL Database
 Home-page: https://github.com/MacHu-GWU/acore_db_ssh_tunnel-project
-Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_db_ssh_tunnel-0.1.1/README.rst` & `acore_db_ssh_tunnel-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/acore_ssh_tunnel.py` & `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/acore_ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/paths.py` & `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/paths.py`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/ssh_tunnel.py` & `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/ssh_tunnel.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 127.0.0.1 作为数据库的 host, 这样所有的流量都会被自动转发到跳板机, 然后再转发到数据库.
 
 .. note::
 
     本模块不考虑用一个 pem 秘钥开启多个 SSH Tunnel 连接到不同跳板机的情况. 我们假设同一时间
     一个秘钥只能创建一个 SSH Tunnel.
 """
-
+import sys
 import typing as T
 import subprocess
 from pathlib import Path
 
 import sqlalchemy as sa
 
 
@@ -64,21 +64,36 @@
         "-f",
         "-N",
         "-L",
         f"{db_port}:{db_host}:{db_port}",
         f"{jump_host_username}@{jump_host_public_ip}",
         "-v",
     ]
+    ssh_cmd = " ".join(args)
     if verbose:
-        ssh_cmd = " ".join(args)
         print_func(f"Open ssh tunnel by running the following command:")
-        print_func("")
         print_func(f"  {ssh_cmd}")
-    subprocess.run(args)
-    return args
+
+    res = subprocess.run(args)
+    if res.returncode == 0:
+        print_func("SSH Tunnel created successfully.")
+        return
+
+    # something wrong, let's check if you have to do it in terminal
+    res = subprocess.run(args, capture_output=True)
+    error_message = res.stderr.decode("utf-8")
+    error_keyword = "can't open /dev/tty: Device not configured"
+    if error_keyword in error_message:
+        print_func(
+            "You may need to run this script in terminal, NOT in Python IDE. "
+            "Enter the following command in terminal to create SSH tunnel: "
+        )
+        print_func(f"  {ssh_cmd}")
+    else:
+        print_func("Failed to create SSH Tunnel.")
 
 
 def list_ssh_tunnel_pid(path_pem_file) -> T.List[str]:
     """
     List the PID of SSH Tunnel processes.
 
     找出在本地机器上已有的 SSH Tunnel 的 PID (process id, 即进程 ID). 其原理是用
```

### Comparing `acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py` & `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/PKG-INFO` & `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-db-ssh-tunnel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create Database SSH Tunnel for Azerothcore World of Warcraft MySQL Database
 Home-page: https://github.com/MacHu-GWU/acore_db_ssh_tunnel-project
-Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_db_ssh_tunnel/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_db_ssh_tunnel-0.1.1/acore_db_ssh_tunnel.egg-info/SOURCES.txt` & `acore_db_ssh_tunnel-0.1.2/acore_db_ssh_tunnel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/requirements-doc.txt` & `acore_db_ssh_tunnel-0.1.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_db_ssh_tunnel-0.1.1/setup.py` & `acore_db_ssh_tunnel-0.1.2/setup.py`

 * *Files identical despite different names*

