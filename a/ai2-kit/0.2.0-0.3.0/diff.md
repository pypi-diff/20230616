# Comparing `tmp/ai2_kit-0.2.0.tar.gz` & `tmp/ai2_kit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.2.0.tar", max compression
+gzip compressed data, was "ai2_kit-0.3.0.tar", max compression
```

## Comparing `ai2_kit-0.2.0.tar` & `ai2_kit-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.2.0/LICENSE
--rw-r--r--   0        0        0     1170 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     3327 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7717 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/executor.py
--rw-r--r--   0        0        0     1074 2023-02-22 05:58:23.102960 ai2_kit-0.2.0/ai2_kit/core/future.py
--rw-r--r--   0        0        0     2995 2023-02-17 02:09:28.820341 ai2_kit-0.2.0/ai2_kit/core/job.py
--rw-r--r--   0        0        0      118 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/core/log.py
--rw-r--r--   0        0        0     8346 2023-03-02 05:16:23.680695 ai2_kit-0.2.0/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2358 2023-02-27 06:41:41.002117 ai2_kit-0.2.0/ai2_kit/core/script.py
--rw-r--r--   0        0        0     1949 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     2232 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/cll.py
--rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.2.0/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     8122 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     4121 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/data_helper.py
--rw-r--r--   0        0        0     6523 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    15627 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     3173 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0      949 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/tools/__init__.py
--rw-r--r--   0        0        0      239 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/tools/demo.yaml
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     7426 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     7755 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/workflow/ec_fep.py
--rw-r--r--   0        0        0      821 2023-06-13 03:51:03.222343 ai2_kit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 ai2_kit-0.2.0/setup.py
--rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 ai2_kit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1205 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     3327 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     7731 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0     1074 2023-02-22 05:58:23.102960 ai2_kit-0.3.0/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     2995 2023-02-17 02:09:28.820341 ai2_kit-0.3.0/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      118 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     8476 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2358 2023-02-27 06:41:41.002117 ai2_kit-0.3.0/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     2264 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     2232 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/domain/cll.py
+-rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.0/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     8202 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     4121 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/domain/data_helper.py
+-rw-r--r--   0        0        0     6797 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0    15572 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     3173 2023-06-15 07:40:02.514859 ai2_kit-0.3.0/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     1465 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      744 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     7426 2023-06-15 09:06:34.322595 ai2_kit-0.3.0/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     8519 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      821 2023-06-16 03:38:30.319717 ai2_kit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 ai2_kit-0.3.0/PKG-INFO
```

### Comparing `ai2_kit-0.2.0/LICENSE` & `ai2_kit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/README.md` & `ai2_kit-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,13 +28,14 @@
 
 ./ai2-kit --help
 ```
 
 ## Manuals
 
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
+* [ASE Toolkit](doc/manual/ase.md)
 * [CLL MLP Training Workflow](doc/manual/cll-workflow.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ## Tutorials
 
 ## Notebooks
```

### Comparing `ai2_kit-0.2.0/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.3.0/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/artifact.py` & `ai2_kit-0.3.0/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/checkpoint.py` & `ai2_kit-0.3.0/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/connector.py` & `ai2_kit-0.3.0/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/executor.py` & `ai2_kit-0.3.0/ai2_kit/core/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .queue_system import QueueSystemConfig, BaseQueueSystem, Slrum, Lsf
+from .queue_system import QueueSystemConfig, BaseQueueSystem, Slurm, Lsf
 from .job import JobFuture
 from .artifact import Artifact
 from .connector import SshConfig, BaseConnector, SshConnector, LocalConnector
 from .util import s_uuid
 from .log import get_logger
 
 logger = get_logger(__name__)
@@ -11,14 +11,15 @@
 from typing import Optional, Dict, List, TypeVar, Callable, Mapping
 from abc import ABC, abstractmethod
 from invoke import Result
 import os
 import shlex
 import base64
 import bz2
+import pickle
 import cloudpickle
 
 
 class BaseExecutorConfig(BaseModel):
     ssh: Optional[SshConfig]
     queue_system: QueueSystemConfig
     work_dir: str
@@ -95,15 +96,15 @@
     def from_config(cls, config: BaseExecutorConfig, name: str):
         if config.ssh:
             connector = SshConnector.from_config(config.ssh)
         else:
             connector = LocalConnector()
         queue_system = None
         if config.queue_system.slurm:
