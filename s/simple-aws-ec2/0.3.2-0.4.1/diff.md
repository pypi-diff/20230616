# Comparing `tmp/simple_aws_ec2-0.3.2.tar.gz` & `tmp/simple_aws_ec2-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_ec2-0.3.2.tar", last modified: Wed Jun 14 19:10:21 2023, max compression
+gzip compressed data, was "simple_aws_ec2-0.4.1.tar", last modified: Fri Jun 16 01:24:31 2023, max compression
```

## Comparing `simple_aws_ec2-0.3.2.tar` & `simple_aws_ec2-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:10:21.450364 simple_aws_ec2-0.3.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-14 19:10:21.450194 simple_aws_ec2-0.3.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5722 2023-06-14 19:01:43.000000 simple_aws_ec2-0.3.2/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     2176 2023-06-14 19:10:01.000000 simple_aws_ec2-0.3.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.3.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.3.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-14 19:10:21.450414 simple_aws_ec2-0.3.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.3.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:10:21.448525 simple_aws_ec2-0.3.2/simple_aws_ec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.3.2/simple_aws_ec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-14 19:09:15.000000 simple_aws_ec2-0.3.2/simple_aws_ec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1186 2023-06-14 18:22:49.000000 simple_aws_ec2-0.3.2/simple_aws_ec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:10:21.449268 simple_aws_ec2-0.3.2/simple_aws_ec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.3.2/simple_aws_ec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    27989 2023-06-14 19:09:09.000000 simple_aws_ec2-0.3.2/simple_aws_ec2/ec2.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:10:21.449149 simple_aws_ec2-0.3.2/simple_aws_ec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-14 19:10:21.000000 simple_aws_ec2-0.3.2/simple_aws_ec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-06-14 19:10:21.000000 simple_aws_ec2-0.3.2/simple_aws_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-14 19:10:21.000000 simple_aws_ec2-0.3.2/simple_aws_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-14 19:10:21.000000 simple_aws_ec2-0.3.2/simple_aws_ec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-14 19:10:21.000000 simple_aws_ec2-0.3.2/simple_aws_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 19:10:21.449830 simple_aws_ec2-0.3.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      693 2023-06-14 18:52:23.000000 simple_aws_ec2-0.3.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7061 2023-06-14 18:29:00.000000 simple_aws_ec2-0.3.2/tests/test_ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.637974 simple_aws_ec2-0.4.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:16.000000 simple_aws_ec2-0.4.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-16 01:24:31.637837 simple_aws_ec2-0.4.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5722 2023-06-14 19:01:43.000000 simple_aws_ec2-0.4.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2621 2023-06-16 01:09:03.000000 simple_aws_ec2-0.4.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.4.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.4.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 01:24:31.638017 simple_aws_ec2-0.4.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.4.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.635519 simple_aws_ec2-0.4.1/simple_aws_ec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 01:21:55.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1389 2023-06-16 01:11:20.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.636559 simple_aws_ec2-0.4.1/simple_aws_ec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    33285 2023-06-16 01:10:53.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/exc.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.637065 simple_aws_ec2-0.4.1/simple_aws_ec2/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.636425 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.637524 simple_aws_ec2-0.4.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3071 2023-06-16 01:21:32.000000 simple_aws_ec2-0.4.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8114 2023-06-16 01:06:20.000000 simple_aws_ec2-0.4.1/tests/test_ec2.py
```

### Comparing `simple_aws_ec2-0.3.2/LICENSE.txt` & `simple_aws_ec2-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.3.2/PKG-INFO` & `simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: simple_aws_ec2
-Version: 0.3.2
+Name: simple-aws-ec2
+Version: 0.4.1
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.3.2/README.rst` & `simple_aws_ec2-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.3.2/release-history.rst` & `simple_aws_ec2-0.4.1/release-history.rst`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.1 (2023-06-15)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add :meth:`~simple_aws_ec2.ec2.Ec2Instance.wait_for_status` waiter method.
+- add :meth:`~simple_aws_ec2.ec2.Ec2Instance.wait_for_running` waiter method.
+- add :meth:`~simple_aws_ec2.ec2.Ec2Instance.wait_for_stopped` waiter method.
+- add :meth:`~simple_aws_ec2.ec2.Ec2Instance.wait_for_terminated` waiter method.
+
+
 0.3.2 (2023-06-14)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - Fix a bug that :meth:`~simple_aws_ec2.ec2.Image.os_type` returns ``None`` when it fails to guess, however, it should raise an exception.
```

