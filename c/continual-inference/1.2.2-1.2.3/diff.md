# Comparing `tmp/continual-inference-1.2.2.tar.gz` & `tmp/continual-inference-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continual-inference-1.2.2.tar", last modified: Fri Jun  2 15:30:11 2023, max compression
+gzip compressed data, was "continual-inference-1.2.3.tar", last modified: Fri Jun 16 09:28:24 2023, max compression
```

## Comparing `continual-inference-1.2.2.tar` & `continual-inference-1.2.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.422211 continual-inference-1.2.2/
--rw-r--r--   0 au478108 (794351465) 357318537    36011 2023-06-02 15:30:11.421918 continual-inference-1.2.2/PKG-INFO
--rw-r--r--   0 au478108 (794351465) 357318537    30378 2023-05-24 13:22:59.000000 continual-inference-1.2.2/README.md
-drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.416265 continual-inference-1.2.2/continual/
--rw-r--r--   0 au478108 (794351465) 357318537      359 2023-06-02 07:52:08.000000 continual-inference-1.2.2/continual/__about__.py
--rw-r--r--   0 au478108 (794351465) 357318537     1492 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/__init__.py
--rw-r--r--   0 au478108 (794351465) 357318537     6550 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/closure.py
--rw-r--r--   0 au478108 (794351465) 357318537    35637 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/container.py
--rw-r--r--   0 au478108 (794351465) 357318537    24313 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/conv.py
--rw-r--r--   0 au478108 (794351465) 357318537     7742 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/convert.py
--rw-r--r--   0 au478108 (794351465) 357318537     4803 2023-03-24 09:21:27.000000 continual-inference-1.2.2/continual/delay.py
--rw-r--r--   0 au478108 (794351465) 357318537     4293 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/linear.py
--rw-r--r--   0 au478108 (794351465) 357318537     1135 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/logging.py
--rw-r--r--   0 au478108 (794351465) 357318537    14683 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/module.py
-drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.419000 continual-inference-1.2.2/continual/multihead_attention/
--rw-r--r--   0 au478108 (794351465) 357318537      149 2022-07-04 15:01:36.000000 continual-inference-1.2.2/continual/multihead_attention/__init__.py
--rw-r--r--   0 au478108 (794351465) 357318537    24049 2022-12-02 09:07:24.000000 continual-inference-1.2.2/continual/multihead_attention/mha_base.py
--rw-r--r--   0 au478108 (794351465) 357318537    14015 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/multihead_attention/retroactive_mha.py
--rw-r--r--   0 au478108 (794351465) 357318537    15027 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/multihead_attention/single_output_mha.py
--rw-r--r--   0 au478108 (794351465) 357318537    15136 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/onnx.py
--rw-r--r--   0 au478108 (794351465) 357318537    46663 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/pooling.py
--rw-r--r--   0 au478108 (794351465) 357318537     7056 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/positional_encoding.py
--rw-r--r--   0 au478108 (794351465) 357318537     2657 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/ptflops.py
--rw-r--r--   0 au478108 (794351465) 357318537    28266 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/rnn.py
--rw-r--r--   0 au478108 (794351465) 357318537     1813 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/shape.py
--rw-r--r--   0 au478108 (794351465) 357318537     1604 2023-05-24 13:22:59.000000 continual-inference-1.2.2/continual/skip.py
--rw-r--r--   0 au478108 (794351465) 357318537    22532 2023-06-02 07:52:08.000000 continual-inference-1.2.2/continual/transformer.py
--rw-r--r--   0 au478108 (794351465) 357318537     7059 2022-12-21 08:00:31.000000 continual-inference-1.2.2/continual/utils.py
-drwxr-xr-x   0 au478108 (794351465) 357318537        0 2023-06-02 15:30:11.421240 continual-inference-1.2.2/continual_inference.egg-info/
--rw-r--r--   0 au478108 (794351465) 357318537    36011 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/PKG-INFO
--rw-r--r--   0 au478108 (794351465) 357318537      815 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/SOURCES.txt
--rw-r--r--   0 au478108 (794351465) 357318537        1 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/dependency_links.txt
--rw-r--r--   0 au478108 (794351465) 357318537      345 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/requires.txt
--rw-r--r--   0 au478108 (794351465) 357318537       10 2023-06-02 15:30:11.000000 continual-inference-1.2.2/continual_inference.egg-info/top_level.txt
--rw-r--r--   0 au478108 (794351465) 357318537       38 2023-06-02 15:30:11.422336 continual-inference-1.2.2/setup.cfg
--rw-r--r--   0 au478108 (794351465) 357318537     2938 2022-12-21 08:00:31.000000 continual-inference-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:28:24.243167 continual-inference-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 09:26:24.000000 continual-inference-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31590 2023-06-16 09:28:24.243167 continual-inference-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30378 2023-06-16 09:26:24.000000 continual-inference-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:28:24.239167 continual-inference-1.2.3/continual/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35637 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:28:24.239167 continual-inference-1.2.3/continual/multihead_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/multihead_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24049 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/multihead_attention/mha_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/multihead_attention/retroactive_mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/multihead_attention/single_output_mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46696 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/ptflops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28266 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-16 09:26:24.000000 continual-inference-1.2.3/continual/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:28:24.243167 continual-inference-1.2.3/continual_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31590 2023-06-16 09:28:24.000000 continual-inference-1.2.3/continual_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-16 09:28:24.000000 continual-inference-1.2.3/continual_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:28:24.000000 continual-inference-1.2.3/continual_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 09:28:24.000000 continual-inference-1.2.3/continual_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 09:28:24.000000 continual-inference-1.2.3/continual_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:28:24.243167 continual-inference-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-16 09:26:24.000000 continual-inference-1.2.3/setup.py
```

### Comparing `continual-inference-1.2.2/PKG-INFO` & `continual-inference-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,570 +1,15 @@
 Metadata-Version: 2.1
 Name: continual-inference
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python library for Continual Inference Networks in PyTorch
 Home-page: https://github.com/lukashedegaard/continual-inference
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
-Description: <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/logo_name.svg" style="width: 400px;">
-        
-        __A Python library for Continual Inference Networks in PyTorch__
-        
-        [Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/README.html#quick-start) • 
-        [Docs](https://continual-inference.readthedocs.io/en/latest/generated/README.html) • 
-        [Principles](https://continual-inference.readthedocs.io/en/latest/generated/README.html#library-principles) • 
-        [Paper](https://arxiv.org/abs/2204.03418) • 
-        [Examples](https://continual-inference.readthedocs.io/en/latest/generated/README.html#composition-examples) • 
-        [Modules](https://continual-inference.readthedocs.io/en/latest/common/modules.html) • 
-        [Model Zoo](https://continual-inference.readthedocs.io/en/latest/generated/README.html#model-zoo-and-benchmarks) • 
-        [Contribute](https://continual-inference.readthedocs.io/en/latest/generated/CONTRIBUTING.html) • 
-        [License](https://github.com/LukasHedegaard/continual-inference/blob/main/LICENSE)
-        
-        <div>
-          <a href="https://pypi.org/project/continual-inference/" style="display:inline-block;">
-            <img src="https://img.shields.io/pypi/pyversions/continual-inference" height="20" >
-          </a>
-          <a href="https://badge.fury.io/py/continual-inference" style="display:inline-block;">
-            <img src="https://badge.fury.io/py/continual-inference.svg" height="20" >
-          </a>
-          <a href="https://continual-inference.readthedocs.io/en/latest/generated/README.html" style="display:inline-block;">
-            <img src="https://readthedocs.org/projects/continual-inference/badge/?version=latest" alt="Documentation Status" height="20"/>
-          </a>
-          <a href="https://pepy.tech/project/continual-inference" style="display:inline-block;">
-            <img src="https://pepy.tech/badge/continual-inference" height="20">
-          </a>
-          <a href="https://codecov.io/gh/LukasHedegaard/continual-inference" style="display:inline-block;">
-            <img src="https://codecov.io/gh/LukasHedegaard/continual-inference/branch/main/graph/badge.svg?token=XW1UQZSEOG" height="20"/>
-          </a>
-          <a href="https://opensource.org/licenses/Apache-2.0" style="display:inline-block;">
-            <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" height="20">
-          </a>
-          <!-- <a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
-            <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
-          </a> -->
-          <a href="https://github.com/psf/black" style="display:inline-block;">
-            <img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="20">
-          </a>
-          <a href="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/overview/main" style="display:inline-block;">
-            <img src="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/badge/main" alt="We match PyTorch interfaces exactly. Method arguments named 'input' reduce the codefactor to 'A-'" height="20" />
-          </a>
-        </div>
-        
-        ## Continual Inference Networks ensure efficient stream processing
-        Many of our favorite Deep Neural Network architectures (e.g., [CNNs](https://arxiv.org/abs/2106.00050) and [Transformers](https://arxiv.org/abs/2201.06268)) were built with offline-processing for offline processing. Rather than processing inputs one sequence element at a time, they require the whole (spatio-)temporal sequence to be passed as a single input.
-        Yet, **many important real-life applications need online predictions on a continual input stream**. 
-        While CNNs and Transformers can be applied by re-assembling and passing sequences within a sliding window, this is _inefficient_ due to the redundant intermediary computations from overlapping clips.
-        
-        **Continual Inference Networks** (CINs) are built to ensure efficient stream processing by employing an alternative computational ordering, which allows sequential computations without the use of sliding window processing.
-        In general, CINs requires approx. _L_ ×  fewer FLOPs per prediction compared to sliding window-based inference with non-CINs, where _L_ is the corresponding sequence length of a non-CIN network. For more details, check out the videos below describing Continual 3D CNNs [[1](https://arxiv.org/abs/2106.00050)] and Transformers [[2](https://arxiv.org/abs/2201.06268)].
-        
-        
-        <div align="center">
-          <a href="http://www.youtube.com/watch?feature=player_embedded&v=Jm2A7dVEaF4" target="_blank">
-             <img src="http://img.youtube.com/vi/Jm2A7dVEaF4/hqdefault.jpg" alt="Presentation of Continual 3D CNNs" style="width:240px;height:auto;" />
-          </a>
-          <a href="http://www.youtube.com/watch?feature=player_embedded&v=gy802Tlp-eQ" target="_blank">
-             <img src="http://img.youtube.com/vi/gy802Tlp-eQ/hqdefault.jpg" alt="Presentation of Continual Transformers" style="width:240px;height:auto;" />
-          </a>
-        </div>
-        
-        ## News
-        - 2022-12-02: ONNX compatibility for all modules is available from v1.0.0. See [test_onnx.py](tests/continual/test_onnx.py) for examples.
-        
-        
-        ## Quick-start
-        
-        ### Install 
-        ```bash
-        pip install continual-inference
-        ```
-        
-        
-        
-        ### Example
-        `co` modules are weight-compatible drop-in replacement for `torch.nn`, enhanced with the capability of efficient _continual inference_:
-        
-        ```python3
-        import torch
-        import continual as co
-                                                                   
-        #                      B, C, T, H, W
-        example = torch.randn((1, 1, 5, 3, 3))
-        
-        conv = co.Conv3d(in_channels=1, out_channels=1, kernel_size=(3, 3, 3))
-        
-        # Same exact computation as torch.nn.Conv3d ✅
-        output = conv(example)
-        
-        # But can also perform online inference efficiently 🚀
-        firsts = conv.forward_steps(example[:, :, :4])
-        last = conv.forward_step(example[:, :, 4])
-        
-        assert torch.allclose(output[:, :, : conv.delay], firsts)
-        assert torch.allclose(output[:, :, conv.delay], last)
-        
-        # Temporal properties
-        assert conv.receptive_field == 3
-        assert conv.delay == 2
-        ```
-        
-        See the [network composition](#composition) and [model zoo](#model-zoo-and-benchmarks) sections for additional examples.
-        
-        ## Library principles
-        
-        ### Forward modes
-        The library components feature three distinct forward modes, which are handy for different situations, namely `forward`, `forward_step`, and `forward_steps`:
-        
-        #### `forward(input)`
-        Performs a forward computation over multiple time-steps. This function is identical to the corresponding module in _torch.nn_, ensuring cross-compatibility. Moreover, it's handy for efficient training on clip-based data.
-        
-        ```
-                 O            (O: output)
-                 ↑ 
-                 N            (N: network module)
-                 ↑ 
-         -----------------    (-: aggregation)
-         P   I   I   I   P    (I: input frame, P: padding)
-        ```
-        
-        
-        #### `forward_step(input, update_state=True)`
-        Performs a forward computation for a single frame and (optionally) updates internal states accordingly. This function performs efficient continual inference.
-        
-        ```
-        O+S O+S O+S O+S   (O: output, S: updated internal state)
-         ↑   ↑   ↑   ↑ 
-         N   N   N   N    (N: network module)
-         ↑   ↑   ↑   ↑ 
-         I   I   I   I    (I: input frame)
-        ```
-        
-        #### `forward_steps(input, pad_end=False, update_state=True)`
-        Performs a forward computation across multiple time-steps while updating internal states for continual inference (if update_state=True).
-        Start-padding is always accounted for, but end-padding is omitted per default in expectance of the next input step. It can be added by specifying pad_end=True. If so, the output-input mapping the exact same as that of forward.
-        ```
-                 O            (O: output)
-                 ↑ 
-         -----------------    (-: aggregation)
-         O  O+S O+S O+S  O    (O: output, S: updated internal state)
-         ↑   ↑   ↑   ↑   ↑
-         N   N   N   N   N    (N: network module)
-         ↑   ↑   ↑   ↑   ↑
-         P   I   I   I   P    (I: input frame, P: padding)
-        ```
-        
-        #### `__call__`
-        Per default, the `__call__` function operates identically to _torch.nn_ and executes forward. We supply two options for changing this behavior, namely the _call_mode_ property and the _call_mode_ context manager. An example of their use follows:
-        
-        ```python
-        timeseries = torch.randn(batch, channel, time)
-        timestep = timeseries[:, :, 0]
-        
-        net(timeseries)  # Invokes net.forward(timeseries)
-        
-        # Assign permanent call_mode property
-        net.call_mode = "forward_step"
-        net(timestep)  # Invokes net.forward_step(timestep)
-        
-        # Assign temporary call_mode with context manager
-        with co.call_mode("forward_steps"):
-            net(timeseries)  # Invokes net.forward_steps(timeseries)
-        
-        net(timestep)  # Invokes net.forward_step(timestep) again
-        ```
-        
-        ### Composition
-        
-        Continual Inference Networks require strict handling of internal data delays to guarantee correspondence between [forward modes](#forward-modes). While it is possible to compose neural networks by defining _forward_, _forward_step_, and _forward_steps_ manually, correct handling of delays is cumbersome and time-consuming. Instead, we provide a rich interface of container modules, which handles delays automatically. On top of `co.Sequential` (which is a drop-in replacement of _torch.nn.Sequential_), we provide modules for handling parallel and conditional dataflow. 
-        
-        - [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
-        - [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
-        - [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
-        - [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
-        - [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
-        - [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
-        - [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
-        - [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
-        
-        
-        #### Composition examples:
-        
-        <details>
-        <summary><b>Residual module</b></summary>
-        
-        Short-hand:
-        ```python3
-        residual = co.Residual(co.Conv3d(32, 32, kernel_size=3, padding=1))
-        ```
-        
-        Explicit:
-        ```python3
-        residual = co.Sequential(
-            co.Broadcast(2),
-            co.Parallel(
-                co.Conv3d(32, 32, kernel_size=3, padding=1),
-                co.Delay(2),
-            ),
-            co.Reduce("sum"),
-        )
-        ```
-        
-        </details>
-        
-        <details>
-        <summary><b>3D MobileNetV2 Inverted residual block</b></summary>
-        
-        Continual 3D version of the [MobileNetV2 Inverted residual block](https://arxiv.org/pdf/1801.04381.pdf).
-        
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/mb_conv.png" style="width: 15vw; min-width: 200px;">
-          <br>
-          MobileNetV2 Inverted residual block. Source: https://arxiv.org/pdf/1801.04381.pdf
-        </div>
-        
-        ```python3
-        mb_conv = co.Residual(
-            co.Sequential(
-              co.Conv3d(32, 64, kernel_size=(1, 1, 1)),
-              nn.BatchNorm3d(64),
-              nn.ReLU6(),
-              co.Conv3d(64, 64, kernel_size=(3, 3, 3), padding=(1, 1, 1), groups=64),
-              nn.ReLU6(),
-              co.Conv3d(64, 32, kernel_size=(1, 1, 1)),
-              nn.BatchNorm3d(32),
-            )
-        )
-        ```
-        
-        </details>
-        
-        <details>
-        <summary><b>3D Squeeze-and-Excitation module</b></summary>
-        
-        Continual 3D version of the [Squeeze-and-Excitation module](https://arxiv.org/pdf/1709.01507.pdf)
-        
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/se_block.png" style="width: 15vw; min-width: 200px;">
-          <br>
-          Squeeze-and-Excitation block. 
-          Scale refers to a broadcasted element-wise multiplication.
-          Adapted from: https://arxiv.org/pdf/1709.01507.pdf
-        </div>
-        
-        ```python3
-        se = co.Residual(
-            co.Sequential(
-                OrderedDict([
-                    ("pool", co.AdaptiveAvgPool3d((1, 1, 1), kernel_size=7)),
-                    ("down", co.Conv3d(256, 16, kernel_size=1)),
-                    ("act1", nn.ReLU()),
-                    ("up", co.Conv3d(16, 256, kernel_size=1)),
-                    ("act2", nn.Sigmoid()),
-                ])
-            ),
-            reduce="mul",
-        )
-        ```
-        
-        </details>
-        
-        <details>
-        <summary><b>3D Inception module</b></summary>
-        
-        Continual 3D version of the [Inception module](https://arxiv.org/pdf/1409.4842v1.pdf):
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/inception_block.png" style="width: 25vw; min-width: 350px;">
-          <br>
-          Inception module. Source: https://arxiv.org/pdf/1409.4842v1.pdf
-           
-        </div>
-        
-        ```python3
-        def norm_relu(module, channels):
-            return co.Sequential(
-                module,
-                nn.BatchNorm3d(channels),
-                nn.ReLU(),
-            )
-        
-        inception_module = co.BroadcastReduce(
-            co.Conv3d(192, 64, kernel_size=1),
-            co.Sequential(
-                norm_relu(co.Conv3d(192, 96, kernel_size=1), 96),
-                norm_relu(co.Conv3d(96, 128, kernel_size=3, padding=1), 128),
-            ),
-            co.Sequential(
-                norm_relu(co.Conv3d(192, 16, kernel_size=1), 16),
-                norm_relu(co.Conv3d(16, 32, kernel_size=5, padding=2), 32),
-            ),
-            co.Sequential(
-                co.MaxPool3d(kernel_size=(1, 3, 3), padding=(0, 1, 1), stride=1),
-                norm_relu(co.Conv3d(192, 32, kernel_size=1), 32),
-            ),
-            reduce="concat",
-        )
-        ```
-        </details>
-        
-        
-        ### Input shapes
-        We enforce a unified ordering of input dimensions for all library modules, namely:
-        
-            (batch, channel, time, optional_dim2, optional_dim3)
-        
-        ### Outputs
-        The outputs produces by `forward_step` and `forward_steps` are identical to those of `forward`, provided the same data was input beforehand and state update was enabled. We know that input and output shapes aren't necessarily the same when using `forward` in the PyTorch library, and  generally depends on padding, stride and receptive field of a module. 
-        
-        For the `forward_step` function, this comes to show by some `None`-valued outputs. Specifically, modules with a _delay_ (i.e. with receptive fields larger than the padding + 1) will produce `None` until the input count exceeds the delay. Moreover, _stride_ > 1 will produce `Tensor` outputs every _stride_ steps and `None` the remaining steps. A visual example is shown below:
-        
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/continual/continual-stride.png" style="width:300px;height:auto;"/>
-          </br>
-          A mixed example of delay and outputs under padding and stride. Here, we illustrate the step-wise operation of two co module layers, l1 with with receptive_field = 3, padding = 2, and stride = 2 and l2 with receptive_field = 3, no padding and stride = 1. ⧇ denotes a padded zero, ■ is a non-zero step-feature, and ☒ is an empty output.
-        </div>
-        
-        For more information, please see the [library paper](https://arxiv.org/abs/2204.03418).
-        
-        ### Handling state
-        During stream processing, network modules which operate over multiple time-steps, e.g., a convolution with `kernel_size > 1` in the temporal dimension, will aggregate and cache state internally. Each module has its own local state, which can be inspected using `module.get_state()`. During `forward_step` and `forward_steps`, the state is updated unless the forward_step(s) is invoked with an `update_state = False` argument.
-        
-        A __state cleanup__ can be accomplished via `module.clean_state()`.
-        
-        
-        ## Module library
-        _Continual Inference_ features a rich collection of modules for defining Continual Inference Networks. Specific care was taken to create CIN versions of the PyTorch modules found in [_torch.nn_](https://pytorch.org/docs/stable/nn.html):
-        
-        <details>
-        <summary><b>Convolutions</b></summary>
-        
-        - [`co.Conv1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv1d.html)
-        - [`co.Conv2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv2d.html)
-        - [`co.Conv3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv3d.html)
-        
-        </details>
-        
-        <details>
-        <summary><b>Pooling</b></summary>
-        
-          - [`co.AvgPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool1d.html)
-          - [`co.AvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool2d.html)
-          - [`co.AvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool3d.html)
-          - [`co.MaxPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool1d.html)
-          - [`co.MaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool2d.html)
-          - [`co.MaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool3d.html)
-          - [`co.AdaptiveAvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool2d.html)
-          - [`co.AdaptiveAvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool3d.html)
-          - [`co.AdaptiveMaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool2d.html)
-          - [`co.AdaptiveMaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool3d.html)
-        
-        </details>
-        
-        <details>
-        <summary><b>Linear</b></summary>
-        
-          - [`co.Linear`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Linear.html)
-          - [`co.Identity`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Identity.html): Maps input to output without modification.
-          - [`co.Add`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Add.html): Adds a constant value.
-          - [`co.Multiply`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Multiply.html): Multiplies with a constant factor.
-        
-        </details>
-        
-        <details>
-        <summary><b>Recurrent</b></summary>
-        
-          - [`co.RNN`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RNN.html)
-          - [`co.LSTM`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.LSTM.html)
-          - [`co.GRU`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.GRU.html)
-        
-        </details>
-        
-        <details>
-        <summary><b>Transformers</b></summary>
-        
-          - [`co.TransformerEncoder`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoder.html)
-          - [`co.TransformerEncoderLayerFactory`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoderLayerFactory.html): Factory function corresponding to `nn.TransformerEncoderLayer`.
-          - [`co.SingleOutputTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.SingleOutputTransformerEncoderLayer.html): SingleOutputMHA version of `nn.TransformerEncoderLayer`.
-          - [`co.RetroactiveTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RetroactiveTransformerEncoderLayer.html): RetroactiveMHA version of `nn.TransformerEncoderLayer`.
-          - [`co.RetroactiveMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.retroactive_mha.html.RetroactiveMultiheadAttention): Retroactive version of `nn.MultiheadAttention`.
-          - [`co.SingleOutputMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.single_output_mha.html.SingleOutputMultiheadAttention): Single-output version of `nn.MultiheadAttention`.
-          - [`co.RecyclingPositionalEncoding`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RecyclingPositionalEncoding.html): Positional Encoding used for Continual Transformers.
-        
-        </details>
-        
-        
-        Modules for composing and converting networks. Both _composition_ and _utility_ modules can be used for regular definition of PyTorch modules as well.
-        
-        <details>
-        <summary><b>Composition modules</b></summary>
-        
-          - [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
-          - [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
-          - [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
-          - [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
-          - [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
-          - [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
-          - [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
-          - [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
-        
-        </details>
-        
-        <details>
-        <summary><b>Utility modules</b></summary>
-        
-          - [`co.Delay`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Delay.html): Pure delay module (e.g. needed in residuals).
-          - [`co.Skip`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Skip.html): Skip a predefined number of input steps.
-          - [`co.Reshape`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reshape.html): Reshape non-temporal dimensions.
-          - [`co.Lambda`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Lambda.html): Lambda module which wraps any function.
-          - [`co.Constant`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Constant.html): Maps input to and output with constant value.
-          - [`co.Zero`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Zero.html): Maps input to output of zeros.
-          - [`co.One`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.One.html): Maps input to output of ones.
-        
-        </details>
-        
-        <details>
-        <summary><b>Converters</b></summary>
-        
-          - [`co.continual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.continual.html): conversion function from `torch.nn` modules to `co` modules.
-          - [`co.forward_stepping`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.forward_stepping.html): functional wrapper, which enhances temporally local `torch.nn` modules with the forward_stepping functions.
-        
-        </details>
-        
-        We support drop-in interoperability with with the following _torch.nn_ modules:
-        
-        <details>
-        <summary><b>Activation</b></summary>
-        
-          - `nn.Threshold`
-          - `nn.ReLU`
-          - `nn.RReLU`
-          - `nn.Hardtanh`
-          - `nn.ReLU6`
-          - `nn.Sigmoid`
-          - `nn.Hardsigmoid`
-          - `nn.Tanh`
-          - `nn.SiLU`
-          - `nn.Hardswish`
-          - `nn.ELU`
-          - `nn.CELU`
-          - `nn.SELU`
-          - `nn.GLU`
-          - `nn.GELU`
-          - `nn.Hardshrink`
-          - `nn.LeakyReLU`
-          - `nn.LogSigmoid`
-          - `nn.Softplus`
-          - `nn.Softshrink`
-          - `nn.PReLU`
-          - `nn.Softsign`
-          - `nn.Tanhshrink`
-          - `nn.Softmin`
-          - `nn.Softmax`
-          - `nn.Softmax2d`
-          - `nn.LogSoftmax`
-        
-        </details>
-        
-        <details>
-        <summary><b>Normalization</b></summary>
-        
-          - `nn.BatchNorm1d`
-          - `nn.BatchNorm2d`
-          - `nn.BatchNorm3d`
-          - `nn.GroupNorm`,
-          - `nn.InstanceNorm1d` (affine=True, track_running_stats=True required)
-          - `nn.InstanceNorm2d` (affine=True, track_running_stats=True required)
-          - `nn.InstanceNorm3d` (affine=True, track_running_stats=True required)
-          - `nn.LayerNorm` (only non-temporal dimensions must be specified)
-        
-        </details>
-        
-        <details>
-        <summary><b>Dropout</b></summary>
-        
-          - `nn.Dropout`
-          - `nn.Dropout1d`
-          - `nn.Dropout2d`
-          - `nn.Dropout3d`
-          - `nn.AlphaDropout`
-          - `nn.FeatureAlphaDropout`
-        
-        </details>
-        
-        
-        ## Model Zoo and Benchmarks
-        
-        ### Continual 3D CNNs
-        
-        Benchmark results for 1-view testing on __Kinetics400__. For reference, _X3D-L_ scores 69.3% top-1 acc with 19.2 GFLOPs per prediction. 
-        
-        Arch     | Avg. pool size | Top 1 (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                   | Weights
-        -------- | -------------- | --------- | ------------------ | --------------- | ---------- | ---------------------------------------------------------------------- | ---- 
-        CoX3D-L  | 64             | 71.6      | 1.25               | 15.3x           | 6.2        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_L.pyth)
-        CoX3D-M  | 64             | 71.0      | 0.33               | 15.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_M.pyth)
-        CoX3D-S  | 64             | 64.7      | 0.17               | 12.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_S.pyth)
-        CoSlow   | 64             | 73.1      | 6.90               |  8.0x           | 32.5       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coslow) | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/SLOW\_8x8\_R50.pyth)
-        CoI3D    | 64             | 64.0      | 5.68               |  5.0x           | 28.0       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coi3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/I3D\_8x8\_R50.pyth)
-        
-        FLOPs reduction is noted relative to non-continual inference.
-        Note that [on-hardware inference](https://arxiv.org/abs/2106.00050) doesn't reach the same speedups as "FLOPs reductions" might suggest due to overhead of state reads and writes. This overhead is less important for large batch sizes. This applies to all models in the model zoo.
-        
-        ### Continual ST-GCNs
-        
-        Benchmark results for on __NTU RGB+D 60__ for the joint modality. For reference, _ST-GCN_ achieves 86% X-Sub and 93.4 X-View accuracy with 16.73 GFLOPs per prediction. 
-        
-        Arch      | Receptive field | X-Sub Acc (%) | X-View Acc (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                  
-        --------  | --------------- | ------------- | -------------- | ------------------ | --------------- | ---------- | -----
-        CoST-GCN  | 300             | 86.3          | 93.8           | 0.16               | 107.7x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cost_gcn_mod/cost_gcn_mod.py)
-        CoA-GCN   | 300             | 84.1          | 92.6           | 0.17               | 108.7x          | 3.5        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/coa_gcn_mod/coa_gcn_mod.py)
-        CoST-GCN  | 300             | 86.3          | 92.4           | 0.15               | 107.6x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cos_tr_mod/cos_tr_mod.py)
-        
-        [Here](https://drive.google.com/drive/u/4/folders/1m6aV5Zv8tAytvxF6qY4m9nyqlkKv0y72), you can download pre-trained,model weights for the above architectures on NTU RGB+D 60, NTU RGB+D 120, and Kinetics-400 on joint and bone modalities.
-        
-        
-        ### Continual Transformers
-        
-        Benchmark results for on __THUMOS14__ on top of features extracted using a TSN-ResNet50 backbone pre-trained on Kinetics400. For reference, _OadTR_ achieves 64.4 % mAP with 2.5 GFLOPs per prediction. 
-        
-        Arch        | Receptive field | mAP (%) | FLOPs (G) per step |  Params (M) | Code                                                                  
-        ----------  | --------------- | ------- | ------------------ |  ---------- | -----
-        CoOadTR-b1  | 64              | 64.2    | 0.41               |  15.9       | [link](https://github.com/LukasHedegaard/CoOadTR)
-        CoOadTR-b2  | 64              | 64.4    | 0.01               |   9.6       | [link](https://github.com/LukasHedegaard/CoOadTR)
-        
-        The library features complete implementations of the [one](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L8)- and [two](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L59)-block continual transformer encoders as well.
-        
-        
-        ## Compatibility
-        The library modules are built to integrate seamlessly with other PyTorch projects.
-        Specifically, extra care was taken to ensure out-of-the-box compatibility with:
-        - [pytorch-lightning](https://github.com/PyTorchLightning/pytorch-lightning)
-        - [ptflops](https://github.com/sovrasov/flops-counter.pytorch)
-        - [ride](https://github.com/LukasHedegaard/ride)
-        - [onnx](https://github.com/onnx/onnx)
-        <!-- - [onnxruntime](https://github.com/microsoft/onnxruntime) -->
-        
-        
-        ## Citation
-        <a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
-          <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
-        </a>
-        
-        ```bibtex
-        @inproceedings{hedegaard2022colib,
-          title={Continual Inference: A Library for Efficient Online Inference with Deep Neural Networks in PyTorch},
-          author={Lukas Hedegaard and Alexandros Iosifidis},
-          booktitle={European Conference on Computer Vision Workshops (ECCVW)},
-          year={2022}
-        }
-        ```
-        
-        
-        ## Acknowledgement
-        This work has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 871449 (OpenDR).
-        
 Keywords: deep learning,pytorch,AI,online,inference,continual
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -577,7 +22,565 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE
+
+<img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/logo_name.svg" style="width: 400px;">
+
+__A Python library for Continual Inference Networks in PyTorch__
+
+[Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/README.html#quick-start) • 
+[Docs](https://continual-inference.readthedocs.io/en/latest/generated/README.html) • 
+[Principles](https://continual-inference.readthedocs.io/en/latest/generated/README.html#library-principles) • 
+[Paper](https://arxiv.org/abs/2204.03418) • 
+[Examples](https://continual-inference.readthedocs.io/en/latest/generated/README.html#composition-examples) • 
+[Modules](https://continual-inference.readthedocs.io/en/latest/common/modules.html) • 
+[Model Zoo](https://continual-inference.readthedocs.io/en/latest/generated/README.html#model-zoo-and-benchmarks) • 
+[Contribute](https://continual-inference.readthedocs.io/en/latest/generated/CONTRIBUTING.html) • 
+[License](https://github.com/LukasHedegaard/continual-inference/blob/main/LICENSE)
+
+<div>
+  <a href="https://pypi.org/project/continual-inference/" style="display:inline-block;">
+    <img src="https://img.shields.io/pypi/pyversions/continual-inference" height="20" >
+  </a>
+  <a href="https://badge.fury.io/py/continual-inference" style="display:inline-block;">
+    <img src="https://badge.fury.io/py/continual-inference.svg" height="20" >
+  </a>
+  <a href="https://continual-inference.readthedocs.io/en/latest/generated/README.html" style="display:inline-block;">
+    <img src="https://readthedocs.org/projects/continual-inference/badge/?version=latest" alt="Documentation Status" height="20"/>
+  </a>
+  <a href="https://pepy.tech/project/continual-inference" style="display:inline-block;">
+    <img src="https://pepy.tech/badge/continual-inference" height="20">
+  </a>
+  <a href="https://codecov.io/gh/LukasHedegaard/continual-inference" style="display:inline-block;">
+    <img src="https://codecov.io/gh/LukasHedegaard/continual-inference/branch/main/graph/badge.svg?token=XW1UQZSEOG" height="20"/>
+  </a>
+  <a href="https://opensource.org/licenses/Apache-2.0" style="display:inline-block;">
+    <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" height="20">
+  </a>
+  <!-- <a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
+    <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
+  </a> -->
+  <a href="https://github.com/psf/black" style="display:inline-block;">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="20">
+  </a>
+  <a href="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/overview/main" style="display:inline-block;">
+    <img src="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/badge/main" alt="We match PyTorch interfaces exactly. Method arguments named 'input' reduce the codefactor to 'A-'" height="20" />
+  </a>
+</div>
+
+## Continual Inference Networks ensure efficient stream processing
+Many of our favorite Deep Neural Network architectures (e.g., [CNNs](https://arxiv.org/abs/2106.00050) and [Transformers](https://arxiv.org/abs/2201.06268)) were built with offline-processing for offline processing. Rather than processing inputs one sequence element at a time, they require the whole (spatio-)temporal sequence to be passed as a single input.
+Yet, **many important real-life applications need online predictions on a continual input stream**. 
+While CNNs and Transformers can be applied by re-assembling and passing sequences within a sliding window, this is _inefficient_ due to the redundant intermediary computations from overlapping clips.
+
+**Continual Inference Networks** (CINs) are built to ensure efficient stream processing by employing an alternative computational ordering, which allows sequential computations without the use of sliding window processing.
+In general, CINs requires approx. _L_ ×  fewer FLOPs per prediction compared to sliding window-based inference with non-CINs, where _L_ is the corresponding sequence length of a non-CIN network. For more details, check out the videos below describing Continual 3D CNNs [[1](https://arxiv.org/abs/2106.00050)] and Transformers [[2](https://arxiv.org/abs/2201.06268)].
+
+
+<div align="center">
+  <a href="http://www.youtube.com/watch?feature=player_embedded&v=Jm2A7dVEaF4" target="_blank">
+     <img src="http://img.youtube.com/vi/Jm2A7dVEaF4/hqdefault.jpg" alt="Presentation of Continual 3D CNNs" style="width:240px;height:auto;" />
+  </a>
+  <a href="http://www.youtube.com/watch?feature=player_embedded&v=gy802Tlp-eQ" target="_blank">
+     <img src="http://img.youtube.com/vi/gy802Tlp-eQ/hqdefault.jpg" alt="Presentation of Continual Transformers" style="width:240px;height:auto;" />
+  </a>
+</div>
+
+## News
+- 2022-12-02: ONNX compatibility for all modules is available from v1.0.0. See [test_onnx.py](tests/continual/test_onnx.py) for examples.
+
+
+## Quick-start
+
+### Install 
+```bash
+pip install continual-inference
+```
+
+
+
+### Example
+`co` modules are weight-compatible drop-in replacement for `torch.nn`, enhanced with the capability of efficient _continual inference_:
+
+```python3
+import torch
+import continual as co
+                                                           
+#                      B, C, T, H, W
+example = torch.randn((1, 1, 5, 3, 3))
+
+conv = co.Conv3d(in_channels=1, out_channels=1, kernel_size=(3, 3, 3))
+
+# Same exact computation as torch.nn.Conv3d ✅
+output = conv(example)
+
+# But can also perform online inference efficiently 🚀
+firsts = conv.forward_steps(example[:, :, :4])
+last = conv.forward_step(example[:, :, 4])
+
+assert torch.allclose(output[:, :, : conv.delay], firsts)
+assert torch.allclose(output[:, :, conv.delay], last)
+
+# Temporal properties
+assert conv.receptive_field == 3
+assert conv.delay == 2
+```
+
+See the [network composition](#composition) and [model zoo](#model-zoo-and-benchmarks) sections for additional examples.
+
+## Library principles
+
+### Forward modes
+The library components feature three distinct forward modes, which are handy for different situations, namely `forward`, `forward_step`, and `forward_steps`:
+
+#### `forward(input)`
+Performs a forward computation over multiple time-steps. This function is identical to the corresponding module in _torch.nn_, ensuring cross-compatibility. Moreover, it's handy for efficient training on clip-based data.
+
+```
+         O            (O: output)
+         ↑ 
+         N            (N: network module)
+         ↑ 
+ -----------------    (-: aggregation)
+ P   I   I   I   P    (I: input frame, P: padding)
+```
+
+
+#### `forward_step(input, update_state=True)`
+Performs a forward computation for a single frame and (optionally) updates internal states accordingly. This function performs efficient continual inference.
+
+```
+O+S O+S O+S O+S   (O: output, S: updated internal state)
+ ↑   ↑   ↑   ↑ 
+ N   N   N   N    (N: network module)
+ ↑   ↑   ↑   ↑ 
+ I   I   I   I    (I: input frame)
+```
+
+#### `forward_steps(input, pad_end=False, update_state=True)`
+Performs a forward computation across multiple time-steps while updating internal states for continual inference (if update_state=True).
+Start-padding is always accounted for, but end-padding is omitted per default in expectance of the next input step. It can be added by specifying pad_end=True. If so, the output-input mapping the exact same as that of forward.
+```
+         O            (O: output)
+         ↑ 
+ -----------------    (-: aggregation)
+ O  O+S O+S O+S  O    (O: output, S: updated internal state)
+ ↑   ↑   ↑   ↑   ↑
+ N   N   N   N   N    (N: network module)
+ ↑   ↑   ↑   ↑   ↑
+ P   I   I   I   P    (I: input frame, P: padding)
+```
+
+#### `__call__`
+Per default, the `__call__` function operates identically to _torch.nn_ and executes forward. We supply two options for changing this behavior, namely the _call_mode_ property and the _call_mode_ context manager. An example of their use follows:
+
+```python
+timeseries = torch.randn(batch, channel, time)
+timestep = timeseries[:, :, 0]
+
+net(timeseries)  # Invokes net.forward(timeseries)
+
+# Assign permanent call_mode property
+net.call_mode = "forward_step"
+net(timestep)  # Invokes net.forward_step(timestep)
+
+# Assign temporary call_mode with context manager
+with co.call_mode("forward_steps"):
+    net(timeseries)  # Invokes net.forward_steps(timeseries)
+
+net(timestep)  # Invokes net.forward_step(timestep) again
+```
+
+### Composition
+
+Continual Inference Networks require strict handling of internal data delays to guarantee correspondence between [forward modes](#forward-modes). While it is possible to compose neural networks by defining _forward_, _forward_step_, and _forward_steps_ manually, correct handling of delays is cumbersome and time-consuming. Instead, we provide a rich interface of container modules, which handles delays automatically. On top of `co.Sequential` (which is a drop-in replacement of _torch.nn.Sequential_), we provide modules for handling parallel and conditional dataflow. 
+
+- [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
+- [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
+- [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
+- [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
+- [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
+- [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
+- [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
+- [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
+
+
+#### Composition examples:
+
+<details>
+<summary><b>Residual module</b></summary>
+
+Short-hand:
+```python3
+residual = co.Residual(co.Conv3d(32, 32, kernel_size=3, padding=1))
+```
+
+Explicit:
+```python3
+residual = co.Sequential(
+    co.Broadcast(2),
+    co.Parallel(
+        co.Conv3d(32, 32, kernel_size=3, padding=1),
+        co.Delay(2),
+    ),
+    co.Reduce("sum"),
+)
+```
+
+</details>
+
+<details>
+<summary><b>3D MobileNetV2 Inverted residual block</b></summary>
+
+Continual 3D version of the [MobileNetV2 Inverted residual block](https://arxiv.org/pdf/1801.04381.pdf).
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/mb_conv.png" style="width: 15vw; min-width: 200px;">
+  <br>
+  MobileNetV2 Inverted residual block. Source: https://arxiv.org/pdf/1801.04381.pdf
+</div>
+
+```python3
+mb_conv = co.Residual(
+    co.Sequential(
+      co.Conv3d(32, 64, kernel_size=(1, 1, 1)),
+      nn.BatchNorm3d(64),
+      nn.ReLU6(),
+      co.Conv3d(64, 64, kernel_size=(3, 3, 3), padding=(1, 1, 1), groups=64),
+      nn.ReLU6(),
+      co.Conv3d(64, 32, kernel_size=(1, 1, 1)),
+      nn.BatchNorm3d(32),
+    )
+)
+```
+
+</details>
+
+<details>
+<summary><b>3D Squeeze-and-Excitation module</b></summary>
+
+Continual 3D version of the [Squeeze-and-Excitation module](https://arxiv.org/pdf/1709.01507.pdf)
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/se_block.png" style="width: 15vw; min-width: 200px;">
+  <br>
+  Squeeze-and-Excitation block. 
+  Scale refers to a broadcasted element-wise multiplication.
+  Adapted from: https://arxiv.org/pdf/1709.01507.pdf
+</div>
+
+```python3
+se = co.Residual(
+    co.Sequential(
+        OrderedDict([
+            ("pool", co.AdaptiveAvgPool3d((1, 1, 1), kernel_size=7)),
+            ("down", co.Conv3d(256, 16, kernel_size=1)),
+            ("act1", nn.ReLU()),
+            ("up", co.Conv3d(16, 256, kernel_size=1)),
+            ("act2", nn.Sigmoid()),
+        ])
+    ),
+    reduce="mul",
+)
+```
+
+</details>
+
+<details>
+<summary><b>3D Inception module</b></summary>
+
+Continual 3D version of the [Inception module](https://arxiv.org/pdf/1409.4842v1.pdf):
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/inception_block.png" style="width: 25vw; min-width: 350px;">
+  <br>
+  Inception module. Source: https://arxiv.org/pdf/1409.4842v1.pdf
+   
+</div>
+
+```python3
+def norm_relu(module, channels):
+    return co.Sequential(
+        module,
+        nn.BatchNorm3d(channels),
+        nn.ReLU(),
+    )
+
+inception_module = co.BroadcastReduce(
+    co.Conv3d(192, 64, kernel_size=1),
+    co.Sequential(
+        norm_relu(co.Conv3d(192, 96, kernel_size=1), 96),
+        norm_relu(co.Conv3d(96, 128, kernel_size=3, padding=1), 128),
+    ),
+    co.Sequential(
+        norm_relu(co.Conv3d(192, 16, kernel_size=1), 16),
+        norm_relu(co.Conv3d(16, 32, kernel_size=5, padding=2), 32),
+    ),
+    co.Sequential(
+        co.MaxPool3d(kernel_size=(1, 3, 3), padding=(0, 1, 1), stride=1),
+        norm_relu(co.Conv3d(192, 32, kernel_size=1), 32),
+    ),
+    reduce="concat",
+)
+```
+</details>
+
+
+### Input shapes
+We enforce a unified ordering of input dimensions for all library modules, namely:
+
+    (batch, channel, time, optional_dim2, optional_dim3)
+
+### Outputs
+The outputs produces by `forward_step` and `forward_steps` are identical to those of `forward`, provided the same data was input beforehand and state update was enabled. We know that input and output shapes aren't necessarily the same when using `forward` in the PyTorch library, and  generally depends on padding, stride and receptive field of a module. 
+
+For the `forward_step` function, this comes to show by some `None`-valued outputs. Specifically, modules with a _delay_ (i.e. with receptive fields larger than the padding + 1) will produce `None` until the input count exceeds the delay. Moreover, _stride_ > 1 will produce `Tensor` outputs every _stride_ steps and `None` the remaining steps. A visual example is shown below:
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/continual/continual-stride.png" style="width:300px;height:auto;"/>
+  </br>
+  A mixed example of delay and outputs under padding and stride. Here, we illustrate the step-wise operation of two co module layers, l1 with with receptive_field = 3, padding = 2, and stride = 2 and l2 with receptive_field = 3, no padding and stride = 1. ⧇ denotes a padded zero, ■ is a non-zero step-feature, and ☒ is an empty output.
+</div>
+
+For more information, please see the [library paper](https://arxiv.org/abs/2204.03418).
+
+### Handling state
+During stream processing, network modules which operate over multiple time-steps, e.g., a convolution with `kernel_size > 1` in the temporal dimension, will aggregate and cache state internally. Each module has its own local state, which can be inspected using `module.get_state()`. During `forward_step` and `forward_steps`, the state is updated unless the forward_step(s) is invoked with an `update_state = False` argument.
+
+A __state cleanup__ can be accomplished via `module.clean_state()`.
+
+
+## Module library
+_Continual Inference_ features a rich collection of modules for defining Continual Inference Networks. Specific care was taken to create CIN versions of the PyTorch modules found in [_torch.nn_](https://pytorch.org/docs/stable/nn.html):
+
+<details>
+<summary><b>Convolutions</b></summary>
+
+- [`co.Conv1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv1d.html)
+- [`co.Conv2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv2d.html)
+- [`co.Conv3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv3d.html)
+
+</details>
+
+<details>
+<summary><b>Pooling</b></summary>
+
+  - [`co.AvgPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool1d.html)
+  - [`co.AvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool2d.html)
+  - [`co.AvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool3d.html)
+  - [`co.MaxPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool1d.html)
+  - [`co.MaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool2d.html)
+  - [`co.MaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool3d.html)
+  - [`co.AdaptiveAvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool2d.html)
+  - [`co.AdaptiveAvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool3d.html)
+  - [`co.AdaptiveMaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool2d.html)
+  - [`co.AdaptiveMaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool3d.html)
+
+</details>
+
+<details>
+<summary><b>Linear</b></summary>
+
+  - [`co.Linear`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Linear.html)
+  - [`co.Identity`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Identity.html): Maps input to output without modification.
+  - [`co.Add`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Add.html): Adds a constant value.
+  - [`co.Multiply`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Multiply.html): Multiplies with a constant factor.
+
+</details>
+
+<details>
+<summary><b>Recurrent</b></summary>
+
+  - [`co.RNN`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RNN.html)
+  - [`co.LSTM`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.LSTM.html)
+  - [`co.GRU`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.GRU.html)
+
+</details>
+
+<details>
+<summary><b>Transformers</b></summary>
+
+  - [`co.TransformerEncoder`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoder.html)
+  - [`co.TransformerEncoderLayerFactory`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoderLayerFactory.html): Factory function corresponding to `nn.TransformerEncoderLayer`.
+  - [`co.SingleOutputTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.SingleOutputTransformerEncoderLayer.html): SingleOutputMHA version of `nn.TransformerEncoderLayer`.
+  - [`co.RetroactiveTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RetroactiveTransformerEncoderLayer.html): RetroactiveMHA version of `nn.TransformerEncoderLayer`.
+  - [`co.RetroactiveMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.retroactive_mha.html.RetroactiveMultiheadAttention): Retroactive version of `nn.MultiheadAttention`.
+  - [`co.SingleOutputMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.single_output_mha.html.SingleOutputMultiheadAttention): Single-output version of `nn.MultiheadAttention`.
+  - [`co.RecyclingPositionalEncoding`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RecyclingPositionalEncoding.html): Positional Encoding used for Continual Transformers.
+
+</details>
+
+
+Modules for composing and converting networks. Both _composition_ and _utility_ modules can be used for regular definition of PyTorch modules as well.
+
+<details>
+<summary><b>Composition modules</b></summary>
+
+  - [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
+  - [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
+  - [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
+  - [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
+  - [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
+  - [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
+  - [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
+  - [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
+
+</details>
+
+<details>
+<summary><b>Utility modules</b></summary>
+
+  - [`co.Delay`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Delay.html): Pure delay module (e.g. needed in residuals).
+  - [`co.Skip`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Skip.html): Skip a predefined number of input steps.
+  - [`co.Reshape`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reshape.html): Reshape non-temporal dimensions.
+  - [`co.Lambda`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Lambda.html): Lambda module which wraps any function.
+  - [`co.Constant`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Constant.html): Maps input to and output with constant value.
+  - [`co.Zero`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Zero.html): Maps input to output of zeros.
+  - [`co.One`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.One.html): Maps input to output of ones.
+
+</details>
+
+<details>
+<summary><b>Converters</b></summary>
+
+  - [`co.continual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.continual.html): conversion function from `torch.nn` modules to `co` modules.
+  - [`co.forward_stepping`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.forward_stepping.html): functional wrapper, which enhances temporally local `torch.nn` modules with the forward_stepping functions.
+
+</details>
+
+We support drop-in interoperability with with the following _torch.nn_ modules:
+
+<details>
+<summary><b>Activation</b></summary>
+
+  - `nn.Threshold`
+  - `nn.ReLU`
+  - `nn.RReLU`
+  - `nn.Hardtanh`
+  - `nn.ReLU6`
+  - `nn.Sigmoid`
+  - `nn.Hardsigmoid`
+  - `nn.Tanh`
+  - `nn.SiLU`
+  - `nn.Hardswish`
+  - `nn.ELU`
+  - `nn.CELU`
+  - `nn.SELU`
+  - `nn.GLU`
+  - `nn.GELU`
+  - `nn.Hardshrink`
+  - `nn.LeakyReLU`
+  - `nn.LogSigmoid`
+  - `nn.Softplus`
+  - `nn.Softshrink`
+  - `nn.PReLU`
+  - `nn.Softsign`
+  - `nn.Tanhshrink`
+  - `nn.Softmin`
+  - `nn.Softmax`
+  - `nn.Softmax2d`
+  - `nn.LogSoftmax`
+
+</details>
+
+<details>
+<summary><b>Normalization</b></summary>
+
+  - `nn.BatchNorm1d`
+  - `nn.BatchNorm2d`
+  - `nn.BatchNorm3d`
+  - `nn.GroupNorm`,
+  - `nn.InstanceNorm1d` (affine=True, track_running_stats=True required)
+  - `nn.InstanceNorm2d` (affine=True, track_running_stats=True required)
+  - `nn.InstanceNorm3d` (affine=True, track_running_stats=True required)
+  - `nn.LayerNorm` (only non-temporal dimensions must be specified)
+
+</details>
+
+<details>
+<summary><b>Dropout</b></summary>
+
+  - `nn.Dropout`
+  - `nn.Dropout1d`
+  - `nn.Dropout2d`
+  - `nn.Dropout3d`
+  - `nn.AlphaDropout`
+  - `nn.FeatureAlphaDropout`
+
+</details>
+
+
+## Model Zoo and Benchmarks
+
+### Continual 3D CNNs
+
+Benchmark results for 1-view testing on __Kinetics400__. For reference, _X3D-L_ scores 69.3% top-1 acc with 19.2 GFLOPs per prediction. 
+
+Arch     | Avg. pool size | Top 1 (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                   | Weights
+-------- | -------------- | --------- | ------------------ | --------------- | ---------- | ---------------------------------------------------------------------- | ---- 
+CoX3D-L  | 64             | 71.6      | 1.25               | 15.3x           | 6.2        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_L.pyth)
+CoX3D-M  | 64             | 71.0      | 0.33               | 15.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_M.pyth)
+CoX3D-S  | 64             | 64.7      | 0.17               | 12.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_S.pyth)
+CoSlow   | 64             | 73.1      | 6.90               |  8.0x           | 32.5       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coslow) | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/SLOW\_8x8\_R50.pyth)
+CoI3D    | 64             | 64.0      | 5.68               |  5.0x           | 28.0       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coi3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/I3D\_8x8\_R50.pyth)
+
+FLOPs reduction is noted relative to non-continual inference.
+Note that [on-hardware inference](https://arxiv.org/abs/2106.00050) doesn't reach the same speedups as "FLOPs reductions" might suggest due to overhead of state reads and writes. This overhead is less important for large batch sizes. This applies to all models in the model zoo.
+
+### Continual ST-GCNs
+
+Benchmark results for on __NTU RGB+D 60__ for the joint modality. For reference, _ST-GCN_ achieves 86% X-Sub and 93.4 X-View accuracy with 16.73 GFLOPs per prediction. 
+
+Arch      | Receptive field | X-Sub Acc (%) | X-View Acc (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                  
+--------  | --------------- | ------------- | -------------- | ------------------ | --------------- | ---------- | -----
+CoST-GCN  | 300             | 86.3          | 93.8           | 0.16               | 107.7x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cost_gcn_mod/cost_gcn_mod.py)
+CoA-GCN   | 300             | 84.1          | 92.6           | 0.17               | 108.7x          | 3.5        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/coa_gcn_mod/coa_gcn_mod.py)
+CoST-GCN  | 300             | 86.3          | 92.4           | 0.15               | 107.6x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cos_tr_mod/cos_tr_mod.py)
+
+[Here](https://drive.google.com/drive/u/4/folders/1m6aV5Zv8tAytvxF6qY4m9nyqlkKv0y72), you can download pre-trained,model weights for the above architectures on NTU RGB+D 60, NTU RGB+D 120, and Kinetics-400 on joint and bone modalities.
+
+
+### Continual Transformers
+
+Benchmark results for on __THUMOS14__ on top of features extracted using a TSN-ResNet50 backbone pre-trained on Kinetics400. For reference, _OadTR_ achieves 64.4 % mAP with 2.5 GFLOPs per prediction. 
+
+Arch        | Receptive field | mAP (%) | FLOPs (G) per step |  Params (M) | Code                                                                  
+----------  | --------------- | ------- | ------------------ |  ---------- | -----
+CoOadTR-b1  | 64              | 64.2    | 0.41               |  15.9       | [link](https://github.com/LukasHedegaard/CoOadTR)
+CoOadTR-b2  | 64              | 64.4    | 0.01               |   9.6       | [link](https://github.com/LukasHedegaard/CoOadTR)
+
+The library features complete implementations of the [one](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L8)- and [two](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L59)-block continual transformer encoders as well.
+
+
+## Compatibility
+The library modules are built to integrate seamlessly with other PyTorch projects.
+Specifically, extra care was taken to ensure out-of-the-box compatibility with:
+- [pytorch-lightning](https://github.com/PyTorchLightning/pytorch-lightning)
+- [ptflops](https://github.com/sovrasov/flops-counter.pytorch)
+- [ride](https://github.com/LukasHedegaard/ride)
+- [onnx](https://github.com/onnx/onnx)
+<!-- - [onnxruntime](https://github.com/microsoft/onnxruntime) -->
+
+
+## Citation
+<a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
+  <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
+</a>
+
+```bibtex
+@inproceedings{hedegaard2022colib,
+  title={Continual Inference: A Library for Efficient Online Inference with Deep Neural Networks in PyTorch},
+  author={Lukas Hedegaard and Alexandros Iosifidis},
+  booktitle={European Conference on Computer Vision Workshops (ECCVW)},
+  year={2022}
+}
+```
+
+
+## Acknowledgement
+This work has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 871449 (OpenDR).
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,37 @@
-Metadata-Version: 2.1 Name: continual-inference Version: 1.2.2 Summary: A
+Metadata-Version: 2.1 Name: continual-inference Version: 1.2.3 Summary: A
 Python library for Continual Inference Networks in PyTorch Home-page: https://
 github.com/lukashedegaard/continual-inference Author: Lukas Hedegaard Author-
-email: lukasxhedegaard@gmail.com License: UNKNOWN Description: [https://
-raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/
-logo_name.svg] __A Python library for Continual Inference Networks in PyTorch__
-[Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/
-README.html#quick-start) â¢ [Docs](https://continual-inference.readthedocs.io/
-en/latest/generated/README.html) â¢ [Principles](https://continual-
-inference.readthedocs.io/en/latest/generated/README.html#library-principles)
-â¢ [Paper](https://arxiv.org/abs/2204.03418) â¢ [Examples](https://continual-
-inference.readthedocs.io/en/latest/generated/README.html#composition-examples)
-â¢ [Modules](https://continual-inference.readthedocs.io/en/latest/common/
-modules.html) â¢ [Model Zoo](https://continual-inference.readthedocs.io/en/
-latest/generated/README.html#model-zoo-and-benchmarks) â¢ [Contribute](https:/
-/continual-inference.readthedocs.io/en/latest/generated/CONTRIBUTING.html) â¢
-[License](https://github.com/LukasHedegaard/continual-inference/blob/main/
-LICENSE)
+email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
+learning,pytorch,AI,online,inference,continual Platform: UNKNOWN Classifier:
+Environment :: Console Classifier: Natural Language :: English Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Recognition Classifier:
+Topic :: Scientific/Engineering :: Information Analysis Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
+Provides-Extra: build Provides-Extra: dev Provides-Extra: docs License-File:
+LICENSE [https://raw.githubusercontent.com/LukasHedegaard/continual-inference/
+main/figures/logo/logo_name.svg] __A Python library for Continual Inference
+Networks in PyTorch__ [Quick-start](https://continual-inference.readthedocs.io/
+en/latest/generated/README.html#quick-start) â¢ [Docs](https://continual-
+inference.readthedocs.io/en/latest/generated/README.html) â¢ [Principles]
+(https://continual-inference.readthedocs.io/en/latest/generated/
+README.html#library-principles) â¢ [Paper](https://arxiv.org/abs/2204.03418)
+â¢ [Examples](https://continual-inference.readthedocs.io/en/latest/generated/
+README.html#composition-examples) â¢ [Modules](https://continual-
+inference.readthedocs.io/en/latest/common/modules.html) â¢ [Model Zoo](https:/
+/continual-inference.readthedocs.io/en/latest/generated/README.html#model-zoo-
+and-benchmarks) â¢ [Contribute](https://continual-inference.readthedocs.io/en/
+latest/generated/CONTRIBUTING.html) â¢ [License](https://github.com/
+LukasHedegaard/continual-inference/blob/main/LICENSE)
 [https://img.shields.io/pypi/pyversions/continual-inference] [https://
 badge.fury.io/py/continual-inference.svg] [Documentation_Status] [https://
 pepy.tech/badge/continual-inference] [https://codecov.io/gh/LukasHedegaard/
 continual-inference/branch/main/graph/badge.svg?token=XW1UQZSEOG] [https://
 img.shields.io/badge/License-Apache%202.0-blue.svg]  [https://img.shields.io/
 badge/code%20style-black-000000.svg] [We_match_PyTorch_interfaces_exactly.
 Method_arguments_named_'input'_reduce_the_codefactor_to_'A-']
@@ -349,20 +361,8 @@
 [onnx](https://github.com/onnx/onnx)  ## Citation [http://img.shields.io/badge/
 paper-arxiv.2204.03418-B31B1B.svg] ```bibtex @inproceedings{hedegaard2022colib,
 title={Continual Inference: A Library for Efficient Online Inference with Deep
 Neural Networks in PyTorch}, author={Lukas Hedegaard and Alexandros Iosifidis},
 booktitle={European Conference on Computer Vision Workshops (ECCVW)}, year=
 {2022} } ``` ## Acknowledgement This work has received funding from the
 European Unionâs Horizon 2020 research and innovation programme under grant
-agreement No 871449 (OpenDR). Keywords: deep
-learning,pytorch,AI,online,inference,continual Platform: UNKNOWN Classifier:
-Environment :: Console Classifier: Natural Language :: English Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition Classifier:
-Topic :: Scientific/Engineering :: Information Analysis Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
-Provides-Extra: build Provides-Extra: dev Provides-Extra: docs
+agreement No 871449 (OpenDR).
```

### Comparing `continual-inference-1.2.2/README.md` & `continual-inference-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/__init__.py` & `continual-inference-1.2.3/continual/__init__.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/closure.py` & `continual-inference-1.2.3/continual/closure.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/container.py` & `continual-inference-1.2.3/continual/container.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/conv.py` & `continual-inference-1.2.3/continual/conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         state_index = torch.tensor(0)
         stride_index = torch.tensor(
             self.stride[0] - len(state_buffer) - 1 + self.padding[0]
         )
         return (state_buffer, state_index, stride_index)
 
     def clean_state(self):
-        self.state_buffer = torch.tensor([])
+        self.state_buffer = torch.tensor([], device=self.state_buffer.device)
         self.state_index = torch.tensor(0)
         self.stride_index = torch.tensor(0)
 
     def get_state(self) -> Optional[State]:
         if len(self.state_buffer) > 0:
             return (self.state_buffer, self.state_index, self.stride_index)
         return None
```

### Comparing `continual-inference-1.2.2/continual/convert.py` & `continual-inference-1.2.3/continual/convert.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/delay.py` & `continual-inference-1.2.3/continual/delay.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             -2 * self.delay
             if self.auto_shrink and isinstance(self.auto_shrink, bool)
             else -self.delay
         )
         return state_buffer, state_index
 
     def clean_state(self):
-        self.state_buffer = torch.tensor([])
+        self.state_buffer = torch.tensor([], device=self.state_buffer.device)
         self.state_index = torch.tensor(0)
 
     def get_state(self):
         if len(self.state_buffer) > 0:
             return (self.state_buffer, self.state_index)
         return None
```

### Comparing `continual-inference-1.2.2/continual/linear.py` & `continual-inference-1.2.3/continual/linear.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/logging.py` & `continual-inference-1.2.3/continual/logging.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/module.py` & `continual-inference-1.2.3/continual/module.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/multihead_attention/mha_base.py` & `continual-inference-1.2.3/continual/multihead_attention/mha_base.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/multihead_attention/retroactive_mha.py` & `continual-inference-1.2.3/continual/multihead_attention/retroactive_mha.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,19 +272,19 @@
             self.Q_mem,
             self.K_T_mem,
             self.V_mem,
             self.stride_index,
         ) = state
 
     def clean_state(self):
-        self.d_mem = torch.tensor([])
-        self.AV_mem = torch.tensor([])
-        self.Q_mem = torch.tensor([])
-        self.K_T_mem = torch.tensor([])
-        self.V_mem = torch.tensor([])
+        self.d_mem = torch.tensor([], device=self.d_mem.device)
+        self.AV_mem = torch.tensor([], device=self.AV_mem.device)
+        self.Q_mem = torch.tensor([], device=self.Q_mem.device)
+        self.K_T_mem = torch.tensor([], device=self.K_T_mem.device)
+        self.V_mem = torch.tensor([], device=self.V_mem.device)
         self.stride_index = torch.tensor(0)
 
     def _forward_step(
         self,
         query: Tensor,
         key: Tensor = None,
         value: Tensor = None,
```

### Comparing `continual-inference-1.2.2/continual/multihead_attention/single_output_mha.py` & `continual-inference-1.2.3/continual/multihead_attention/single_output_mha.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,17 +248,17 @@
             self.Q_mem,
             self.K_T_mem,
             self.V_mem,
             self.stride_index,
         ) = state
 
     def clean_state(self):
-        self.Q_mem = torch.tensor([])
-        self.K_T_mem = torch.tensor([])
-        self.V_mem = torch.tensor([])
+        self.Q_mem = torch.tensor([], device=self.Q_mem.device)
+        self.K_T_mem = torch.tensor([], device=self.K_T_mem.device)
+        self.V_mem = torch.tensor([], device=self.V_mem.device)
         self.stride_index = torch.tensor(0)
 
     @property
     def delay(self) -> int:
         return (
             self.sequence_len - self.query_index - 1
             if self.query_index >= 0
```

### Comparing `continual-inference-1.2.2/continual/onnx.py` & `continual-inference-1.2.3/continual/onnx.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/pooling.py` & `continual-inference-1.2.3/continual/pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         )
         state_index = torch.tensor(0)
         stride_index = torch.tensor(self.stride[0] - buf_len + self.padding[0])
 
         return state_buffer, state_index, stride_index
 
     def clean_state(self):
-        self.state_buffer = torch.tensor([])
+        self.state_buffer = torch.tensor([], device=self.state_buffer.device)
         self.state_index = torch.tensor(0)
         self.stride_index = torch.tensor(0)
 
     def get_state(self):
         if len(self.state_buffer) > 0:
             return (self.state_buffer, self.state_index, self.stride_index)
```

### Comparing `continual-inference-1.2.2/continual/positional_encoding.py` & `continual-inference-1.2.3/continual/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/ptflops.py` & `continual-inference-1.2.3/continual/ptflops.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/rnn.py` & `continual-inference-1.2.3/continual/rnn.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/shape.py` & `continual-inference-1.2.3/continual/shape.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/skip.py` & `continual-inference-1.2.3/continual/skip.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/transformer.py` & `continual-inference-1.2.3/continual/transformer.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual/utils.py` & `continual-inference-1.2.3/continual/utils.py`

 * *Files identical despite different names*

### Comparing `continual-inference-1.2.2/continual_inference.egg-info/PKG-INFO` & `continual-inference-1.2.3/continual_inference.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,570 +1,15 @@
 Metadata-Version: 2.1
 Name: continual-inference
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python library for Continual Inference Networks in PyTorch
 Home-page: https://github.com/lukashedegaard/continual-inference
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
-Description: <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/logo_name.svg" style="width: 400px;">
-        
-        __A Python library for Continual Inference Networks in PyTorch__
-        
-        [Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/README.html#quick-start) • 
-        [Docs](https://continual-inference.readthedocs.io/en/latest/generated/README.html) • 
-        [Principles](https://continual-inference.readthedocs.io/en/latest/generated/README.html#library-principles) • 
-        [Paper](https://arxiv.org/abs/2204.03418) • 
-        [Examples](https://continual-inference.readthedocs.io/en/latest/generated/README.html#composition-examples) • 
-        [Modules](https://continual-inference.readthedocs.io/en/latest/common/modules.html) • 
-        [Model Zoo](https://continual-inference.readthedocs.io/en/latest/generated/README.html#model-zoo-and-benchmarks) • 
-        [Contribute](https://continual-inference.readthedocs.io/en/latest/generated/CONTRIBUTING.html) • 
-        [License](https://github.com/LukasHedegaard/continual-inference/blob/main/LICENSE)
-        
-        <div>
-          <a href="https://pypi.org/project/continual-inference/" style="display:inline-block;">
-            <img src="https://img.shields.io/pypi/pyversions/continual-inference" height="20" >
-          </a>
-          <a href="https://badge.fury.io/py/continual-inference" style="display:inline-block;">
-            <img src="https://badge.fury.io/py/continual-inference.svg" height="20" >
-          </a>
-          <a href="https://continual-inference.readthedocs.io/en/latest/generated/README.html" style="display:inline-block;">
-            <img src="https://readthedocs.org/projects/continual-inference/badge/?version=latest" alt="Documentation Status" height="20"/>
-          </a>
-          <a href="https://pepy.tech/project/continual-inference" style="display:inline-block;">
-            <img src="https://pepy.tech/badge/continual-inference" height="20">
-          </a>
-          <a href="https://codecov.io/gh/LukasHedegaard/continual-inference" style="display:inline-block;">
-            <img src="https://codecov.io/gh/LukasHedegaard/continual-inference/branch/main/graph/badge.svg?token=XW1UQZSEOG" height="20"/>
-          </a>
-          <a href="https://opensource.org/licenses/Apache-2.0" style="display:inline-block;">
-            <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" height="20">
-          </a>
-          <!-- <a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
-            <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
-          </a> -->
-          <a href="https://github.com/psf/black" style="display:inline-block;">
-            <img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="20">
-          </a>
-          <a href="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/overview/main" style="display:inline-block;">
-            <img src="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/badge/main" alt="We match PyTorch interfaces exactly. Method arguments named 'input' reduce the codefactor to 'A-'" height="20" />
-          </a>
-        </div>
-        
-        ## Continual Inference Networks ensure efficient stream processing
-        Many of our favorite Deep Neural Network architectures (e.g., [CNNs](https://arxiv.org/abs/2106.00050) and [Transformers](https://arxiv.org/abs/2201.06268)) were built with offline-processing for offline processing. Rather than processing inputs one sequence element at a time, they require the whole (spatio-)temporal sequence to be passed as a single input.
-        Yet, **many important real-life applications need online predictions on a continual input stream**. 
-        While CNNs and Transformers can be applied by re-assembling and passing sequences within a sliding window, this is _inefficient_ due to the redundant intermediary computations from overlapping clips.
-        
-        **Continual Inference Networks** (CINs) are built to ensure efficient stream processing by employing an alternative computational ordering, which allows sequential computations without the use of sliding window processing.
-        In general, CINs requires approx. _L_ ×  fewer FLOPs per prediction compared to sliding window-based inference with non-CINs, where _L_ is the corresponding sequence length of a non-CIN network. For more details, check out the videos below describing Continual 3D CNNs [[1](https://arxiv.org/abs/2106.00050)] and Transformers [[2](https://arxiv.org/abs/2201.06268)].
-        
-        
-        <div align="center">
-          <a href="http://www.youtube.com/watch?feature=player_embedded&v=Jm2A7dVEaF4" target="_blank">
-             <img src="http://img.youtube.com/vi/Jm2A7dVEaF4/hqdefault.jpg" alt="Presentation of Continual 3D CNNs" style="width:240px;height:auto;" />
-          </a>
-          <a href="http://www.youtube.com/watch?feature=player_embedded&v=gy802Tlp-eQ" target="_blank">
-             <img src="http://img.youtube.com/vi/gy802Tlp-eQ/hqdefault.jpg" alt="Presentation of Continual Transformers" style="width:240px;height:auto;" />
-          </a>
-        </div>
-        
-        ## News
-        - 2022-12-02: ONNX compatibility for all modules is available from v1.0.0. See [test_onnx.py](tests/continual/test_onnx.py) for examples.
-        
-        
-        ## Quick-start
-        
-        ### Install 
-        ```bash
-        pip install continual-inference
-        ```
-        
-        
-        
-        ### Example
-        `co` modules are weight-compatible drop-in replacement for `torch.nn`, enhanced with the capability of efficient _continual inference_:
-        
-        ```python3
-        import torch
-        import continual as co
-                                                                   
-        #                      B, C, T, H, W
-        example = torch.randn((1, 1, 5, 3, 3))
-        
-        conv = co.Conv3d(in_channels=1, out_channels=1, kernel_size=(3, 3, 3))
-        
-        # Same exact computation as torch.nn.Conv3d ✅
-        output = conv(example)
-        
-        # But can also perform online inference efficiently 🚀
-        firsts = conv.forward_steps(example[:, :, :4])
-        last = conv.forward_step(example[:, :, 4])
-        
-        assert torch.allclose(output[:, :, : conv.delay], firsts)
-        assert torch.allclose(output[:, :, conv.delay], last)
-        
-        # Temporal properties
-        assert conv.receptive_field == 3
-        assert conv.delay == 2
-        ```
-        
-        See the [network composition](#composition) and [model zoo](#model-zoo-and-benchmarks) sections for additional examples.
-        
-        ## Library principles
-        
-        ### Forward modes
-        The library components feature three distinct forward modes, which are handy for different situations, namely `forward`, `forward_step`, and `forward_steps`:
-        
-        #### `forward(input)`
-        Performs a forward computation over multiple time-steps. This function is identical to the corresponding module in _torch.nn_, ensuring cross-compatibility. Moreover, it's handy for efficient training on clip-based data.
-        
-        ```
-                 O            (O: output)
-                 ↑ 
-                 N            (N: network module)
-                 ↑ 
-         -----------------    (-: aggregation)
-         P   I   I   I   P    (I: input frame, P: padding)
-        ```
-        
-        
-        #### `forward_step(input, update_state=True)`
-        Performs a forward computation for a single frame and (optionally) updates internal states accordingly. This function performs efficient continual inference.
-        
-        ```
-        O+S O+S O+S O+S   (O: output, S: updated internal state)
-         ↑   ↑   ↑   ↑ 
-         N   N   N   N    (N: network module)
-         ↑   ↑   ↑   ↑ 
-         I   I   I   I    (I: input frame)
-        ```
-        
-        #### `forward_steps(input, pad_end=False, update_state=True)`
-        Performs a forward computation across multiple time-steps while updating internal states for continual inference (if update_state=True).
-        Start-padding is always accounted for, but end-padding is omitted per default in expectance of the next input step. It can be added by specifying pad_end=True. If so, the output-input mapping the exact same as that of forward.
-        ```
-                 O            (O: output)
-                 ↑ 
-         -----------------    (-: aggregation)
-         O  O+S O+S O+S  O    (O: output, S: updated internal state)
-         ↑   ↑   ↑   ↑   ↑
-         N   N   N   N   N    (N: network module)
-         ↑   ↑   ↑   ↑   ↑
-         P   I   I   I   P    (I: input frame, P: padding)
-        ```
-        
-        #### `__call__`
-        Per default, the `__call__` function operates identically to _torch.nn_ and executes forward. We supply two options for changing this behavior, namely the _call_mode_ property and the _call_mode_ context manager. An example of their use follows:
-        
-        ```python
-        timeseries = torch.randn(batch, channel, time)
-        timestep = timeseries[:, :, 0]
-        
-        net(timeseries)  # Invokes net.forward(timeseries)
-        
-        # Assign permanent call_mode property
-        net.call_mode = "forward_step"
-        net(timestep)  # Invokes net.forward_step(timestep)
-        
-        # Assign temporary call_mode with context manager
-        with co.call_mode("forward_steps"):
-            net(timeseries)  # Invokes net.forward_steps(timeseries)
-        
-        net(timestep)  # Invokes net.forward_step(timestep) again
-        ```
-        
-        ### Composition
-        
-        Continual Inference Networks require strict handling of internal data delays to guarantee correspondence between [forward modes](#forward-modes). While it is possible to compose neural networks by defining _forward_, _forward_step_, and _forward_steps_ manually, correct handling of delays is cumbersome and time-consuming. Instead, we provide a rich interface of container modules, which handles delays automatically. On top of `co.Sequential` (which is a drop-in replacement of _torch.nn.Sequential_), we provide modules for handling parallel and conditional dataflow. 
-        
-        - [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
-        - [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
-        - [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
-        - [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
-        - [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
-        - [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
-        - [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
-        - [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
-        
-        
-        #### Composition examples:
-        
-        <details>
-        <summary><b>Residual module</b></summary>
-        
-        Short-hand:
-        ```python3
-        residual = co.Residual(co.Conv3d(32, 32, kernel_size=3, padding=1))
-        ```
-        
-        Explicit:
-        ```python3
-        residual = co.Sequential(
-            co.Broadcast(2),
-            co.Parallel(
-                co.Conv3d(32, 32, kernel_size=3, padding=1),
-                co.Delay(2),
-            ),
-            co.Reduce("sum"),
-        )
-        ```
-        
-        </details>
-        
-        <details>
-        <summary><b>3D MobileNetV2 Inverted residual block</b></summary>
-        
-        Continual 3D version of the [MobileNetV2 Inverted residual block](https://arxiv.org/pdf/1801.04381.pdf).
-        
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/mb_conv.png" style="width: 15vw; min-width: 200px;">
-          <br>
-          MobileNetV2 Inverted residual block. Source: https://arxiv.org/pdf/1801.04381.pdf
-        </div>
-        
-        ```python3
-        mb_conv = co.Residual(
-            co.Sequential(
-              co.Conv3d(32, 64, kernel_size=(1, 1, 1)),
-              nn.BatchNorm3d(64),
-              nn.ReLU6(),
-              co.Conv3d(64, 64, kernel_size=(3, 3, 3), padding=(1, 1, 1), groups=64),
-              nn.ReLU6(),
-              co.Conv3d(64, 32, kernel_size=(1, 1, 1)),
-              nn.BatchNorm3d(32),
-            )
-        )
-        ```
-        
-        </details>
-        
-        <details>
-        <summary><b>3D Squeeze-and-Excitation module</b></summary>
-        
-        Continual 3D version of the [Squeeze-and-Excitation module](https://arxiv.org/pdf/1709.01507.pdf)
-        
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/se_block.png" style="width: 15vw; min-width: 200px;">
-          <br>
-          Squeeze-and-Excitation block. 
-          Scale refers to a broadcasted element-wise multiplication.
-          Adapted from: https://arxiv.org/pdf/1709.01507.pdf
-        </div>
-        
-        ```python3
-        se = co.Residual(
-            co.Sequential(
-                OrderedDict([
-                    ("pool", co.AdaptiveAvgPool3d((1, 1, 1), kernel_size=7)),
-                    ("down", co.Conv3d(256, 16, kernel_size=1)),
-                    ("act1", nn.ReLU()),
-                    ("up", co.Conv3d(16, 256, kernel_size=1)),
-                    ("act2", nn.Sigmoid()),
-                ])
-            ),
-            reduce="mul",
-        )
-        ```
-        
-        </details>
-        
-        <details>
-        <summary><b>3D Inception module</b></summary>
-        
-        Continual 3D version of the [Inception module](https://arxiv.org/pdf/1409.4842v1.pdf):
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/inception_block.png" style="width: 25vw; min-width: 350px;">
-          <br>
-          Inception module. Source: https://arxiv.org/pdf/1409.4842v1.pdf
-           
-        </div>
-        
-        ```python3
-        def norm_relu(module, channels):
-            return co.Sequential(
-                module,
-                nn.BatchNorm3d(channels),
-                nn.ReLU(),
-            )
-        
-        inception_module = co.BroadcastReduce(
-            co.Conv3d(192, 64, kernel_size=1),
-            co.Sequential(
-                norm_relu(co.Conv3d(192, 96, kernel_size=1), 96),
-                norm_relu(co.Conv3d(96, 128, kernel_size=3, padding=1), 128),
-            ),
-            co.Sequential(
-                norm_relu(co.Conv3d(192, 16, kernel_size=1), 16),
-                norm_relu(co.Conv3d(16, 32, kernel_size=5, padding=2), 32),
-            ),
-            co.Sequential(
-                co.MaxPool3d(kernel_size=(1, 3, 3), padding=(0, 1, 1), stride=1),
-                norm_relu(co.Conv3d(192, 32, kernel_size=1), 32),
-            ),
-            reduce="concat",
-        )
-        ```
-        </details>
-        
-        
-        ### Input shapes
-        We enforce a unified ordering of input dimensions for all library modules, namely:
-        
-            (batch, channel, time, optional_dim2, optional_dim3)
-        
-        ### Outputs
-        The outputs produces by `forward_step` and `forward_steps` are identical to those of `forward`, provided the same data was input beforehand and state update was enabled. We know that input and output shapes aren't necessarily the same when using `forward` in the PyTorch library, and  generally depends on padding, stride and receptive field of a module. 
-        
-        For the `forward_step` function, this comes to show by some `None`-valued outputs. Specifically, modules with a _delay_ (i.e. with receptive fields larger than the padding + 1) will produce `None` until the input count exceeds the delay. Moreover, _stride_ > 1 will produce `Tensor` outputs every _stride_ steps and `None` the remaining steps. A visual example is shown below:
-        
-        <div align="center">
-          <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/continual/continual-stride.png" style="width:300px;height:auto;"/>
-          </br>
-          A mixed example of delay and outputs under padding and stride. Here, we illustrate the step-wise operation of two co module layers, l1 with with receptive_field = 3, padding = 2, and stride = 2 and l2 with receptive_field = 3, no padding and stride = 1. ⧇ denotes a padded zero, ■ is a non-zero step-feature, and ☒ is an empty output.
-        </div>
-        
-        For more information, please see the [library paper](https://arxiv.org/abs/2204.03418).
-        
-        ### Handling state
-        During stream processing, network modules which operate over multiple time-steps, e.g., a convolution with `kernel_size > 1` in the temporal dimension, will aggregate and cache state internally. Each module has its own local state, which can be inspected using `module.get_state()`. During `forward_step` and `forward_steps`, the state is updated unless the forward_step(s) is invoked with an `update_state = False` argument.
-        
-        A __state cleanup__ can be accomplished via `module.clean_state()`.
-        
-        
-        ## Module library
-        _Continual Inference_ features a rich collection of modules for defining Continual Inference Networks. Specific care was taken to create CIN versions of the PyTorch modules found in [_torch.nn_](https://pytorch.org/docs/stable/nn.html):
-        
-        <details>
-        <summary><b>Convolutions</b></summary>
-        
-        - [`co.Conv1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv1d.html)
-        - [`co.Conv2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv2d.html)
-        - [`co.Conv3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv3d.html)
-        
-        </details>
-        
-        <details>
-        <summary><b>Pooling</b></summary>
-        
-          - [`co.AvgPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool1d.html)
-          - [`co.AvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool2d.html)
-          - [`co.AvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool3d.html)
-          - [`co.MaxPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool1d.html)
-          - [`co.MaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool2d.html)
-          - [`co.MaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool3d.html)
-          - [`co.AdaptiveAvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool2d.html)
-          - [`co.AdaptiveAvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool3d.html)
-          - [`co.AdaptiveMaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool2d.html)
-          - [`co.AdaptiveMaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool3d.html)
-        
-        </details>
-        
-        <details>
-        <summary><b>Linear</b></summary>
-        
-          - [`co.Linear`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Linear.html)
-          - [`co.Identity`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Identity.html): Maps input to output without modification.
-          - [`co.Add`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Add.html): Adds a constant value.
-          - [`co.Multiply`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Multiply.html): Multiplies with a constant factor.
-        
-        </details>
-        
-        <details>
-        <summary><b>Recurrent</b></summary>
-        
-          - [`co.RNN`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RNN.html)
-          - [`co.LSTM`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.LSTM.html)
-          - [`co.GRU`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.GRU.html)
-        
-        </details>
-        
-        <details>
-        <summary><b>Transformers</b></summary>
-        
-          - [`co.TransformerEncoder`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoder.html)
-          - [`co.TransformerEncoderLayerFactory`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoderLayerFactory.html): Factory function corresponding to `nn.TransformerEncoderLayer`.
-          - [`co.SingleOutputTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.SingleOutputTransformerEncoderLayer.html): SingleOutputMHA version of `nn.TransformerEncoderLayer`.
-          - [`co.RetroactiveTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RetroactiveTransformerEncoderLayer.html): RetroactiveMHA version of `nn.TransformerEncoderLayer`.
-          - [`co.RetroactiveMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.retroactive_mha.html.RetroactiveMultiheadAttention): Retroactive version of `nn.MultiheadAttention`.
-          - [`co.SingleOutputMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.single_output_mha.html.SingleOutputMultiheadAttention): Single-output version of `nn.MultiheadAttention`.
-          - [`co.RecyclingPositionalEncoding`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RecyclingPositionalEncoding.html): Positional Encoding used for Continual Transformers.
-        
-        </details>
-        
-        
-        Modules for composing and converting networks. Both _composition_ and _utility_ modules can be used for regular definition of PyTorch modules as well.
-        
-        <details>
-        <summary><b>Composition modules</b></summary>
-        
-          - [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
-          - [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
-          - [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
-          - [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
-          - [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
-          - [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
-          - [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
-          - [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
-        
-        </details>
-        
-        <details>
-        <summary><b>Utility modules</b></summary>
-        
-          - [`co.Delay`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Delay.html): Pure delay module (e.g. needed in residuals).
-          - [`co.Skip`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Skip.html): Skip a predefined number of input steps.
-          - [`co.Reshape`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reshape.html): Reshape non-temporal dimensions.
-          - [`co.Lambda`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Lambda.html): Lambda module which wraps any function.
-          - [`co.Constant`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Constant.html): Maps input to and output with constant value.
-          - [`co.Zero`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Zero.html): Maps input to output of zeros.
-          - [`co.One`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.One.html): Maps input to output of ones.
-        
-        </details>
-        
-        <details>
-        <summary><b>Converters</b></summary>
-        
-          - [`co.continual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.continual.html): conversion function from `torch.nn` modules to `co` modules.
-          - [`co.forward_stepping`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.forward_stepping.html): functional wrapper, which enhances temporally local `torch.nn` modules with the forward_stepping functions.
-        
-        </details>
-        
-        We support drop-in interoperability with with the following _torch.nn_ modules:
-        
-        <details>
-        <summary><b>Activation</b></summary>
-        
-          - `nn.Threshold`
-          - `nn.ReLU`
-          - `nn.RReLU`
-          - `nn.Hardtanh`
-          - `nn.ReLU6`
-          - `nn.Sigmoid`
-          - `nn.Hardsigmoid`
-          - `nn.Tanh`
-          - `nn.SiLU`
-          - `nn.Hardswish`
-          - `nn.ELU`
-          - `nn.CELU`
-          - `nn.SELU`
-          - `nn.GLU`
-          - `nn.GELU`
-          - `nn.Hardshrink`
-          - `nn.LeakyReLU`
-          - `nn.LogSigmoid`
-          - `nn.Softplus`
-          - `nn.Softshrink`
-          - `nn.PReLU`
-          - `nn.Softsign`
-          - `nn.Tanhshrink`
-          - `nn.Softmin`
-          - `nn.Softmax`
-          - `nn.Softmax2d`
-          - `nn.LogSoftmax`
-        
-        </details>
-        
-        <details>
-        <summary><b>Normalization</b></summary>
-        
-          - `nn.BatchNorm1d`
-          - `nn.BatchNorm2d`
-          - `nn.BatchNorm3d`
-          - `nn.GroupNorm`,
-          - `nn.InstanceNorm1d` (affine=True, track_running_stats=True required)
-          - `nn.InstanceNorm2d` (affine=True, track_running_stats=True required)
-          - `nn.InstanceNorm3d` (affine=True, track_running_stats=True required)
-          - `nn.LayerNorm` (only non-temporal dimensions must be specified)
-        
-        </details>
-        
-        <details>
-        <summary><b>Dropout</b></summary>
-        
-          - `nn.Dropout`
-          - `nn.Dropout1d`
-          - `nn.Dropout2d`
-          - `nn.Dropout3d`
-          - `nn.AlphaDropout`
-          - `nn.FeatureAlphaDropout`
-        
-        </details>
-        
-        
-        ## Model Zoo and Benchmarks
-        
-        ### Continual 3D CNNs
-        
-        Benchmark results for 1-view testing on __Kinetics400__. For reference, _X3D-L_ scores 69.3% top-1 acc with 19.2 GFLOPs per prediction. 
-        
-        Arch     | Avg. pool size | Top 1 (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                   | Weights
-        -------- | -------------- | --------- | ------------------ | --------------- | ---------- | ---------------------------------------------------------------------- | ---- 
-        CoX3D-L  | 64             | 71.6      | 1.25               | 15.3x           | 6.2        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_L.pyth)
-        CoX3D-M  | 64             | 71.0      | 0.33               | 15.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_M.pyth)
-        CoX3D-S  | 64             | 64.7      | 0.17               | 12.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_S.pyth)
-        CoSlow   | 64             | 73.1      | 6.90               |  8.0x           | 32.5       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coslow) | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/SLOW\_8x8\_R50.pyth)
-        CoI3D    | 64             | 64.0      | 5.68               |  5.0x           | 28.0       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coi3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/I3D\_8x8\_R50.pyth)
-        
-        FLOPs reduction is noted relative to non-continual inference.
-        Note that [on-hardware inference](https://arxiv.org/abs/2106.00050) doesn't reach the same speedups as "FLOPs reductions" might suggest due to overhead of state reads and writes. This overhead is less important for large batch sizes. This applies to all models in the model zoo.
-        
-        ### Continual ST-GCNs
-        
-        Benchmark results for on __NTU RGB+D 60__ for the joint modality. For reference, _ST-GCN_ achieves 86% X-Sub and 93.4 X-View accuracy with 16.73 GFLOPs per prediction. 
-        
-        Arch      | Receptive field | X-Sub Acc (%) | X-View Acc (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                  
-        --------  | --------------- | ------------- | -------------- | ------------------ | --------------- | ---------- | -----
-        CoST-GCN  | 300             | 86.3          | 93.8           | 0.16               | 107.7x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cost_gcn_mod/cost_gcn_mod.py)
-        CoA-GCN   | 300             | 84.1          | 92.6           | 0.17               | 108.7x          | 3.5        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/coa_gcn_mod/coa_gcn_mod.py)
-        CoST-GCN  | 300             | 86.3          | 92.4           | 0.15               | 107.6x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cos_tr_mod/cos_tr_mod.py)
-        
-        [Here](https://drive.google.com/drive/u/4/folders/1m6aV5Zv8tAytvxF6qY4m9nyqlkKv0y72), you can download pre-trained,model weights for the above architectures on NTU RGB+D 60, NTU RGB+D 120, and Kinetics-400 on joint and bone modalities.
-        
-        
-        ### Continual Transformers
-        
-        Benchmark results for on __THUMOS14__ on top of features extracted using a TSN-ResNet50 backbone pre-trained on Kinetics400. For reference, _OadTR_ achieves 64.4 % mAP with 2.5 GFLOPs per prediction. 
-        
-        Arch        | Receptive field | mAP (%) | FLOPs (G) per step |  Params (M) | Code                                                                  
-        ----------  | --------------- | ------- | ------------------ |  ---------- | -----
-        CoOadTR-b1  | 64              | 64.2    | 0.41               |  15.9       | [link](https://github.com/LukasHedegaard/CoOadTR)
-        CoOadTR-b2  | 64              | 64.4    | 0.01               |   9.6       | [link](https://github.com/LukasHedegaard/CoOadTR)
-        
-        The library features complete implementations of the [one](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L8)- and [two](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L59)-block continual transformer encoders as well.
-        
-        
-        ## Compatibility
-        The library modules are built to integrate seamlessly with other PyTorch projects.
-        Specifically, extra care was taken to ensure out-of-the-box compatibility with:
-        - [pytorch-lightning](https://github.com/PyTorchLightning/pytorch-lightning)
-        - [ptflops](https://github.com/sovrasov/flops-counter.pytorch)
-        - [ride](https://github.com/LukasHedegaard/ride)
-        - [onnx](https://github.com/onnx/onnx)
-        <!-- - [onnxruntime](https://github.com/microsoft/onnxruntime) -->
-        
-        
-        ## Citation
-        <a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
-          <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
-        </a>
-        
-        ```bibtex
-        @inproceedings{hedegaard2022colib,
-          title={Continual Inference: A Library for Efficient Online Inference with Deep Neural Networks in PyTorch},
-          author={Lukas Hedegaard and Alexandros Iosifidis},
-          booktitle={European Conference on Computer Vision Workshops (ECCVW)},
-          year={2022}
-        }
-        ```
-        
-        
-        ## Acknowledgement
-        This work has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 871449 (OpenDR).
-        
 Keywords: deep learning,pytorch,AI,online,inference,continual
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -577,7 +22,565 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 Provides-Extra: docs
+License-File: LICENSE
+
+<img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/logo_name.svg" style="width: 400px;">
+
+__A Python library for Continual Inference Networks in PyTorch__
+
+[Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/README.html#quick-start) • 
+[Docs](https://continual-inference.readthedocs.io/en/latest/generated/README.html) • 
+[Principles](https://continual-inference.readthedocs.io/en/latest/generated/README.html#library-principles) • 
+[Paper](https://arxiv.org/abs/2204.03418) • 
+[Examples](https://continual-inference.readthedocs.io/en/latest/generated/README.html#composition-examples) • 
+[Modules](https://continual-inference.readthedocs.io/en/latest/common/modules.html) • 
+[Model Zoo](https://continual-inference.readthedocs.io/en/latest/generated/README.html#model-zoo-and-benchmarks) • 
+[Contribute](https://continual-inference.readthedocs.io/en/latest/generated/CONTRIBUTING.html) • 
+[License](https://github.com/LukasHedegaard/continual-inference/blob/main/LICENSE)
+
+<div>
+  <a href="https://pypi.org/project/continual-inference/" style="display:inline-block;">
+    <img src="https://img.shields.io/pypi/pyversions/continual-inference" height="20" >
+  </a>
+  <a href="https://badge.fury.io/py/continual-inference" style="display:inline-block;">
+    <img src="https://badge.fury.io/py/continual-inference.svg" height="20" >
+  </a>
+  <a href="https://continual-inference.readthedocs.io/en/latest/generated/README.html" style="display:inline-block;">
+    <img src="https://readthedocs.org/projects/continual-inference/badge/?version=latest" alt="Documentation Status" height="20"/>
+  </a>
+  <a href="https://pepy.tech/project/continual-inference" style="display:inline-block;">
+    <img src="https://pepy.tech/badge/continual-inference" height="20">
+  </a>
+  <a href="https://codecov.io/gh/LukasHedegaard/continual-inference" style="display:inline-block;">
+    <img src="https://codecov.io/gh/LukasHedegaard/continual-inference/branch/main/graph/badge.svg?token=XW1UQZSEOG" height="20"/>
+  </a>
+  <a href="https://opensource.org/licenses/Apache-2.0" style="display:inline-block;">
+    <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" height="20">
+  </a>
+  <!-- <a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
+    <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
+  </a> -->
+  <a href="https://github.com/psf/black" style="display:inline-block;">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="20">
+  </a>
+  <a href="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/overview/main" style="display:inline-block;">
+    <img src="https://www.codefactor.io/repository/github/lukashedegaard/continual-inference/badge/main" alt="We match PyTorch interfaces exactly. Method arguments named 'input' reduce the codefactor to 'A-'" height="20" />
+  </a>
+</div>
+
+## Continual Inference Networks ensure efficient stream processing
+Many of our favorite Deep Neural Network architectures (e.g., [CNNs](https://arxiv.org/abs/2106.00050) and [Transformers](https://arxiv.org/abs/2201.06268)) were built with offline-processing for offline processing. Rather than processing inputs one sequence element at a time, they require the whole (spatio-)temporal sequence to be passed as a single input.
+Yet, **many important real-life applications need online predictions on a continual input stream**. 
+While CNNs and Transformers can be applied by re-assembling and passing sequences within a sliding window, this is _inefficient_ due to the redundant intermediary computations from overlapping clips.
+
+**Continual Inference Networks** (CINs) are built to ensure efficient stream processing by employing an alternative computational ordering, which allows sequential computations without the use of sliding window processing.
+In general, CINs requires approx. _L_ ×  fewer FLOPs per prediction compared to sliding window-based inference with non-CINs, where _L_ is the corresponding sequence length of a non-CIN network. For more details, check out the videos below describing Continual 3D CNNs [[1](https://arxiv.org/abs/2106.00050)] and Transformers [[2](https://arxiv.org/abs/2201.06268)].
+
+
+<div align="center">
+  <a href="http://www.youtube.com/watch?feature=player_embedded&v=Jm2A7dVEaF4" target="_blank">
+     <img src="http://img.youtube.com/vi/Jm2A7dVEaF4/hqdefault.jpg" alt="Presentation of Continual 3D CNNs" style="width:240px;height:auto;" />
+  </a>
+  <a href="http://www.youtube.com/watch?feature=player_embedded&v=gy802Tlp-eQ" target="_blank">
+     <img src="http://img.youtube.com/vi/gy802Tlp-eQ/hqdefault.jpg" alt="Presentation of Continual Transformers" style="width:240px;height:auto;" />
+  </a>
+</div>
+
+## News
+- 2022-12-02: ONNX compatibility for all modules is available from v1.0.0. See [test_onnx.py](tests/continual/test_onnx.py) for examples.
+
+
+## Quick-start
+
+### Install 
+```bash
+pip install continual-inference
+```
+
+
+
+### Example
+`co` modules are weight-compatible drop-in replacement for `torch.nn`, enhanced with the capability of efficient _continual inference_:
+
+```python3
+import torch
+import continual as co
+                                                           
+#                      B, C, T, H, W
+example = torch.randn((1, 1, 5, 3, 3))
+
+conv = co.Conv3d(in_channels=1, out_channels=1, kernel_size=(3, 3, 3))
+
+# Same exact computation as torch.nn.Conv3d ✅
+output = conv(example)
+
+# But can also perform online inference efficiently 🚀
+firsts = conv.forward_steps(example[:, :, :4])
+last = conv.forward_step(example[:, :, 4])
+
+assert torch.allclose(output[:, :, : conv.delay], firsts)
+assert torch.allclose(output[:, :, conv.delay], last)
+
+# Temporal properties
+assert conv.receptive_field == 3
+assert conv.delay == 2
+```
+
+See the [network composition](#composition) and [model zoo](#model-zoo-and-benchmarks) sections for additional examples.
+
+## Library principles
+
+### Forward modes
+The library components feature three distinct forward modes, which are handy for different situations, namely `forward`, `forward_step`, and `forward_steps`:
+
+#### `forward(input)`
+Performs a forward computation over multiple time-steps. This function is identical to the corresponding module in _torch.nn_, ensuring cross-compatibility. Moreover, it's handy for efficient training on clip-based data.
+
+```
+         O            (O: output)
+         ↑ 
+         N            (N: network module)
+         ↑ 
+ -----------------    (-: aggregation)
+ P   I   I   I   P    (I: input frame, P: padding)
+```
+
+
+#### `forward_step(input, update_state=True)`
+Performs a forward computation for a single frame and (optionally) updates internal states accordingly. This function performs efficient continual inference.
+
+```
+O+S O+S O+S O+S   (O: output, S: updated internal state)
+ ↑   ↑   ↑   ↑ 
+ N   N   N   N    (N: network module)
+ ↑   ↑   ↑   ↑ 
+ I   I   I   I    (I: input frame)
+```
+
+#### `forward_steps(input, pad_end=False, update_state=True)`
+Performs a forward computation across multiple time-steps while updating internal states for continual inference (if update_state=True).
+Start-padding is always accounted for, but end-padding is omitted per default in expectance of the next input step. It can be added by specifying pad_end=True. If so, the output-input mapping the exact same as that of forward.
+```
+         O            (O: output)
+         ↑ 
+ -----------------    (-: aggregation)
+ O  O+S O+S O+S  O    (O: output, S: updated internal state)
+ ↑   ↑   ↑   ↑   ↑
+ N   N   N   N   N    (N: network module)
+ ↑   ↑   ↑   ↑   ↑
+ P   I   I   I   P    (I: input frame, P: padding)
+```
+
+#### `__call__`
+Per default, the `__call__` function operates identically to _torch.nn_ and executes forward. We supply two options for changing this behavior, namely the _call_mode_ property and the _call_mode_ context manager. An example of their use follows:
+
+```python
+timeseries = torch.randn(batch, channel, time)
+timestep = timeseries[:, :, 0]
+
+net(timeseries)  # Invokes net.forward(timeseries)
+
+# Assign permanent call_mode property
+net.call_mode = "forward_step"
+net(timestep)  # Invokes net.forward_step(timestep)
+
+# Assign temporary call_mode with context manager
+with co.call_mode("forward_steps"):
+    net(timeseries)  # Invokes net.forward_steps(timeseries)
+
+net(timestep)  # Invokes net.forward_step(timestep) again
+```
+
+### Composition
+
+Continual Inference Networks require strict handling of internal data delays to guarantee correspondence between [forward modes](#forward-modes). While it is possible to compose neural networks by defining _forward_, _forward_step_, and _forward_steps_ manually, correct handling of delays is cumbersome and time-consuming. Instead, we provide a rich interface of container modules, which handles delays automatically. On top of `co.Sequential` (which is a drop-in replacement of _torch.nn.Sequential_), we provide modules for handling parallel and conditional dataflow. 
+
+- [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
+- [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
+- [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
+- [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
+- [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
+- [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
+- [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
+- [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
+
+
+#### Composition examples:
+
+<details>
+<summary><b>Residual module</b></summary>
+
+Short-hand:
+```python3
+residual = co.Residual(co.Conv3d(32, 32, kernel_size=3, padding=1))
+```
+
+Explicit:
+```python3
+residual = co.Sequential(
+    co.Broadcast(2),
+    co.Parallel(
+        co.Conv3d(32, 32, kernel_size=3, padding=1),
+        co.Delay(2),
+    ),
+    co.Reduce("sum"),
+)
+```
+
+</details>
+
+<details>
+<summary><b>3D MobileNetV2 Inverted residual block</b></summary>
+
+Continual 3D version of the [MobileNetV2 Inverted residual block](https://arxiv.org/pdf/1801.04381.pdf).
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/mb_conv.png" style="width: 15vw; min-width: 200px;">
+  <br>
+  MobileNetV2 Inverted residual block. Source: https://arxiv.org/pdf/1801.04381.pdf
+</div>
+
+```python3
+mb_conv = co.Residual(
+    co.Sequential(
+      co.Conv3d(32, 64, kernel_size=(1, 1, 1)),
+      nn.BatchNorm3d(64),
+      nn.ReLU6(),
+      co.Conv3d(64, 64, kernel_size=(3, 3, 3), padding=(1, 1, 1), groups=64),
+      nn.ReLU6(),
+      co.Conv3d(64, 32, kernel_size=(1, 1, 1)),
+      nn.BatchNorm3d(32),
+    )
+)
+```
+
+</details>
+
+<details>
+<summary><b>3D Squeeze-and-Excitation module</b></summary>
+
+Continual 3D version of the [Squeeze-and-Excitation module](https://arxiv.org/pdf/1709.01507.pdf)
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/se_block.png" style="width: 15vw; min-width: 200px;">
+  <br>
+  Squeeze-and-Excitation block. 
+  Scale refers to a broadcasted element-wise multiplication.
+  Adapted from: https://arxiv.org/pdf/1709.01507.pdf
+</div>
+
+```python3
+se = co.Residual(
+    co.Sequential(
+        OrderedDict([
+            ("pool", co.AdaptiveAvgPool3d((1, 1, 1), kernel_size=7)),
+            ("down", co.Conv3d(256, 16, kernel_size=1)),
+            ("act1", nn.ReLU()),
+            ("up", co.Conv3d(16, 256, kernel_size=1)),
+            ("act2", nn.Sigmoid()),
+        ])
+    ),
+    reduce="mul",
+)
+```
+
+</details>
+
+<details>
+<summary><b>3D Inception module</b></summary>
+
+Continual 3D version of the [Inception module](https://arxiv.org/pdf/1409.4842v1.pdf):
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/examples/inception_block.png" style="width: 25vw; min-width: 350px;">
+  <br>
+  Inception module. Source: https://arxiv.org/pdf/1409.4842v1.pdf
+   
+</div>
+
+```python3
+def norm_relu(module, channels):
+    return co.Sequential(
+        module,
+        nn.BatchNorm3d(channels),
+        nn.ReLU(),
+    )
+
+inception_module = co.BroadcastReduce(
+    co.Conv3d(192, 64, kernel_size=1),
+    co.Sequential(
+        norm_relu(co.Conv3d(192, 96, kernel_size=1), 96),
+        norm_relu(co.Conv3d(96, 128, kernel_size=3, padding=1), 128),
+    ),
+    co.Sequential(
+        norm_relu(co.Conv3d(192, 16, kernel_size=1), 16),
+        norm_relu(co.Conv3d(16, 32, kernel_size=5, padding=2), 32),
+    ),
+    co.Sequential(
+        co.MaxPool3d(kernel_size=(1, 3, 3), padding=(0, 1, 1), stride=1),
+        norm_relu(co.Conv3d(192, 32, kernel_size=1), 32),
+    ),
+    reduce="concat",
+)
+```
+</details>
+
+
+### Input shapes
+We enforce a unified ordering of input dimensions for all library modules, namely:
+
+    (batch, channel, time, optional_dim2, optional_dim3)
+
+### Outputs
+The outputs produces by `forward_step` and `forward_steps` are identical to those of `forward`, provided the same data was input beforehand and state update was enabled. We know that input and output shapes aren't necessarily the same when using `forward` in the PyTorch library, and  generally depends on padding, stride and receptive field of a module. 
+
+For the `forward_step` function, this comes to show by some `None`-valued outputs. Specifically, modules with a _delay_ (i.e. with receptive fields larger than the padding + 1) will produce `None` until the input count exceeds the delay. Moreover, _stride_ > 1 will produce `Tensor` outputs every _stride_ steps and `None` the remaining steps. A visual example is shown below:
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/continual/continual-stride.png" style="width:300px;height:auto;"/>
+  </br>
+  A mixed example of delay and outputs under padding and stride. Here, we illustrate the step-wise operation of two co module layers, l1 with with receptive_field = 3, padding = 2, and stride = 2 and l2 with receptive_field = 3, no padding and stride = 1. ⧇ denotes a padded zero, ■ is a non-zero step-feature, and ☒ is an empty output.
+</div>
+
+For more information, please see the [library paper](https://arxiv.org/abs/2204.03418).
+
+### Handling state
+During stream processing, network modules which operate over multiple time-steps, e.g., a convolution with `kernel_size > 1` in the temporal dimension, will aggregate and cache state internally. Each module has its own local state, which can be inspected using `module.get_state()`. During `forward_step` and `forward_steps`, the state is updated unless the forward_step(s) is invoked with an `update_state = False` argument.
+
+A __state cleanup__ can be accomplished via `module.clean_state()`.
+
+
+## Module library
+_Continual Inference_ features a rich collection of modules for defining Continual Inference Networks. Specific care was taken to create CIN versions of the PyTorch modules found in [_torch.nn_](https://pytorch.org/docs/stable/nn.html):
+
+<details>
+<summary><b>Convolutions</b></summary>
+
+- [`co.Conv1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv1d.html)
+- [`co.Conv2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv2d.html)
+- [`co.Conv3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conv3d.html)
+
+</details>
+
+<details>
+<summary><b>Pooling</b></summary>
+
+  - [`co.AvgPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool1d.html)
+  - [`co.AvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool2d.html)
+  - [`co.AvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AvgPool3d.html)
+  - [`co.MaxPool1d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool1d.html)
+  - [`co.MaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool2d.html)
+  - [`co.MaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.MaxPool3d.html)
+  - [`co.AdaptiveAvgPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool2d.html)
+  - [`co.AdaptiveAvgPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveAvgPool3d.html)
+  - [`co.AdaptiveMaxPool2d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool2d.html)
+  - [`co.AdaptiveMaxPool3d`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.AdaptiveMaxPool3d.html)
+
+</details>
+
+<details>
+<summary><b>Linear</b></summary>
+
+  - [`co.Linear`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Linear.html)
+  - [`co.Identity`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Identity.html): Maps input to output without modification.
+  - [`co.Add`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Add.html): Adds a constant value.
+  - [`co.Multiply`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Multiply.html): Multiplies with a constant factor.
+
+</details>
+
+<details>
+<summary><b>Recurrent</b></summary>
+
+  - [`co.RNN`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RNN.html)
+  - [`co.LSTM`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.LSTM.html)
+  - [`co.GRU`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.GRU.html)
+
+</details>
+
+<details>
+<summary><b>Transformers</b></summary>
+
+  - [`co.TransformerEncoder`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoder.html)
+  - [`co.TransformerEncoderLayerFactory`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.TransformerEncoderLayerFactory.html): Factory function corresponding to `nn.TransformerEncoderLayer`.
+  - [`co.SingleOutputTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.SingleOutputTransformerEncoderLayer.html): SingleOutputMHA version of `nn.TransformerEncoderLayer`.
+  - [`co.RetroactiveTransformerEncoderLayer`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RetroactiveTransformerEncoderLayer.html): RetroactiveMHA version of `nn.TransformerEncoderLayer`.
+  - [`co.RetroactiveMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.retroactive_mha.html.RetroactiveMultiheadAttention): Retroactive version of `nn.MultiheadAttention`.
+  - [`co.SingleOutputMultiheadAttention`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.single_output_mha.html.SingleOutputMultiheadAttention): Single-output version of `nn.MultiheadAttention`.
+  - [`co.RecyclingPositionalEncoding`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.RecyclingPositionalEncoding.html): Positional Encoding used for Continual Transformers.
+
+</details>
+
+
+Modules for composing and converting networks. Both _composition_ and _utility_ modules can be used for regular definition of PyTorch modules as well.
+
+<details>
+<summary><b>Composition modules</b></summary>
+
+  - [`co.Sequential`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Sequential.html): Invoke modules sequentially, passing the output of one module onto the next.
+  - [`co.Broadcast`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Broadcast.html): Broadcast one stream to multiple.
+  - [`co.Parallel`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Parallel.html): Invoke modules in parallel given each their input.
+  - [`co.ParallelDispatch`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.ParallelDispatch.html): Dispatch multiple input streams to multiple output streams flexibly.
+  - [`co.Reduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reduce.html): Reduce multiple input streams to one.
+  - [`co.BroadcastReduce`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.BroadcastReduce.html): Shorthand for Sequential(Broadcast, Parallel, Reduce).
+  - [`co.Residual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Residual.html): Residual connection.
+  - [`co.Conditional`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Conditional.html): Conditionally checks whether to invoke a module (or another) at runtime.
+
+</details>
+
+<details>
+<summary><b>Utility modules</b></summary>
+
+  - [`co.Delay`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Delay.html): Pure delay module (e.g. needed in residuals).
+  - [`co.Skip`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Skip.html): Skip a predefined number of input steps.
+  - [`co.Reshape`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Reshape.html): Reshape non-temporal dimensions.
+  - [`co.Lambda`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Lambda.html): Lambda module which wraps any function.
+  - [`co.Constant`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Constant.html): Maps input to and output with constant value.
+  - [`co.Zero`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.Zero.html): Maps input to output of zeros.
+  - [`co.One`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.One.html): Maps input to output of ones.
+
+</details>
+
+<details>
+<summary><b>Converters</b></summary>
+
+  - [`co.continual`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.continual.html): conversion function from `torch.nn` modules to `co` modules.
+  - [`co.forward_stepping`](https://continual-inference.readthedocs.io/en/latest/common/generated/continual.forward_stepping.html): functional wrapper, which enhances temporally local `torch.nn` modules with the forward_stepping functions.
+
+</details>
+
+We support drop-in interoperability with with the following _torch.nn_ modules:
+
+<details>
+<summary><b>Activation</b></summary>
+
+  - `nn.Threshold`
+  - `nn.ReLU`
+  - `nn.RReLU`
+  - `nn.Hardtanh`
+  - `nn.ReLU6`
+  - `nn.Sigmoid`
+  - `nn.Hardsigmoid`
+  - `nn.Tanh`
+  - `nn.SiLU`
+  - `nn.Hardswish`
+  - `nn.ELU`
+  - `nn.CELU`
+  - `nn.SELU`
+  - `nn.GLU`
+  - `nn.GELU`
+  - `nn.Hardshrink`
+  - `nn.LeakyReLU`
+  - `nn.LogSigmoid`
+  - `nn.Softplus`
+  - `nn.Softshrink`
+  - `nn.PReLU`
+  - `nn.Softsign`
+  - `nn.Tanhshrink`
+  - `nn.Softmin`
+  - `nn.Softmax`
+  - `nn.Softmax2d`
+  - `nn.LogSoftmax`
+
+</details>
+
+<details>
+<summary><b>Normalization</b></summary>
+
+  - `nn.BatchNorm1d`
+  - `nn.BatchNorm2d`
+  - `nn.BatchNorm3d`
+  - `nn.GroupNorm`,
+  - `nn.InstanceNorm1d` (affine=True, track_running_stats=True required)
+  - `nn.InstanceNorm2d` (affine=True, track_running_stats=True required)
+  - `nn.InstanceNorm3d` (affine=True, track_running_stats=True required)
+  - `nn.LayerNorm` (only non-temporal dimensions must be specified)
+
+</details>
+
+<details>
+<summary><b>Dropout</b></summary>
+
+  - `nn.Dropout`
+  - `nn.Dropout1d`
+  - `nn.Dropout2d`
+  - `nn.Dropout3d`
+  - `nn.AlphaDropout`
+  - `nn.FeatureAlphaDropout`
+
+</details>
+
+
+## Model Zoo and Benchmarks
+
+### Continual 3D CNNs
+
+Benchmark results for 1-view testing on __Kinetics400__. For reference, _X3D-L_ scores 69.3% top-1 acc with 19.2 GFLOPs per prediction. 
+
+Arch     | Avg. pool size | Top 1 (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                   | Weights
+-------- | -------------- | --------- | ------------------ | --------------- | ---------- | ---------------------------------------------------------------------- | ---- 
+CoX3D-L  | 64             | 71.6      | 1.25               | 15.3x           | 6.2        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_L.pyth)
+CoX3D-M  | 64             | 71.0      | 0.33               | 15.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_M.pyth)
+CoX3D-S  | 64             | 64.7      | 0.17               | 12.1x           | 3.8        | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/cox3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/X3D\_S.pyth)
+CoSlow   | 64             | 73.1      | 6.90               |  8.0x           | 32.5       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coslow) | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/SLOW\_8x8\_R50.pyth)
+CoI3D    | 64             | 64.0      | 5.68               |  5.0x           | 28.0       | [link](https://github.com/LukasHedegaard/co3d/tree/main/models/coi3d)  | [link](https://dl.fbaipublicfiles.com/pytorchvideo/model_zoo/kinetics/I3D\_8x8\_R50.pyth)
+
+FLOPs reduction is noted relative to non-continual inference.
+Note that [on-hardware inference](https://arxiv.org/abs/2106.00050) doesn't reach the same speedups as "FLOPs reductions" might suggest due to overhead of state reads and writes. This overhead is less important for large batch sizes. This applies to all models in the model zoo.
+
+### Continual ST-GCNs
+
+Benchmark results for on __NTU RGB+D 60__ for the joint modality. For reference, _ST-GCN_ achieves 86% X-Sub and 93.4 X-View accuracy with 16.73 GFLOPs per prediction. 
+
+Arch      | Receptive field | X-Sub Acc (%) | X-View Acc (%) | FLOPs (G) per step | FLOPs reduction | Params (M) | Code                                                                  
+--------  | --------------- | ------------- | -------------- | ------------------ | --------------- | ---------- | -----
+CoST-GCN  | 300             | 86.3          | 93.8           | 0.16               | 107.7x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cost_gcn_mod/cost_gcn_mod.py)
+CoA-GCN   | 300             | 84.1          | 92.6           | 0.17               | 108.7x          | 3.5        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/coa_gcn_mod/coa_gcn_mod.py)
+CoST-GCN  | 300             | 86.3          | 92.4           | 0.15               | 107.6x          | 3.1        | [link](https://github.com/LukasHedegaard/continual-skeletons/blob/main/models/cos_tr_mod/cos_tr_mod.py)
+
+[Here](https://drive.google.com/drive/u/4/folders/1m6aV5Zv8tAytvxF6qY4m9nyqlkKv0y72), you can download pre-trained,model weights for the above architectures on NTU RGB+D 60, NTU RGB+D 120, and Kinetics-400 on joint and bone modalities.
+
+
+### Continual Transformers
+
+Benchmark results for on __THUMOS14__ on top of features extracted using a TSN-ResNet50 backbone pre-trained on Kinetics400. For reference, _OadTR_ achieves 64.4 % mAP with 2.5 GFLOPs per prediction. 
+
+Arch        | Receptive field | mAP (%) | FLOPs (G) per step |  Params (M) | Code                                                                  
+----------  | --------------- | ------- | ------------------ |  ---------- | -----
+CoOadTR-b1  | 64              | 64.2    | 0.41               |  15.9       | [link](https://github.com/LukasHedegaard/CoOadTR)
+CoOadTR-b2  | 64              | 64.4    | 0.01               |   9.6       | [link](https://github.com/LukasHedegaard/CoOadTR)
+
+The library features complete implementations of the [one](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L8)- and [two](https://github.com/LukasHedegaard/continual-inference/blob/9895344f50a93ebb5cf5c4f26ecfdf27b6a3fe75/tests/continual/test_transformer.py#L59)-block continual transformer encoders as well.
+
+
+## Compatibility
+The library modules are built to integrate seamlessly with other PyTorch projects.
+Specifically, extra care was taken to ensure out-of-the-box compatibility with:
+- [pytorch-lightning](https://github.com/PyTorchLightning/pytorch-lightning)
+- [ptflops](https://github.com/sovrasov/flops-counter.pytorch)
+- [ride](https://github.com/LukasHedegaard/ride)
+- [onnx](https://github.com/onnx/onnx)
+<!-- - [onnxruntime](https://github.com/microsoft/onnxruntime) -->
+
+
+## Citation
+<a href="https://arxiv.org/abs/2204.03418" style="display:inline-block;">
+  <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
+</a>
+
+```bibtex
+@inproceedings{hedegaard2022colib,
+  title={Continual Inference: A Library for Efficient Online Inference with Deep Neural Networks in PyTorch},
+  author={Lukas Hedegaard and Alexandros Iosifidis},
+  booktitle={European Conference on Computer Vision Workshops (ECCVW)},
+  year={2022}
+}
+```
+
+
+## Acknowledgement
+This work has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 871449 (OpenDR).
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,37 @@
-Metadata-Version: 2.1 Name: continual-inference Version: 1.2.2 Summary: A
+Metadata-Version: 2.1 Name: continual-inference Version: 1.2.3 Summary: A
 Python library for Continual Inference Networks in PyTorch Home-page: https://
 github.com/lukashedegaard/continual-inference Author: Lukas Hedegaard Author-
-email: lukasxhedegaard@gmail.com License: UNKNOWN Description: [https://
-raw.githubusercontent.com/LukasHedegaard/continual-inference/main/figures/logo/
-logo_name.svg] __A Python library for Continual Inference Networks in PyTorch__
-[Quick-start](https://continual-inference.readthedocs.io/en/latest/generated/
-README.html#quick-start) â¢ [Docs](https://continual-inference.readthedocs.io/
-en/latest/generated/README.html) â¢ [Principles](https://continual-
-inference.readthedocs.io/en/latest/generated/README.html#library-principles)
-â¢ [Paper](https://arxiv.org/abs/2204.03418) â¢ [Examples](https://continual-
-inference.readthedocs.io/en/latest/generated/README.html#composition-examples)
-â¢ [Modules](https://continual-inference.readthedocs.io/en/latest/common/
-modules.html) â¢ [Model Zoo](https://continual-inference.readthedocs.io/en/
-latest/generated/README.html#model-zoo-and-benchmarks) â¢ [Contribute](https:/
-/continual-inference.readthedocs.io/en/latest/generated/CONTRIBUTING.html) â¢
-[License](https://github.com/LukasHedegaard/continual-inference/blob/main/
-LICENSE)
+email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
+learning,pytorch,AI,online,inference,continual Platform: UNKNOWN Classifier:
+Environment :: Console Classifier: Natural Language :: English Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Recognition Classifier:
+Topic :: Scientific/Engineering :: Information Analysis Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
+Provides-Extra: build Provides-Extra: dev Provides-Extra: docs License-File:
+LICENSE [https://raw.githubusercontent.com/LukasHedegaard/continual-inference/
+main/figures/logo/logo_name.svg] __A Python library for Continual Inference
+Networks in PyTorch__ [Quick-start](https://continual-inference.readthedocs.io/
+en/latest/generated/README.html#quick-start) â¢ [Docs](https://continual-
+inference.readthedocs.io/en/latest/generated/README.html) â¢ [Principles]
+(https://continual-inference.readthedocs.io/en/latest/generated/
+README.html#library-principles) â¢ [Paper](https://arxiv.org/abs/2204.03418)
+â¢ [Examples](https://continual-inference.readthedocs.io/en/latest/generated/
+README.html#composition-examples) â¢ [Modules](https://continual-
+inference.readthedocs.io/en/latest/common/modules.html) â¢ [Model Zoo](https:/
+/continual-inference.readthedocs.io/en/latest/generated/README.html#model-zoo-
+and-benchmarks) â¢ [Contribute](https://continual-inference.readthedocs.io/en/
+latest/generated/CONTRIBUTING.html) â¢ [License](https://github.com/
+LukasHedegaard/continual-inference/blob/main/LICENSE)
 [https://img.shields.io/pypi/pyversions/continual-inference] [https://
 badge.fury.io/py/continual-inference.svg] [Documentation_Status] [https://
 pepy.tech/badge/continual-inference] [https://codecov.io/gh/LukasHedegaard/
 continual-inference/branch/main/graph/badge.svg?token=XW1UQZSEOG] [https://
 img.shields.io/badge/License-Apache%202.0-blue.svg]  [https://img.shields.io/
 badge/code%20style-black-000000.svg] [We_match_PyTorch_interfaces_exactly.
 Method_arguments_named_'input'_reduce_the_codefactor_to_'A-']
@@ -349,20 +361,8 @@
 [onnx](https://github.com/onnx/onnx)  ## Citation [http://img.shields.io/badge/
 paper-arxiv.2204.03418-B31B1B.svg] ```bibtex @inproceedings{hedegaard2022colib,
 title={Continual Inference: A Library for Efficient Online Inference with Deep
 Neural Networks in PyTorch}, author={Lukas Hedegaard and Alexandros Iosifidis},
 booktitle={European Conference on Computer Vision Workshops (ECCVW)}, year=
 {2022} } ``` ## Acknowledgement This work has received funding from the
 European Unionâs Horizon 2020 research and innovation programme under grant
-agreement No 871449 (OpenDR). Keywords: deep
-learning,pytorch,AI,online,inference,continual Platform: UNKNOWN Classifier:
-Environment :: Console Classifier: Natural Language :: English Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition Classifier:
-Topic :: Scientific/Engineering :: Information Analysis Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
-Provides-Extra: build Provides-Extra: dev Provides-Extra: docs
+agreement No 871449 (OpenDR).
```

### Comparing `continual-inference-1.2.2/continual_inference.egg-info/SOURCES.txt` & `continual-inference-1.2.3/continual_inference.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 continual/__about__.py
 continual/__init__.py
 continual/closure.py
 continual/container.py
 continual/conv.py
```

### Comparing `continual-inference-1.2.2/setup.py` & `continual-inference-1.2.3/setup.py`

 * *Files identical despite different names*

