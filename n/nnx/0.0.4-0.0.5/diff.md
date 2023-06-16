# Comparing `tmp/nnx-0.0.4.tar.gz` & `tmp/nnx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.4.tar", max compression
+gzip compressed data, was "nnx-0.0.5.tar", max compression
```

## Comparing `nnx-0.0.4.tar` & `nnx-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.4/LICENSE
--rw-r--r--   0        0        0    18246 2023-06-11 18:34:14.199541 nnx-0.0.4/README.md
--rw-r--r--   0        0        0     1297 2023-06-08 02:13:58.996364 nnx-0.0.4/nnx/__init__.py
--rw-r--r--   0        0        0     5789 2023-06-09 20:55:00.758150 nnx-0.0.4/nnx/context.py
--rw-r--r--   0        0        0       45 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/errors.py
--rw-r--r--   0        0        0     3700 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/helpers.py
--rw-r--r--   0        0        0    22918 2023-06-10 22:31:26.795914 nnx-0.0.4/nnx/module.py
--rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.4/nnx/nn/__init__.py
--rw-r--r--   0        0        0      763 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/nn/activations.py
--rw-r--r--   0        0        0     2763 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/nn/dtypes.py
--rw-r--r--   0        0        0     1888 2023-06-08 02:13:59.008365 nnx-0.0.4/nnx/nn/initializers.py
--rw-r--r--   0        0        0    16010 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nn/linear.py
--rw-r--r--   0        0        0    13518 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nn/normalization.py
--rw-r--r--   0        0        0     2276 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nn/stochastic.py
--rw-r--r--   0        0        0      348 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/nodes.py
--rw-r--r--   0        0        0     2088 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/partitioning.py
--rw-r--r--   0        0        0    12691 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/pytreelib.py
--rw-r--r--   0        0        0     2280 2023-06-08 02:13:59.012365 nnx-0.0.4/nnx/reprlib.py
--rw-r--r--   0        0        0     9378 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/state.py
--rw-r--r--   0        0        0     2412 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/tracers.py
--rw-r--r--   0        0        0     6775 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/transforms.py
--rw-r--r--   0        0        0      588 2023-06-08 02:13:59.016365 nnx-0.0.4/nnx/utils.py
--rw-r--r--   0        0        0      764 2023-06-11 18:36:11.481330 nnx-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    18779 1970-01-01 00:00:00.000000 nnx-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.5/LICENSE
+-rw-r--r--   0        0        0    18330 2023-06-12 22:45:34.700995 nnx-0.0.5/README.md
+-rw-r--r--   0        0        0     1200 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/__init__.py
+-rw-r--r--   0        0        0     7443 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/containers.py
+-rw-r--r--   0        0        0     5707 2023-06-12 22:45:21.347880 nnx-0.0.5/nnx/contextlib.py
+-rw-r--r--   0        0        0     4495 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/dataclasses.py
+-rw-r--r--   0        0        0       45 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/errors.py
+-rw-r--r--   0        0        0     3628 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/helpers.py
+-rw-r--r--   0        0        0    23360 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/module.py
+-rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.5/nnx/nn/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2763 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     1888 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    16022 2023-06-12 22:45:21.347880 nnx-0.0.5/nnx/nn/linear.py
+-rw-r--r--   0        0        0    13530 2023-06-12 22:45:21.347880 nnx-0.0.5/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2282 2023-06-12 22:45:21.351881 nnx-0.0.5/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0      348 2023-06-08 02:13:59.012365 nnx-0.0.5/nnx/nodes.py
+-rw-r--r--   0        0        0     2224 2023-06-14 04:55:58.785571 nnx-0.0.5/nnx/partitioning.py
+-rw-r--r--   0        0        0     8445 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/pytreelib.py
+-rw-r--r--   0        0        0     2313 2023-06-12 22:45:21.351881 nnx-0.0.5/nnx/reprlib.py
+-rw-r--r--   0        0        0     5276 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/state.py
+-rw-r--r--   0        0        0     2412 2023-06-08 02:13:59.016365 nnx-0.0.5/nnx/tracers.py
+-rw-r--r--   0        0        0     6784 2023-06-12 22:45:21.351881 nnx-0.0.5/nnx/transforms.py
+-rw-r--r--   0        0        0      615 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/utils.py
+-rw-r--r--   0        0        0      764 2023-06-16 17:16:52.104906 nnx-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    18863 1970-01-01 00:00:00.000000 nnx-0.0.5/PKG-INFO
```

### Comparing `nnx-0.0.4/LICENSE` & `nnx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nnx-0.0.4/README.md` & `nnx-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,25 @@
         self.b = nnx.param(jnp.zeros((dout,)))
         self.count = nnx.var("counts", 0)  # track the number of calls
 
     def __call__(self, x):
         self.count += 1
         return x @ self.w + self.b
 
-ctx = nnx.Context(params=jax.random.PRNGKey(0))
-model = Linear(din=12, dout=2, ctx=ctx)
+model = Linear(din=12, dout=2, ctx=nnx.context(0))
 
 # Forward pass and verify the call count
 x = jnp.ones((8, 12))
 y = model(x)
 assert model.count == 1
 ```
 
+In this example `nnx.context(0)` create a `PRNGKey` for `params` with seed `0`, this is used by `make_rng`
+inside `__init__` to generate a random key to initialize the parameters.
+
 ### Training
 
 Here we show case two different approaches to training the model defined in the previous secition. The first one uses lifted transforms and the second one uses the functional API. Both approaches are equivalent and produce the same results.
 
 <details><summary>Lifted Transforms</summary>
 
 In this example, we uset the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD) and `train_step` doesn't require a return statement in this case as the model's state is automatically updated.
@@ -169,16 +171,15 @@
         self.submodule = nnx.Linear(2, 4, ctx=ctx)
         # static attributes
         self.int = 1
         self.float = 2.0
         self.str = "hello"
         self.list = [1, 2, 3]
 
-ctx = nnx.Context(jax.random.PRNGKey(0))
-model = Foo(din=12, dout=2, ctx=ctx)
+model = Foo(din=12, dout=2, ctx=nnx.context(0))
 ```
 As shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Map` Modules.
 
 ### Functional API
 
 NNX Modules are not pytrees so they cannot be passed to JAX transformations. In order to interact with JAX, a Module must be partitioned into a `State` and `ModuleDef` objects. The `State` object is a flat dictionary-like pytree structure that contains all the deduplicated node attributes, and the `ModuleDef` contains the static attributes and structural information needed to reconstruct the Module.
 
@@ -277,16 +278,15 @@
         self.b = nnx.param(jnp.zeros((dout,)))
 
     def __call__(self, x):
         y = x @ self.w + self.b
         self.y = nnx.var("intermediates", y)
         return y
 
-ctx = nnx.Context(jax.random.PRNGKey(0))
-model = Linear(12, 2, ctx=ctx)
+model = Linear(12, 2, ctx=nnx.context(0))
 ```
 Since `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `intermediates`:
 
 ```python
 y = model(jnp.ones((8, 12)))
 intermediates = model.pop_state("intermediates")
 ```
@@ -381,13 +381,13 @@
 
 In this example, the `Model` module contains two instances of the `Block` module. Each instance shares the same `nnx.Linear` module. To run the model, you can use the Context `flags` argument to set the `use_running_average` flag for all `BatchNorm` modules.
 
 Here's an example of computing the loss for a `Model` instance:
 
 ```python
 def loss_fn(model: Model, x: jax.Array, y: jax.Array):
