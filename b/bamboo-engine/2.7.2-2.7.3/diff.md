# Comparing `tmp/bamboo-engine-2.7.2.tar.gz` & `tmp/bamboo-engine-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bamboo-engine-2.7.2.tar", max compression
+gzip compressed data, was "bamboo-engine-2.7.3.tar", max compression
```

## Comparing `bamboo-engine-2.7.2.tar` & `bamboo-engine-2.7.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1069 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/LICENSE
--rw-r--r--   0        0        0      781 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/__init__.py
--rw-r--r--   0        0        0      768 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/__version__.py
--rw-r--r--   0        0        0    20710 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/api.py
--rw-r--r--   0        0        0      805 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/__init__.py
--rw-r--r--   0        0        0     6627 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/builder.py
--rw-r--r--   0        0        0      866 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/flow/__init__.py
--rw-r--r--   0        0        0     2044 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/flow/activity.py
--rw-r--r--   0        0        0     2379 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/flow/base.py
--rw-r--r--   0        0        0     3546 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/flow/data.py
--rw-r--r--   0        0        0     1285 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/flow/event.py
--rw-r--r--   0        0        0     2166 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/builder/flow/gateway.py
--rw-r--r--   0        0        0     1650 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/config.py
--rw-r--r--   0        0        0     5573 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/context.py
--rw-r--r--   0        0        0    45316 2023-06-02 06:24:46.463513 bamboo-engine-2.7.2/bamboo_engine/engine.py
--rw-r--r--   0        0        0      853 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/__init__.py
--rw-r--r--   0        0        0    42073 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/interfaces.py
--rw-r--r--   0        0        0      898 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/models/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/models/event.py
--rw-r--r--   0        0        0     4795 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/models/handler.py
--rw-r--r--   0        0        0     9183 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/models/interrupt.py
--rw-r--r--   0        0        0     6627 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/models/node.py
--rw-r--r--   0        0        0    11555 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/eri/models/runtime.py
--rw-r--r--   0        0        0     1742 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/exceptions.py
--rw-r--r--   0        0        0     5934 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handler.py
--rw-r--r--   0        0        0     1407 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/__init__.py
--rw-r--r--   0        0        0     8106 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/conditional_parallel_gateway.py
--rw-r--r--   0        0        0     2282 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/converge_gateway.py
--rw-r--r--   0        0        0     7561 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/empty_end_event.py
--rw-r--r--   0        0        0     4946 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/empty_start_event.py
--rw-r--r--   0        0        0     7718 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/exclusive_gateway.py
--rw-r--r--   0        0        0     4399 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/executable_end_event.py
--rw-r--r--   0        0        0     3318 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/parallel_gateway.py
--rw-r--r--   0        0        0    22403 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/service_activity.py
--rw-r--r--   0        0        0     6642 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/handlers/subprocess.py
--rw-r--r--   0        0        0     9442 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/interrupt.py
--rw-r--r--   0        0        0     1810 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/local.py
--rw-r--r--   0        0        0    12434 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/metrics.py
--rw-r--r--   0        0        0     2214 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/states.py
--rw-r--r--   0        0        0      825 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/template/__init__.py
--rw-r--r--   0        0        0     1747 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/template/sandbox.py
--rw-r--r--   0        0        0     6822 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/template/template.py
--rw-r--r--   0        0        0      800 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/__init__.py
--rw-r--r--   0        0        0      892 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/boolrule/__init__.py
--rw-r--r--   0        0        0     9057 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/boolrule/boolrule.py
--rw-r--r--   0        0        0     1834 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/collections.py
--rw-r--r--   0        0        0      936 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/constants.py
--rw-r--r--   0        0        0    15396 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/graph.py
--rw-r--r--   0        0        0      879 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/host.py
--rw-r--r--   0        0        0     2092 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/mako_safety.py
--rw-r--r--   0        0        0      778 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/__init__.py
--rw-r--r--   0        0        0     2361 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/checker.py
--rw-r--r--   0        0        0     1803 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/code_extract.py
--rw-r--r--   0        0        0      805 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/exceptions.py
--rw-r--r--   0        0        0     4159 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/visitors.py
--rw-r--r--   0        0        0      884 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/object.py
--rw-r--r--   0        0        0     2064 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/utils/string.py
--rw-r--r--   0        0        0      801 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/validator/__init__.py
--rw-r--r--   0        0        0     1919 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/validator/api.py
--rw-r--r--   0        0        0     2770 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/validator/connection.py
--rw-r--r--   0        0        0    16793 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/validator/gateway.py
--rw-r--r--   0        0        0     2507 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/validator/rules.py
--rw-r--r--   0        0        0     2847 2023-06-02 06:24:46.467513 bamboo-engine-2.7.2/bamboo_engine/validator/utils.py
--rw-r--r--   0        0        0      742 2023-06-02 06:24:46.479513 bamboo-engine-2.7.2/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 bamboo-engine-2.7.2/setup.py
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 bamboo-engine-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/LICENSE
+-rw-r--r--   0        0        0      781 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/__init__.py
+-rw-r--r--   0        0        0      768 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/__version__.py
+-rw-r--r--   0        0        0    20711 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/api.py
+-rw-r--r--   0        0        0      805 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/__init__.py
+-rw-r--r--   0        0        0     6627 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/builder.py
+-rw-r--r--   0        0        0      866 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/__init__.py
+-rw-r--r--   0        0        0     2044 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/activity.py
+-rw-r--r--   0        0        0     2379 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/base.py
+-rw-r--r--   0        0        0     3546 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/data.py
+-rw-r--r--   0        0        0     1285 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/event.py
+-rw-r--r--   0        0        0     2166 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/gateway.py
+-rw-r--r--   0        0        0     1650 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/config.py
+-rw-r--r--   0        0        0     5573 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/context.py
+-rw-r--r--   0        0        0    45316 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/engine.py
+-rw-r--r--   0        0        0      853 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/__init__.py
+-rw-r--r--   0        0        0    42073 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/interfaces.py
+-rw-r--r--   0        0        0      898 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/event.py
+-rw-r--r--   0        0        0     4795 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/handler.py
+-rw-r--r--   0        0        0     9183 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/interrupt.py
+-rw-r--r--   0        0        0     6627 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/node.py
+-rw-r--r--   0        0        0    11555 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/runtime.py
+-rw-r--r--   0        0        0     1742 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/exceptions.py
+-rw-r--r--   0        0        0     5934 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handler.py
+-rw-r--r--   0        0        0     1407 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/__init__.py
+-rw-r--r--   0        0        0     8106 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/conditional_parallel_gateway.py
+-rw-r--r--   0        0        0     2282 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/converge_gateway.py
+-rw-r--r--   0        0        0     7561 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/empty_end_event.py
+-rw-r--r--   0        0        0     4946 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/empty_start_event.py
+-rw-r--r--   0        0        0     7718 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/exclusive_gateway.py
+-rw-r--r--   0        0        0     4399 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/executable_end_event.py
+-rw-r--r--   0        0        0     3318 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/parallel_gateway.py
+-rw-r--r--   0        0        0    22403 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/service_activity.py
+-rw-r--r--   0        0        0     6642 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/subprocess.py
+-rw-r--r--   0        0        0     9442 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/interrupt.py
+-rw-r--r--   0        0        0     1810 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/local.py
+-rw-r--r--   0        0        0    12434 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/metrics.py
+-rw-r--r--   0        0        0     2214 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/states.py
+-rw-r--r--   0        0        0      825 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/template/__init__.py
+-rw-r--r--   0        0        0     1747 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/template/sandbox.py
+-rw-r--r--   0        0        0     6822 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/template/template.py
+-rw-r--r--   0        0        0      800 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/utils/__init__.py
+-rw-r--r--   0        0        0      892 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/__init__.py
+-rw-r--r--   0        0        0     9057 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/boolrule.py
+-rw-r--r--   0        0        0     1834 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/collections.py
+-rw-r--r--   0        0        0      936 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/constants.py
+-rw-r--r--   0        0        0    15396 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/graph.py
+-rw-r--r--   0        0        0      879 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/host.py
+-rw-r--r--   0        0        0     2092 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_safety.py
+-rw-r--r--   0        0        0      778 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/__init__.py
+-rw-r--r--   0        0        0     2361 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/checker.py
+-rw-r--r--   0        0        0     1803 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/code_extract.py
+-rw-r--r--   0        0        0      805 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/exceptions.py
+-rw-r--r--   0        0        0     4159 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/visitors.py
+-rw-r--r--   0        0        0      884 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/object.py
+-rw-r--r--   0        0        0     2064 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/string.py
+-rw-r--r--   0        0        0      801 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/__init__.py
+-rw-r--r--   0        0        0     1919 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/api.py
+-rw-r--r--   0        0        0     2770 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/connection.py
+-rw-r--r--   0        0        0    16793 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/gateway.py
+-rw-r--r--   0        0        0     2507 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/rules.py
+-rw-r--r--   0        0        0     2847 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/utils.py
+-rw-r--r--   0        0        0      742 2023-06-16 07:00:31.828582 bamboo-engine-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 bamboo-engine-2.7.3/setup.py
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 bamboo-engine-2.7.3/PKG-INFO
```

### Comparing `bamboo-engine-2.7.2/LICENSE` & `bamboo-engine-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/__version__.py` & `bamboo-engine-2.7.3/bamboo_engine/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-__version__ = "2.7.2"
+__version__ = "2.7.3"
```

### Comparing `bamboo-engine-2.7.2/bamboo_engine/api.py` & `bamboo-engine-2.7.3/bamboo_engine/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
     :param pipeline_id: 流程 ID
     :type pipeline_id: str
     :return: 执行结果
     :rtype: EngineAPIResult
     """
 
     return {
-        "contex_values": runtime.get_context(pipeline_id),
+        "context_values": runtime.get_context(pipeline_id),
         "processes": runtime.get_process_info_with_root_pipeline(pipeline_id),
     }
 
 
 @_ensure_return_api_result
 def get_node_debug_info(runtime: EngineRuntimeInterface, node_id: str):
     """
