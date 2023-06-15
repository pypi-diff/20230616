# Comparing `tmp/labbench-0.25.0.tar.gz` & `tmp/labbench-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labbench-0.25.0.tar", last modified: Thu Jun  8 18:04:23 2023, max compression
+gzip compressed data, was "labbench-0.26.0.tar", last modified: Thu Jun 15 23:02:28 2023, max compression
```

## Comparing `labbench-0.25.0.tar` & `labbench-0.26.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0        0 2023-06-06 17:19:56.324416 labbench-0.25.0/cli/__init__.py
--rw-r--r--   0        0        0     9144 2023-06-06 17:19:56.324416 labbench-0.25.0/cli/__main__.py
--rw-r--r--   0        0        0     2946 2023-06-06 17:19:56.388415 labbench-0.25.0/labbench/__init__.py
--rw-r--r--   0        0        0     1630 2023-06-06 17:19:56.392414 labbench-0.25.0/labbench/__init__.pyi
--rw-r--r--   0        0        0    46636 2023-06-07 17:02:38.655815 labbench-0.25.0/labbench/_backends.py
--rw-r--r--   0        0        0     5644 2023-06-06 17:19:56.396414 labbench-0.25.0/labbench/_backends.pyi
--rw-r--r--   0        0        0    75388 2023-06-06 17:19:56.400415 labbench-0.25.0/labbench/_data.py
--rw-r--r--   0        0        0     6201 2023-06-06 17:19:56.404415 labbench-0.25.0/labbench/_data.pyi
--rw-r--r--   0        0        0    16241 2023-06-07 20:49:25.251548 labbench-0.25.0/labbench/_device.py
--rw-r--r--   0        0        0     1056 2023-06-06 17:19:56.408414 labbench-0.25.0/labbench/_device.pyi
--rw-r--r--   0        0        0    12576 2023-06-06 17:19:56.408414 labbench-0.25.0/labbench/_host.py
--rw-r--r--   0        0        0     1765 2023-06-06 17:19:56.412414 labbench-0.25.0/labbench/_host.pyi
--rw-r--r--   0        0        0    55225 2023-06-06 17:19:56.416415 labbench-0.25.0/labbench/_rack.py
--rw-r--r--   0        0        0     5419 2023-06-06 17:19:56.420417 labbench-0.25.0/labbench/_rack.pyi
--rw-r--r--   0        0        0    11878 2023-06-06 17:19:56.420417 labbench-0.25.0/labbench/_serialize.py
--rw-r--r--   0        0        0      725 2023-06-06 17:19:56.424414 labbench-0.25.0/labbench/_serialize.pyi
--rw-r--r--   0        0        0    62858 2023-06-07 20:49:14.039044 labbench-0.25.0/labbench/_traits.py
--rw-r--r--   0        0        0    14105 2023-06-06 17:19:56.432415 labbench-0.25.0/labbench/_traits.pyi
--rw-r--r--   0        0        0       60 2023-06-06 17:19:56.432415 labbench-0.25.0/labbench/_version.py
--rw-r--r--   0        0        0        0 2023-06-06 17:19:56.432415 labbench-0.25.0/labbench/_version.pyi
--rw-r--r--   0        0        0     2569 2023-06-06 17:19:56.436416 labbench-0.25.0/labbench/datareturn.py
--rw-r--r--   0        0        0     4144 2023-06-06 17:19:56.436416 labbench-0.25.0/labbench/datareturn.pyi
--rw-r--r--   0        0        0     7451 2023-06-06 17:19:56.440414 labbench-0.25.0/labbench/notebooks.py
--rw-r--r--   0        0        0      784 2023-06-06 17:19:56.440414 labbench-0.25.0/labbench/notebooks.pyi
--rw-r--r--   0        0        0     2568 2023-06-06 17:19:56.444414 labbench-0.25.0/labbench/property.py
--rw-r--r--   0        0        0     4001 2023-06-06 17:19:56.444414 labbench-0.25.0/labbench/property.pyi
--rw-r--r--   0        0        0        0 2023-06-06 17:19:56.444414 labbench-0.25.0/labbench/py.typed
--rw-r--r--   0        0        0    51459 2023-06-06 17:19:56.448415 labbench-0.25.0/labbench/util.py
--rw-r--r--   0        0        0     3285 2023-06-06 17:19:56.452415 labbench-0.25.0/labbench/util.pyi
--rw-r--r--   0        0        0     2600 2023-06-06 17:19:56.452415 labbench-0.25.0/labbench/value.py
--rw-r--r--   0        0        0     4447 2023-06-06 17:19:56.456416 labbench-0.25.0/labbench/value.pyi
--rw-r--r--   0        0        0     2858 2023-06-06 17:19:56.320416 labbench-0.25.0/LICENSE.md
--rw-r--r--   0        0        0     2481 2023-06-08 18:03:54.340433 labbench-0.25.0/pyproject.toml
--rw-r--r--   0        0        0    11272 2023-06-06 17:19:56.320416 labbench-0.25.0/README.md
--rw-r--r--   0        0        0     2119 2023-06-06 17:19:56.464416 labbench-0.25.0/tests/all.py
--rw-r--r--   0        0        0     1880 2023-06-06 17:19:56.468415 labbench-0.25.0/tests/emulate.py
--rw-r--r--   0        0        0     3332 2023-06-06 17:19:56.468415 labbench-0.25.0/tests/module_as_testbed.py
--rw-r--r--   0        0        0       57 2023-06-06 17:19:56.472415 labbench-0.25.0/tests/profile_imports.py
--rw-r--r--   0        0        0     4719 2023-06-06 17:19:56.472415 labbench-0.25.0/tests/test_data_logging.py
--rw-r--r--   0        0        0     2287 2023-06-06 17:19:56.476415 labbench-0.25.0/tests/test_doc.py
--rw-r--r--   0        0        0     2211 2023-06-06 17:19:56.480414 labbench-0.25.0/tests/test_email.py
--rw-r--r--   0        0        0     2211 2023-06-06 17:19:56.480414 labbench-0.25.0/tests/test_notification.py
--rw-r--r--   0        0        0    10850 2023-06-06 17:19:56.484414 labbench-0.25.0/tests/test_property.py
--rw-r--r--   0        0        0     8889 2023-06-06 17:19:56.484414 labbench-0.25.0/tests/test_rack.py
--rw-r--r--   0        0        0    13320 2023-06-06 17:19:56.488414 labbench-0.25.0/tests/test_sequencing.py
--rw-r--r--   0        0        0     4192 2023-06-06 17:19:56.492414 labbench-0.25.0/tests/test_shell.py
--rw-r--r--   0        0        0     7727 2023-06-06 17:19:56.492414 labbench-0.25.0/tests/test_value.py
--rw-r--r--   0        0        0    27290 2023-02-06 21:28:33.062776 labbench-0.25.0/tests/testnb.ipynb
--rw-r--r--   0        0        0    12103 1970-01-01 00:00:00.000000 labbench-0.25.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 17:19:56.324416 labbench-0.26.0/cli/__init__.py
+-rw-r--r--   0        0        0     9144 2023-06-06 17:19:56.324416 labbench-0.26.0/cli/__main__.py
+-rw-r--r--   0        0        0     2946 2023-06-06 17:19:56.388415 labbench-0.26.0/labbench/__init__.py
+-rw-r--r--   0        0        0     1630 2023-06-06 17:19:56.392414 labbench-0.26.0/labbench/__init__.pyi
+-rw-r--r--   0        0        0    46638 2023-06-15 23:00:26.498645 labbench-0.26.0/labbench/_backends.py
+-rw-r--r--   0        0        0     5644 2023-06-06 17:19:56.396414 labbench-0.26.0/labbench/_backends.pyi
+-rw-r--r--   0        0        0    75388 2023-06-06 17:19:56.400415 labbench-0.26.0/labbench/_data.py
+-rw-r--r--   0        0        0     6201 2023-06-06 17:19:56.404415 labbench-0.26.0/labbench/_data.pyi
+-rw-r--r--   0        0        0    16241 2023-06-07 20:49:25.251548 labbench-0.26.0/labbench/_device.py
+-rw-r--r--   0        0        0     1056 2023-06-06 17:19:56.408414 labbench-0.26.0/labbench/_device.pyi
+-rw-r--r--   0        0        0    12576 2023-06-06 17:19:56.408414 labbench-0.26.0/labbench/_host.py
+-rw-r--r--   0        0        0     1765 2023-06-06 17:19:56.412414 labbench-0.26.0/labbench/_host.pyi
+-rw-r--r--   0        0        0    55225 2023-06-06 17:19:56.416415 labbench-0.26.0/labbench/_rack.py
+-rw-r--r--   0        0        0     5419 2023-06-06 17:19:56.420417 labbench-0.26.0/labbench/_rack.pyi
+-rw-r--r--   0        0        0    11878 2023-06-06 17:19:56.420417 labbench-0.26.0/labbench/_serialize.py
+-rw-r--r--   0        0        0      725 2023-06-06 17:19:56.424414 labbench-0.26.0/labbench/_serialize.pyi
+-rw-r--r--   0        0        0    62858 2023-06-07 20:49:14.039044 labbench-0.26.0/labbench/_traits.py
+-rw-r--r--   0        0        0    14105 2023-06-06 17:19:56.432415 labbench-0.26.0/labbench/_traits.pyi
+-rw-r--r--   0        0        0       60 2023-06-06 17:19:56.432415 labbench-0.26.0/labbench/_version.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:19:56.432415 labbench-0.26.0/labbench/_version.pyi
+-rw-r--r--   0        0        0     2569 2023-06-06 17:19:56.436416 labbench-0.26.0/labbench/datareturn.py
+-rw-r--r--   0        0        0     4144 2023-06-06 17:19:56.436416 labbench-0.26.0/labbench/datareturn.pyi
+-rw-r--r--   0        0        0     7451 2023-06-06 17:19:56.440414 labbench-0.26.0/labbench/notebooks.py
+-rw-r--r--   0        0        0      784 2023-06-06 17:19:56.440414 labbench-0.26.0/labbench/notebooks.pyi
+-rw-r--r--   0        0        0     2568 2023-06-06 17:19:56.444414 labbench-0.26.0/labbench/property.py
+-rw-r--r--   0        0        0     4001 2023-06-06 17:19:56.444414 labbench-0.26.0/labbench/property.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 17:19:56.444414 labbench-0.26.0/labbench/py.typed
+-rw-r--r--   0        0        0    51459 2023-06-06 17:19:56.448415 labbench-0.26.0/labbench/util.py
+-rw-r--r--   0        0        0     3285 2023-06-06 17:19:56.452415 labbench-0.26.0/labbench/util.pyi
+-rw-r--r--   0        0        0     2600 2023-06-06 17:19:56.452415 labbench-0.26.0/labbench/value.py
+-rw-r--r--   0        0        0     4447 2023-06-06 17:19:56.456416 labbench-0.26.0/labbench/value.pyi
+-rw-r--r--   0        0        0     2858 2023-06-06 17:19:56.320416 labbench-0.26.0/LICENSE.md
+-rw-r--r--   0        0        0     2481 2023-06-15 23:01:25.542037 labbench-0.26.0/pyproject.toml
+-rw-r--r--   0        0        0    11272 2023-06-06 17:19:56.320416 labbench-0.26.0/README.md
+-rw-r--r--   0        0        0     2119 2023-06-06 17:19:56.464416 labbench-0.26.0/tests/all.py
+-rw-r--r--   0        0        0     1880 2023-06-06 17:19:56.468415 labbench-0.26.0/tests/emulate.py
+-rw-r--r--   0        0        0     3332 2023-06-06 17:19:56.468415 labbench-0.26.0/tests/module_as_testbed.py
+-rw-r--r--   0        0        0       57 2023-06-06 17:19:56.472415 labbench-0.26.0/tests/profile_imports.py
+-rw-r--r--   0        0        0     4719 2023-06-06 17:19:56.472415 labbench-0.26.0/tests/test_data_logging.py
+-rw-r--r--   0        0        0     2287 2023-06-06 17:19:56.476415 labbench-0.26.0/tests/test_doc.py
+-rw-r--r--   0        0        0     2211 2023-06-06 17:19:56.480414 labbench-0.26.0/tests/test_email.py
+-rw-r--r--   0        0        0     2211 2023-06-06 17:19:56.480414 labbench-0.26.0/tests/test_notification.py
+-rw-r--r--   0        0        0    10850 2023-06-06 17:19:56.484414 labbench-0.26.0/tests/test_property.py
+-rw-r--r--   0        0        0     8889 2023-06-06 17:19:56.484414 labbench-0.26.0/tests/test_rack.py
+-rw-r--r--   0        0        0    13320 2023-06-06 17:19:56.488414 labbench-0.26.0/tests/test_sequencing.py
+-rw-r--r--   0        0        0     4192 2023-06-06 17:19:56.492414 labbench-0.26.0/tests/test_shell.py
+-rw-r--r--   0        0        0     7727 2023-06-06 17:19:56.492414 labbench-0.26.0/tests/test_value.py
+-rw-r--r--   0        0        0    27290 2023-02-06 21:28:33.062776 labbench-0.26.0/tests/testnb.ipynb
+-rw-r--r--   0        0        0    12103 1970-01-01 00:00:00.000000 labbench-0.26.0/PKG-INFO
```

### Comparing `labbench-0.25.0/cli/__main__.py` & `labbench-0.26.0/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/__init__.py` & `labbench-0.26.0/labbench/__init__.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/__init__.pyi` & `labbench-0.26.0/labbench/__init__.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_backends.py` & `labbench-0.26.0/labbench/_backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -1034,15 +1034,15 @@
 
         finally:
             self.backend.close()
 
     @classmethod
     def list_resources(cls):
         """autodetects and returns a list of valid resource strings"""