-    ctx = nnx.Context(flags=dict(use_running_average=True))
+    ctx = nnx.context(flags=dict(use_running_average=True))
     y_pred = model(x, ctx=ctx)
     return jnp.mean((y - y_pred) ** 2)
 ```
 
 It's important to note that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.
```

### Comparing `nnx-0.0.4/nnx/__init__.py` & `nnx-0.0.5/nnx/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 __version__ = "0.0.0"
 
 
-from .context import Context, RngStream
+from .containers import (
+    Container,
+    Node,
+    Static,
+    Variable,
+    VarMetadata,
+    node,
+    param,
+    static,
+    var,
+    var_metadata,
+    with_partitioning,
+)
+from .contextlib import Context, RngStream, context
+from .dataclasses import (
+    dataclass,
+    field,
+    node_field,
+    param_field,
+    static_field,
+    var_field,
+)
 from .errors import TraceContextError
 from .helpers import Map, Sequence, TrainState
 from .module import Module, ModuleDef, PureModule
+from .nn import initializers
 from .nn.activations import (
     celu,
     elu,
     gelu,
     glu,
     hard_sigmoid,
     hard_silu,
@@ -28,44 +50,15 @@
     soft_sign,
     softmax,
     softplus,
     standardize,
     swish,
     tanh,
 )
-from .nn.initializers import (
-    Initializer,
-    constant,
-    delta_orthogonal,
-    glorot_normal,
-    glorot_uniform,
-    he_normal,
-    he_uniform,
-    kaiming_normal,
-    kaiming_uniform,
-    lecun_normal,
-    lecun_uniform,
-    normal,
-    ones,
-    orthogonal,
-    uniform,
-    variance_scaling,
-    xavier_normal,
-    xavier_uniform,
-    zeros,
-)
 from .nn.linear import Conv, Embed, Linear
 from .nn.normalization import BatchNorm, LayerNorm
 from .nn.stochastic import Dropout
 from .nodes import is_node, register_node_type
 from .partitioning import buffers
-from .state import (
-    State,
-    Variable,
-    VarMetadata,
-    node,
-    param,
-    var,
-    var_metadata,
-    with_partitioning,
-)
+from .pytreelib import Pytree
+from .state import State
 from .transforms import grad, jit
```

### Comparing `nnx-0.0.4/nnx/context.py` & `nnx-0.0.5/nnx/contextlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,39 +146,19 @@
 
 
 class Context:
     __slots__ = ("_rngs", "_flags")
 
     def __init__(
         self,
-        rngs: tp.Union[
-            tp.Mapping[str, tp.Union[RngStream, KeyArray]], RngStream, KeyArray, None
-        ] = None,
-        *,
-        flags: tp.Optional[tp.Mapping[str, bool]] = None,
-        **rng_updates: tp.Union[RngStream, KeyArray],
+        rngs: tp.Mapping[str, RngStream],
+        flags: tp.Mapping[str, bool],
     ):
-        if rngs is None:
-            _rngs = {}
-        elif isinstance(rngs, tp.Mapping):
-            _rngs = dict(rngs)
-        elif isinstance(rngs, RngStream):
-            _rngs = dict(params=rngs)
-        else:
-            _rngs = dict(params=RngStream(rngs))
-
-        _rngs.update(**rng_updates)
-
-        _rngs = {
-            name: RngStream(key) if not isinstance(key, RngStream) else key
-            for name, key in _rngs.items()
-        }
-
-        self._rngs = _rngs
-        self._flags = MappingProxyType(flags or {})
+        self._rngs = rngs
+        self._flags = flags
 
     def has_rng(self, name: str) -> bool:
         return name in self._rngs
 
     def make_rng(self, name: str) -> KeyArray:
         if name not in self._rngs:
             raise ValueError(f"Unknown Rng Stream: {name}")
@@ -194,7 +174,30 @@
         return self._flags.get(name, None)
 
     def partition(self) -> PureContext:
         rngs = {name: stream.fork() for name, stream in self._rngs.items()}
         keys = {name: stream._key for name, stream in rngs.items()}
         rng_counts = tuple((name, stream.count_path) for name, stream in rngs.items())
         return PureContext.new(keys, ContextDef(rng_counts, tuple(self._flags.items())))
+
+
+def context(
+    params: tp.Union[int, KeyArray, RngStream, None] = None,
+    *,
+    flags: tp.Optional[tp.Mapping[str, bool]] = None,
+    **rngs: tp.Union[int, KeyArray, RngStream],
+) -> Context:
+    _flags = flags or {}
+
+    if params is not None:
+        rngs["params"] = params
+
+    _rngs = {
+        name: RngStream(jax.random.PRNGKey(value))
+        if isinstance(value, int)
+        else RngStream(value)
+        if isinstance(value, jax.Array)
+        else value
+        for name, value in rngs.items()
+    }
+
+    return Context(rngs=_rngs, flags=_flags)
```

### Comparing `nnx-0.0.4/nnx/helpers.py` & `nnx-0.0.5/nnx/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as tp
 
 import optax
 
-from nnx import pytreelib, utils
-from nnx.context import Context
+from nnx import containers, pytreelib, utils
+from nnx.contextlib import Context
 from nnx.module import ApplyCaller, Module, PureModule
 from nnx.state import State
 
 A = tp.TypeVar("A")
 M = tp.TypeVar("M", bound=Module)
 
 
@@ -88,32 +88,28 @@
 
 class ModuleDefApply(tp.Protocol, tp.Generic[M]):
     def __call__(self, state: State, *states: State) -> ApplyCaller["PureModule[M]"]:
         ...
 
 
 class TrainState(pytreelib.Pytree, tp.Generic[M]):
-    params: State = pytreelib.node_field()
-    opt_state: optax.OptState = pytreelib.node_field()
-    step: int = pytreelib.node_field()
-
     def __init__(
         self,
         *,
         apply_fn: ModuleDefApply[M],
         params: State,
         tx: optax.GradientTransformation,
         step: int = 0,
         **kwargs,
     ):
         self.apply_fn = apply_fn
-        self.params: State = params
+        self.params: State = containers.node(params)
         self.tx = tx
-        self.opt_state = tx.init(self.params)
-        self.step = step
+        self.opt_state = containers.node(tx.init(self.params))
+        self.step = containers.node(step)
         for name, value in kwargs.items():
             setattr(self, name, value)
 
     if tp.TYPE_CHECKING:
 
         def __getattr__(self, key: str) -> tp.Any:
             ...
```

### Comparing `nnx-0.0.4/nnx/module.py` & `nnx-0.0.5/nnx/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import dataclasses
 import typing as tp
 from abc import ABCMeta
 from typing import Any
 
 import jax.tree_util as jtu
 
