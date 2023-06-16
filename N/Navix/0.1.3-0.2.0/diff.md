# Comparing `tmp/Navix-0.1.3.tar.gz` & `tmp/Navix-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.1.3.tar", last modified: Tue Jun 13 21:59:21 2023, max compression
+gzip compressed data, was "Navix-0.2.0.tar", last modified: Fri Jun 16 16:52:21 2023, max compression
```

## Comparing `Navix-0.1.3.tar` & `Navix-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.060319 Navix-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.064319 Navix-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 21:59:06.000000 Navix-0.1.3/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 21:59:06.000000 Navix-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 21:59:06.000000 Navix-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 21:59:06.000000 Navix-0.1.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 21:59:06.000000 Navix-0.1.3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-13 21:59:06.000000 Navix-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 21:59:06.000000 Navix-0.1.3/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.064319 Navix-0.1.3/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:59:21.000000 Navix-0.1.3/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:59:21.068319 Navix-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-13 21:59:06.000000 Navix-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.064319 Navix-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-13 21:59:06.000000 Navix-0.1.3/docs/profiling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/navix/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:59:06.000000 Navix-0.1.3/navix/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 21:59:06.000000 Navix-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:59:06.000000 Navix-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:59:21.068319 Navix-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:59:21.068319 Navix-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-13 21:59:06.000000 Navix-0.1.3/tests/test_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.424184 Navix-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.396184 Navix-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.408184 Navix-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-16 16:52:09.000000 Navix-0.2.0/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-16 16:52:09.000000 Navix-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-16 16:52:09.000000 Navix-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 16:52:09.000000 Navix-0.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 16:52:09.000000 Navix-0.2.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-16 16:52:09.000000 Navix-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 16:52:09.000000 Navix-0.2.0/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.412184 Navix-0.2.0/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-16 16:52:21.424184 Navix-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-16 16:52:09.000000 Navix-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.412184 Navix-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 16:52:09.000000 Navix-0.2.0/docs/design_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-16 16:52:09.000000 Navix-0.2.0/docs/profiling.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.416184 Navix-0.2.0/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.420184 Navix-0.2.0/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/keydoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/terminations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-16 16:52:09.000000 Navix-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 16:52:09.000000 Navix-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:52:21.424184 Navix-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.420184 Navix-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_tasks.py
```

### Comparing `Navix-0.1.3/.github/workflows/CD.yml` & `Navix-0.2.0/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.3/.github/workflows/CI.yml` & `Navix-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.3/.gitignore` & `Navix-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.1.3/COPYRIGHT` & `Navix-0.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.1.3/LICENSE` & `Navix-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.1.3/Navix.egg-info/PKG-INFO` & `Navix-0.2.0/Navix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.3
+Version: 0.2.0
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -250,15 +250,15 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>10000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
```

### Comparing `Navix-0.1.3/Navix.egg-info/SOURCES.txt` & `Navix-0.2.0/Navix.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 .github/workflows/CD.yml
 .github/workflows/CI.yml
 Navix.egg-info/PKG-INFO
 Navix.egg-info/SOURCES.txt
 Navix.egg-info/dependency_links.txt
 Navix.egg-info/requires.txt
 Navix.egg-info/top_level.txt
+docs/design_notes.md
 docs/profiling.ipynb
 navix/__init__.py
 navix/actions.py
 navix/components.py
 navix/grid.py
 navix/observations.py
 navix/tasks.py
-navix/termination.py
-navix/transitions.py
+navix/terminations.py
 navix/environments/__init__.py
 navix/environments/environment.py
+navix/environments/keydoor.py
 navix/environments/room.py
-tests/test_environment.py
+tests/test_actions.py
+tests/test_environments.py
+tests/test_grid.py
+tests/test_tasks.py
```

### Comparing `Navix-0.1.3/PKG-INFO` & `Navix-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.3
+Version: 0.2.0
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -250,15 +250,15 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>10000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
```

### Comparing `Navix-0.1.3/README.md` & `Navix-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>10000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
```

### Comparing `Navix-0.1.3/docs/profiling.ipynb` & `Navix-0.2.0/docs/profiling.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982142857142857%*

 * *Differences: {"'cells'": "{3: {'source': ['# running 10_000 seeds in parallel\\n', '%timeit -n 5 -r 1 "*

 * *            "f(jnp.arange(10_000)).state.grid.block_until_ready()']}}"}*

