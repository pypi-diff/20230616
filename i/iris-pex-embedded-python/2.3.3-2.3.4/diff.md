# Comparing `tmp/iris_pex_embedded_python-2.3.3.tar.gz` & `tmp/iris_pex_embedded_python-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.3.3.tar", last modified: Mon Jun  5 14:57:35 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.3.4.tar", last modified: Fri Jun 16 16:07:39 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.3.3.tar` & `iris_pex_embedded_python-2.3.4.tar`

### file list

```diff
@@ -1,35 +1,57 @@
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.713297 iris_pex_embedded_python-2.3.3/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.3/LICENSE
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49406 2023-06-05 14:57:35.712189 iris_pex_embedded_python-2.3.3/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.3/README.md
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.3/pyproject.toml
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-06-05 14:57:35.713620 iris_pex_embedded_python-2.3.3/setup.cfg
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2295 2023-06-05 14:57:10.000000 iris_pex_embedded_python-2.3.3/setup.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.650513 iris_pex_embedded_python-2.3.3/src/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.649877 iris_pex_embedded_python-2.3.3/src/grongier/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.659170 iris_pex_embedded_python-2.3.3/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.696950 iris_pex_embedded_python-2.3.3/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/__main__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5320 2023-06-02 13:11:45.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_cli.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8810 2023-06-02 13:08:23.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.3/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-06-05 14:57:35.709898 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49406 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      933 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       47 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/entry_points.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       43 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-06-05 14:57:35.000000 iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:39.009221 iris_pex_embedded_python-2.3.4/
+-rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.4/LICENSE
+-rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-16 16:07:39.008309 iris_pex_embedded_python-2.3.4/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.4/README.md
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.4/pyproject.toml
+-rw-r--r--   0 grongier (902446405) 1252422112       38 2023-06-16 16:07:39.009491 iris_pex_embedded_python-2.3.4/setup.cfg
+-rw-r--r--   0 grongier (902446405) 1252422112     2322 2023-06-16 16:03:46.000000 iris_pex_embedded_python-2.3.4/setup.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.923551 iris_pex_embedded_python-2.3.4/src/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.920246 iris_pex_embedded_python-2.3.4/src/grongier/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.959245 iris_pex_embedded_python-2.3.4/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) 1252422112      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/__main__.py
+-rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-06-16 07:35:26.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5647 2023-06-16 15:49:29.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_cli.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15158 2023-06-15 13:47:53.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) 1252422112     8810 2023-06-02 13:08:23.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15066 2023-06-16 16:06:46.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.921263 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.982206 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/
+-rw-r--r--   0 grongier (902446405) 1252422112      932 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessOperation.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     2633 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessProcess.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1039 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/BusinessService.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     3538 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Common.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1894 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Director.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.987563 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/
+-rw-r--r--   0 grongier (902446405) 1252422112      543 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Operation.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     7103 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Process.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      179 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Duplex/Service.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      628 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/InboundAdapter.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     8227 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Message.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      976 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/OutboundAdapter.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1691 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PickleMessage.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.989240 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/
+-rw-r--r--   0 grongier (902446405) 1252422112     8065 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Duplex.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:38.996611 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/
+-rw-r--r--   0 grongier (902446405) 1252422112      986 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Ack.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      987 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Poll.cls
+-rw-r--r--   0 grongier (902446405) 1252422112      994 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Start.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1435 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/PrivateSession/Message/Stop.cls
+-rw-r--r--   0 grongier (902446405) 1252422112     1622 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Test.cls
+-rw-r--r--   0 grongier (902446405) 1252422112    13498 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.4/src/grongier/pex/data/PEX/Utils.cls
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-16 16:07:39.006493 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112     1784 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        1 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       47 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/entry_points.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       43 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        9 2023-06-16 16:07:38.000000 iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.3.3/LICENSE` & `iris_pex_embedded_python-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/PKG-INFO` & `iris_pex_embedded_python-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.3.3
+Version: 2.3.4
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.3.3/README.md` & `iris_pex_embedded_python-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/setup.py` & `iris_pex_embedded_python-2.3.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.3.3',
+        version='2.3.4',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
@@ -42,16 +42,16 @@
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             'Topic :: Utilities'
         ],
         package_dir={'': 'src'},
-        packages=['grongier.pex','grongier.iris'],
-        include_package_data=True,
+        packages=['grongier.pex','grongier.pex.data'],
+        package_data={'grongier.pex.data': ['**/*.cls']},
         python_requires='>=3.6',
         install_requires=[
             "dacite>=1.6.0",
             "xmltodict>=0.12.0",
             "irissqlcli"
         ],
         entry_points={
```

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_cli.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     parser.add_argument('-d', '--default', help='set the default production', nargs='?', const='not_set')
     parser.add_argument('-l', '--lists', help='list productions', action='store_true')
     parser.add_argument('-s', '--start', help='start a production', nargs='?', const='not_set')
     parser.add_argument('-S', '--stop', help='stop a production', action='store_true')
     parser.add_argument('-k', '--kill', help='kill a production', action='store_true')
     parser.add_argument('-r', '--restart', help='restart a production', action='store_true')
     parser.add_argument('-x', '--status', help='status a production', action='store_true')