-from nnx import errors, partitioning, reprlib, tracers
-from nnx.nodes import is_node, register_node_type
-from nnx.state import Node, Sharding, State, Variable
+from nnx import errors, nodes, partitioning, reprlib, tracers
+from nnx.containers import Container, Sharding, Variable
+from nnx.state import State
 
 A = tp.TypeVar("A")
 M = tp.TypeVar("M", bound="Module")
 
 Path = tp.Tuple[str, ...]
 StateDict = tp.Dict[Path, tp.Any]
 StateMapping = tp.Mapping[Path, tp.Any]
@@ -347,47 +347,55 @@
         def __call__(self, *args: Any, **kwargs: Any) -> Any:
             return self.call(*args, **kwargs)
 
     def call(self: tp.Type[M], *args, **kwargs) -> M:
         module = self.__new__(self, *args, **kwargs)
         vars(module)["_module__state"] = ModuleState(tracers.TraceState())
         module.__init__(*args, **kwargs)
+
+        if dataclasses.is_dataclass(module):
+            assert isinstance(module, Module)
+            for field in dataclasses.fields(module):
+                if "nnx_container_fn" not in field.metadata:
+                    continue
+
+                container_fn = field.metadata["nnx_container_fn"]
+                value = vars(module)[field.name]
+                value = container_fn(value)
+                vars(module)[field.name] = value
+
         return module
 
 
 class Module(reprlib.Representable, metaclass=ModuleMeta):
     if tp.TYPE_CHECKING:
         _module__state: ModuleState
 
     if not tp.TYPE_CHECKING:
 
         def __getattribute__(self, name: str) -> Any:
             value = object.__getattribute__(self, name)
-            if isinstance(value, Node):
+            if isinstance(value, Container):
                 return value.value
             return value
 
         def __setattr__(self, name: str, value: Any) -> None:
             self._setattr(name, value)
 
     def _setattr(self, name: str, value: Any) -> None:
         if not self._module__state.trace_state.is_valid():
             raise errors.TraceContextError(
                 "Cannot mutate Module from different trace level"
             )
 
         vars_dict = vars(self)
-        if (
-            name in vars_dict
-            and isinstance(vars_dict[name], Node)
-            and not isinstance(value, Node)
-        ):
-            vars_dict[name] = vars_dict[name].replace(value=value)
+        if name in vars_dict and isinstance(vars_dict[name], Container):
+            vars_dict[name] = vars_dict[name].replace_value(value)
         else:
-            if isinstance(value, Node):
+            if isinstance(value, Container):
                 value = value.copy()
             vars_dict[name] = value
 
     def __hash__(self) -> int:
         return id(self)
 
     def __nnx_repr__(self):
@@ -397,15 +405,15 @@
 
         yield reprlib.Object(type=type(self))
         SEEN_MODULES_REPR.add(id(self))
 
         try:
             for name, value in vars(self).items():
                 if isinstance(value, Module) or (
-                    not is_node(value) and not name.startswith("_")
+                    not nodes.is_node(value) and not name.startswith("_")
                 ):
                     yield reprlib.Attr(name, value)
         finally:
             SEEN_MODULES_REPR.remove(id(self))
 
     def clone(self: M) -> M:
         return self.partition().merge()
@@ -609,27 +617,27 @@
 
     @value.setter
     def value(self, value: tp.Any) -> None:
         setattr(self._module, self._name, value)
 
     @property
     def collection(self) -> tp.Optional[str]:
-        obj = vars(self._module)[self._name]
-        if not isinstance(obj, Variable):
+        module = vars(self._module)[self._name]
+        if not isinstance(module, Variable):
             return None
 
-        return obj.collection
+        return module.collection
 
     @property
     def sharding(self) -> tp.Optional[Sharding]:
-        obj = vars(self._module)[self._name]
-        if not isinstance(obj, Variable):
+        module = vars(self._module)[self._name]
+        if not isinstance(module, Variable):
             return None
 
-        return obj.sharding
+        return module.sharding
 
 
 def _get_module_state(module: Module) -> State:
     return State(_iter_state(module))
 
 
 def _get_module_def(module: M) -> ModuleDef[M]:
@@ -657,15 +665,15 @@
     static_fields = []
 
     for name, value in sorted(vars(module).items(), key=lambda x: x[0]):
         value_path = (*path, name)
         if isinstance(value, Module):
             submodule_def = _make_module_def_recursive(value, module_index, value_path)
             submodules.append((name, submodule_def))
-        elif not is_node(value) and not name.startswith("_module__"):
+        elif not nodes.is_node(value) and not name.startswith("_module__"):
             static_fields.append((name, value))
 
     module_def = ModuleDef(
         type=type(module),
         index=index,
         submodules=tuple(submodules),
         static_fields=tuple(static_fields),
@@ -688,30 +696,30 @@
 
     seen_modules.add(id(module))
 
     for name, value in sorted(vars(module).items(), key=lambda x: x[0]):
         value_path = (*path, name)
         if isinstance(value, Module):
             yield from _iter_state_recursive(value, seen_modules, value_path)
-        elif is_node(value):
+        elif nodes.is_node(value):
             yield value_path, value
 
 
-def _set_value_at_path(obj: tp.Any, path: tp.Sequence[str], value: tp.Any):
+def _set_value_at_path(module: tp.Any, path: tp.Sequence[str], value: tp.Any):
     if len(path) == 1:
-        vars(obj)[path[0]] = value
+        setattr(module, path[0], value)
     else:
-        _set_value_at_path(vars(obj)[path[0]], path[1:], value)
+        _set_value_at_path(vars(module)[path[0]], path[1:], value)
 
 
-def _get_value_path(obj: tp.Any, path: tp.Sequence[str]) -> tp.Any:
+def _get_value_path(module: tp.Any, path: tp.Sequence[str]) -> tp.Any:
     if len(path) == 0:
-        return obj
+        return module
     else:
-        return _get_value_path(vars(obj)[path[0]], path[1:])
+        return _get_value_path(vars(module)[path[0]], path[1:])
 
 
 def _build_module(moduledef: ModuleDef[M]) -> M:
     index_module: tp.Dict[int, Module] = {}
     module = _build_module_recursive(moduledef, index_module)
     return module
 
@@ -765,15 +773,15 @@
         return
 
     for name, value in list(vars(module).items()):
         value_path = (*path, name)
         if isinstance(value, Module):
             _pop_recursive(value, module_index, value_path, states, predicates)
             continue
-        elif not is_node(value):
+        elif not nodes.is_node(value):
             continue
 
         for state, predicate in zip(states, predicates):
             if predicate(value_path, value):
                 state[value_path] = value
                 delattr(module, name)
                 break
@@ -796,9 +804,9 @@
         state.update(new_state)
 
     for path, value in state.items():
         _set_value_at_path(module, path, value)
 
 
 # register nodes
-register_node_type(Module)
-register_node_type(PureModule)
+nodes.register_node_type(Module)
+nodes.register_node_type(PureModule)
```

### Comparing `nnx-0.0.4/nnx/nn/activations.py` & `nnx-0.0.5/nnx/nn/activations.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.4/nnx/nn/dtypes.py` & `nnx-0.0.5/nnx/nn/dtypes.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.4/nnx/nn/initializers.py` & `nnx-0.0.5/nnx/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.4/nnx/nn/linear.py` & `nnx-0.0.5/nnx/nn/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from jax import lax
 
 import nnx
-from nnx import context
+from nnx import contextlib
 from nnx.module import Module
 from nnx.nn import dtypes, initializers
 
 Array = jax.Array
 PRNGKey = tp.Any
 Shape = tp.Tuple[int, ...]
 Dtype = tp.Any  # this could be a real type?
@@ -81,15 +81,15 @@
         use_bias: bool = True,
         dtype: tp.Optional[Dtype] = None,
         param_dtype: Dtype = jnp.float32,
         precision: PrecisionLike = None,
         kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = default_kernel_init,
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         dot_general: DotGeneralT = lax.dot_general,
-        ctx: context.Context,
+        ctx: contextlib.Context,
     ):
         kernel_key = ctx.make_rng("params")
         self.kernel = nnx.param(
             kernel_init(kernel_key, (in_features, out_features), param_dtype)
         )
         if use_bias:
             bias_key = ctx.make_rng("params")
