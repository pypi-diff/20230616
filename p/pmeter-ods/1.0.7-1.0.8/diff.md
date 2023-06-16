# Comparing `tmp/pmeter_ods-1.0.7.tar.gz` & `tmp/pmeter_ods-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmeter_ods-1.0.7.tar", last modified: Tue Sep 20 20:48:13 2022, max compression
+gzip compressed data, was "dist/pmeter_ods-1.0.8.tar", last modified: Fri Jun 16 16:12:10 2023, max compression
```

## Comparing `pmeter_ods-1.0.7.tar` & `pmeter_ods-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7368 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)   380409 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.14.05 AM.png
--rw-r--r--   0 runner    (1001) docker     (121)   237650 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.14.13 AM.png
--rw-r--r--   0 runner    (1001) docker     (121)   377171 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.15.09 AM.png
--rw-r--r--   0 runner    (1001) docker     (121)   569631 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.15.54 AM.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/pmeter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/pmeter/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/pmeter/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5789 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/pmeter/helpers/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9301 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/pmeter/pmeter_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter_ods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter_ods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter_ods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter_ods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter_ods.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter_ods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/pmeter_ods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-20 20:48:13.000000 pmeter_ods-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-20 20:47:48.000000 pmeter_ods-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   380409 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.14.05 AM.png
+-rw-r--r--   0 runner    (1001) docker     (123)   237650 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.14.13 AM.png
+-rw-r--r--   0 runner    (1001) docker     (123)   377171 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.15.09 AM.png
+-rw-r--r--   0 runner    (1001) docker     (123)   569631 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.15.54 AM.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/pmeter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/pmeter/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/pmeter/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/pmeter/helpers/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/pmeter/pmeter_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter_ods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter_ods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter_ods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter_ods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter_ods.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter_ods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/pmeter_ods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:12:10.000000 pmeter_ods-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 16:11:56.000000 pmeter_ods-1.0.8/setup.py
```

### Comparing `pmeter_ods-1.0.7/PKG-INFO` & `pmeter_ods-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmeter_ods
-Version: 1.0.7
+Version: 1.0.8
 Summary: A CLI tool that helps capture metrics from the Operating System
 Home-page: https://github.com/didclab/pmeter
 Author: OneDataShare
 Author-email: onedatashare@gmail.com
 License: UNKNOWN
 Description: # pmeter
         A python tool that measures the tcp and udp network metrics
```

### Comparing `pmeter_ods-1.0.7/README.md` & `pmeter_ods-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.14.05 AM.png` & `pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.14.05 AM.png`

 * *Files identical despite different names*

### Comparing `pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.14.13 AM.png` & `pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.14.13 AM.png`

 * *Files identical despite different names*

### Comparing `pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.15.09 AM.png` & `pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.15.09 AM.png`

 * *Files identical despite different names*

### Comparing `pmeter_ods-1.0.7/docs/images/Screenshot 2022-03-28 at 11.15.54 AM.png` & `pmeter_ods-1.0.8/docs/images/Screenshot 2022-03-28 at 11.15.54 AM.png`

 * *Files identical despite different names*

### Comparing `pmeter_ods-1.0.7/pmeter/helpers/constants.py` & `pmeter_ods-1.0.8/pmeter/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `pmeter_ods-1.0.7/pmeter/helpers/file_writer.py` & `pmeter_ods-1.0.8/pmeter/helpers/file_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,25 +117,22 @@
         self.nic_mtu = interface_stats[3]
         self.nic_speed = interface_stats[2]
 
     def get_system_interfaces(self):
         nic_counter_dic = psutil.net_io_counters(pernic=True, nowrap=True)
         return nic_counter_dic.keys()
 
-    def to_file(self, folder_path=Path.home(), folder_name=".pmeter", file_name="pmeter_measure.txt"):
-        if folder_path is None or len(folder_path) < 2:
-            folder_path = Path.home()
-        if not folder_path:
-            full_path = os.path.join(Path.home(), folder_name)
-        else:
-            full_path = os.path.join(folder_path, folder_name)
-        if not os.path.exists(full_path):
-            os.makedirs(full_path)
-            print('Will be dumping data into the folder path ', folder_path)
-        full_path = os.path.join(full_path, file_name)
+    def to_file(self, folder_path, folder_name=".pmeter", file_name="pmeter_measure.txt"):
+        if folder_path is None:
+            folder_path = str(Path.home() / 'config' / '.pmeter')
+
+        if not os.path.exists(folder_path):
+            os.makedirs(folder_path)
+
+        full_path = os.path.join(folder_path, file_name)
         j = json.dumps(self.__dict__)
         with open(full_path, "a+") as f:
             f.write(j + "\n")
 
     def do_deltas(self, old_metric):
         self.bytes_sent_delta = self.bytes_sent - old_metric.bytes_sent
         self.bytes_recv_delta = self.bytes_recv - old_metric.bytes_recv
```

### Comparing `pmeter_ods-1.0.7/pmeter/pmeter_cli.py` & `pmeter_ods-1.0.8/pmeter/pmeter_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
   --version                Show version
   -N --measure_network     Set if we monitor only the network interface [default: True]
   -K --measure_kernel      Set if we monitor only the kernel [default: True]
   -U --measure_udp         Set UDP monitoring only [default: True]
   -T --measure_tcp         Set TCP monitoring only [default: True]
   -S --enable_std_out      Disable printing the results to standard output [default: False]
   --file_name=FILENAME     Set the file name used to measure [default: pmeter_measure.txt]
-  --folder_path=FOLDERPATH Set the path to store the measurement files in the default is the users home directory under ~/.pmeter/
-  --folder_name=FOLDERNAME Set the folder name for pmeter to dump data into [default: .pmeter]
+  --folder_path=FOLDERPATH Set the path to store the measurement files in the default is the users home directory under
+  --folder_name=FOLDERNAME Set the folder name for pmeter to dump data into
   --interval=INTERVAL      Set the time to run the measurement in the format HH:MM:SS [default: 00:00:01]
   --measure=MEASUREMENTS   The max number of times to measure your system. Set this value to 0 to ignore this and use only the length [default: 1]
   --length=LENGTH          The amount of time to run for: 5w, 4d 3h, 2m, 1s are some examples of 5 weeks, 4 days, 3 hours, 2 min, 1 sec. Set this value to '-1s' to ignore this field and use only measurement [default: 10s]
   --user=USER              This will override the user we try to pick up from the environment variable(ODS_USER). If no user is passed then we will not submit the data generated to the ODS backend [default: ]
 
 """
```

### Comparing `pmeter_ods-1.0.7/pmeter_ods.egg-info/PKG-INFO` & `pmeter_ods-1.0.8/pmeter_ods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmeter-ods
-Version: 1.0.7
+Version: 1.0.8
 Summary: A CLI tool that helps capture metrics from the Operating System
 Home-page: https://github.com/didclab/pmeter
 Author: OneDataShare
 Author-email: onedatashare@gmail.com
 License: UNKNOWN
 Description: # pmeter
         A python tool that measures the tcp and udp network metrics
```

### Comparing `pmeter_ods-1.0.7/pmeter_ods.egg-info/SOURCES.txt` & `pmeter_ods-1.0.8/pmeter_ods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmeter_ods-1.0.7/setup.py` & `pmeter_ods-1.0.8/setup.py`

 * *Files identical despite different names*

