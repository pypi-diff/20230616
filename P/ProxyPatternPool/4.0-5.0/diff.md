# Comparing `tmp/ProxyPatternPool-4.0.tar.gz` & `tmp/ProxyPatternPool-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProxyPatternPool-4.0.tar", last modified: Sun Feb  5 08:05:37 2023, max compression
+gzip compressed data, was "ProxyPatternPool-5.0.tar", last modified: Fri Jun 16 10:17:52 2023, max compression
```

## Comparing `ProxyPatternPool-4.0.tar` & `ProxyPatternPool-5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-02-05 08:05:37.822568 ProxyPatternPool-4.0/
--rw-------   0 fabien    (1001) fabien    (1001)       33 2022-10-28 15:14:31.000000 ProxyPatternPool-4.0/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)     7737 2023-02-05 08:05:37.822568 ProxyPatternPool-4.0/PKG-INFO
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-02-05 08:05:37.822568 ProxyPatternPool-4.0/ProxyPatternPool.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)     7737 2023-02-05 08:05:37.000000 ProxyPatternPool-4.0/ProxyPatternPool.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      216 2023-02-05 08:05:37.000000 ProxyPatternPool-4.0/ProxyPatternPool.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2023-02-05 08:05:37.000000 ProxyPatternPool-4.0/ProxyPatternPool.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)       17 2023-02-05 08:05:37.000000 ProxyPatternPool-4.0/ProxyPatternPool.egg-info/top_level.txt
--rw-------   0 fabien    (1001) fabien    (1001)    14472 2023-02-05 07:18:27.000000 ProxyPatternPool-4.0/ProxyPatternPool.py
--rw-------   0 fabien    (1001) fabien    (1001)     6778 2023-02-04 18:54:29.000000 ProxyPatternPool-4.0/README.md
--rw-------   0 fabien    (1001) fabien    (1001)      925 2023-02-05 08:05:37.822568 ProxyPatternPool-4.0/setup.cfg
--rw-------   0 fabien    (1001) fabien    (1001)       89 2022-10-28 15:15:43.000000 ProxyPatternPool-4.0/setup.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/
+-rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:31:46.000000 ProxyPatternPool-5.0/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)     7841 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/PKG-INFO
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)     7841 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      251 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)       98 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)       17 2023-06-16 10:17:52.000000 ProxyPatternPool-5.0/ProxyPatternPool.egg-info/top_level.txt
+-rw-------   0 fabien    (1001) fabien    (1001)    14612 2023-06-16 10:13:04.000000 ProxyPatternPool-5.0/ProxyPatternPool.py
+-rw-------   0 fabien    (1001) fabien    (1001)     6951 2023-06-16 10:07:28.000000 ProxyPatternPool-5.0/README.md
+-rw-------   0 fabien    (1001) fabien    (1001)     1095 2023-06-16 10:05:55.000000 ProxyPatternPool-5.0/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2023-06-16 10:17:52.413589 ProxyPatternPool-5.0/setup.cfg
```

### Comparing `ProxyPatternPool-4.0/PKG-INFO` & `ProxyPatternPool-5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ProxyPatternPool
-Version: 4.0
+Version: 5.0
 Summary: Generic Proxy and Pool Classes for Python
-Home-page: https://github.com/zx80/proxy-pattern-pool
-Author: Fabien Coelho
-Author-email: proxy.pool@coelho.net
-License: UNKNOWN
+Author-email: Fabien Coelho <proxy.pool@coelho.net>
+License: CC0
+Project-URL: repository, https://github.com/zx80/proxy-pattern-pool
 Project-URL: documentation, https://zx80.github.io/proxy-pattern-pool/
 Project-URL: issues, https://github.com/zx80/proxy-pattern-pool/issues