@@ -186,15 +186,15 @@
         mask_fn: tp.Optional[tp.Callable[[Array], Array]] = None,
         dtype: tp.Optional[Dtype] = None,
         param_dtype: Dtype = jnp.float32,
         precision: PrecisionLike = None,
         kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = default_kernel_init,
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         conv_general_dilated: ConvGeneralDilatedT = lax.conv_general_dilated,
-        ctx: context.Context,
+        ctx: contextlib.Context,
     ):
         if isinstance(kernel_size, int):
             raise TypeError(
                 "Expected Conv kernel_size to be a"
                 " tuple/list of integers (eg.: [3, 3]) but got"
                 f" {kernel_size}."
             )
@@ -362,15 +362,15 @@
         features: int,
         *,
         dtype: tp.Optional[Dtype] = None,
         param_dtype: Dtype = jnp.float32,
         embedding_init: tp.Callable[
             [PRNGKey, Shape, Dtype], Array
         ] = default_embed_init,
-        ctx: context.Context,
+        ctx: contextlib.Context,
     ):
         self.embedding = nnx.param(
             embedding_init(
                 ctx.make_rng("params"), (num_embeddings, features), param_dtype
             )
         )
```

### Comparing `nnx-0.0.4/nnx/nn/normalization.py` & `nnx-0.0.5/nnx/nn/normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as tp
 
 import jax
 import jax.numpy as jnp
 from jax import lax
 
 import nnx
-from nnx import context, utils
+from nnx import contextlib, utils
 from nnx.module import Module
 from nnx.nn import dtypes, initializers
 
 PRNGKey = jax.Array
 Array = jax.Array
 Shape = tp.Tuple[int, ...]
 Dtype = tp.Any  # this could be a real type?
@@ -187,15 +187,15 @@
         param_dtype: Dtype = jnp.float32,
         use_bias: bool = True,
         use_scale: bool = True,
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         scale_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones(),
         axis_name: tp.Optional[str] = None,
         axis_index_groups: tp.Any = None,
-        ctx: context.Context,
+        ctx: contextlib.Context,
     ):
         feature_shape = (num_features,)
         self.mean = nnx.var("batch_stats", jnp.zeros(feature_shape, jnp.float32))
         self.var = nnx.var("batch_stats", jnp.ones(feature_shape, jnp.float32))
 
         if use_scale:
             key = ctx.make_rng("params")
@@ -224,15 +224,15 @@
         self.axis_index_groups = axis_index_groups
 
     def __call__(
         self,
         x,
         use_running_average: tp.Optional[bool] = None,
         *,
-        ctx: tp.Optional[context.Context] = None,
+        ctx: tp.Optional[contextlib.Context] = None,
     ):
         """Normalizes the input using batch statistics.
 
         Args:
           x: the input to be normalized.
           use_running_average: if true, the statistics stored in batch_stats
             will be used instead of computing the batch statistics on the input.
@@ -318,15 +318,15 @@
         use_scale: bool = True,
         bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
         scale_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones(),
         reduction_axes: Axes = -1,
         feature_axes: Axes = -1,
         axis_name: tp.Optional[str] = None,
         axis_index_groups: tp.Any = None,
-        ctx: context.Context,
+        ctx: contextlib.Context,
     ):
         feature_shape = (num_features,)
 
         if use_scale:
             key = ctx.make_rng("params")
             self.scale = nnx.param(scale_init(key, feature_shape, param_dtype))
         else:
```

### Comparing `nnx-0.0.4/nnx/nn/stochastic.py` & `nnx-0.0.5/nnx/nn/stochastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 from typing import Optional, Sequence
 
 import jax.numpy as jnp
 from jax import lax, random
 
-from nnx import context, utils
+from nnx import contextlib, utils
 from nnx.module import Module
 
 
 @dataclasses.dataclass
 class Dropout(Module):
     """Create a dropout layer.
 
