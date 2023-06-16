# Comparing `tmp/pyroscope-io-0.8.3.tar.gz` & `tmp/pyroscope-io-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscope-io-0.8.3.tar", last modified: Fri May 19 14:24:16 2023, max compression
+gzip compressed data, was "pyroscope-io-0.8.4.tar", last modified: Thu Jun 15 14:36:00 2023, max compression
```

## Comparing `pyroscope-io-0.8.3.tar` & `pyroscope-io-0.8.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/.cargo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/.cargo/config
--rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/cbindgen.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/include/pyroscope_ffi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/pyroscope/
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/pyroscope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/pyroscope_io/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/pyroscope_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 14:24:16.728547 pyroscope-io-0.8.3/pyroscope_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 14:24:16.000000 pyroscope-io-0.8.3/pyroscope_io.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-19 14:24:16.732547 pyroscope-io-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-19 14:24:01.000000 pyroscope-io-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/.cargo/config
+-rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/cbindgen.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/include/pyroscope_ffi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/pyroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/pyroscope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/pyroscope_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/pyroscope_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/pyroscope_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-15 14:36:00.469034 pyroscope-io-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/setup.py
```

### Comparing `pyroscope-io-0.8.3/LICENSE` & `pyroscope-io-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.3/PKG-INFO` & `pyroscope-io-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.3
+Version: 0.8.4
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
```

### Comparing `pyroscope-io-0.8.3/README.md` & `pyroscope-io-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.3/lib/Cargo.lock` & `pyroscope-io-0.8.4/lib/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.3/lib/cbindgen.toml` & `pyroscope-io-0.8.4/lib/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.3/lib/include/pyroscope_ffi.h` & `pyroscope-io-0.8.4/lib/include/pyroscope_ffi.h`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.3/lib/src/lib.rs` & `pyroscope-io-0.8.4/lib/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,24 @@
     // application_name
     let application_name = unsafe { CStr::from_ptr(application_name) }
         .to_str()
         .unwrap()
         .to_string();
 
     // server_address
-    let server_address = unsafe { CStr::from_ptr(server_address) }
+    let mut server_address = unsafe { CStr::from_ptr(server_address) }
         .to_str()
         .unwrap()
         .to_string();
 
+    let adhoc_server_address = std::env::var("PYROSCOPE_ADHOC_SERVER_ADDRESS");
+    if let Ok(adhoc_server_address) = adhoc_server_address {
+        server_address = adhoc_server_address
+    }
+
     let auth_token = unsafe { CStr::from_ptr(auth_token) }
         .to_str()
         .unwrap()
         .to_string();
 
     let basic_auth_username = unsafe { CStr::from_ptr(basic_auth_username) }
         .to_str()
```

### Comparing `pyroscope-io-0.8.3/pyroscope/__init__.py` & `pyroscope-io-0.8.4/pyroscope/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.3/pyroscope_io.egg-info/PKG-INFO` & `pyroscope-io-0.8.4/pyroscope_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.3
+Version: 0.8.4
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
```

### Comparing `pyroscope-io-0.8.3/setup.cfg` & `pyroscope-io-0.8.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroscope-io
-version = 0.8.3
+version = 0.8.4
 description = Pyroscope Python integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pyroscope.io
 maintainer = Abid Omar
 maintainer_email = contact@pyroscope.io
 license = Apache 2.0
```

### Comparing `pyroscope-io-0.8.3/setup.py` & `pyroscope-io-0.8.4/setup.py`

 * *Files identical despite different names*