### Comparing `simple_aws_ec2-0.3.2/requirements-doc.txt` & `simple_aws_ec2-0.4.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.3.2/setup.py` & `simple_aws_ec2-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.3.2/simple_aws_ec2/ec2.py` & `simple_aws_ec2-0.4.1/simple_aws_ec2/ec2.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 import dataclasses
 from datetime import datetime
 from urllib import request
 
 from func_args import resolve_kwargs, NOTHING
 from iterproxy import IterProxy
 
+from .vendor.waiter import Waiter
+from .exc import StatusError
+
 
 class CannotDetectOSTypeError(TypeError):
     """
     raised when unable to use the name and description to detect the OS type
     of the AMI.
     """
 
@@ -54,14 +57,31 @@
     running = "running"
     shutting_down = "shutting-down"
     terminated = "terminated"
     stopping = "stopping"
     stopped = "stopped"
 
 
+T_STATUS_ENUM_SET = T.Set[EC2InstanceStatusEnum]
+
+
+class EC2InstanceStatusGroupEnum:
+    ended: T_STATUS_ENUM_SET = {
+        EC2InstanceStatusEnum.running,
+        EC2InstanceStatusEnum.terminated,
+        EC2InstanceStatusEnum.stopped,
+    }
+
+    in_transition: T_STATUS_ENUM_SET = {
+        EC2InstanceStatusEnum.pending,
+        EC2InstanceStatusEnum.shutting_down,
+        EC2InstanceStatusEnum.stopping,
+    }
+
+
 class EC2InstanceArchitectureEnum(str, enum.Enum):
     """
     Ec2 instance architecture enumerations.
     """
 
     i386 = "i386"
     x86_64 = "x86_64"