@@ -27,15 +27,15 @@
     rng_collection: str = "dropout"
 
     def __call__(
         self,
         inputs,
         *,
         deterministic: Optional[bool] = None,
-        ctx: Optional[context.Context] = None,
+        ctx: Optional[contextlib.Context] = None,
     ):
         """Applies a random dropout mask to the input.
 
         Args:
           inputs: the inputs that should be randomly masked.
           deterministic: if false the inputs are scaled by `1 / (1 - rate)` and
             masked, whereas if true, no mask is applied and the inputs are returned
```

### Comparing `nnx-0.0.4/nnx/partitioning.py` & `nnx-0.0.5/nnx/partitioning.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,89 @@
 import builtins
 import dataclasses
-import functools
 import typing as tp
-from math import e
 
 import jax
-import jax.tree_util as jtu
 import numpy as np
 
 import nnx
 
 if tp.TYPE_CHECKING:
     ellipsis = builtins.ellipsis
 else:
     ellipsis = tp.Any
 
-Predicate = tp.Callable[[tp.Tuple[str, ...], tp.Any], bool]
+FilterLiteral = tp.Union[str, type]
+Path = tp.Tuple[str, ...]
+Predicate = tp.Callable[[Path, tp.Any], bool]
 CollectionFilter = tp.Union[
-    str,
-    tp.Sequence[str],
-    Predicate,
-    ellipsis,
+    FilterLiteral, tp.Sequence[FilterLiteral], Predicate, ellipsis
 ]
 
 
 def to_predicate(collection_filter: CollectionFilter) -> Predicate:
     if isinstance(collection_filter, str):
-        return Is(collection_filter)
+        return FromCollection(collection_filter)
+    elif isinstance(collection_filter, type):
+        return OfType(collection_filter)
     elif collection_filter is Ellipsis:
         return Everything()
     elif callable(collection_filter):
         return collection_filter
     elif isinstance(collection_filter, tp.Sequence):
         return Any(collection_filter)
     else:
         raise TypeError(f"Invalid collection filter: {collection_filter}")
 
 
 @dataclasses.dataclass
-class Is:
+class FromCollection:
     collection: str
 
-    def __call__(self, path: tp.Tuple[str, ...], x: tp.Any):
+    def __call__(self, path: Path, x: tp.Any):
         if isinstance(x, nnx.Variable):
             return x.collection == self.collection
         return False
 
 
+@dataclasses.dataclass
+class OfType:
+    type: type
+
+    def __call__(self, path: Path, x: tp.Any):
+        return isinstance(x, self.type)
+
+
 class Any:
     def __init__(self, collection_filters: tp.Sequence[CollectionFilter]):
         self.predicates = tuple(
             to_predicate(collection_filter) for collection_filter in collection_filters
         )
 
-    def __call__(self, path: tp.Tuple[str, ...], x: tp.Any):
+    def __call__(self, path: Path, x: tp.Any):
         return any(predicate(path, x) for predicate in self.predicates)
 
 
 class Not:
     def __init__(self, collection_filter: CollectionFilter):
         self.predicate = to_predicate(collection_filter)
 
-    def __call__(self, path: tp.Tuple[str, ...], x: tp.Any):
+    def __call__(self, path: Path, x: tp.Any):
         return not self.predicate(path, x)
 
 
 class Everything:
-    def __call__(self, path: tp.Tuple[str, ...], x: tp.Any):
+    def __call__(self, path: Path, x: tp.Any):
         return True
 
 
-class NonConstant:
-    def __call__(self, path: tp.Tuple[str, ...], x: tp.Any):
+class NonVariable:
+    def __call__(self, path: Path, x: tp.Any):
         return not isinstance(x, nnx.Variable)
 
 
 class Buffers:
-    def __call__(self, path: tp.Tuple[str, ...], x: tp.Any):
+    def __call__(self, path: Path, x: tp.Any):
         return isinstance(x, (jax.Array, np.ndarray))
 
 
-buffers = NonConstant()
 buffers = Buffers()
```

### Comparing `nnx-0.0.4/nnx/reprlib.py` & `nnx-0.0.5/nnx/reprlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import dataclasses
 import threading
 import typing as tp
 from abc import abstractmethod
 
 
 @dataclasses.dataclass
-class Context(threading.local):
+class ReprContext(threading.local):
     indent_stack: tp.List[str] = dataclasses.field(default_factory=lambda: [""])
 
 
-CONTEXT = Context()
+REPR_CONTEXT = ReprContext()
 
 
 @dataclasses.dataclass
 class Object:
     type: tp.Union[str, type]
     start: str = "("
     end: str = ")"
@@ -40,24 +40,24 @@
 
     def __repr__(self) -> str:
         return get_repr(self)
 
 
 @contextlib.contextmanager
 def add_indent(indent: str) -> tp.Iterator[None]:
-    CONTEXT.indent_stack.append(CONTEXT.indent_stack[-1] + indent)
+    REPR_CONTEXT.indent_stack.append(REPR_CONTEXT.indent_stack[-1] + indent)
 
     try:
         yield
     finally:
-        CONTEXT.indent_stack.pop()
+        REPR_CONTEXT.indent_stack.pop()
 
 
 def get_indent() -> str:
-    return CONTEXT.indent_stack[-1]
+    return REPR_CONTEXT.indent_stack[-1]
 
 
 def get_repr(obj: Representable) -> str:
     if not isinstance(obj, Representable):
         raise TypeError(f"Object {obj!r} is not representable")
 
     iterator = obj.__nnx_repr__()
```

### Comparing `nnx-0.0.4/nnx/state.py` & `nnx-0.0.5/nnx/pytreelib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,373 +1,261 @@
+import contextlib
 import dataclasses
-import functools
+import importlib.util
+import inspect
 import typing as tp
+from abc import ABCMeta
+from copy import copy
 from functools import partial
+from types import MappingProxyType
 
 import jax
-import jax.tree_util as jtu
 
-from nnx import partitioning, reprlib, tracers
-from nnx.nn import initializers
-from nnx.nodes import register_node_type
+from nnx import nodes
+from nnx.containers import Container
 
 A = tp.TypeVar("A")
+P = tp.TypeVar("P", bound="Pytree")
 
-Leaf = tp.Any
-Path = tp.Tuple[str, ...]
-Sharding = jax.sharding.PartitionSpec
-StateDict = tp.Dict[Path, tp.Any]
-StateMapping = tp.Mapping[Path, tp.Any]
-
-
-class State(tp.Mapping[tp.Tuple[str, ...], Leaf], reprlib.Representable):
-    __slots__ = ("_mapping",)
-
-    def __init__(
-        self,
-        __input: tp.Union[
-            tp.Mapping[tp.Tuple[str, ...], Leaf],
-            tp.Iterator[tp.Tuple[tp.Tuple[str, ...], Leaf]],
-        ],
-        /,
-    ):
-        if isinstance(__input, tp.Mapping):
-            self._mapping = dict(sorted(__input.items(), key=lambda x: x[0]))
-        else:
-            self._mapping = dict(sorted(__input, key=lambda x: x[0]))
-
-    def get_collections(self) -> tp.Set[tp.Union[str, None]]:
-        return {
-            value.collection if isinstance(value, Variable) else None
-            for value in self._mapping.values()
-        }
-
-    def __getitem__(self, __key: tp.Tuple[str, ...]) -> Leaf:
-        return self._mapping[__key]
 
-    def __iter__(self) -> tp.Iterator[tp.Tuple[str, ...]]:
-        return iter(self._mapping)
-
-    def __len__(self) -> int:
-        return len(self._mapping)
-
-    def __nnx_repr__(self):
-        yield reprlib.Object(type(self), value_sep=": ", start="({", end="})")
-
-        for k, v in self._mapping.items():
-            yield reprlib.Attr(str(k), v)
-
-    @tp.overload
-    def partition(self, first: partitioning.CollectionFilter, /) -> "State":
-        ...
-
-    @tp.overload
-    def partition(
-        self,
-        first: partitioning.CollectionFilter,
-        second: partitioning.CollectionFilter,
-        /,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Tuple["State", ...]:
-        ...
-
-    def partition(
-        self,
-        first: partitioning.CollectionFilter,
-        /,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Union["State", tp.Tuple["State", ...]]:
-        *states, rest = _split_state(self, first, *filters)
-
-        if rest:
-            raise ValueError(
-                f"Non-exhaustive filters, got a non-empty remainder: "
-                f"{list(rest.keys())}.\nUse `...` to match all remaining elements."
+@contextlib.contextmanager
+def _mutable(obj: P) -> tp.Iterator[None]:
+    vars(obj)["_pytree__is_mutable"] = True
+    try:
+        yield
+    finally:
+        del vars(obj)["_pytree__is_mutable"]
+
+
+@contextlib.contextmanager
+def _initializing(obj: P) -> tp.Iterator[None]:
+    vars(obj)["_pytree__initializing"] = True
+    try:
+        yield
+    finally:
+        del vars(obj)["_pytree__initializing"]
+
+
+class PytreeMeta(ABCMeta):
+    if not tp.TYPE_CHECKING:
+
+        def __call__(cls: tp.Type[P], *args: tp.Any, **kwargs: tp.Any) -> P:
+            return cls.call(*args, **kwargs)
+
+    def call(cls: tp.Type[P], *args: tp.Any, **kwargs: tp.Any) -> P:
+        obj: P = cls.__new__(cls, *args, **kwargs)
+        vars(obj)["_pytree__sorted_fields"] = ["_pytree__sorted_fields"]
+
+        with _mutable(obj), _initializing(obj):
+            obj.__init__(*args, **kwargs)
+
+        if dataclasses.is_dataclass(obj):
+            assert isinstance(obj, Pytree)
+            for field in dataclasses.fields(obj):
+                if "nnx_container_fn" not in field.metadata:
+                    continue
+
+                container_fn = field.metadata["nnx_container_fn"]
+                value = vars(obj)[field.name]
+                value = container_fn(value)
+                vars(obj)[field.name] = value
+
+        vars(obj)["_pytree__sorted_fields"] = sorted(vars(obj))
+
+        return obj
+
+
+class Pytree(metaclass=PytreeMeta):
+    _pytree__is_mutable: bool
+    _pytree__class_is_mutable: bool
+    _pytree__sorted_fields: tp.Tuple[str, ...]
+
+    if not tp.TYPE_CHECKING:
+
+        def __getattribute__(self, name: str) -> tp.Any:
+            value = object.__getattribute__(self, name)
+            if isinstance(value, Container):
+                return value.value
+            return value
+
+        def __setattr__(self, name: str, value: tp.Any) -> None:
+            self._setattr(name, value)
+
+    def _setattr(self: P, name: str, value: tp.Any):
+        vars_dict = vars(self)
+        if "_pytree__initializing" in vars_dict:
+            pass
+        elif name not in vars_dict:
+            raise AttributeError(r"Cannot add new fields to an initialized Pytree")
+        elif (
+            "_pytree__is_mutable" not in vars_dict
+            and not self._pytree__class_is_mutable
+        ):
+            raise AttributeError(
+                f"{type(self)} is immutable, trying to update field {name}"
             )
 
-        if len(states) == 1:
-            states = State(states[0])
+        if name in vars_dict and isinstance(vars_dict[name], Container):
+            vars_dict[name] = vars_dict[name].replace_value(value)
         else:
-            states = tuple(State(state) for state in states)
-        return states
-
-    @tp.overload
-    def filter(
-        self,
-        first: partitioning.CollectionFilter,
-        /,
-    ) -> "State":
-        ...
-
-    @tp.overload
-    def filter(
-        self,
-        first: partitioning.CollectionFilter,
-        second: partitioning.CollectionFilter,
-        /,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Tuple["State", ...]:
-        ...
-
-    def filter(
-        self,
-        first: partitioning.CollectionFilter,
-        /,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Union["State", tp.Tuple["State", ...]]:
-        (*states, _rest) = _split_state(self, first, *filters)
-
-        assert len(states) == len(filters) + 1
-
-        if len(states) == 1:
-            states = State(states[0])
-        else:
-            states = tuple(State(state) for state in states)
-
-        return states
-
-    @staticmethod
-    def merge(state: "State", /, *states: "State") -> "State":
-        states = (state, *states)
-
-        if len(states) == 1:
-            return states[0]
-
-        new_state: StateDict = {}
-
-        for state in states:
-            new_state.update(state)
-
-        return State(new_state)
-
-    def __or__(self, other: "State") -> "State":
-        if not other:
-            return self
-        return State.merge(self, other)
-
-    def __sub__(self, other: "State") -> "State":
-        if not other:
-            return self
-
-        # create new State via __new__ to avoid __init__ sorting
-        _mapping = {k: v for k, v in self.items() if k not in other}
-        state = object.__new__(State)
-        state._mapping = _mapping
-        return state
-
-
-def _state_flatten_with_keys(
-    x: State,
-):
-    children = tuple((jtu.DictKey(key), value) for key, value in x.items())
-    return children, tuple(x.keys())
-
-
-def _state_unflatten(
-    keys: tp.Tuple[Path, ...],
-    leaves: tp.Tuple[Leaf, ...],
-):
-    state = object.__new__(State)
-    state._mapping = dict(zip(keys, leaves))
-    return state
-
-
-jax.tree_util.register_pytree_with_keys(
-    State, _state_flatten_with_keys, _state_unflatten
-)
-
-
-def _split_state(
-    state: StateMapping,
-    *filters: partitioning.CollectionFilter,
-) -> tp.Tuple[StateDict, ...]:
-    predicates = tuple(map(partitioning.to_predicate, filters))
-
-    # we have n + 1 states, where n is the number of predicates
-    # the last state is for values that don't match any predicate
-    states: tp.Tuple[StateDict, ...] = tuple({} for _ in range(len(predicates) + 1))
-
-    for path, value in state.items():
-        for i, predicate in enumerate(predicates):
-            if predicate(path, value):
-                states[i][path] = value
-                break
+            if isinstance(value, Container):
+                value = value.copy()
+            vars_dict[name] = value
+
+    def __init_subclass__(cls, mutable: bool = False):
+        super().__init_subclass__()
+        # init class variables
+        cls._pytree__is_mutable = False
+        cls._pytree__class_is_mutable = mutable
+
+        # TODO: clean up this in the future once minimal supported version is 0.4.7
+        if hasattr(jax.tree_util, "register_pytree_with_keys"):
+            if (
+                "flatten_func"
+                in inspect.signature(jax.tree_util.register_pytree_with_keys).parameters
+            ):
+                jax.tree_util.register_pytree_with_keys(
+                    cls,
+                    partial(
+                        cls._pytree__flatten,
+                        with_key_paths=True,
+                    ),
+                    cls._pytree__unflatten,
+                    flatten_func=partial(
+                        cls._pytree__flatten,
+                        with_key_paths=False,
+                    ),
+                )
+            else:
+                jax.tree_util.register_pytree_with_keys(
+                    cls,
+                    partial(
+                        cls._pytree__flatten,
+                        with_key_paths=True,
+                    ),
+                    cls._pytree__unflatten,
+                )
         else:
-            # if we didn't break, set leaf to last state
-            states[-1][path] = value
-
-    return states
-
-
-class Node(tp.Generic[A], reprlib.Representable):
-    __slots__ = ("_value",)
-
-    def __init__(self, value: A):
-        self._value = value
-
-    @property
-    def value(self) -> A:
-        return self._value
-
-    def __nnx_repr__(self):
-        yield reprlib.Object(type=type(self))
-        yield reprlib.Attr(
-            "value", repr(self._value) if isinstance(self._value, str) else self._value
-        )
-
-    def copy(self) -> "Node[A]":
-        return Node(self._value)
-
-    def replace(
-        self,
-        **kwargs: tp.Any,
-    ) -> "Node[tp.Any]":
-        updates: tp.Dict[str, tp.Any] = {"value": self._value}
-        updates.update(kwargs)
-        return Node(**updates)
-
-
-def _node_flatten(
-    x: Node[tp.Any],
-    *,
-    with_keys: bool,
-):
-    if with_keys:
-        node = (jtu.GetAttrKey("value"), x._value)
-    else:
-        node = x._value
-
-    return (node,), None
-
-
-def _node_unflatten(metadata: None, children: tp.Tuple[A]) -> Node[A]:
-    return Node(children[0])
-
-
-jtu.register_pytree_with_keys(
-    Node,
-    partial(_node_flatten, with_keys=True),
-    _node_unflatten,
-    flatten_func=partial(_node_flatten, with_keys=False),
-)
-
-
-@dataclasses.dataclass
-class VarMetadata(tp.Generic[A]):
-    value: A
-    sharding: Sharding
-
-
-def with_partitioning(
-    initializer: initializers.Initializer,
-    sharding: Sharding,
-) -> initializers.Initializer:
-    @functools.wraps(initializer)
-    def wrapper(*args):
-        return VarMetadata(initializer(*args), sharding)
-
-    return wrapper  # type: ignore
-
-
-def var_metadata(value: A, sharding: Sharding) -> VarMetadata[A]:
-    return VarMetadata(value, sharding)
+            jax.tree_util.register_pytree_node(
+                cls,
+                partial(
+                    cls._pytree__flatten,
+                    with_key_paths=False,
+                ),
+                cls._pytree__unflatten,
+            )
 
+        # flax serialization support
+        if importlib.util.find_spec("flax") is not None:
+            from flax import serialization
 
-class Variable(Node[A]):
-    __slots__ = ("_collection", "_sharding")
+            serialization.register_serialization_state(
+                cls, cls._to_flax_state_dict, cls._from_flax_state_dict
+            )
 
-    def __init__(
-        self,
-        value: A,
-        collection: str,
-        sharding: tp.Optional[Sharding],
+    @classmethod
+    def _pytree__flatten(
+        cls,
+        pytree: "Pytree",
+        *,
+        with_key_paths: bool,
     ):
-        self._value = value
-        self._collection = collection
-        self._sharding = sharding
-
-    @property
-    def collection(self) -> str:
-        return self._collection
-
-    @property
-    def sharding(self) -> tp.Optional[Sharding]:
-        return self._sharding
-
-    def __nnx_repr__(self):
-        yield reprlib.Object(type=type(self))
-        yield reprlib.Attr("collection", repr(self._collection))
-        yield reprlib.Attr(
-            "value", repr(self._value) if isinstance(self._value, str) else self._value
-        )
-        if self._sharding is not None:
-            yield reprlib.Attr("sharding", self._sharding)
-
-    def copy(self) -> "Variable[A]":
-        return Variable(self._value, self._collection, self._sharding)
-
-    def replace(
-        self,
-        **kwargs: tp.Any,
-    ) -> "Variable[A]":
-        updates: tp.Dict[str, tp.Any] = {
-            "value": self._value,
-            "collection": self._collection,
-            "sharding": self._sharding,
+        all_vars = vars(pytree)
+        static = {}
+        node_values = []
+        node_names = []
+
+        for field in pytree._pytree__sorted_fields:
+            value = all_vars[field]
+
+            if nodes.is_node(value):
+                node_names.append(field)
+                if with_key_paths:
+                    node_values.append((jax.tree_util.GetAttrKey(field), value))
+                else:
+                    node_values.append(value)
+            else:
+                static[field] = value
+
+        return node_values, (tuple(node_names), MappingProxyType(static))
+
+    @classmethod
+    def _pytree__unflatten(
+        cls: tp.Type[P],
+        metadata: tp.Tuple[tp.Tuple[str, ...], tp.Mapping[str, tp.Any]],
+        node_values: tp.Tuple[tp.Any, ...],
+    ) -> P:
+        node_names, static_fields = metadata
+        pytree = object.__new__(cls)
+        pytree.__dict__.update(zip(node_names, node_values))
+        pytree.__dict__.update(static_fields)
+        return pytree
+
+    @classmethod
+    def _to_flax_state_dict(cls, pytree: "Pytree") -> tp.Dict[str, tp.Any]:
+        from flax import serialization
+
+        state_dict = {
+            name: serialization.to_state_dict(getattr(pytree, name))
+            for name, value in vars(pytree).items()
+            if nodes.is_node(value)
         }
-        updates.update(kwargs)
-        return Variable(**updates)
-
-
-def _variable_flatten(
-    x: Variable[tp.Any],
-    *,
-    with_keys: bool,
-):
-    if with_keys:
-        node = (jtu.GetAttrKey("value"), x._value)
-    else:
-        node = x._value
-
-    return (node,), (x._collection, x._sharding)
-
+        return state_dict
 
-def _variable_unflatten(
-    metadata: tp.Tuple[str, tp.Optional[Sharding]], children: tp.Tuple[A]
-) -> Variable[A]:
-    return Variable(children[0], *metadata)
-
-
-jtu.register_pytree_with_keys(
-    Variable,
-    partial(_variable_flatten, with_keys=True),
-    _variable_unflatten,
-    flatten_func=partial(_variable_flatten, with_keys=False),
-)
-
-
-def var(
-    collection: str,
-    value: tp.Union[A, VarMetadata[A]],
-    sharding: tp.Optional[Sharding] = None,
-) -> A:
-    return Variable(  # type: ignore
-        value,
-        collection=collection,
-        sharding=sharding,
-    )
+    @classmethod
+    def _from_flax_state_dict(
+        cls,
+        pytree: P,
+        state: tp.Dict[str, tp.Any],
+    ) -> P:
+        """Restore the state of a data class."""
+        from flax import serialization
+
+        state = state.copy()  # copy the state so we can pop the restored fields.
+        updates = {}
+        for name, value in vars(pytree).items():
+            if not nodes.is_node(value):
+                continue
+            if name not in state:
+                raise ValueError(
+                    f"Missing field {name} in state dict while restoring"
+                    f" an instance of {type(pytree).__name__},"
+                    f" at path {serialization.current_path()}"
+                )
+            value_state = state.pop(name)
+            updates[name] = serialization.from_state_dict(value, value_state, name=name)
+        if state:
+            names = ",".join(state.keys())
+            raise ValueError(
+                f'Unknown field(s) "{names}" in state dict while'
+                f" restoring an instance of {type(pytree).__name__}"
+                f" at path {serialization.current_path()}"
+            )
+        return pytree.replace(**updates)
 
+    def replace(self: P, **kwargs: tp.Any) -> P:
+        """
+        Replace the values of the fields of the object with the values of the
+        keyword arguments. If the object is a dataclass, `dataclasses.replace`
+        will be used. Otherwise, a new object will be created with the same
+        type as the original object.
+        """
+        if dataclasses.is_dataclass(self):
+            return dataclasses.replace(self, **kwargs)
 
-def param(
-    value: tp.Union[A, VarMetadata[A]],
-    sharding: tp.Optional[Sharding] = None,
-) -> A:
-    return var("params", value, sharding=sharding)
+        unknown_keys = set(kwargs) - set(vars(self))
+        if unknown_keys and not self._pytree__class_is_mutable:
+            raise ValueError(
+                f"Trying to replace unknown fields {unknown_keys} "
+                f"for '{type(self).__name__}'"
+            )
 
+        pytree = copy(self)
+        with _mutable(pytree):
+            for key, value in kwargs.items():
+                setattr(pytree, key, value)
 
-def node(value: A) -> A:
-    return Node(value)  # type: ignore
+        return pytree
 
 
-# register nodes
-register_node_type(State)
-register_node_type(Node)
+# register node types
+nodes.register_node_type(Pytree)
```

### Comparing `nnx-0.0.4/nnx/tracers.py` & `nnx-0.0.5/nnx/tracers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.4/nnx/transforms.py` & `nnx-0.0.5/nnx/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 import typing as tp
 
 import jax
 import jax.stages
 
-from nnx import context, partitioning, tracers
+from nnx import contextlib, partitioning, tracers
 from nnx.module import Module, ModuleDef, PureModule
 from nnx.state import State
 
 A = tp.TypeVar("A")
 F = tp.TypeVar("F", bound=tp.Callable[..., tp.Any])
 G = tp.TypeVar("G", bound=tp.Callable[..., tp.Any])
 
@@ -22,15 +22,15 @@
         self,
         fun: tp.Callable[..., tp.Any],
         stateful: bool,
         **jit_kwargs,
     ):
         @functools.partial(jax.jit, **jit_kwargs)
         def jitted_fn(pure_module: PureModule[Module], *args, **kwargs):
-            if "ctx" in kwargs and isinstance(kwargs["ctx"], context.PureContext):
+            if "ctx" in kwargs and isinstance(kwargs["ctx"], contextlib.PureContext):
                 kwargs["ctx"] = kwargs["ctx"].merge()
 
             nnx_trace = tracers.get_top_trace((args, kwargs))
             with tracers.nnx_trace(nnx_trace):
                 module = pure_module.merge()
                 out = fun(module, *args, **kwargs)
 
@@ -42,15 +42,15 @@
 
         self.jitted_fn = jitted_fn
         self.stateful = stateful
 
     def __call__(self, module: tp.Any, *args, **kwargs):
         if not isinstance(module, Module):
             raise TypeError(f"Expected Module, got {type(module).__name__}")
-        if "ctx" in kwargs and isinstance(kwargs["ctx"], context.Context):
+        if "ctx" in kwargs and isinstance(kwargs["ctx"], contextlib.Context):
             kwargs["ctx"] = kwargs["ctx"].partition()
 
         pure_module = module.partition()
         out = self.jitted_fn(pure_module, *args, **kwargs)
         if self.stateful:
             updates: State
             updates, out = out
```

### Comparing `nnx-0.0.4/nnx/utils.py` & `nnx-0.0.5/nnx/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,10 +11,11 @@
             return arg
     raise ValueError("No non-None arguments found.")
 
 
 def has_keyword_arg(func: tp.Callable[..., tp.Any], name: str) -> bool:
     """Return True if func has keyword-only arguments with the given name."""
     return any(
-        param.name == name and param.kind == inspect.Parameter.KEYWORD_ONLY
+        param.name == name
+        and param.kind in (param.KEYWORD_ONLY, param.POSITIONAL_OR_KEYWORD)
         for param in inspect.signature(func).parameters.values()
     )
```

### Comparing `nnx-0.0.4/pyproject.toml` & `nnx-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nnx"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 jax = "*"
```

### Comparing `nnx-0.0.4/PKG-INFO` & `nnx-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnx
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Cristian Garcia
 Author-email: cgarcia.e88@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -66,23 +66,25 @@
         self.b = nnx.param(jnp.zeros((dout,)))
         self.count = nnx.var("counts", 0)  # track the number of calls
 
     def __call__(self, x):
         self.count += 1
         return x @ self.w + self.b
 
-ctx = nnx.Context(params=jax.random.PRNGKey(0))
-model = Linear(din=12, dout=2, ctx=ctx)
+model = Linear(din=12, dout=2, ctx=nnx.context(0))
 
 # Forward pass and verify the call count
 x = jnp.ones((8, 12))
 y = model(x)
 assert model.count == 1
 ```
 
+In this example `nnx.context(0)` create a `PRNGKey` for `params` with seed `0`, this is used by `make_rng`
+inside `__init__` to generate a random key to initialize the parameters.
+
 ### Training
 
 Here we show case two different approaches to training the model defined in the previous secition. The first one uses lifted transforms and the second one uses the functional API. Both approaches are equivalent and produce the same results.
 
 <details><summary>Lifted Transforms</summary>
 
 In this example, we uset the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD) and `train_step` doesn't require a return statement in this case as the model's state is automatically updated.
@@ -187,16 +189,15 @@
         self.submodule = nnx.Linear(2, 4, ctx=ctx)
         # static attributes
         self.int = 1
         self.float = 2.0
         self.str = "hello"
         self.list = [1, 2, 3]
 
-ctx = nnx.Context(jax.random.PRNGKey(0))
-model = Foo(din=12, dout=2, ctx=ctx)
+model = Foo(din=12, dout=2, ctx=nnx.context(0))
 ```
 As shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Map` Modules.
 
 ### Functional API
 
 NNX Modules are not pytrees so they cannot be passed to JAX transformations. In order to interact with JAX, a Module must be partitioned into a `State` and `ModuleDef` objects. The `State` object is a flat dictionary-like pytree structure that contains all the deduplicated node attributes, and the `ModuleDef` contains the static attributes and structural information needed to reconstruct the Module.
 
@@ -295,16 +296,15 @@
         self.b = nnx.param(jnp.zeros((dout,)))
 
     def __call__(self, x):
         y = x @ self.w + self.b
         self.y = nnx.var("intermediates", y)
         return y
 
-ctx = nnx.Context(jax.random.PRNGKey(0))
-model = Linear(12, 2, ctx=ctx)
+model = Linear(12, 2, ctx=nnx.context(0))
 ```
 Since `y` is only created when the module is called, it is not available upon initialization. However, once you call the module `y` will be created. It is recommended that you use `pop_state` to retrieve temporary collections like `intermediates`:
 
 ```python
 y = model(jnp.ones((8, 12)))
 intermediates = model.pop_state("intermediates")
 ```
@@ -399,14 +399,14 @@
 
 In this example, the `Model` module contains two instances of the `Block` module. Each instance shares the same `nnx.Linear` module. To run the model, you can use the Context `flags` argument to set the `use_running_average` flag for all `BatchNorm` modules.
 
 Here's an example of computing the loss for a `Model` instance:
 
 ```python
 def loss_fn(model: Model, x: jax.Array, y: jax.Array):
-    ctx = nnx.Context(flags=dict(use_running_average=True))
+    ctx = nnx.context(flags=dict(use_running_average=True))
     y_pred = model(x, ctx=ctx)
     return jnp.mean((y - y_pred) ** 2)
 ```
 
 It's important to note that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.
```

