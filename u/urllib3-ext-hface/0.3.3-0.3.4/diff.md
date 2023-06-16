# Comparing `tmp/urllib3_ext_hface-0.3.3.tar.gz` & `tmp/urllib3_ext_hface-0.3.4.tar.gz`

## Comparing `urllib3_ext_hface-0.3.3.tar` & `urllib3_ext_hface-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/dev-requirements.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/_aioquic.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/helpers.py
--rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/test_http1.py
--rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/test_http2.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/NOTICE
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/dev-requirements.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http3/_aioquic.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/tests/helpers.py
+-rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/tests/test_http1.py
+-rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/tests/test_http2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/NOTICE
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/README.rst
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.4/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.3.3/CHANGELOG.rst` & `urllib3_ext_hface-0.3.4/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v0.3.4 (2023-06-16)
+-------------------
+
+* Switch ``aioquic`` to (own) fork ``qh3`` that fixes numerous issues. The dependency chain is simpler. Pending discussions with original owner to merge.
+
 v0.3.3 (2023-06-12)
 -------------------
 
 * Push the ``HandshakeCompleted`` event for the ``HTTP2ProtocolHyperImpl``.
 
 v0.3.2 (2023-06-12)
 -------------------
```

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_h11.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/_h2.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http2/_h2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/_aioquic.py` & `urllib3_ext_hface-0.3.4/src/urllib3_ext_hface/protocols/http3/_aioquic.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 from __future__ import annotations
 
 import ssl
 from collections import deque
 from time import monotonic
 from typing import Iterable, Sequence
 
-import aioquic.h3.events as h3_events
-import aioquic.quic.events as quic_events
-from aioquic.h3.connection import H3Connection, ProtocolError
-from aioquic.h3.exceptions import H3Error
-from aioquic.quic.configuration import QuicConfiguration
-from aioquic.quic.connection import QuicConnection, QuicConnectionError
-from aioquic.tls import SessionTicket
+import qh3.h3.events as h3_events
+import qh3.quic.events as quic_events
+from qh3.h3.connection import H3Connection, ProtocolError
+from qh3.h3.exceptions import H3Error
+from qh3.quic.configuration import QuicConfiguration
+from qh3.quic.connection import QuicConnection, QuicConnectionError
+from qh3.tls import SessionTicket
 
 from ..._configuration import QuicTLSConfig
 from ..._typing import AddressType, HeadersType
 from ...events import ConnectionTerminated, DataReceived, Event
 from ...events import HandshakeCompleted as _HandshakeCompleted
 from ...events import HeadersReceived, StreamResetReceived
 from .._protocols import HTTP3Protocol
```

### Comparing `urllib3_ext_hface-0.3.3/tests/helpers.py` & `urllib3_ext_hface-0.3.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/tests/test_http1.py` & `urllib3_ext_hface-0.3.4/tests/test_http1.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/tests/test_http2.py` & `urllib3_ext_hface-0.3.4/tests/test_http2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/tests/test_integration.py` & `urllib3_ext_hface-0.3.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/LICENSE` & `urllib3_ext_hface-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/NOTICE` & `urllib3_ext_hface-0.3.4/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/README.rst` & `urllib3_ext_hface-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.3/pyproject.toml` & `urllib3_ext_hface-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
-  "aioquic>=0.9.20,<1.0.0",
+  "qh3>=0.10.0,<1.0.0",
   "h11>=0.11.0,<1.0.0",
   "h2>=4.0.0,<5.0.0",
 ]
 
 [project.urls]
 "Changelog" = "https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst"
 "Documentation" = "https://urllib3.readthedocs.io"
```

### Comparing `urllib3_ext_hface-0.3.3/PKG-INFO` & `urllib3_ext_hface-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.3.3
+Version: 0.3.4
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -29,17 +29,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: aioquic<1.0.0,>=0.9.20
 Requires-Dist: h11<1.0.0,>=0.11.0
 Requires-Dist: h2<5.0.0,>=4.0.0
+Requires-Dist: qh3<1.0.0,>=0.10.0
 Description-Content-Type: text/x-rst
 
 
 ===================================================
 urllib3 extension: hface
 ===================================================
```