@@ -219,14 +239,150 @@
         """
         return ec2_client.stop_instances(
             InstanceIds=[self.id],
             DryRun=False,
         )
 
     # --------------------------------------------------------------------------
+    # Waiter
+    # --------------------------------------------------------------------------
+    def wait_for_status(
+        self,
+        ec2_client,
+        stop_status: T.Union[EC2InstanceStatusEnum, T.List[EC2InstanceStatusEnum]],
+        delays: T.Union[int, float] = 10,
+        timeout: T.Union[int, float] = 300,
+        error_status: T.Optional[
+            T.Union[EC2InstanceStatusEnum, T.List[EC2InstanceStatusEnum]]
+        ] = None,
+        indent: int = 0,
+        verbose: bool = True,
+    ) -> "Ec2Instance":  # pragma: no cover
+        """
+        wait until the EC2 instance reaches the specified status defined in
+        ``stop_status``. If reaches any of ``error_status ``, raise error.
+
+        :param ec2_client:
+        :param stop_status: status to stop waiting
+        :param delays: delay between each check
+        :param timeout: timeout in seconds
+        :param error_status: status to raise error
+        :param indent: indent level for logging
+        :param verbose: whether to print log
+
+        :return: the :class:`Ec2Instance` representing the latest status
+            of DB instance.
+        """
+        if isinstance(stop_status, EC2InstanceStatusEnum):
+            stop_status_set = {stop_status.value}
+        else:
+            stop_status_set = {status.value for status in EC2InstanceStatusEnum}
+        if error_status is None:
+            error_status_set = set()
+        elif isinstance(error_status, EC2InstanceStatusEnum):
+            error_status_set = {error_status.value}
+        else:
+            error_status_set = {status.value for status in EC2InstanceStatusEnum}
+
+        for attempt, elapse in Waiter(
+            delays=delays,
+            timeout=timeout,
+            indent=indent,
+            verbose=verbose,
+        ):
+            ec2_inst = self.from_id(ec2_client, self.id)
+            if ec2_inst.status in stop_status_set:
+                return ec2_inst
+            elif ec2_inst.status in error_status_set:
+                raise StatusError(f"stop because status reaches {ec2_inst.status!r}")
+            else:
+                pass
+
+    def wait_for_running(
+        self,
+        ec2_client,
+        delays: T.Union[int, float] = 10,
+        timeout: T.Union[int, float] = 300,
+        indent: int = 0,
+        verbose: bool = True,
+    ) -> "Ec2Instance":  # pragma: no cover
+        """
+        Similar to :meth:`Ec2Instance.wait_for_status`, but wait for
+        EC2 instance to reach "running" status.
+        """
+        return self.wait_for_status(
+            ec2_client=ec2_client,
+            stop_status=EC2InstanceStatusEnum.running,
+            delays=delays,
+            timeout=timeout,
+            error_status=[
+                EC2InstanceStatusEnum.shutting_down,
+                EC2InstanceStatusEnum.terminated,
+                EC2InstanceStatusEnum.stopping,
+                EC2InstanceStatusEnum.stopped,
+            ],
+            indent=indent,
+            verbose=verbose,
+        )
+
+    def wait_for_stopped(
+        self,
+        ec2_client,
+        delays: T.Union[int, float] = 10,
+        timeout: T.Union[int, float] = 300,
+        indent: int = 0,
+        verbose: bool = True,
+    ) -> "Ec2Instance":  # pragma: no cover
+        """
+        Similar to :meth:`Ec2Instance.wait_for_status`, but wait for
+        EC2 instance to reach "stopped" status.
+        """
+        return self.wait_for_status(
+            ec2_client=ec2_client,
+            stop_status=EC2InstanceStatusEnum.stopped,
+            delays=delays,
+            timeout=timeout,
+            error_status=[
+                EC2InstanceStatusEnum.pending,
+                EC2InstanceStatusEnum.running,
+                EC2InstanceStatusEnum.shutting_down,
+                EC2InstanceStatusEnum.terminated,
+            ],
+            indent=indent,
+            verbose=verbose,
+        )
+
+    def wait_for_terminated(
+        self,
+        ec2_client,
+        delays: T.Union[int, float] = 10,
+        timeout: T.Union[int, float] = 300,
+        indent: int = 0,
+        verbose: bool = True,
+    ) -> "Ec2Instance":  # pragma: no cover
+        """
+        Similar to :meth:`Ec2Instance.wait_for_status`, but wait for
+        EC2 instance to reach "terminated" status.
+        """
+        return self.wait_for_status(
+            ec2_client=ec2_client,
+            stop_status=EC2InstanceStatusEnum.terminated,
+            delays=delays,
+            timeout=timeout,
+            error_status=[
+                EC2InstanceStatusEnum.pending,
+                EC2InstanceStatusEnum.running,
+                EC2InstanceStatusEnum.stopping,
+                EC2InstanceStatusEnum.stopped,
+            ],
+            indent=indent,
+            verbose=verbose,
+        )
+
+    # --------------------------------------------------------------------------
     # more constructor methods
     # --------------------------------------------------------------------------
     @classmethod
     def _yield_dict_from_describe_instances_response(
         cls, res: dict
     ) -> T.Iterable["Ec2Instance"]:
         for reservation in res.get("Reservations", []):
```

### Comparing `simple_aws_ec2-0.3.2/simple_aws_ec2.egg-info/PKG-INFO` & `simple_aws_ec2-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: simple-aws-ec2
-Version: 0.3.2
+Name: simple_aws_ec2
+Version: 0.4.1
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.3.2/tests/test_ec2.py` & `simple_aws_ec2-0.4.1/tests/test_ec2.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import os
 import pytest
 import moto
 from boto_session_manager import BotoSesManager
 
 from simple_aws_ec2.ec2 import (
+    StatusError,
+    EC2InstanceStatusEnum,
     Ec2Instance,
     Image,
     ImageOwnerGroupEnum,
     ImageOSTypeEnum,
 )
 
 
@@ -189,16 +191,44 @@
 
         image = Image.from_id(self.bsm.ec2_client, self.image_id_1)
         image.name = "ubuntu"
         image.description = "Ubuntu"
         assert image.os_type is ImageOSTypeEnum.Ubuntu
         assert "ubuntu" in image.users
 
+    def _test_wait_for_status(self):
+        ec2_inst = Ec2Instance.from_id(self.bsm.ec2_client, self.inst_id_1)
+        assert ec2_inst.is_running() is True
+        with pytest.raises(StatusError):
+            ec2_inst.wait_for_stopped(
+                ec2_client=self.bsm.ec2_client,
+                verbose=False,
+            )
+        with pytest.raises(StatusError):
+            ec2_inst.wait_for_terminated(
+                ec2_client=self.bsm.ec2_client,
+                verbose=False,
+            )
+
+        ec2_inst.stop_instance(self.bsm.ec2_client)
+        new_ec2_inst = ec2_inst.wait_for_status(
+            ec2_client=self.bsm.ec2_client,
+            stop_status=EC2InstanceStatusEnum.stopped,
+            verbose=False,
+        )
+        assert new_ec2_inst.is_stopped() is True
+        with pytest.raises(StatusError):
+            new_ec2_inst.wait_for_running(
+                ec2_client=self.bsm.ec2_client,
+                verbose=False,
+            )
+
     def test(self):
         self._test_ec2()
         self._test_ec2_start_and_stop()
+        self._test_wait_for_status()
         self._test_image()
 
 
 if __name__ == "__main__":
     basename = os.path.basename(__file__)
     pytest.main([basename, "-s", "--tb=native"])
```