-            queue_system = Slrum()
+            queue_system = Slurm()
             queue_system.config = config.queue_system.slurm
         elif config.queue_system.lsf:
             queue_system = Lsf()
             queue_system.config = config.queue_system.lsf
         if queue_system is None:
             raise ValueError('Queue system config is missing!')
         queue_system.connector = connector
```

### Comparing `ai2_kit-0.2.0/ai2_kit/core/future.py` & `ai2_kit-0.3.0/ai2_kit/core/future.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/job.py` & `ai2_kit-0.3.0/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/queue_system.py` & `ai2_kit-0.3.0/ai2_kit/core/queue_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional, Dict
 from abc import ABC, abstractmethod
 import shlex
 import os
 import re
 import shortuuid
 import time
+import asyncio
 
 
 from .connector import BaseConnector
 from .log import get_logger
 from .job import JobFuture, JobState
 
 logger = get_logger(__name__)
@@ -102,15 +103,15 @@
                        cwd=cwd,
                        polling_interval=self.get_polling_interval() // 2,
                        )
         self._post_submit(job)
         return job
 
 
-class Slrum(BaseQueueSystem):
+class Slurm(BaseQueueSystem):
 
     config: QueueSystemConfig.Slurm
 
     _last_states: Optional[Dict[str, JobState]]
     _last_update_at: float = 0
 
     translate_table = {
@@ -268,25 +269,25 @@
     def cancel(self):
         self._queue_system.cancel(self._job_id)
 
     def done(self):
         return self.get_job_state().terminal
 
     def result(self, timeout: float = float('inf')) -> JobState:
+        return asyncio.run(self.async_result(timeout))
 
+    async def async_result(self, timeout: float = float('inf')) -> JobState:
         timeout_ts = time.time() + timeout
-
         while time.time() < timeout_ts:
             if self.done():
                 return self.get_job_state()
             else:
-                time.sleep(self._polling_interval)
+                await asyncio.sleep(self._polling_interval)
         else:
-            raise RuntimeError(
-                'Timeout of polling job: {}'.format(self._job_id))
+            raise RuntimeError(f'Timeout of polling job: {self._job_id}')
 
     def __repr__(self):
         return repr(dict(
             name=self._name,
             cwd=self._cwd,
             job_id=self._job_id,
             success_indicator=self._success_indicator,
```

### Comparing `ai2_kit-0.2.0/ai2_kit/core/resource_manager.py` & `ai2_kit-0.3.0/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/script.py` & `ai2_kit-0.3.0/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/core/util.py` & `ai2_kit-0.3.0/ai2_kit/core/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,17 +58,28 @@
 
 def s_uuid():
     """short uuid"""
     return shortuuid.uuid()
 
 
 def parse_cp2k_input(text: str):
-    parser = CP2KInputParserSimplified()
+    parser = CP2KInputParserSimplified(key_trafo=str.upper)
     return parser.parse(io.StringIO(text))
 
+def dict_nested_get(d: dict, keys: List[str]):
+    """get value from nested dict"""
+    for key in keys:
+        d = d[key]
+    return d
+
+def dict_nested_set(d: dict, keys: List[str], value):
+    """set value to nested dict"""
+    for key in keys[:-1]:
+        d = d[key]
+    d[keys[-1]] = value
 
 def sort_unique_str_list(l: List[str]) -> List[str]:
     """remove duplicate str and sort"""
     return list(sorted(set(l)))
 
 
 T = TypeVar('T')
```

### Comparing `ai2_kit-0.2.0/ai2_kit/domain/cll.py` & `ai2_kit-0.3.0/ai2_kit/domain/cll.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/domain/cp2k.py` & `ai2_kit-0.3.0/ai2_kit/domain/cp2k.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.script import BashScript, BashStep, BashTemplate
 from ai2_kit.core.job import GatherJobsFuture, retry_fn
 
 from ai2_kit.core.future import DummyFuture, IFuture, map_future
 
-from ai2_kit.core.util import merge_dict, parse_cp2k_input
+from ai2_kit.core.util import merge_dict, parse_cp2k_input, dict_nested_get, dict_nested_set
 from ai2_kit.core.log import get_logger
 
 from typing import List, Union
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 import copy
@@ -77,26 +77,31 @@
 
     # prepare input template
     if isinstance(input.config.input_template, str):
         input_template = parse_cp2k_input(input.config.input_template)
     else:
         input_template = copy.deepcopy(input.config.input_template)
 
-    # resolve artifacts resources in the input template
-    basic_set_file: str = input_template['FORCE_EVAL']['DFT']['BASIS_SET_FILE_NAME']
-    if basic_set_file.startswith('@'):
-        logger.info(f'resolve artifact {basic_set_file}')
-        input_template['FORCE_EVAL']['DFT']['BASIS_SET_FILE_NAME'] = \
-            ctx.resource_manager.resolve_artifact(basic_set_file[1:])[0].url
-
-    potential_file: str = input_template['FORCE_EVAL']['DFT']['POTENTIAL_FILE_NAME']
-    if potential_file.startswith('@'):
-        logger.info(f'resolve artifact {potential_file}')
-        input_template['FORCE_EVAL']['DFT']['POTENTIAL_FILE_NAME'] = \
-            ctx.resource_manager.resolve_artifact(potential_file[1:])[0].url
+    fields_with_artifact = [
+        ['FORCE_EVAL', 'DFT', 'BASIS_SET_FILE_NAME'],
+        ['FORCE_EVAL', 'DFT', 'POTENTIAL_FILE_NAME'],
+        ['FORCE_EVAL', 'DFT', 'XC', 'VDW_POTENTIAL', 'PAIR_POTENTIAL', 'PARAMETER', 'PARAMETER_FILE_NAME' ],
+    ]
+    for field_path in fields_with_artifact:
+        try :
+            field_value = dict_nested_get(input_template, field_path)
+            if isinstance(field_value, str) and field_value.startswith('@'):
+                logger.info(f'resolve artifact {field_value}')
+                dict_nested_set(
+                    input_template,
+                    field_path,
+                    ctx.resource_manager.resolve_artifact(field_value[1:])[0].url
+                )
+        except KeyError:
+            pass
 
     # resolve data files
     lammps_dump_files: List[Artifact] = []
     xyz_files: List[Artifact] = []
 
     # TODO: support POSCAR in the future
     # TODO: refactor the way of handling different file formats
```

### Comparing `ai2_kit-0.2.0/ai2_kit/domain/data_helper.py` & `ai2_kit-0.3.0/ai2_kit/domain/data_helper.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/domain/deepmd.py` & `ai2_kit-0.3.0/ai2_kit/domain/deepmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -110,15 +110,14 @@
     for i in range(input.config.model_num):
         # each model should be trained in its own task_dir
         task_dir = os.path.join(tasks_dir, str(i).zfill(3))
         executor.mkdir(task_dir)
 
         # create dp train input file
         # NOTE: dp v1 format is supported currently
-        # TODO: migrate to dp v2 format
         # TODO: support more params if it is necessary
 
         # ref: https://github.com/deepmodeling/dpgen2/blob/master/examples/ch4/param_CH4_deepmd-kit-2.1.1.json
         # ref: https://github.com/deepmodeling/dpgen2/blob/master/dpgen2/op/prep_dp_train.py
         # ref: https://github.com/deepmodeling/dpgen2/blob/master/dpgen2/op/run_dp_train.py
 
         dp_input = copy.deepcopy(input.config.input_template)
@@ -138,23 +137,32 @@
             discriptor['seed'] = _random_seed()
         dp_input['model']['fitting_net']['seed'] = _random_seed()
         dp_input['training']['seed'] = _random_seed()
 
         # set training data
         systems = [a.url for a in input.old_dataset + input.new_dataset]
         training['systems'] = systems
-
-        # set other params
-        dp_input['model']['type_map'] = input.type_map
         set_prefix: str = training.setdefault(
             'set_prefix', 'set')  # respect user input
         auto_prob_str = "prob_sys_size"
         training.setdefault('batch_size', 'auto')
         training['auto_prob_style'] = auto_prob_str
 
+        # v2 training data
+        training_data = {
+            'systems': training['systems'],
+            'set_prefix': training['set_prefix'],
+            'auto_prob_style': training['auto_prob_style'],
+            'batch_size': training['batch_size'],
+        }
+        training['training_data'] = training_data
+
+        # other params
+        dp_input['model']['type_map'] = input.type_map
+
         # write config to executor
         dp_input_text = json.dumps(dp_input, indent=2)
         dp_input_path = os.path.join(task_dir, DP_INPUT_FILE)
         executor.dump_text(dp_input_text, dp_input_path)
 
         # build script
         dp_cmd = ctx.config.dp_cmd
```

### Comparing `ai2_kit-0.2.0/ai2_kit/domain/lammps.py` & `ai2_kit-0.3.0/ai2_kit/domain/lammps.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,19 +186,18 @@
         executor.mkdir(os.path.join(lammps_task_dir, LAMMPS_TRAJ_DIR))  # create dump directory for lammps or else will get error
 
         if input.md_options:
             force_field_section = make_md_force_field_section(
                 models=[a.url for a in input.md_options.models],
             )
         elif input.fep_options:
-            logger.info('FEP mode is used, please remember to set LAMBDA_f in others variants')
             if 'LAMBDA_f' not in others_dict:
                 raise ValueError('LAMBDA_f must be set when using FEP mode!')
             # inject the following variables for FEP mode
-            others_dict['LAMBDA_i'] = '1 - v_LAMBDA_f'
+            others_dict['LAMBDA_i'] = '1-v_LAMBDA_f' # should not have space, or you must quote
             others_dict['plus'] = 1
             others_dict['minus'] = -1
             force_field_section = make_fep_force_field_section(
                 neu_models=[a.url for a in input.fep_options.neu_models],
                 red_models=[a.url for a in input.fep_options.red_models],
             )
         else:
```

### Comparing `ai2_kit-0.2.0/ai2_kit/domain/selector.py` & `ai2_kit-0.3.0/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/main.py` & `ai2_kit-0.3.0/ai2_kit/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,64 @@
 from fire import Fire
-from ai2_kit.workflow.cll_mlp import cll_train_mlp
-from ai2_kit.workflow.ec_fep import fep_train_mlp
-from ai2_kit.algorithm import proton_transfer
 
 
 class Group:
-
     def __init__(self, items: dict, doc: str = '') -> None:
         self.__doc__ = doc
         self.__dict__.update(items)
 
 
-# TODO: use lazy loading to speed up the startup time
-kit = Group({
-    'workflow': Group({
-        'cll-mlp-training': cll_train_mlp,
-        'fep-mlp-training': fep_train_mlp,
+class ProtonTransferGroup:
+    @property
+    def analyze(self):
+        from ai2_kit.algorithm import proton_transfer
+        return proton_transfer.proton_transfer_detection
+
+    @property
+    def visualize(self):
+        from ai2_kit.algorithm import proton_transfer
+        return proton_transfer.visualize_transfer
+
+    @property
+    def show_transfer_paths(self):
+        from ai2_kit.algorithm import proton_transfer
+        return proton_transfer.analysis_transfer_paths
+
+    @property
+    def show_type_change(self):
+        from ai2_kit.algorithm import proton_transfer
+        return proton_transfer.detect_type_change
+
+
+class WorkflowGroup:
+    @property
+    def cll_mlp_training(self):
+        from ai2_kit.workflow.cll_mlp import cll_train_mlp
+        return cll_train_mlp
+
+    @property
+    def fep_mlp_training(self):
+        from ai2_kit.workflow.fep_mlp import fep_train_mlp
+        return fep_train_mlp
+
+class ToolGroup:
+
+    @property
+    def ase(self):
+        from ai2_kit.tool.ase import AseHelper
+        return AseHelper
 
-    }),
+
+kit = Group({
+    'workflow': WorkflowGroup(),
     'algorithm': Group({
-        'proton-transfer': Group({
-            'analyze': proton_transfer.proton_transfer_detection,
-            'visualize': proton_transfer.visualize_transfer,
-            'show-transfer-paths': proton_transfer.analysis_transfer_paths,
-            'show-type-change': proton_transfer.detect_type_change,
-        })
+        'proton-transfer': ProtonTransferGroup(),
     }),
+    'tool': ToolGroup(),
 }, doc="Welcome to use ai2-kit!")
 
 
-
 def main():
     Fire(kit)
 
 if __name__ == '__main__':
     main()
```

### Comparing `ai2_kit-0.2.0/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.3.0/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.2.0/ai2_kit/workflow/ec_fep.py` & `ai2_kit-0.3.0/ai2_kit/workflow/fep_mlp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-from ai2_kit.core.executor import BaseExecutorConfig, ExecutorManager
+from ai2_kit.core.executor import BaseExecutorConfig
 from ai2_kit.core.artifact import ArtifactMap
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.util import load_yaml_files
-from ai2_kit.domain import deepmd
-from ai2_kit.domain import lammps
-from ai2_kit.domain import selector
-from ai2_kit.domain import cp2k
-from ai2_kit.domain import constant as const
+from ai2_kit.core.resource_manager import ResourceManager
+from ai2_kit.domain import (
+    deepmd,
+    lammps,
+    selector,
+    cp2k,
+    constant as const,
+    updater,
+    cll,
+)
 
 from pydantic import BaseModel
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Any
 from fire import Fire
 
+import copy
+import itertools
 import os
 
 logger = get_logger(__name__)
 
 
 class FepExecutorConfig(BaseExecutorConfig):
     class Context(BaseModel):
@@ -23,178 +30,212 @@
         deepmd: deepmd.GenericDeepmdContextConfig
         lammps: lammps.GenericLammpsContextConfig
         cp2k: cp2k.GenericCp2kContextConfig
 
     context: Context
 
 
-class FepConfig(BaseModel):
-    class Workflow(BaseModel):
-        class General(BaseModel):
-            type_map: List[str]
-            mass_map: List[float]
-            max_iters: int = 10
-
-        class Branch(BaseModel):
-            deepmd: deepmd.GenericDeepmdInputConfig
-            cp2k: cp2k.GenericCp2kInputConfig
-            threshold: selector.ThresholdSelectorInputConfig
-
-        general: General
-        neu: Branch
-        red: Branch
-        lammps: lammps.GenericLammpsInputConfig
+class WorkflowConfig(BaseModel):
+    class General(BaseModel):
+        type_map: List[str]
+        mass_map: List[float]
+        max_iters: int = 10
+
+    class Branch(BaseModel):
+        deepmd: deepmd.GenericDeepmdInputConfig
+        cp2k: cp2k.GenericCp2kInputConfig
+        threshold: selector.ThresholdSelectorInputConfig
+
+    class Update(BaseModel):
+        walkthrough: updater.WalkthroughUpdaterInputConfig
+
+    general: General
+    neu: Branch
+    red: Branch
+    lammps: lammps.GenericLammpsInputConfig
+    update: Update
 
+
+class FepWorkflowConfig(BaseModel):
     executors: Dict[str, FepExecutorConfig]
     artifacts: ArtifactMap
-    workflow: Workflow
+    workflow: Any
 
 def fep_train_mlp(*config_files, executor: Optional[str] = None, path_prefix: Optional[str] = None):
     """
     Training ML potential for FEP
     """
 
     config_data = load_yaml_files(*config_files)
-    config = FepConfig.parse_obj(config_data)
+    config = FepWorkflowConfig.parse_obj(config_data)
 
     if executor not in config.executors:
         raise ValueError(f'executor {executor} is not found')
     if path_prefix is None:
         raise ValueError('path_prefix should not be empty')
 
-    executor_manager = ExecutorManager(config.executors)  # type: ignore
-    default_executor = executor_manager.get_executor(executor)
+    resource_manager = ResourceManager(
+        executor_configs=config.executors,
+        artifacts=config.artifacts,
+        default_executor=executor,
+    )
 
-    context_cfg = config.executors[executor].context
+    context_config = config.executors[executor].context
+    raw_workflow_config = copy.deepcopy(config.workflow)
 
-    type_map = config.workflow.general.type_map
-    mass_map = config.workflow.general.mass_map
+    # output of each step
+    neu_label_output: Optional[cll.ICllLabelOutput] = None
+    red_label_output: Optional[cll.ICllLabelOutput] = None
 
-    # Init Setting
-    neu_deepmd_input = deepmd.GenericDeepmdInput(
-        config=config.workflow.neu.deepmd,
-        type_map=type_map,
-        old_dataset=[],
-        new_dataset=[config.artifacts[key] for key in config.workflow.neu.deepmd.init_dataset],
-    )
-    neu_deepmd_context = deepmd.GenericDeepmdContext(
-        path_prefix='',
-        executor=default_executor,
-        config=context_cfg.deepmd,
-    )
+    neu_selector_output: Optional[cll.ICllSelectorOutput] = None
+    red_selector_output: Optional[cll.ICllSelectorOutput] = None
 
-    red_deepmd_input = deepmd.GenericDeepmdInput(
-        config=config.workflow.red.deepmd,
-        type_map=type_map,
-        old_dataset=[],
-        new_dataset=[config.artifacts[key] for key in config.workflow.red.deepmd.init_dataset],
-    )
-    red_deepmd_context = deepmd.GenericDeepmdContext(
-        path_prefix='',
-        executor=default_executor,
-        config=context_cfg.deepmd,
-    )
+    neu_train_output: Optional[cll.ICllTrainOutput] = None
+    red_train_output: Optional[cll.ICllTrainOutput] = None
+
+    explore_output: Optional[cll.ICllExploreOutput] = None
 
+    # cursor of update table
+    update_cursor = 0
     # Start iteration
-    for i in range(config.workflow.general.max_iters):
-        # update path prefix for each iteration
-        iter_path_prefix = os.path.join(path_prefix, f'iters-{str(i).zfill(3)}')
-
-        # train
-        neu_deepmd_context.path_prefix = os.path.join(iter_path_prefix, 'train-neu-deepmd')
-        neu_deepmd_output_future = deepmd.generic_deepmd(neu_deepmd_input, neu_deepmd_context)
+    for i in itertools.count(0):
 
-        red_deepmd_context.path_prefix = os.path.join(iter_path_prefix, 'train-red-deepmd')
-        red_deepmd_output_future = deepmd.generic_deepmd(red_deepmd_input, red_deepmd_context)
+        # parse workflow config
+        workflow_config = WorkflowConfig.parse_obj(raw_workflow_config)
+        if i >= workflow_config.general.max_iters:
+            logger.info(f'Iteration {i} exceeds max_iters, stop iteration.')
+            break
+
+        # shortcut for type_map and mass_map
+        type_map = workflow_config.general.type_map
+        mass_map = workflow_config.general.mass_map
 
-        neu_deepmd_output, red_deepmd_output = neu_deepmd_output_future.result(), red_deepmd_output_future.result()
+        # decide path prefix for each iteration
+        iter_path_prefix = os.path.join(path_prefix, f'iters-{i:03d}')
 
-        # explore
-        neu_models = [a.output_dir.join(a.output_dir.attrs['frozen_model']) for a in neu_deepmd_output.results]
-        red_models = [a.output_dir.join(a.output_dir.attrs['frozen_model']) for a in red_deepmd_output.results]
+        # label: cp2k
+        red_cp2k_input = cp2k.GenericCp2kInput(
+            config=workflow_config.red.cp2k,
+            type_map=type_map,
+            system_files=[] if red_selector_output is None else red_selector_output.get_model_devi_dataset(),
+            initiated= i > 0,
+        )
+        red_cpk2_context = cp2k.GenericCp2kContext(
+            config=context_config.cp2k,
+            path_prefix=os.path.join(iter_path_prefix, 'red-label-cp2k'),
+            resource_manager=resource_manager,
+        )
+
+        neu_cp2k_input = cp2k.GenericCp2kInput(
+            config=workflow_config.neu.cp2k,
+            type_map=type_map,
+            system_files=[] if neu_selector_output is None else neu_selector_output.get_model_devi_dataset(),
+            initiated= i > 0,
+        )
+        neu_cp2k_context = cp2k.GenericCp2kContext(
+            config=context_config.cp2k,
+            path_prefix=os.path.join(iter_path_prefix, 'neu-label-cp2k'),
+            resource_manager=resource_manager,
+        )
+
+
+        red_label_output_future = cp2k.generic_cp2k(red_cp2k_input, red_cpk2_context)
+        neu_label_output_future = cp2k.generic_cp2k(neu_cp2k_input, neu_cp2k_context)
 
-        lammps_iters = config.workflow.lammps.iters
-        md_vars = lammps_iters[i % len(lammps_iters)]
+        red_label_output = red_label_output_future.result()
+        neu_label_output = neu_label_output_future.result()
 
+        # Train
+        red_deepmd_input = deepmd.GenericDeepmdInput(
+            config=workflow_config.red.deepmd,
+            type_map=type_map,
+            old_dataset=[] if red_train_output is None else red_train_output.get_training_dataset(),
+            new_dataset=red_label_output.get_labeled_system_dataset(),
+            initiated= i > 0,
+        )
+        red_deepmd_context = deepmd.GenericDeepmdContext(
+            path_prefix=os.path.join(iter_path_prefix, 'red-train-deepmd'),
+            config=context_config.deepmd,
+            resource_manager=resource_manager,
+        )
+
+        neu_deepmd_input = deepmd.GenericDeepmdInput(
+            config=workflow_config.neu.deepmd,
+            type_map=type_map,
+            old_dataset=[] if neu_train_output is None else neu_train_output.get_training_dataset(),
+            new_dataset=neu_label_output.get_labeled_system_dataset(),
+            initiated= i > 0,
+        )
+        neu_deepmd_context = deepmd.GenericDeepmdContext(
+            path_prefix=os.path.join(iter_path_prefix, 'neu-train-deepmd'),
+            config=context_config.deepmd,
+            resource_manager=resource_manager,
+        )
+
+        red_train_output_future = deepmd.generic_deepmd(red_deepmd_input, red_deepmd_context)
+        neu_train_output_future = deepmd.generic_deepmd(neu_deepmd_input, neu_deepmd_context)
+
+        red_train_output = red_train_output_future.result()
+        neu_train_output = neu_train_output_future.result()
+
+        # explore
         lammps_input = lammps.GenericLammpsInput(
-            config=config.workflow.lammps,
+            config=workflow_config.lammps,
             type_map=type_map,
             mass_map=mass_map,
-            md_vars=md_vars,
-            system_vars=[config.artifacts[key] for key in md_vars.system_vars],
-            fep_options=lammps.GenericLammpsInput.FepOptions(red_models=red_models, neu_models=neu_models)
+            fep_options=lammps.GenericLammpsInput.FepOptions(
+                neu_models=neu_train_output.get_mlp_models(),
+                red_models=red_train_output.get_mlp_models(),
+            ),
         )
         lammps_context = lammps.GenericLammpsContext(
-            config=context_cfg.lammps,
             path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
-            executor=default_executor,
+            config=context_config.lammps,
+            resource_manager=resource_manager,
         )
-        lammps_output = lammps.generic_lammps(lammps_input, lammps_context).result()
+        explore_output = lammps.generic_lammps(lammps_input, lammps_context).result()
 
-        # select
-        neu_selector_input = selector.ThresholdSelectorInput(
-            config=config.workflow.neu.threshold,
-            model_devi_data=lammps_output.systems,
-            model_devi_out_filename=const.MODEL_DEVI_NEU_OUT,
-        )
-        neu_selector_context = selector.ThresholdSelectorContext(
-            executor=default_executor,
-        )
 
+        # select
         red_selector_input = selector.ThresholdSelectorInput(
-            config=config.workflow.red.threshold,
-            model_devi_data=lammps_output.systems,
+            config=workflow_config.red.threshold,
+            model_devi_data=explore_output.get_model_devi_dataset(),
             model_devi_out_filename=const.MODEL_DEVI_RED_OUT,
         )
         red_selector_context = selector.ThresholdSelectorContext(
-            executor=default_executor,
+            path_prefix=os.path.join(iter_path_prefix, 'red-selector-threshold'),
+            resource_manager=resource_manager,
         )
 
-        neu_selector_output_future = selector.threshold_selector(neu_selector_input, neu_selector_context)
-        red_selector_output_future = selector.threshold_selector(red_selector_input, red_selector_context)
-
-        neu_selector_output, red_selector_output = neu_selector_output_future.result(), red_selector_output_future.result()
-
-        # label
-        neu_cp2k_input = cp2k.GenericCp2kInput(
-            config=config.workflow.neu.cp2k,
-            type_map=config.workflow.general.type_map,
-            system_files=neu_selector_output.model_devi_data,
-            basic_set_file=config.artifacts.get(config.workflow.neu.cp2k.basic_set_file or ''),
-            potential_file=config.artifacts.get(config.workflow.neu.cp2k.potential_file or ''),
+        neu_selector_input = selector.ThresholdSelectorInput(
+            config=workflow_config.neu.threshold,
+            model_devi_data=explore_output.get_model_devi_dataset(),
+            model_devi_out_filename=const.MODEL_DEVI_NEU_OUT,
         )
-        neu_cp2k_context = cp2k.GenericCp2kContext(
-            config=context_cfg.cp2k,
-            path_prefix=os.path.join(iter_path_prefix, 'label-neu-cp2k'),
-            executor=default_executor,
+        neu_selector_context = selector.ThresholdSelectorContext(
+            path_prefix=os.path.join(iter_path_prefix, 'neu-selector-threshold'),
+            resource_manager=resource_manager,
         )
 
-        red_cp2k_input = cp2k.GenericCp2kInput(
-            config=config.workflow.red.cp2k,
-            type_map=config.workflow.general.type_map,
-            system_files=red_selector_output.model_devi_data,
-            basic_set_file=config.artifacts.get(config.workflow.red.cp2k.basic_set_file or ''),
-            potential_file=config.artifacts.get(config.workflow.red.cp2k.potential_file or ''),
-        )
-        red_cp2k_context = cp2k.GenericCp2kContext(
-            config=context_cfg.cp2k,
-            path_prefix=os.path.join(iter_path_prefix, 'label-red-cp2k'),
-            executor=default_executor,
-        )
+        red_selector_output_future = selector.threshold_selector(red_selector_input, red_selector_context)
+        neu_selector_output_future = selector.threshold_selector(neu_selector_input, neu_selector_context)
 
-        neu_cp2k_output_future = cp2k.generic_cp2k(neu_cp2k_input, neu_cp2k_context)
-        red_cp2k_output_future = cp2k.generic_cp2k(red_cp2k_input, red_cp2k_context)
+        red_selector_output = red_selector_output_future.result()
+        neu_selector_output = neu_selector_output_future.result()
 
-        neu_cp2k_output, red_cp2k_output = neu_cp2k_output_future.result(), red_cp2k_output_future.result()
 
-        # update input for the next round
-        neu_deepmd_input.old_dataset.extend(neu_deepmd_input.new_dataset)
-        neu_deepmd_input.new_dataset = neu_cp2k_output.dp_data_sets
+        # Update
+        update_config = workflow_config.update.walkthrough
 
-        red_deepmd_input.old_dataset.extend(red_deepmd_input.new_dataset)
-        red_deepmd_input.new_dataset = red_cp2k_output.dp_data_sets
+        # nothing to update because the table is empty
+        if not update_config.table:
+            continue
+        # keep using the latest config when it reach the end of table
+        if update_cursor >= len(update_config.table):
+            continue
+        # update config
+        update_cursor += 1
 
 
 if __name__ == '__main__':
-    # for test, e.g:
-    # python -m ai2_kit.workflow.fep fep_config.yaml --executor=hpc01 --path-prefix=fep-test
-    Fire(fep_train_mlp)
+    # use python-fire to parse command line arguments
+    Fire(fep_train_mlp)
```

### Comparing `ai2_kit-0.2.0/pyproject.toml` & `ai2_kit-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-fire = "^0.4.0"
+fire = "^0.5.0"
 fabric = "^2.7.1"
 pydantic = "^1.10.2"
 invoke = "^1.7.3"
 ruamel-yaml = "^0.17.21"
 cloudpickle = "^2.2.0"
 shortuuid = "^1.0.11"
 dpdata = "^0.2.13"
```

### Comparing `ai2_kit-0.2.0/PKG-INFO` & `ai2_kit-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
 Requires-Dist: cp2k-input-tools (>=0.8.2,<0.9.0)
 Requires-Dist: dpdata (>=0.2.13,<0.3.0)
 Requires-Dist: fabric (>=2.7.1,<3.0.0)
-Requires-Dist: fire (>=0.4.0,<0.5.0)
+Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: invoke (>=1.7.3,<2.0.0)
 Requires-Dist: mdanalysis (>=2.4.3,<3.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pymatgen (>=2023.2.22,<2024.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
@@ -55,14 +55,15 @@
 
 ./ai2-kit --help
 ```
 
 ## Manuals
 
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
+* [ASE Toolkit](doc/manual/ase.md)
 * [CLL MLP Training Workflow](doc/manual/cll-workflow.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ## Tutorials
 
 ## Notebooks
```