-        return cls._get_rm().list_resources()
+        return cls()._get_rm().list_resources()
 
     def write(self, msg: str):
         """sends an SCPI message to the device.
 
         Wraps `self.backend.write`, and handles debug logging and adjustments
         when in overlap_and_block
         contexts as appropriate.
```

### Comparing `labbench-0.25.0/labbench/_backends.pyi` & `labbench-0.26.0/labbench/_backends.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_data.py` & `labbench-0.26.0/labbench/_data.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_data.pyi` & `labbench-0.26.0/labbench/_data.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_device.py` & `labbench-0.26.0/labbench/_device.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_device.pyi` & `labbench-0.26.0/labbench/_device.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_host.py` & `labbench-0.26.0/labbench/_host.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_host.pyi` & `labbench-0.26.0/labbench/_host.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_rack.py` & `labbench-0.26.0/labbench/_rack.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_rack.pyi` & `labbench-0.26.0/labbench/_rack.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_serialize.py` & `labbench-0.26.0/labbench/_serialize.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_serialize.pyi` & `labbench-0.26.0/labbench/_serialize.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_traits.py` & `labbench-0.26.0/labbench/_traits.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/_traits.pyi` & `labbench-0.26.0/labbench/_traits.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/datareturn.py` & `labbench-0.26.0/labbench/datareturn.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/datareturn.pyi` & `labbench-0.26.0/labbench/datareturn.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/notebooks.py` & `labbench-0.26.0/labbench/notebooks.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/notebooks.pyi` & `labbench-0.26.0/labbench/notebooks.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/property.py` & `labbench-0.26.0/labbench/property.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/property.pyi` & `labbench-0.26.0/labbench/property.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/util.py` & `labbench-0.26.0/labbench/util.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/util.pyi` & `labbench-0.26.0/labbench/util.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/value.py` & `labbench-0.26.0/labbench/value.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/labbench/value.pyi` & `labbench-0.26.0/labbench/value.pyi`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/LICENSE.md` & `labbench-0.26.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/pyproject.toml` & `labbench-0.26.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "labbench"
-version = "0.25.0"
+version = "0.26.0"
 description = "A set of python tools for clear, concise, and explainable laboratory automation. Codethat achieves these goals should read like a pseudocode expression of the experimentalprocedure. The labbench module supports this goal through an object protocol and support functions.These separate repetitive and error-prone boilerplate code, Use of these capabilitiesamong multiple experimental runs also helps to produced data sets with consistentstructure."
 authors = [
     { name = "Dan Kuester", email = "daniel.kuester@nist.gov" },
     { name = "Shane Allman" },
     { name = "Paul Blanchard" },
     { name = "Yao Ma", email = "yao.ma@nist.gov" },
 ]
```

### Comparing `labbench-0.25.0/README.md` & `labbench-0.26.0/README.md`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/all.py` & `labbench-0.26.0/tests/all.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/emulate.py` & `labbench-0.26.0/tests/emulate.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/module_as_testbed.py` & `labbench-0.26.0/tests/module_as_testbed.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_data_logging.py` & `labbench-0.26.0/tests/test_data_logging.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_doc.py` & `labbench-0.26.0/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_email.py` & `labbench-0.26.0/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_notification.py` & `labbench-0.26.0/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_property.py` & `labbench-0.26.0/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_rack.py` & `labbench-0.26.0/tests/test_rack.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_sequencing.py` & `labbench-0.26.0/tests/test_sequencing.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_shell.py` & `labbench-0.26.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/test_value.py` & `labbench-0.26.0/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/tests/testnb.ipynb` & `labbench-0.26.0/tests/testnb.ipynb`

 * *Files identical despite different names*

### Comparing `labbench-0.25.0/PKG-INFO` & `labbench-0.26.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labbench
-Version: 0.25.0
+Version: 0.26.0
 Summary: A set of python tools for clear, concise, and explainable laboratory automation. Codethat achieves these goals should read like a pseudocode expression of the experimentalprocedure. The labbench module supports this goal through an object protocol and support functions.These separate repetitive and error-prone boilerplate code, Use of these capabilitiesamong multiple experimental runs also helps to produced data sets with consistentstructure.
 Author: Shane Allman,Paul Blanchard
 Author-email: Dan Kuester <daniel.kuester@nist.gov>,Yao Ma <yao.ma@nist.gov>
 Maintainer-email: Dan Kuester <daniel.kuester@nist.gov>
 Requires-Python: >=3.8,<3.12
 Provides-Extra: dotnet
 Provides-Extra: jupyter
```

