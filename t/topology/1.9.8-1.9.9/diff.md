# Comparing `tmp/topology-1.9.8.tar.gz` & `tmp/topology-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/topology-1.9.8.tar", last modified: Wed Jun 12 20:16:12 2019, max compression
+gzip compressed data, was "dist/topology-1.9.9.tar", last modified: Wed Jun 12 20:17:45 2019, max compression
```

## Comparing `topology-1.9.8.tar` & `topology-1.9.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       38 2019-06-12 20:16:12.000000 topology-1.9.8/setup.cfg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25118 2019-06-12 20:16:01.000000 topology-1.9.8/README.rst
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       28 2019-06-12 20:12:14.000000 topology-1.9.8/requirements.txt
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2943 2019-06-12 20:13:23.000000 topology-1.9.8/setup.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11325 2018-09-07 23:15:10.000000 topology-1.9.8/LICENSE
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/lib/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology.egg-info/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       28 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        9 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31705 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      968 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology.egg-info/SOURCES.txt
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology/pytest/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10184 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/pytest/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      799 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/pytest/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology/platforms/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5892 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/platforms/platform.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1714 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/platforms/service.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15388 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/platforms/node.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3798 2019-06-12 20:16:01.000000 topology-1.9.8/lib/topology/platforms/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4227 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/platforms/debug.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      795 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/platforms/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1659 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/platforms/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3153 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/platforms/manager.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27374 2019-06-12 20:14:53.000000 topology-1.9.8/lib/topology/platforms/shell.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3468 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/main.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5356 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/interact.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4695 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/args.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/lib/topology/libraries/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2978 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/libraries/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      795 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/libraries/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4935 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/libraries/manager.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1730 2018-09-07 23:15:10.000000 topology-1.9.8/lib/topology/libraries/common.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      907 2019-06-12 20:16:01.000000 topology-1.9.8/lib/topology/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18433 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/logging.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10088 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/injection.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7385 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/parser.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11777 2019-06-12 20:12:14.000000 topology-1.9.8/lib/topology/manager.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31705 2019-06-12 20:16:12.000000 topology-1.9.8/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      103 2018-09-07 23:15:10.000000 topology-1.9.8/MANIFEST.in
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:16:12.000000 topology-1.9.8/bin/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      957 2018-09-07 23:15:10.000000 topology-1.9.8/bin/topology
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       38 2019-06-12 20:17:45.000000 topology-1.9.9/setup.cfg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25313 2019-06-12 20:17:14.000000 topology-1.9.9/README.rst
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       28 2019-06-12 20:12:14.000000 topology-1.9.9/requirements.txt
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     2943 2019-06-12 20:13:23.000000 topology-1.9.9/setup.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11325 2018-09-07 23:15:10.000000 topology-1.9.9/LICENSE
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/lib/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology.egg-info/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       28 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        9 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31980 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      968 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology.egg-info/SOURCES.txt
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology/pytest/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10184 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/pytest/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      799 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/pytest/__init__.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology/platforms/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5892 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/platforms/platform.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1714 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/platforms/service.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15388 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/platforms/node.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3798 2019-06-12 20:16:01.000000 topology-1.9.9/lib/topology/platforms/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4227 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/platforms/debug.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      795 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/platforms/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1659 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/platforms/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3153 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/platforms/manager.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27712 2019-06-12 20:17:14.000000 topology-1.9.9/lib/topology/platforms/shell.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3468 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/main.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5356 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/interact.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4695 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/args.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/lib/topology/libraries/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2978 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/libraries/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      795 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/libraries/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4935 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/libraries/manager.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1730 2018-09-07 23:15:10.000000 topology-1.9.9/lib/topology/libraries/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      907 2019-06-12 20:17:14.000000 topology-1.9.9/lib/topology/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18433 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/logging.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10088 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/injection.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7385 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11777 2019-06-12 20:12:14.000000 topology-1.9.9/lib/topology/manager.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31980 2019-06-12 20:17:45.000000 topology-1.9.9/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      103 2018-09-07 23:15:10.000000 topology-1.9.9/MANIFEST.in
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2019-06-12 20:17:45.000000 topology-1.9.9/bin/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      957 2018-09-07 23:15:10.000000 topology-1.9.9/bin/topology
```

### Comparing `topology-1.9.8/README.rst` & `topology-1.9.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,24 @@
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 Changelog
 =========
+1.9.9 (2017-07-26)
+------------------
+
+New
+~~~
+- Adding support for sending control characters. [Diego Antonio Hurtado Pimentel]
+
+Fix
+~~~
+- Increased delay_after_echo_off a bit. [Javier Peralta]
 
 
 1.9.8 (2017-06-13)
 ------------------
 
 Changes
 ~~~~~~~
```

### Comparing `topology-1.9.8/setup.py` & `topology-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/LICENSE` & `topology-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology.egg-info/PKG-INFO` & `topology-1.9.9/lib/topology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: topology
-Version: 1.9.8
+Version: 1.9.9
 Summary: Network Topology Framework using NML, with support for pytest.
 Home-page: http://topology.rtfd.org/
 Author: Hewlett Packard Enterprise Development LP
 Author-email: hpe-networking@lists.hp.com
 License: UNKNOWN
 Description: ==========================
         Topology Modular Framework
@@ -40,14 +40,24 @@
            "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
            KIND, either express or implied.  See the License for the
            specific language governing permissions and limitations
            under the License.
         
         Changelog
         =========