-    parser.add_argument('-M', '--migrate', help='migrate production and classes with settings file')
+    parser.add_argument('-M', '-m', '--migrate', help='migrate production and classes with settings file')
     parser.add_argument('-e', '--export', help='export a production', nargs='?', const='not_set')
     parser.add_argument('-v', '--version', help='display version', action='store_true')
     parser.add_argument('-L', '--log', help='display log', action='store_true')
+    parser.add_argument('-i', '--init', help='init the pex module in iris', nargs='?', const='not_set')
     return parser.parse_args(argv)
 
 def main(argv=None):
     # build arguments
     args = parse_args(argv)
 
     if args.default:
@@ -51,14 +52,20 @@
 
     elif args.start:
         if args.start == 'not_set':
             # start default production
             args.start = _Director.get_default_production()
         _Director.start_production_with_log(args.start)
 
+    elif args.init:
+        if args.init == 'not_set':
+            # set arg to None
+            args.init = None
+        _Utils.setup(args.start)
+
     elif args.kill:
         # kill a production
         _Director.shutdown_production()
 
     elif args.restart:
         # restart a production
         _Director.restart_production()
@@ -108,13 +115,14 @@
         print("  -M MIGRATE, --migrate MIGRATE")
         print("                        migrate production and classes with settings file")
         print("  -e EXPORT, --export EXPORT")
         print("                        export a production")
         print("  -x, --status          status a production")
         print("  -v, --version         display version")
         print("  -L, --log             display log")
+        print("  -i, --init            init the pex module in iris")
         print("")
         print("default production: " + _Director.get_default_production())
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import traceback
 import dataclasses
 import inspect
 import iris
+import abc
 
-class _Common():
+class _Common(metaclass=abc.ABCMeta):
     """ This is a common superclass for all component types that defines common methods."""
 
     INFO_URL: str
     ICON_URL: str
     iris_handle = None
 
     def on_init(self):
@@ -126,16 +127,16 @@
             icon_url = inspect.getattr_static(cls,"ICON_URL","")
 
             ret.append(info_url)
             ret.append(icon_url)
             
             if ""!=adapter:
                 ret.append(adapter)
-        except:
-            pass
+        except Exception as e:
+            raise e
         return ret
 
     @classmethod
     def _get_properties(cls):
         """ Get a list of the Attributes and Properties of this Python class.
         Return value is a list of lists of form $lb(propName,data_type,defaultVal,required,category,description).
         which can be used by the Production Configuration to display them as settings.
```

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.3/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.3.4/src/grongier/pex/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import ast
 import iris
 import inspect
 import xmltodict
+import pkg_resources
 
 class _Utils():
     @staticmethod
     def raise_on_error(sc):
         """
         If the status code is an error, raise an exception
         
@@ -15,17 +16,16 @@
         if iris.system.Status.IsError(sc):
             raise RuntimeError(iris.system.Status.GetOneStatusText(sc))
 
     @staticmethod
     def setup(path:str = None):
 
         if path is None:
-            # get the parent directory of the current module
-            # and append 'iris/Grongier/PEX' to it
-            path = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'iris/Grongier/PEX')
+            # get the path of the data folder with pkg_resources
+            path = pkg_resources.resource_filename(__name__, 'data')
 
         _Utils.raise_on_error(iris.cls('%SYSTEM.OBJ').LoadDir(path,'cubk',"*.cls",1))
 
     @staticmethod
     def register_component(module:str,classname:str,path:str,overwrite:int=1,iris_classname:str='Python'):
         """
         It registers a component in the Iris database.
```

### Comparing `iris_pex_embedded_python-2.3.3/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.3.4/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.3.3
+Version: 2.3.4
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