-Project-URL: sources, https://github.com/zx80/proxy-pattern-pool
 Project-URL: package, https://pypi.org/project/ProxyPatternPool/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Flask
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: local
+Provides-Extra: dev
+Provides-Extra: pub
 License-File: LICENSE
 
 # Proxy Pattern Pool
 
 Generic Proxy and Pool Classes for Python.
 
 ![Status](https://github.com/zx80/proxy-pattern-pool/actions/workflows/ppp.yml/badge.svg?branch=main&style=flat)
@@ -188,15 +187,20 @@
 [Sources](https://github.com/zx80/proxy-pattern-pool),
 [documentation](https://zx80.github.io/proxy-pattern-pool/) and
 [issues](https://github.com/zx80/proxy-pattern-pool/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/ProxyPatternPool/) from
 [PyPI](https://pypi.org/).
 
-### 4.0 on ?
+### 5.0 on 2023-06-16
+
+Use `pyproject.toml` only.
+Require Python *3.10* for simpler code.
+
+### 4.0 on 2023-02-05
 
 Add `max_using_delay` for warnings.
 Add `with` support to both `Pool` and `Proxy` classes.
 Add module-specific exceptions: `PoolException`, `ProxyException`.
 
 ### 3.0 on 2022-12-27
 
@@ -225,9 +229,9 @@
 
 Initial release with code extracted from `FlaskSimpleAuth`.
 
 ## TODO
 
 - greenlet, eventlet, or gevent?
 - add a method to delete the proxy?
-
-
+- add an actual timeout feature?
+- how to manage a return automatically?
```

### Comparing `ProxyPatternPool-4.0/ProxyPatternPool.egg-info/PKG-INFO` & `ProxyPatternPool-5.0/ProxyPatternPool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ProxyPatternPool
-Version: 4.0
+Version: 5.0
 Summary: Generic Proxy and Pool Classes for Python
-Home-page: https://github.com/zx80/proxy-pattern-pool
-Author: Fabien Coelho
-Author-email: proxy.pool@coelho.net
-License: UNKNOWN
+Author-email: Fabien Coelho <proxy.pool@coelho.net>
+License: CC0
+Project-URL: repository, https://github.com/zx80/proxy-pattern-pool
 Project-URL: documentation, https://zx80.github.io/proxy-pattern-pool/
 Project-URL: issues, https://github.com/zx80/proxy-pattern-pool/issues
-Project-URL: sources, https://github.com/zx80/proxy-pattern-pool
 Project-URL: package, https://pypi.org/project/ProxyPatternPool/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Flask
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: local
+Provides-Extra: dev
+Provides-Extra: pub
 License-File: LICENSE
 
 # Proxy Pattern Pool
 
 Generic Proxy and Pool Classes for Python.
 
 ![Status](https://github.com/zx80/proxy-pattern-pool/actions/workflows/ppp.yml/badge.svg?branch=main&style=flat)
@@ -188,15 +187,20 @@
 [Sources](https://github.com/zx80/proxy-pattern-pool),
 [documentation](https://zx80.github.io/proxy-pattern-pool/) and
 [issues](https://github.com/zx80/proxy-pattern-pool/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/ProxyPatternPool/) from
 [PyPI](https://pypi.org/).
 
-### 4.0 on ?
+### 5.0 on 2023-06-16
+
+Use `pyproject.toml` only.
+Require Python *3.10* for simpler code.
+
+### 4.0 on 2023-02-05
 
 Add `max_using_delay` for warnings.
 Add `with` support to both `Pool` and `Proxy` classes.
 Add module-specific exceptions: `PoolException`, `ProxyException`.
 
 ### 3.0 on 2022-12-27
 
@@ -225,9 +229,9 @@
 
 Initial release with code extracted from `FlaskSimpleAuth`.
 
 ## TODO
 
 - greenlet, eventlet, or gevent?
 - add a method to delete the proxy?
-
-
+- add an actual timeout feature?
+- how to manage a return automatically?
```

### Comparing `ProxyPatternPool-4.0/ProxyPatternPool.py` & `ProxyPatternPool-5.0/ProxyPatternPool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Generic Proxy Pattern Pool for Python.
 
 This code is public domain.
 """
 
-from typing import Optional, Callable, Dict, Set, Any
+from typing import Callable, Any
 from enum import Enum
 from dataclasses import dataclass
 from contextlib import contextmanager
 import threading
 import datetime
 import time
 import logging
 
 # get module version
-import pkg_resources as pkg  # type: ignore
+from importlib.metadata import version as pkg_version
 
-__version__ = pkg.require("ProxyPatternPool")[0].version
+__version__ = pkg_version("ProxyPatternPool")
 
 
 log = logging.getLogger("ppp")
 
 
 class PoolException(Exception):
     pass
@@ -58,15 +58,15 @@
         fun: Callable[[int], Any],
         max_size: int = 0,
         min_size: int = 1,
         timeout: float = None,
         max_use: int = 0,
         max_avail_delay: float = 0.0,
         max_using_delay: float = 0.0,
-        close: Optional[str] = None,
+        close: str|None = None,
         # temporary upward compatibility
         max_delay: float = 0.0,
     ):
         # data attributes
         self._fun = fun
         self._nobjs = 0
         self._nuses = 0
@@ -75,28 +75,28 @@
         self._min_size = min_size
         self._timeout = timeout
         self._max_use = max_use
         self._max_avail_delay = max_avail_delay or max_delay
         self._max_using_delay = max_using_delay
         self._close = close
         # pool's content: available vs in use objects
-        self._avail: Set[Any] = set()
-        self._using: Set[Any] = set()
+        self._avail: set[Any] = set()
+        self._using: set[Any] = set()
         # keep track of usage count and last ops
-        self._uses: Dict[Any, Pool.UseInfo] = {}
+        self._uses: dict[Any, Pool.UseInfo] = {}
         # global pool re-entrant lock to manage attributes
         self._lock = threading.RLock()
-        self._sem: Optional[threading.Semaphore] = None
+        self._sem: threading.Semaphore|None = None
         if self._max_size:
             self._sem = threading.BoundedSemaphore(self._max_size)
         # create the minimum number of objects
         while self._nobjs < self._min_size:
             self._new()
         # start housekeeper thread if needed
-        self._housekeeper: Optional[threading.Thread] = None
+        self._housekeeper: threading.Thread|None = None
         if self._max_avail_delay or self._max_using_delay:
             self._delay = self._max_avail_delay
             if not self._delay or \
                self._max_using_delay and self._delay > self._max_using_delay:  # fmt: skip
                 self._delay = self._max_using_delay
             self._delay /= 2.0
         else:
@@ -116,33 +116,36 @@
     def _houseKeeping(self):
         """Housekeeping thread."""
         log.info(f"housekeeper running every {self._delay}")
         while True:
             time.sleep(self._delay)
             log.debug(str(self))
             if self._nobjs <= self._min_size and not self._max_using_delay:
+                # nothing to do this round
                 continue
             with self._lock:
                 now = self._now()
                 if self._max_using_delay:
                     # warn about long running objects
                     long_running, long_time = 0, 0.0
                     for obj in list(self._using):
                         if now - self._uses[obj].last_get >= self._max_using_delay:
                             long_running += 1
                             long_time += now - self._uses[obj].last_get
                     if long_running:
+                        # TODO what to do about these? force return?
                         log.warning(
                             f"long running objects: {long_running} ({long_time / long_running})"
                         )
                 if self._max_avail_delay:
                     # close objects unused for too long
                     for obj in list(self._avail):
                         if now - self._uses[obj].last_ret >= self._max_avail_delay:
                             self._del(obj)
+                            # stop deleting objects if min size is reached
                             if self._nobjs <= self._min_size:
                                 break
 
     def __delete__(self):
         """This should be done automatically, but eventually."""
         with self._lock:
             # using should be empty
@@ -269,15 +272,15 @@
         max_size: int = 0,
         min_size: int = 1,
         max_use: int = 0,
         max_avail_delay: float = 0.0,
         max_using_delay: float = 0.0,
         timeout: float = None,
         scope: Scope = Scope.AUTO,
-        close: Optional[str] = None,
+        close: str|None = None,
         # temporary backward compatibility
         max_delay: float = 0.0,
     ):
         """Constructor parameters:
 
         - set_name: provide another prefix for the "set" functions.
         - obj: object to be wrapped, can also be provided later.
@@ -343,15 +346,15 @@
 
             self._local = Local()
         return self
 
     def _set(
         self,
         obj: Any = None,
-        fun: Optional[Callable[[int], Any]] = None,
+        fun: Callable[[int], Any]|None = None,
         mandatory=True,
     ):
         """Set current wrapped object or generation function."""
         if obj and fun:
             raise ProxyException("Proxy cannot set both obj and fun")
         elif obj:
             return self._set_obj(obj)
```

### Comparing `ProxyPatternPool-4.0/README.md` & `ProxyPatternPool-5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -165,15 +165,20 @@
 [Sources](https://github.com/zx80/proxy-pattern-pool),
 [documentation](https://zx80.github.io/proxy-pattern-pool/) and
 [issues](https://github.com/zx80/proxy-pattern-pool/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/ProxyPatternPool/) from
 [PyPI](https://pypi.org/).
 
-### 4.0 on ?
+### 5.0 on 2023-06-16
+
+Use `pyproject.toml` only.
+Require Python *3.10* for simpler code.
+
+### 4.0 on 2023-02-05
 
 Add `max_using_delay` for warnings.
 Add `with` support to both `Pool` and `Proxy` classes.
 Add module-specific exceptions: `PoolException`, `ProxyException`.
 
 ### 3.0 on 2022-12-27
 
@@ -202,7 +207,9 @@
 
 Initial release with code extracted from `FlaskSimpleAuth`.
 
 ## TODO
 
 - greenlet, eventlet, or gevent?
 - add a method to delete the proxy?
+- add an actual timeout feature?
+- how to manage a return automatically?
```

