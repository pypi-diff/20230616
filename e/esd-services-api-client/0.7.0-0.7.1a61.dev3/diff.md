# Comparing `tmp/esd_services_api_client-0.7.0.tar.gz` & `tmp/esd_services_api_client-0.7.1a61.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-0.7.0.tar", max compression
+gzip compressed data, was "esd_services_api_client-0.7.1a61.dev3.tar", max compression
```

## Comparing `esd_services_api_client-0.7.0.tar` & `esd_services_api_client-0.7.1a61.dev3.tar`

### file list

```diff
@@ -1,26 +1,22 @@
--rw-r--r--   0        0        0    10693 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/LICENSE
--rw-r--r--   0        0        0      120 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/README.md
--rw-r--r--   0        0        0      598 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       22 2023-05-03 15:02:41.141281 esd_services_api_client-0.7.0/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      791 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/_api_versions.py
--rw-r--r--   0        0        0     6934 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/_connector.py
--rw-r--r--   0        0        0     5703 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/arcane/_models.py
--rw-r--r--   0        0        0      743 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0     2666 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/beast/_auth.py
--rw-r--r--   0        0        0    10369 2023-05-03 15:02:16.213182 esd_services_api_client-0.7.0/esd_services_api_client/beast/_connector.py
--rw-r--r--   0        0        0     9442 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/beast/_models.py
--rw-r--r--   0        0        0     2221 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      780 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     5214 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      976 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8272 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1736 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_helpers.py
--rw-r--r--   0        0        0     3105 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      598 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      787 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      832 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0     9493 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4025 2023-05-03 15:02:16.217182 esd_services_api_client-0.7.0/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0      949 2023-05-03 15:02:41.141281 esd_services_api_client-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 esd_services_api_client-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/LICENSE
+-rw-r--r--   0        0        0      111 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/README.md
+-rw-r--r--   0        0        0      598 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-16 13:04:12.476672 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      743 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0     2666 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_auth.py
+-rw-r--r--   0        0        0    10369 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_connector.py
+-rw-r--r--   0        0        0     9442 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_models.py
+-rw-r--r--   0        0        0     2221 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      780 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     5214 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      976 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8272 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1736 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_helpers.py
+-rw-r--r--   0        0        0     3105 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      598 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      787 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0    12015 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4025 2023-06-16 13:03:51.676208 esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0      958 2023-06-16 13:04:12.476672 esd_services_api_client-0.7.1a61.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 esd_services_api_client-0.7.1a61.dev3/PKG-INFO
```

### Comparing `esd_services_api_client-0.7.0/LICENSE` & `esd_services_api_client-0.7.1a61.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/__init__.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/arcane/__init__.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-from esd_services_api_client.arcane._models import *
-from esd_services_api_client.arcane._connector import *
-from esd_services_api_client.arcane._api_versions import *
+from esd_services_api_client.boxer._models import *
+from esd_services_api_client.boxer._connector import *
+from esd_services_api_client.boxer._auth import *
```

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/beast/_auth.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/beast/_connector.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/beast/_models.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/beast/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/boxer/README.md` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
- Import index.
-"""
+"""init file"""
 
 #  Copyright (c) 2023. ECCO Sneaks & Data
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
@@ -13,10 +11,10 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-from esd_services_api_client.boxer._models import *
-from esd_services_api_client.boxer._connector import *
-from esd_services_api_client.boxer._auth import *
+from esd_services_api_client.crystal._connector import *
+from esd_services_api_client.crystal._models import *
+from esd_services_api_client.crystal._api_versions import *
```

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_helpers.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_helpers.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/common/__init__.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_api_versions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""init file"""
-
+"""
+API versioning for arcane connector
+"""
 #  Copyright (c) 2023. ECCO Sneaks & Data
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -11,10 +12,17 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-from esd_services_api_client.crystal._connector import *
-from esd_services_api_client.crystal._models import *
-from esd_services_api_client.crystal._api_versions import *
+from enum import Enum
+
+
+class ApiVersion(Enum):
+    """
+    API Versions
+    V1_2 - Boxer token authentication and updated API for run submission and result read
+    """
+
+    V1_2 = "v1.2"
```

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_connector.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,25 +19,27 @@
 import json
 from argparse import Namespace, ArgumentParser
 from datetime import timedelta
 from typing import Dict, Optional, Type, TypeVar, List
 
 from adapta.logs import SemanticLogger
 from adapta.storage.models.format import SerializationFormat
-from adapta.utils import session_with_retries
+from adapta.utils import session_with_retries, doze
+from adapta.utils.concurrent_task_runner import ConcurrentTaskRunner, Executable
 from requests.auth import AuthBase
 
 from esd_services_api_client.boxer import BoxerTokenAuth
 from esd_services_api_client.crystal._api_versions import ApiVersion
 from esd_services_api_client.crystal._models import (
     RequestResult,
     AlgorithmRunResult,
     CrystalEntrypointArguments,
     AlgorithmRequest,
     AlgorithmConfiguration,
+    RequestLifeCycleStage,
 )
 
 T = TypeVar("T")  # pylint: disable=C0103
 
 
 def add_crystal_args(parser: Optional[ArgumentParser] = None) -> ArgumentParser:
     """
@@ -99,14 +101,20 @@
         self._logger = logger
         if isinstance(auth, BoxerTokenAuth):
             assert (
                 api_version == ApiVersion.V1_2
             ), "Cannot use BoxerTokenAuth with Crystal API versions prior to 1.2."
 
         self.http.auth = auth
+        self._finished_statuses = [
+            RequestLifeCycleStage.COMPLETED,
+            RequestLifeCycleStage.FAILED,
+            RequestLifeCycleStage.SCHEDULING_TIMEOUT,
+            RequestLifeCycleStage.DEADLINE_EXCEEDED,
+        ]
 
     @classmethod
     def create_anonymous(
         cls,
         base_url: str,
         logger: Optional[SemanticLogger] = None,
         api_version: ApiVersion = ApiVersion.V1_2,
@@ -173,14 +181,19 @@
         """
         Retrieves a submitted Crystal job.
 
         :param run_id: Request identifier assigned to the job by Crystal.
         :param algorithm: Name of an algorithm.
         """
 
+        return self._retrieve_run(run_id=run_id, algorithm=algorithm)
+
+    def _retrieve_run(
+        self, run_id: str, algorithm: Optional[str] = None
+    ) -> RequestResult:
         def get_api_path() -> str:
             if self._api_version == ApiVersion.V1_2:
                 return f"{self.base_url}/algorithm/{self._api_version.value}/results/{algorithm}/requests/{run_id}"
 
             raise ValueError(f"Unsupported API version {self._api_version}")
 
         response = self.http.get(url=get_api_path())
@@ -198,14 +211,19 @@
         """
         Retrieves all submitted Crystal jobs with matching tags.
 
         :param tag: A request tag assigned by a client.
         :param algorithm: Name of an algorithm.
         """
 
+        return self._retrieve_runs(tag=tag, algorithm=algorithm)
+
+    def _retrieve_runs(
+        self, tag: str, algorithm: Optional[str] = None
+    ) -> List[RequestResult]:
         def get_api_path() -> str:
             if self._api_version == ApiVersion.V1_2:
                 return f"{self.base_url}/algorithm/{self._api_version.value}/results/{algorithm}/tags/{tag}"
 
             raise ValueError(f"Unsupported API version {self._api_version}")
 
         response = self.http.get(url=get_api_path())
@@ -276,7 +294,62 @@
         return serialization_format().deserialize(http_response.content)
 
     def dispose(self) -> None:
         """
         Gracefully dispose object.
         """
         self.http.close()
+
+    def await_tagged_runs(
+        self, algorithm: str, tags: List[str]
+    ) -> Dict[str, RequestResult]:
+        """
+        Await for a list of tagged Crystal jobs to finish.
+
+        :param algorithm: Name of an algorithm.
+        :param tags: Request tags assigned to the jobs by a client.
+        """
+
+        results = {}
+        unfinished_tasks = []
+        runs = [self._retrieve_runs(tag=tag, algorithm=algorithm) for tag in tags]
+        for tag_runs in runs:
+            for run in tag_runs:
+                if run.status not in self._finished_statuses:
+                    unfinished_tasks.append(run.run_id)
+                else:
+                    results[run.run_id] = run
+
+        return {
+            **results,
+            **self._await_runs(algorithm=algorithm, run_ids=unfinished_tasks),
+        }
+
+    def await_runs(
+        self, algorithm: str, run_ids: List[str]
+    ) -> Dict[str, RequestResult]:
+        """
+        Await for a list of submitted Crystal jobs to finish.
+
+        :param algorithm: Name of an algorithm.
+        :param run_ids: Request identifiers assigned to the jobs by Crystal.
+        """
+        return self._await_runs(algorithm=algorithm, run_ids=run_ids)
+
+    def _await_runs(
+        self, algorithm: str, run_ids: List[str]
+    ) -> Dict[str, RequestResult]:
+        def await_run(run_id: str) -> RequestResult:
+            while True:
+                result = self._retrieve_run(run_id=run_id, algorithm=algorithm)
+                if result.status in self._finished_statuses:
+                    return result
+                doze(1)
+
+        ctr = ConcurrentTaskRunner(
+            func_list=[
+                Executable(func=await_run, alias=run_id, args=[run_id])
+                for run_id in run_ids
+            ]
+        )
+
+        return ctr.eager()
```

### Comparing `esd_services_api_client-0.7.0/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-0.7.1a61.dev3/esd_services_api_client/crystal/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.7.0/pyproject.toml` & `esd_services_api_client-0.7.1a61.dev3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "0.7.0"
+version = "v0.7.1a61.dev3"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
```

### Comparing `esd_services_api_client-0.7.0/PKG-INFO` & `esd_services_api_client-0.7.1a61.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 0.7.0
+Version: 0.7.1a61.dev3
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
@@ -22,12 +22,11 @@
 Requires-Dist: pyjwt (>=2.4.0,<2.5.0)
 Project-URL: Repository, https://github.com/SneaksAndData/esd-services-api-client
 Description-Content-Type: text/markdown
 
 # ESD services Api client
 
 This repository contains connectors to internal services:
-- Arcane
 - Beast
 - Boxer
 - Crystal
```