+        1.9.9 (2017-07-26)
+        ------------------
+        
+        New
+        ~~~
+        - Adding support for sending control characters. [Diego Antonio Hurtado Pimentel]
+        
+        Fix
+        ~~~
+        - Increased delay_after_echo_off a bit. [Javier Peralta]
         
         
         1.9.8 (2017-06-13)
         ------------------
         
         Changes
         ~~~~~~~
```

### Comparing `topology-1.9.8/lib/topology.egg-info/SOURCES.txt` & `topology-1.9.9/lib/topology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/pytest/plugin.py` & `topology-1.9.9/lib/topology/pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/pytest/__init__.py` & `topology-1.9.9/lib/topology/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/platform.py` & `topology-1.9.9/lib/topology/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/service.py` & `topology-1.9.9/lib/topology/platforms/service.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/node.py` & `topology-1.9.9/lib/topology/platforms/node.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/utils.py` & `topology-1.9.9/lib/topology/platforms/utils.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/debug.py` & `topology-1.9.9/lib/topology/platforms/debug.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/__init__.py` & `topology-1.9.9/lib/topology/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/base.py` & `topology-1.9.9/lib/topology/platforms/base.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/manager.py` & `topology-1.9.9/lib/topology/platforms/manager.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/platforms/shell.py` & `topology-1.9.9/lib/topology/platforms/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,18 +448,23 @@
             raise NonExistingConnectionError(connection)
 
         return self._connections[connection]
 
     def send_command(
         self, command,
         matches=None, newline=True,
-        timeout=None, connection=None, silent=False
+        timeout=None, connection=None, silent=False, control=False
     ):
         """
         See :meth:`BaseShell.send_command` for more information.
+
+        :param bool control: This is to be used with single character commands
+         only. If enabled, the character sent will be interpreted as a control
+         character. Enabling this option makes ``newline`` irrelevant. Defaults
+         to ``False``.
         """
         # If auto connect is false, fail if:
         # 1. Connection is missing
         # 2. Connection is disconnected
         if not self._auto_connect:
             if not self.is_connected(connection):
                 raise DisconnectedError(connection)
@@ -484,15 +489,17 @@
         if self._prefix is not None:
             command = '{}{}'.format(self._prefix, command)
 
         # Save last command in cache to allow to remove echos in get_response()
         self._last_command = command
 
         # Send line and expect matches
-        if newline:
+        if control:
+            spawn.sendcontrol(command)
+        elif newline:
             spawn.sendline(command)
         else:
             spawn.send(command)
 
         # Log log_send_command
         if not silent:
             spawn._connection_logger.log_send_command(
@@ -687,15 +694,15 @@
            this allows bash enough time to properly turn echo off.
     """
     FORCED_PROMPT = '@~~==::BASH_PROMPT::==~~@'
 
     def __init__(
             self,
             initial_prompt='\w+@.+:.+[#$] ', try_filter_echo=False,
-            delay_after_echo_off=0.15, **kwargs):
+            delay_after_echo_off=0.25, **kwargs):
 
         self._delay_after_echo_off = delay_after_echo_off
 
         super(PExpectBashShell, self).__init__(
             PExpectBashShell.FORCED_PROMPT,
             initial_prompt=initial_prompt,
             try_filter_echo=try_filter_echo,
```

### Comparing `topology-1.9.8/lib/topology/main.py` & `topology-1.9.9/lib/topology/main.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/interact.py` & `topology-1.9.9/lib/topology/interact.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/args.py` & `topology-1.9.9/lib/topology/args.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/libraries/utils.py` & `topology-1.9.9/lib/topology/libraries/utils.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/libraries/__init__.py` & `topology-1.9.9/lib/topology/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/libraries/manager.py` & `topology-1.9.9/lib/topology/libraries/manager.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/libraries/common.py` & `topology-1.9.9/lib/topology/libraries/common.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/__init__.py` & `topology-1.9.9/lib/topology/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 """
 
 from __future__ import unicode_literals, absolute_import
 from __future__ import print_function, division
 
 __author__ = 'Hewlett Packard Enterprise Development LP'
 __email__ = 'hpe-networking@lists.hp.com'
-__version__ = '1.9.8'
+__version__ = '1.9.9'
```

### Comparing `topology-1.9.8/lib/topology/logging.py` & `topology-1.9.9/lib/topology/logging.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/injection.py` & `topology-1.9.9/lib/topology/injection.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/parser.py` & `topology-1.9.9/lib/topology/parser.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/lib/topology/manager.py` & `topology-1.9.9/lib/topology/manager.py`

 * *Files identical despite different names*

### Comparing `topology-1.9.8/PKG-INFO` & `topology-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: topology
-Version: 1.9.8
+Version: 1.9.9
 Summary: Network Topology Framework using NML, with support for pytest.
 Home-page: http://topology.rtfd.org/
 Author: Hewlett Packard Enterprise Development LP
 Author-email: hpe-networking@lists.hp.com
 License: UNKNOWN
 Description: ==========================
         Topology Modular Framework
@@ -40,14 +40,24 @@
            "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
            KIND, either express or implied.  See the License for the
            specific language governing permissions and limitations
            under the License.
         
         Changelog
         =========
+        1.9.9 (2017-07-26)
+        ------------------
+        
+        New
+        ~~~
+        - Adding support for sending control characters. [Diego Antonio Hurtado Pimentel]
+        
+        Fix
+        ~~~
+        - Increased delay_after_echo_off a bit. [Javier Peralta]
         
         
         1.9.8 (2017-06-13)
         ------------------
         
         Changes
         ~~~~~~~
```

### Comparing `topology-1.9.8/bin/topology` & `topology-1.9.9/bin/topology`

 * *Files identical despite different names*