```

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/builder.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/builder.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/flow/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/flow/activity.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/flow/activity.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/flow/base.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/flow/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/flow/data.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/flow/data.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/flow/event.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/flow/event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/builder/flow/gateway.py` & `bamboo-engine-2.7.3/bamboo_engine/builder/flow/gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/config.py` & `bamboo-engine-2.7.3/bamboo_engine/config.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/context.py` & `bamboo-engine-2.7.3/bamboo_engine/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/engine.py` & `bamboo-engine-2.7.3/bamboo_engine/engine.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/interfaces.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/interfaces.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/models/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/models/event.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/models/event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/models/handler.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/models/handler.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/models/interrupt.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/models/interrupt.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/models/node.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/models/node.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/eri/models/runtime.py` & `bamboo-engine-2.7.3/bamboo_engine/eri/models/runtime.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/exceptions.py` & `bamboo-engine-2.7.3/bamboo_engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handler.py` & `bamboo-engine-2.7.3/bamboo_engine/handler.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/conditional_parallel_gateway.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/conditional_parallel_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/converge_gateway.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/converge_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/empty_end_event.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/empty_end_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/empty_start_event.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/empty_start_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/exclusive_gateway.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/exclusive_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/executable_end_event.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/executable_end_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/parallel_gateway.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/parallel_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/service_activity.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/service_activity.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/handlers/subprocess.py` & `bamboo-engine-2.7.3/bamboo_engine/handlers/subprocess.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/interrupt.py` & `bamboo-engine-2.7.3/bamboo_engine/interrupt.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/local.py` & `bamboo-engine-2.7.3/bamboo_engine/local.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/metrics.py` & `bamboo-engine-2.7.3/bamboo_engine/metrics.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/states.py` & `bamboo-engine-2.7.3/bamboo_engine/states.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/template/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/template/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/template/sandbox.py` & `bamboo-engine-2.7.3/bamboo_engine/template/sandbox.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/template/template.py` & `bamboo-engine-2.7.3/bamboo_engine/template/template.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/boolrule/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/boolrule/boolrule.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/boolrule.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/collections.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/collections.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/constants.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/constants.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/graph.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/graph.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/host.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/host.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/mako_safety.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/mako_safety.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/checker.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/checker.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/code_extract.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/code_extract.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/exceptions.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/mako_utils/visitors.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/visitors.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/object.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/object.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/utils/string.py` & `bamboo-engine-2.7.3/bamboo_engine/utils/string.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/validator/__init__.py` & `bamboo-engine-2.7.3/bamboo_engine/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/validator/api.py` & `bamboo-engine-2.7.3/bamboo_engine/validator/api.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/validator/connection.py` & `bamboo-engine-2.7.3/bamboo_engine/validator/connection.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/validator/gateway.py` & `bamboo-engine-2.7.3/bamboo_engine/validator/gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/validator/rules.py` & `bamboo-engine-2.7.3/bamboo_engine/validator/rules.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/bamboo_engine/validator/utils.py` & `bamboo-engine-2.7.3/bamboo_engine/validator/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.2/pyproject.toml` & `bamboo-engine-2.7.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bamboo-engine"
-version = "2.7.2"
+version = "2.7.3"
 description = "Bamboo-engine is a general-purpose workflow engine"
 authors = ["homholueng <homholueng@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">= 3.6, < 4"
 Werkzeug = "^1.0.0"
```

### Comparing `bamboo-engine-2.7.2/setup.py` & `bamboo-engine-2.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ['Mako>=1.1.4,<2.0.0',
  'Werkzeug>=1.0.0,<2.0.0',
  'prometheus-client>=0.9.0,<0.10.0',
  'pyparsing>=2.2.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bamboo-engine',
-    'version': '2.7.2',
+    'version': '2.7.3',
     'description': 'Bamboo-engine is a general-purpose workflow engine',
     'long_description': 'None',
     'author': 'homholueng',
     'author_email': 'homholueng@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bamboo-engine-2.7.2/PKG-INFO` & `bamboo-engine-2.7.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboo-engine
-Version: 2.7.2
+Version: 2.7.3
 Summary: Bamboo-engine is a general-purpose workflow engine
 License: MIT
 Author: homholueng
 Author-email: homholueng@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

