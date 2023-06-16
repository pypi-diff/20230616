# Comparing `tmp/pyEmby-1.8.tar.gz` & `tmp/pyEmby-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyEmby-1.8.tar", last modified: Sun Nov  7 03:13:37 2021, max compression
+gzip compressed data, was "dist/pyEmby-1.9.tar", last modified: Fri Jun 16 16:56:36 2023, max compression
```

## Comparing `pyEmby-1.8.tar` & `pyEmby-1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-11-07 03:13:37.000000 pyEmby-1.8/
--rw-rw-r--   0 john      (1000) john      (1000)     1080 2016-10-18 03:54:42.000000 pyEmby-1.8/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)       41 2016-10-19 14:30:15.000000 pyEmby-1.8/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)      388 2021-11-07 03:13:37.000000 pyEmby-1.8/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1424 2018-12-15 04:21:30.000000 pyEmby-1.8/README.md
--rw-r--r--   0 john      (1000) john      (1000)      812 2021-11-07 03:10:17.000000 pyEmby-1.8/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-11-07 03:13:37.000000 pyEmby-1.8/pyemby/
--rw-r--r--   0 john      (1000) john      (1000)      232 2018-12-15 04:24:54.000000 pyEmby-1.8/pyemby/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     1799 2021-11-07 03:09:46.000000 pyEmby-1.8/pyemby/helpers.py
--rw-r--r--   0 john      (1000) john      (1000)     8480 2021-11-07 03:09:33.000000 pyEmby-1.8/pyemby/device.py
--rw-r--r--   0 john      (1000) john      (1000)      501 2021-11-07 03:09:20.000000 pyEmby-1.8/pyemby/constants.py
--rw-r--r--   0 john      (1000) john      (1000)    16983 2021-11-07 03:09:56.000000 pyEmby-1.8/pyemby/server.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-16 16:56:36.000000 pyEmby-1.9/
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-16 16:56:36.000000 pyEmby-1.9/pyemby/
+-rwxr--r--   0 john      (1000) john      (1000)      501 2023-06-16 15:43:44.000000 pyEmby-1.9/pyemby/constants.py
+-rw-r--r--   0 john      (1000) john      (1000)     1799 2021-11-07 03:09:46.000000 pyEmby-1.9/pyemby/helpers.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17043 2023-06-16 15:41:23.000000 pyEmby-1.9/pyemby/server.py
+-rw-r--r--   0 john      (1000) john      (1000)      232 2018-12-15 04:24:54.000000 pyEmby-1.9/pyemby/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     8480 2021-11-07 03:09:33.000000 pyEmby-1.9/pyemby/device.py
+-rw-rw-r--   0 john      (1000) john      (1000)       41 2016-10-19 14:30:15.000000 pyEmby-1.9/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1080 2016-10-18 03:54:42.000000 pyEmby-1.9/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      388 2023-06-16 16:56:36.000000 pyEmby-1.9/PKG-INFO
+-rwxr--r--   0 john      (1000) john      (1000)      812 2023-06-16 15:43:30.000000 pyEmby-1.9/setup.py
+-rw-r--r--   0 john      (1000) john      (1000)     1424 2018-12-15 04:21:30.000000 pyEmby-1.9/README.md
```

### Comparing `pyEmby-1.8/LICENSE.txt` & `pyEmby-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyEmby-1.8/README.md` & `pyEmby-1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyEmby-1.8/setup.py` & `pyEmby-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # python setup.py sdist upload -r pypi
 
 
 from distutils.core import setup
 setup(
     name='pyEmby',
     packages=['pyemby'],
-    version='1.8',
+    version='1.9',
     description='Provides a python interface to interact with a Emby media server.',
     author='John Mihalic',
     author_email='mezz64@users.noreply.github.com',
     url='https://github.com/mezz64/pyemby',
-    download_url = 'https://github.com/mezz64/pyemby/tarball/1.8',
+    download_url = 'https://github.com/mezz64/pyemby/tarball/1.9',
     keywords= ['emby', 'media sever', 'api wrapper'],
     classifiers = [],
     )
```

### Comparing `pyEmby-1.8/pyemby/helpers.py` & `pyEmby-1.9/pyemby/helpers.py`

 * *Files identical despite different names*

### Comparing `pyEmby-1.8/pyemby/device.py` & `pyEmby-1.9/pyemby/device.py`

 * *Files identical despite different names*

### Comparing `pyEmby-1.8/pyemby/server.py` & `pyEmby-1.9/pyemby/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,39 +290,40 @@
                     elif msg.type == aiohttp.WSMsgType.error:
                         _LOGGER.debug(
                             'Websocket encountered an error: %s', msg)
                         raise ValueError('Websocket error.')
 
             except (aiohttp.ClientError, asyncio.TimeoutError,
                     aiohttp.WSServerHandshakeError,
-                    ConnectionRefusedError, OSError, ValueError) as err:
+                    ConnectionRefusedError, OSError, KeyError, ValueError) as err:
                 if not self._shutdown:
                     fail_count += 1
                     _LOGGER.debug('Websocket unintentionally closed.'
                                   ' Trying reconnect in %ss. Error: %s',
                                   (fail_count * 5) + 5, err)
                     await asyncio.sleep(15, self._event_loop)
                     continue
                 else:
                     break
 
     def process_msg(self, msg):
         """Process messages from the event stream."""
         jmsg = json.loads(msg)
-        msgtype = jmsg['MessageType']
-        msgdata = jmsg['Data']
+        msgtype = jmsg.get('MessageType', 'unknown')
+        msgdata = jmsg.get('Data', None)
 
         _LOGGER.debug('New websocket message recieved of type: %s', msgtype)
         if msgtype == 'Sessions':
             self._sessions = clean_none_dict_values(msgdata)
             # Check for new devices and update as needed.
             self.update_device_list(self._sessions)
         """
         May process other message types in the future.
         Other known types are:
+        - Ping (no data)
         - PlaybackStarted
         - PlaybackStopped
         - SessionEnded
         """
 
     def update_device_list(self, sessions):
         """ Update device list. """
```

