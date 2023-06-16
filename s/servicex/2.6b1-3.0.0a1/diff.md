# Comparing `tmp/servicex-2.6b1.tar.gz` & `tmp/servicex-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ServiceX_frontend/ServiceX_frontend/dist/.tmp-_ow85y6s/servicex-2.6b1.tar", last modified: Thu Nov 24 14:35:20 2022, max compression
+gzip compressed data, was "servicex-3.0.0a1.tar", max compression
```

## Comparing `servicex-2.6b1.tar` & `servicex-3.0.0a1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:35:20.000000 servicex-2.6b1/
--rw-r--r--   0 runner    (1001) docker     (122)    25091 2022-11-24 14:35:20.000000 servicex-2.6b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24217 2022-11-24 14:35:04.000000 servicex-2.6b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex/
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/ConfigSettings.py
--rw-r--r--   0 runner    (1001) docker     (122)      524 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17870 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5775 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9347 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/minio_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (122)    42677 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex.py
--rw-r--r--   0 runner    (1001) docker     (122)    10203 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (122)     8121 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2763 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_python_function.py
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7266 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicexabc.py
--rw-r--r--   0 runner    (1001) docker     (122)    21388 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    25091 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      511 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      318 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 14:35:20.000000 servicex-2.6b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2022-11-24 14:35:04.000000 servicex-2.6b1/setup.py
+-rw-r--r--   0        0        0     1499 2023-06-16 21:24:27.546614 servicex-3.0.0a1/LICENSE
+-rw-r--r--   0        0        0     2574 2023-06-16 21:24:27.546614 servicex-3.0.0a1/README.md
+-rw-r--r--   0        0        0     1070 2023-06-16 21:25:15.907111 servicex-3.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1535 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/__init__.py
+-rw-r--r--   0        0        0       96 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/_version.py
+-rw-r--r--   0        0        0     1535 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/__init__.py
+-rw-r--r--   0        0        0     3157 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/cache.py
+-rw-r--r--   0        0        0     1776 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/cli_options.py
+-rw-r--r--   0        0        0     2643 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/main.py
+-rw-r--r--   0        0        0     5414 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/app/transforms.py
+-rw-r--r--   0        0        0     3362 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/configuration.py
+-rw-r--r--   0        0        0    15385 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/dataset.py
+-rw-r--r--   0        0        0     1984 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/dataset_group.py
+-rw-r--r--   0        0        0     2700 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/dataset_identifier.py
+-rw-r--r--   0        0        0     1535 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/func_adl/__init__.py
+-rw-r--r--   0        0        0     9275 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/func_adl/func_adl_dataset.py
+-rw-r--r--   0        0        0     4013 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/func_adl/util.py
+-rw-r--r--   0        0        0     4184 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/minio_adpater.py
+-rw-r--r--   0        0        0     4410 2023-06-16 21:24:27.546614 servicex-3.0.0a1/servicex_client/models.py
+-rw-r--r--   0        0        0     3111 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/python_dataset.py
+-rw-r--r--   0        0        0     4405 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/query_cache.py
+-rw-r--r--   0        0        0     5374 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/servicex_adapter.py
+-rw-r--r--   0        0        0     5031 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/servicex_client.py
+-rw-r--r--   0        0        0     1692 2023-06-16 21:24:27.550614 servicex-3.0.0a1/servicex_client/types.py
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 servicex-3.0.0a1/setup.py
+-rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 servicex-3.0.0a1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `servicex-2.6b1/servicex/servicex_python_function.py` & `servicex-3.0.0a1/servicex_client/python_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,70 @@
-#  Copyright (c) 2022 , IRIS-HEP
-#   All rights reserved.
-#
-#   Redistribution and use in source and binary forms, with or without
-#   modification, are permitted provided that the following conditions are met:
-#
-#   * Redistributions of source code must retain the above copyright notice, this
-#     list of conditions and the following disclaimer.
-#
-#   * Redistributions in binary form must reproduce the above copyright notice,
-#     this list of conditions and the following disclaimer in the documentation
-#     and/or other materials provided with the distribution.
-#
-#   * Neither the name of the copyright holder nor the names of its
-#     contributors may be used to endorse or promote products derived from
-#     this software without specific prior written permission.
-#
-#   THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-#   AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-#   IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-#   DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-#   FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-#   DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-#   SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-#   CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-#   OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-#   OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
-
+# Copyright (c) 2022, IRIS-HEP
+# All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
+# * Redistributions of source code must retain the above copyright notice, this
+#   list of conditions and the following disclaimer.
 #
-#
-#
+# * Redistributions in binary form must reproduce the above copyright notice,
+#   this list of conditions and the following disclaimer in the documentation
+#   and/or other materials provided with the distribution.
+#
+# * Neither the name of the copyright holder nor the names of its
+#   contributors may be used to endorse or promote products derived from
+#   this software without specific prior written permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 import inspect
+import typing
 from base64 import b64encode
-from pathlib import Path
-from typing import Optional, List, Callable
-
-from servicex import ServiceXDataset
-
 
-class ServiceXPythonFunction(ServiceXDataset):
-    @staticmethod
-    def _encode_function(selection_function: Callable):
-        return b64encode(inspect.getsource(selection_function).encode("utf-8")).decode(
-            "utf-8"
-        )
-
-    async def get_data_rootfiles_async(
-        self, selection_function: Callable, title: Optional[str] = None
-    ) -> List[Path]:
-        return await self._file_return(
-            self._encode_function(selection_function), "root-file", title
-        )
-
-    async def get_data_awkward_async(
-        self, selection_function: Callable, title: Optional[str] = None
-    ):
-        return self._converter.combine_awkward(
-            await self._data_return(
-                self._encode_function(selection_function),
-                lambda f: self._converter.convert_to_awkward(f),
-                title,
-            )
-        )
+from servicex_client.configuration import Configuration
+from servicex_client.dataset import Dataset
+from servicex_client.models import ResultFormat
+from servicex_client.query_cache import QueryCache
+from servicex_client.servicex_adapter import ServiceXAdapter
+from servicex_client.types import DID
+
+
+class PythonDataset(Dataset):
+
+    def __init__(self, dataset_identifier: DID,
+                 sx_adapter: ServiceXAdapter = None,
+                 title: str = "ServiceX Client",
+                 codegen: str = None,
+                 config: Configuration = None,
+                 query_cache: QueryCache = None,
+                 result_format: typing.Optional[ResultFormat] = None
+                 ):
+        super().__init__(dataset_identifier=dataset_identifier,
+                         title=title,
+                         codegen=codegen,
+                         sx_adapter=sx_adapter,
+                         config=config,
+                         query_cache=query_cache,
+                         result_format=result_format)
+
+        self.python_function = None
+
+    def with_uproot_function(self, f: typing.Callable) -> Dataset:
+        self.python_function = f
+        return self
+
+    def generate_selection_string(self) -> str:
+        if not self.python_function:
+            raise ValueError("You must provide a python function using with_uproot_function")
+
+        return b64encode(inspect.getsource(self.python_function)
+                         .encode("utf-8"))\
+            .decode("utf-8")
```