```diff
@@ -64,16 +64,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "44SbP_tOp1dP"
             },
             "outputs": [],
             "source": [
-                "# running 1000 seeds in parallel\n",
-                "%timeit -n 5 -r 1 f(jnp.arange(1000)).state.grid.block_until_ready()"
+                "# running 10_000 seeds in parallel\n",
+                "%timeit -n 5 -r 1 f(jnp.arange(10_000)).state.grid.block_until_ready()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "iSeCh6H4qRdx"
```

### Comparing `Navix-0.1.3/navix/__init__.py` & `Navix-0.2.0/navix/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,20 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-from __future__ import annotations
-
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
 
 
 from . import (
     actions,
     components,
     grid,
     observations,
     tasks,
-    termination,
-    transitions,
     environments,
+    terminations,
 )
```

### Comparing `Navix-0.1.3/navix/environments/__init__.py` & `Navix-0.2.0/navix/environments/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,9 +15,12 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
+
+
 from .environment import Environment
 from .room import Room
+from .keydoor import KeyDoor
```

### Comparing `Navix-0.1.3/navix/environments/environment.py` & `Navix-0.2.0/navix/environments/environment.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,80 +21,72 @@
 from __future__ import annotations
 
 import abc
 from typing import Callable
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
-from chex import Array
+from jax import Array
 from flax import struct
 
-from ..tasks import navigation
+from .. import tasks
 from ..components import State, Timestep, StepType
-from ..transitions import deterministic_transition
-from ..termination import on_navigation_completion, check_truncation
+from .. import terminations
 from ..actions import ACTIONS
+from .. import observations
 
 
 class Environment(struct.PyTreeNode):
     width: int = struct.field(pytree_node=False)
     height: int = struct.field(pytree_node=False)
     max_steps: int = struct.field(pytree_node=False)
     gamma: float = struct.field(pytree_node=False, default=1.0)
     observation_fn: Callable[[State], Array] = struct.field(
-        pytree_node=False, default=lambda x: None
+        pytree_node=False, default=observations.categorical
     )
