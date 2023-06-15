# Comparing `tmp/motion_python-0.1.64.tar.gz` & `tmp/motion_python-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.64.tar", max compression
+gzip compressed data, was "motion_python-0.1.65.tar", max compression
```

## Comparing `motion_python-0.1.64.tar` & `motion_python-0.1.65.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-14 22:35:09.463752 motion_python-0.1.64/README.md
--rw-r--r--   0        0        0      276 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/cli.py
--rw-r--r--   0        0        0    23922 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/component.py
--rw-r--r--   0        0        0    17508 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/execute.py
--rw-r--r--   0        0        0    12849 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/route.py
--rw-r--r--   0        0        0     5815 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/server/fit_task.py
--rw-r--r--   0        0        0     8853 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-14 22:35:37.176000 motion_python-0.1.64/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.64/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-15 21:58:24.341203 motion_python-0.1.65/README.md
+-rw-r--r--   0        0        0      276 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/cli.py
+-rw-r--r--   0        0        0    23922 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/component.py
+-rw-r--r--   0        0        0    17554 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/execute.py
+-rw-r--r--   0        0        0    12849 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/route.py
+-rw-r--r--   0        0        0     5815 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/server/fit_task.py
+-rw-r--r--   0        0        0     8853 2023-06-15 21:58:24.341203 motion_python-0.1.65/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-15 21:58:45.189559 motion_python-0.1.65/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.65/PKG-INFO
```

### Comparing `motion_python-0.1.64/README.md` & `motion_python-0.1.65/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/motion/cli.py` & `motion_python-0.1.65/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/motion/component.py` & `motion_python-0.1.65/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/motion/execute.py` & `motion_python-0.1.65/motion/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
                         load_state_func=self._load_state_func,
                         queue_identifier=self._get_queue_identifier(rkey, udf_name),
                         channel_identifier=self._get_channel_identifier(rkey, udf_name),
                         redis_host=rp.host,
                         redis_port=rp.port,
                         redis_db=rp.db,
                         redis_password=rp.password,  # type: ignore
+                        running=self.running,
                     )
                     self.worker_tasks[pname].start()
 
             if self.stop_event.is_set():
                 break
 
             # Sleep for a minute
```

### Comparing `motion_python-0.1.64/motion/instance.py` & `motion_python-0.1.65/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.65/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/motion/route.py` & `motion_python-0.1.65/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/motion/server/fit_task.py` & `motion_python-0.1.65/motion/server/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/motion/utils.py` & `motion_python-0.1.65/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.64/pyproject.toml` & `motion_python-0.1.65/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.64"
+version = "0.1.65"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.64/PKG-INFO` & `motion_python-0.1.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.64
+Version: 0.1.65
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