-    reward_fn: Callable[[State], Array] = struct.field(
-        pytree_node=False, default=navigation
+    reward_fn: Callable[[State, Array, State], Array] = struct.field(
+        pytree_node=False, default=tasks.navigation
     )
-    state_transition_fn: Callable[[State, Array], State] = struct.field(
-        pytree_node=False, default=deterministic_transition
-    )
-    termination_fn: Callable[[State], Array] = struct.field(
-        pytree_node=False, default=on_navigation_completion
+    termination_fn: Callable[[State, Array, State], Array] = struct.field(
+        pytree_node=False, default=terminations.on_navigation_completion
     )
 
     @abc.abstractmethod
     def reset(self, key: KeyArray) -> Timestep:
         raise NotImplementedError()
 
-    def step(self, timestep: Timestep, action: Array, ACTIONS=ACTIONS) -> Timestep:
+    def _step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
+        # update agents
+        state = jax.lax.switch(action, actions_set.values(), timestep.state)
+
+        # build timestep
+        return Timestep(
+            t=timestep.t + 1,
+            state=state,
+            action=jnp.asarray(action),
+            reward=self.reward(timestep.state, action, state),
+            step_type=self.termination(timestep.state, action, state, timestep.t + 1),
+            observation=self.observation(state),
+        )
+
+    def step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
         # autoreset if necessary: 0 = transition, 1 = truncation, 2 = termination
         should_reset = timestep.step_type > 0
         return jax.lax.cond(
             should_reset,
             lambda timestep: self.reset(timestep.state.key),
-            lambda timestep: self.transition(timestep, action, ACTIONS),
+            lambda timestep: self._step(timestep, action, actions_set),
             timestep,
         )
 
     def observation(self, state: State):
         return self.observation_fn(state)
 
-    def reward(self, state: State):
-        return self.reward_fn(state)
+    def reward(self, state: State, action: Array, new_state: State):
+        return self.reward_fn(state, action, new_state)
 
-    def termination(self, state: State, t: Array) -> Array:
-        terminated = self.termination_fn(state)
+    def termination(
+        self, prev_state: State, action: Array, state: State, t: Array
+    ) -> Array:
+        terminated = self.termination_fn(prev_state, action, state)
         truncated = t >= self.max_steps
-        return check_truncation(terminated, truncated)
-
-    def transition(
-        self, timestep: Timestep, action: Array, ACTIONS=ACTIONS
-    ) -> Timestep:
-        # apply actions
-        state = jax.lax.switch(action, ACTIONS.values(), timestep.state)
-        # apply environment transition
-        state = self.state_transition_fn(state, action)
-        # build timestep
-        return Timestep(
-            t=timestep.t + 1,
-            state=state,
-            action=jnp.asarray(action),
-            reward=self.reward(state),
-            step_type=self.termination(state, timestep.t + 1),
-            observation=self.observation(state),
-        )
-
-    def discount(self, state: State, t: int) -> Array:
-        discount_t = (self.gamma**t) * self.termination_fn(state)
-        return jnp.asarray(discount_t, dtype=jnp.float32)
+        return terminations.check_truncation(terminated, truncated)
```

### Comparing `Navix-0.1.3/navix/environments/room.py` & `Navix-0.2.0/navix/environments/room.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,38 +17,42 @@
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
 import jax
-from jax.random import KeyArray
 import jax.numpy as jnp
+from jax.random import KeyArray
+
+from ..components import Goal, Player, State, Timestep
+from ..grid import random_positions, random_directions, room
 from .environment import Environment
-from ..components import State, Component, StepType, Timestep
-from ..grid import room, spawn_entity
 
 
 class Room(Environment):
     def reset(self, key: KeyArray) -> Timestep:
         key, k1, k2 = jax.random.split(key, 3)
 
-        # entities
-        player = Component(id=1, direction=0)
-        goal = Component(id=2)
-        entities = {
-            "player/0": player,
-            "goal/0": goal,
-        }
-
-        # system
+        # map
         grid = room(self.width, self.height)
-        grid = spawn_entity(grid, player.id, k1)
-        grid = spawn_entity(grid, goal.id, k2)
-        state = State(key=key, grid=grid, entities=entities)
+        positions = random_positions(k1, grid, n=2)
+        direction = random_directions(k2, n=1)
+        # player
+        player = Player(position=positions[0], direction=direction)
+        # goal
+        goal = Goal(position=positions[1][None])
+
+        # systems
+        state = State(
+            key=key,
+            grid=grid,
+            player=player,
+            goals=goal,
+        )
 
         return Timestep(
             t=jnp.asarray(0, dtype=jnp.int32),
             observation=self.observation(state),
             action=jnp.asarray(0, dtype=jnp.int32),
             reward=jnp.asarray(0.0, dtype=jnp.float32),
             step_type=jnp.asarray(0, dtype=jnp.int32),
```

### Comparing `Navix-0.1.3/navix/observations.py` & `Navix-0.2.0/navix/terminations.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,30 +16,20 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
-from chex import Array
-
+from jax import Array
+import jax
+import jax.numpy as jnp
 from .components import State
 
 
-def third_person_view(state: State, radius: int) -> Array:
-    raise NotImplementedError()
-
-
-def first_person_view(state: State, radius: int) -> Array:
-    raise NotImplementedError()
-
-
-def categorical(state: State) -> Array:
-    raise NotImplementedError()
-
-
-def one_hot(state: State) -> Array:
-    raise NotImplementedError()
+def check_truncation(terminated: Array, truncated: Array) -> Array:
+    return jnp.asarray(truncated + 2 * terminated, dtype=jnp.int32)
 
 
-def pixels(state: State) -> Array:
-    raise NotImplementedError()
+def on_navigation_completion(prev_state: State, action: Array, state: State) -> Array:
+    reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(state.player.position, state.goals.position)
+    return jnp.any(reached)
```

### Comparing `Navix-0.1.3/pyproject.toml` & `Navix-0.2.0/pyproject.toml`

 * *Files identical despite different names*

