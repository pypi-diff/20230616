# Comparing `tmp/dedeshot-0.0.1.tar.gz` & `tmp/dedeshot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedeshot-0.0.1.tar", max compression
+gzip compressed data, was "dedeshot-0.0.2.tar", max compression
```

## Comparing `dedeshot-0.0.1.tar` & `dedeshot-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1084 2023-06-15 21:40:06.574964 dedeshot-0.0.1/LICENSE
--rw-r--r--   0        0        0    19296 2023-06-15 21:40:06.575266 dedeshot-0.0.1/README.md
--rw-r--r--   0        0        0     3033 2023-06-15 21:40:06.575497 dedeshot-0.0.1/d3dshot/__init__.py
--rw-r--r--   0        0        0     2249 2023-06-15 21:40:06.575647 dedeshot-0.0.1/d3dshot/capture_output.py
--rw-r--r--   0        0        0        0 2023-06-15 21:40:06.575781 dedeshot-0.0.1/d3dshot/capture_outputs/__init__.py
--rw-r--r--   0        0        0     1763 2023-06-15 21:40:06.575966 dedeshot-0.0.1/d3dshot/capture_outputs/numpy_capture_output.py
--rw-r--r--   0        0        0      478 2023-06-15 21:40:06.576101 dedeshot-0.0.1/d3dshot/capture_outputs/numpy_float_capture_output.py
--rw-r--r--   0        0        0     1589 2023-06-15 21:40:06.576235 dedeshot-0.0.1/d3dshot/capture_outputs/pil_capture_output.py
--rw-r--r--   0        0        0     1960 2023-06-15 21:40:06.576354 dedeshot-0.0.1/d3dshot/capture_outputs/pytorch_capture_output.py
--rw-r--r--   0        0        0      476 2023-06-15 21:40:06.576474 dedeshot-0.0.1/d3dshot/capture_outputs/pytorch_float_capture_output.py
--rw-r--r--   0        0        0      537 2023-06-15 21:40:06.576584 dedeshot-0.0.1/d3dshot/capture_outputs/pytorch_float_gpu_capture_output.py
--rw-r--r--   0        0        0      607 2023-06-15 21:40:06.576696 dedeshot-0.0.1/d3dshot/capture_outputs/pytorch_gpu_capture_output.py
--rw-r--r--   0        0        0    10242 2023-06-15 21:40:06.576917 dedeshot-0.0.1/d3dshot/d3dshot.py
--rw-r--r--   0        0        0     4781 2023-06-15 21:40:06.577090 dedeshot-0.0.1/d3dshot/display.py
--rw-r--r--   0        0        0        0 2023-06-15 21:40:06.577222 dedeshot-0.0.1/d3dshot/dll/__init__.py
--rw-r--r--   0        0        0    13399 2023-06-15 21:40:06.577439 dedeshot-0.0.1/d3dshot/dll/d3d.py
--rw-r--r--   0        0        0    11325 2023-06-15 21:40:06.577633 dedeshot-0.0.1/d3dshot/dll/dxgi.py
--rw-r--r--   0        0        0      257 2023-06-15 21:40:06.577741 dedeshot-0.0.1/d3dshot/dll/shcore.py
--rw-r--r--   0        0        0     1583 2023-06-15 21:40:06.577869 dedeshot-0.0.1/d3dshot/dll/user32.py
--rw-r--r--   0        0        0     1277 2023-06-15 21:41:16.339975 dedeshot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    20522 1970-01-01 00:00:00.000000 dedeshot-0.0.1/setup.py
--rw-r--r--   0        0        0    20805 1970-01-01 00:00:00.000000 dedeshot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-15 21:40:06.574964 dedeshot-0.0.2/LICENSE
+-rw-r--r--   0        0        0    19296 2023-06-15 21:40:06.575266 dedeshot-0.0.2/README.md
+-rw-r--r--   0        0        0     3005 2023-06-15 22:10:29.395939 dedeshot-0.0.2/dedeshot/__init__.py
+-rw-r--r--   0        0        0     2256 2023-06-15 22:10:29.949109 dedeshot-0.0.2/dedeshot/capture_output.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:40:06.575781 dedeshot-0.0.2/dedeshot/capture_outputs/__init__.py
+-rw-r--r--   0        0        0     1764 2023-06-15 22:10:37.223749 dedeshot-0.0.2/dedeshot/capture_outputs/numpy_capture_output.py
+-rw-r--r--   0        0        0      479 2023-06-15 22:10:36.652237 dedeshot-0.0.2/dedeshot/capture_outputs/numpy_float_capture_output.py
+-rw-r--r--   0        0        0     1590 2023-06-15 22:10:36.042259 dedeshot-0.0.2/dedeshot/capture_outputs/pil_capture_output.py
+-rw-r--r--   0        0        0     1961 2023-06-15 22:10:35.416253 dedeshot-0.0.2/dedeshot/capture_outputs/pytorch_capture_output.py
+-rw-r--r--   0        0        0      477 2023-06-15 22:10:34.640615 dedeshot-0.0.2/dedeshot/capture_outputs/pytorch_float_capture_output.py
+-rw-r--r--   0        0        0      538 2023-06-15 22:10:34.053038 dedeshot-0.0.2/dedeshot/capture_outputs/pytorch_float_gpu_capture_output.py
+-rw-r--r--   0        0        0      608 2023-06-15 22:10:33.415613 dedeshot-0.0.2/dedeshot/capture_outputs/pytorch_gpu_capture_output.py
+-rw-r--r--   0        0        0    10242 2023-06-15 22:10:28.706286 dedeshot-0.0.2/dedeshot/dedeshot.py
+-rw-r--r--   0        0        0     4808 2023-06-15 22:10:27.466690 dedeshot-0.0.2/dedeshot/display.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:40:06.577222 dedeshot-0.0.2/dedeshot/dll/__init__.py
+-rw-r--r--   0        0        0    13399 2023-06-15 21:40:06.577439 dedeshot-0.0.2/dedeshot/dll/d3d.py
+-rw-r--r--   0        0        0    11342 2023-06-15 22:10:32.733453 dedeshot-0.0.2/dedeshot/dll/dxgi.py
+-rw-r--r--   0        0        0      257 2023-06-15 21:40:06.577741 dedeshot-0.0.2/dedeshot/dll/shcore.py
+-rw-r--r--   0        0        0     1583 2023-06-15 21:40:06.577869 dedeshot-0.0.2/dedeshot/dll/user32.py
+-rw-r--r--   0        0        0     1278 2023-06-15 22:11:05.575229 dedeshot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    20525 1970-01-01 00:00:00.000000 dedeshot-0.0.2/setup.py
+-rw-r--r--   0        0        0    20805 1970-01-01 00:00:00.000000 dedeshot-0.0.2/PKG-INFO
```

### Comparing `dedeshot-0.0.1/LICENSE` & `dedeshot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dedeshot-0.0.1/README.md` & `dedeshot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dedeshot-0.0.1/d3dshot/__init__.py` & `dedeshot-0.0.2/dedeshot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import importlib.util
 
-from d3dshot.d3dshot import D3DShot
-from d3dshot.capture_output import CaptureOutputs
+from dedeshot.dedeshot import D3DShot
+from dedeshot.capture_output import CaptureOutputs
 
 
 pil_is_available = importlib.util.find_spec("PIL") is not None
 numpy_is_available = importlib.util.find_spec("numpy") is not None
 
-pytorch_is_available = (
-    importlib.util.find_spec("torch") is not None and numpy_is_available
-)
+pytorch_is_available = importlib.util.find_spec("torch") is not None and numpy_is_available
 
 pytorch_gpu_is_available = False
 
 if pytorch_is_available:
     import torch
 
     pytorch_gpu_is_available = torch.cuda.is_available()
@@ -80,22 +78,20 @@
 def _validate_capture_output(capture_output):
     available_capture_outputs = determine_available_capture_outputs()
 
     capture_output_name = capture_output
     capture_output = capture_output_mapping.get(capture_output)
 
     if capture_output not in available_capture_outputs:
-        available_capture_outputs = [
-            capture_outputs[co.value] for co in available_capture_outputs
-        ]
+        available_capture_outputs = [capture_outputs[co.value] for co in available_capture_outputs]
         raise AttributeError(
             f"Invalid Capture Output '{capture_output_name}'. Available Options: {', '.join(available_capture_outputs)}"
         )
 
     return capture_output
 
 
 def _validate_frame_buffer_size(frame_buffer_size):
     if not isinstance(frame_buffer_size, int) or frame_buffer_size < 1:
-        raise AttributeError(f"'frame_buffer_size' should be an int greater than 0")
+        raise AttributeError("'frame_buffer_size' should be an int greater than 0")
 
     return frame_buffer_size
```

### Comparing `dedeshot-0.0.1/d3dshot/capture_output.py` & `dedeshot-0.0.2/dedeshot/capture_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,40 +26,40 @@
         return self.backend.to_pil(frame)
 
     def stack(self, frames, stack_dimension):
         return self.backend.stack(frames, stack_dimension)
 
     def _initialize_backend(self, backend):
         if backend == CaptureOutputs.PIL:
-            from d3dshot.capture_outputs.pil_capture_output import PILCaptureOutput
+            from dedeshot.capture_outputs.pil_capture_output import PILCaptureOutput
 
             return PILCaptureOutput()
         elif backend == CaptureOutputs.NUMPY:
-            from d3dshot.capture_outputs.numpy_capture_output import NumpyCaptureOutput
+            from dedeshot.capture_outputs.numpy_capture_output import NumpyCaptureOutput
 
             return NumpyCaptureOutput()
         elif backend == CaptureOutputs.NUMPY_FLOAT:
-            from d3dshot.capture_outputs.numpy_float_capture_output import NumpyFloatCaptureOutput
+            from dedeshot.capture_outputs.numpy_float_capture_output import NumpyFloatCaptureOutput
 
             return NumpyFloatCaptureOutput()
         elif backend == CaptureOutputs.PYTORCH:
-            from d3dshot.capture_outputs.pytorch_capture_output import PytorchCaptureOutput
+            from dedeshot.capture_outputs.pytorch_capture_output import PytorchCaptureOutput
 
             return PytorchCaptureOutput()
         elif backend == CaptureOutputs.PYTORCH_FLOAT:
-            from d3dshot.capture_outputs.pytorch_float_capture_output import (
+            from dedeshot.capture_outputs.pytorch_float_capture_output import (
                 PytorchFloatCaptureOutput,
             )
 
             return PytorchFloatCaptureOutput()
         elif backend == CaptureOutputs.PYTORCH_GPU:
-            from d3dshot.capture_outputs.pytorch_gpu_capture_output import PytorchGPUCaptureOutput
+            from dedeshot.capture_outputs.pytorch_gpu_capture_output import PytorchGPUCaptureOutput
 
             return PytorchGPUCaptureOutput()
         elif backend == CaptureOutputs.PYTORCH_FLOAT_GPU:
-            from d3dshot.capture_outputs.pytorch_float_gpu_capture_output import (
+            from dedeshot.capture_outputs.pytorch_float_gpu_capture_output import (
                 PytorchFloatGPUCaptureOutput,
             )
 
             return PytorchFloatGPUCaptureOutput()
         else:
             raise CaptureOutputError("The specified backend is invalid!")
```

### Comparing `dedeshot-0.0.1/d3dshot/capture_outputs/numpy_capture_output.py` & `dedeshot-0.0.2/dedeshot/capture_outputs/numpy_capture_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ctypes
 
 import numpy as np
 
 from PIL import Image
 
-from d3dshot.capture_output import CaptureOutput
+from dedeshot.capture_output import CaptureOutput
 
 
 class NumpyCaptureOutput(CaptureOutput):
     def __init__(self):
         pass
 
     def process(self, pointer, pitch, size, width, height, region, rotation):
```

### Comparing `dedeshot-0.0.1/d3dshot/capture_outputs/pil_capture_output.py` & `dedeshot-0.0.2/dedeshot/capture_outputs/pil_capture_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ctypes
 
 from PIL import Image
 
-from d3dshot.capture_output import CaptureOutput
+from dedeshot.capture_output import CaptureOutput
 
 
 class PILCaptureOutput(CaptureOutput):
     def __init__(self):
         pass
 
     def process(self, pointer, pitch, size, width, height, region, rotation):
```

### Comparing `dedeshot-0.0.1/d3dshot/capture_outputs/pytorch_capture_output.py` & `dedeshot-0.0.2/dedeshot/capture_outputs/pytorch_capture_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ctypes
 
 import numpy as np
 import torch
 
 from PIL import Image
 
-from d3dshot.capture_output import CaptureOutput
+from dedeshot.capture_output import CaptureOutput
 
 
 class PytorchCaptureOutput(CaptureOutput):
     def __init__(self):
         pass
 
     def process(self, pointer, pitch, size, width, height, region, rotation):
```

### Comparing `dedeshot-0.0.1/d3dshot/capture_outputs/pytorch_float_gpu_capture_output.py` & `dedeshot-0.0.2/dedeshot/capture_outputs/pytorch_float_gpu_capture_output.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import torch
 
 from PIL import Image
 
-from d3dshot.capture_outputs.pytorch_gpu_capture_output import PytorchGPUCaptureOutput
+from dedeshot.capture_outputs.pytorch_gpu_capture_output import PytorchGPUCaptureOutput
 
 
 class PytorchFloatGPUCaptureOutput(PytorchGPUCaptureOutput):
     def process(self, pointer, pitch, size, width, height, region, rotation):
         image = super().process(pointer, pitch, size, width, height, region, rotation)
         return image.type(torch.cuda.FloatTensor) / 255.0
```

### Comparing `dedeshot-0.0.1/d3dshot/capture_outputs/pytorch_gpu_capture_output.py` & `dedeshot-0.0.2/dedeshot/capture_outputs/pytorch_gpu_capture_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import torch
 
 from PIL import Image
 
-from d3dshot.capture_outputs.pytorch_capture_output import PytorchCaptureOutput
+from dedeshot.capture_outputs.pytorch_capture_output import PytorchCaptureOutput
 
 
 class PytorchGPUCaptureOutput(PytorchCaptureOutput):
     def __init__(self):
         self.device = torch.device("cuda")
         torch.tensor([0], device=self.device)  # Warm up CUDA
```

### Comparing `dedeshot-0.0.1/d3dshot/d3dshot.py` & `dedeshot-0.0.2/dedeshot/dedeshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import threading
 import collections
 
 import gc
 import os
 import time
 
-from d3dshot.display import Display
-from d3dshot.capture_output import CaptureOutput, CaptureOutputs
+from dedeshot.display import Display
+from dedeshot.capture_output import CaptureOutput, CaptureOutputs
 
 
 class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
@@ -187,15 +187,15 @@
         if self._capture_thread is not None:
             self._capture_thread.join(timeout=1)
             self._capture_thread = None
 
         return True
 
     def benchmark(self):
-        print(f"Preparing Benchmark...")
+        print("Preparing Benchmark...")
         print("")
         print(f"Capture Output: {self.capture_output.backend.__class__.__name__}")
         print(f"Display: {self.display}")
         print("")
 
         frame_count = 0
 
@@ -254,15 +254,15 @@
                 'bottom' values are greater than their 'left' and 'top' counterparts"""
             )
 
         return region
 
     def _validate_target_fps(self, target_fps):
         if not isinstance(target_fps, int) or target_fps < 1:
-            raise AttributeError(f"'target_fps' should be an int greater than 0")
+            raise AttributeError("'target_fps' should be an int greater than 0")
 
         return target_fps
 
     def _validate_directory(self, directory):
         if directory is None or not isinstance(directory, str):
             directory = "."
```

### Comparing `dedeshot-0.0.1/d3dshot/display.py` & `dedeshot-0.0.2/dedeshot/display.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import d3dshot.dll.dxgi
-import d3dshot.dll.d3d
-import d3dshot.dll.user32
-import d3dshot.dll.shcore
+import dedeshot.dll.dxgi
+import dedeshot.dll.d3d
+import dedeshot.dll.user32
+import dedeshot.dll.shcore
 
 
 class Display:
     def __init__(
         self,
         name=None,
         adapter_name=None,
@@ -42,34 +42,35 @@
         return f"<Display name={self.name} adapter={self.adapter_name} resolution={self.resolution[0]}x{self.resolution[1]} rotation={self.rotation} scale_factor={self.scale_factor} primary={self.is_primary}>"
 
     def capture(self, process_func, region=None):
         region = self._get_clean_region(region)
         frame = None
 
         try:
-            frame = d3dshot.dll.dxgi.get_dxgi_output_duplication_frame(
+            frame = dedeshot.dll.dxgi.get_dxgi_output_duplication_frame(
                 self.dxgi_output_duplication,
                 self.d3d_device,
                 process_func=process_func,
                 width=self.resolution[0],
                 height=self.resolution[1],
                 region=region,
                 rotation=self.rotation,
             )
         except:
             pass
 
         return frame
 
     def _initialize_dxgi_output_duplication(self):
-        (self.d3d_device, self.d3d_device_context,) = d3dshot.dll.d3d.initialize_d3d_device(
-            self.dxgi_adapter
-        )
+        (
+            self.d3d_device,
+            self.d3d_device_context,
+        ) = dedeshot.dll.d3d.initialize_d3d_device(self.dxgi_adapter)
 
-        return d3dshot.dll.dxgi.initialize_dxgi_output_duplication(
+        return dedeshot.dll.dxgi.initialize_dxgi_output_duplication(
             self.dxgi_output, self.d3d_device
         )
 
     def _get_clean_region(self, region):
         if region is None:
             return (0, 0, self.resolution[0], self.resolution[1])
 
@@ -84,41 +85,41 @@
             self.resolution[1] if region[3] < 0 or region[3] > self.resolution[1] else region[3]
         )
 
         return tuple(clean_region)
 
     @classmethod
     def discover_displays(cls):
-        display_device_name_mapping = d3dshot.dll.user32.get_display_device_name_mapping()
+        display_device_name_mapping = dedeshot.dll.user32.get_display_device_name_mapping()
 
-        dxgi_factory = d3dshot.dll.dxgi.initialize_dxgi_factory()
-        dxgi_adapters = d3dshot.dll.dxgi.discover_dxgi_adapters(dxgi_factory)
+        dxgi_factory = dedeshot.dll.dxgi.initialize_dxgi_factory()
+        dxgi_adapters = dedeshot.dll.dxgi.discover_dxgi_adapters(dxgi_factory)
 
         displays = list()
 
         for dxgi_adapter in dxgi_adapters:
-            dxgi_adapter_description = d3dshot.dll.dxgi.describe_dxgi_adapter(dxgi_adapter)
+            dxgi_adapter_description = dedeshot.dll.dxgi.describe_dxgi_adapter(dxgi_adapter)
 
-            for dxgi_output in d3dshot.dll.dxgi.discover_dxgi_outputs(dxgi_adapter):
-                dxgi_output_description = d3dshot.dll.dxgi.describe_dxgi_output(dxgi_output)
+            for dxgi_output in dedeshot.dll.dxgi.discover_dxgi_outputs(dxgi_adapter):
+                dxgi_output_description = dedeshot.dll.dxgi.describe_dxgi_output(dxgi_output)
 
                 if dxgi_output_description["is_attached_to_desktop"]:
                     display_device = display_device_name_mapping.get(
                         dxgi_output_description["name"]
                     )
 
                     if display_device is None:
                         display_device = ("Unknown", False)
 
-                    hmonitor = d3dshot.dll.user32.get_hmonitor_by_point(
+                    hmonitor = dedeshot.dll.user32.get_hmonitor_by_point(
                         dxgi_output_description["position"]["left"],
                         dxgi_output_description["position"]["top"],
                     )
 
-                    scale_factor = d3dshot.dll.shcore.get_scale_factor_for_monitor(hmonitor)
+                    scale_factor = dedeshot.dll.shcore.get_scale_factor_for_monitor(hmonitor)
 
                     display = cls(
                         name=display_device[0],
                         adapter_name=dxgi_adapter_description,
                         resolution=dxgi_output_description["resolution"],
                         position=dxgi_output_description["position"],
                         rotation=dxgi_output_description["rotation"],
```

### Comparing `dedeshot-0.0.1/d3dshot/dll/d3d.py` & `dedeshot-0.0.2/dedeshot/dll/d3d.py`

 * *Files identical despite different names*

### Comparing `dedeshot-0.0.1/d3dshot/dll/dxgi.py` & `dedeshot-0.0.2/dedeshot/dll/dxgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ctypes
 import ctypes.wintypes as wintypes
 
 import comtypes
 
-from d3dshot.dll.d3d import (
+from dedeshot.dll.d3d import (
     ID3D11Device,
     ID3D11DeviceContext,
     ID3D11Texture2D,
     prepare_d3d11_texture_2d_for_cpu,
 )
 
 
@@ -295,15 +295,17 @@
     region=None,
     rotation=0,
 ):
     dxgi_output_duplication_frame_information = DXGI_OUTDUPL_FRAME_INFO()
     dxgi_resource = ctypes.POINTER(IDXGIResource)()
 
     dxgi_output_duplication.AcquireNextFrame(
-        0, ctypes.byref(dxgi_output_duplication_frame_information), ctypes.byref(dxgi_resource),
+        0,
+        ctypes.byref(dxgi_output_duplication_frame_information),
+        ctypes.byref(dxgi_resource),
     )
 
     frame = None
 
     if dxgi_output_duplication_frame_information.LastPresentTime > 0:
         id3d11_texture_2d = dxgi_resource.QueryInterface(ID3D11Texture2D)
         id3d11_texture_2d_cpu = prepare_d3d11_texture_2d_for_cpu(id3d11_texture_2d, d3d_device)
```

### Comparing `dedeshot-0.0.1/d3dshot/dll/user32.py` & `dedeshot-0.0.2/dedeshot/dll/user32.py`

 * *Files identical despite different names*

### Comparing `dedeshot-0.0.1/pyproject.toml` & `dedeshot-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dedeshot"
-version = "0.0.1"
+version = "0.0.2"
 description = "Extremely Fast and Robust Screen Capture on Windows with the Desktop Duplication API"
 readme = "README.md"
 authors = ["Nicholas Brochu <nicholas@serpent.ai>"]
 license = "MIT"
 repository = "https://github.com/SerpentAI/D3DShot"
 keywords = ["Screen Capture", "Screenshot", "Computer Vision", "Windows"]
 classifiers = [
@@ -17,15 +17,15 @@
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Topic :: Multimedia :: Graphics",
     "Topic :: Multimedia :: Graphics :: Capture",
     "Topic :: Multimedia :: Graphics :: Capture :: Screen Capture",
 ]
-packages = [{ include = "d3dshot" }]
+packages = [{ include = "dedeshot" }]
 include = []
 
 [tool.poetry.dependencies]
 python = ">=3.6"
 
 comtypes = "~1.1.7"
 pillow = "*"
```

### Comparing `dedeshot-0.0.1/setup.py` & `dedeshot-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['d3dshot', 'd3dshot.capture_outputs', 'd3dshot.dll']
+['dedeshot', 'dedeshot.capture_outputs', 'dedeshot.dll']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['comtypes>=1.1.7,<1.2.0', 'pillow']
 
 setup_kwargs = {
     'name': 'dedeshot',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Extremely Fast and Robust Screen Capture on Windows with the Desktop Duplication API',
     'long_description': '# D3DShot\n\n\n_D3DShot_ is a pure Python implementation of the [Windows Desktop Duplication API](https://docs.microsoft.com/en-us/windows/desktop/direct3ddxgi/desktop-dup-api). It leverages DXGI and Direct3D system libraries to enable extremely fast and robust screen capture functionality for your Python scripts and applications on Windows. \n\n**D3DShot:**\n\n* Is by far the fastest way to capture the screen with Python on Windows 8.1+\n* Is very easy to use. If you can remember 10-ish methods, you know the entire thing.\n* Covers all common scenarios and use cases:\n\t* Screenshot to memory\n\t* Screenshot to disk\n\t* Screenshot to memory buffer every X seconds (threaded; non-blocking)\n\t* Screenshot to disk every X seconds (threaded; non-blocking)\n\t* High-speed capture to memory buffer (threaded; non-blocking)\n* Captures to PIL Images out of the box. Gracefully adds output options if NumPy or PyTorch can be found.\n* Detects displays in just about any configuration: Single monitor, multiple monitors on one adapter, multiple monitors on multiple adapters.\n* Handles display rotation and scaling for you\n* Supports capturing specific regions of the screen\n* Is robust and very stable. You can run it for hours / days without performance degradation\n* Is even able to capture DirectX 11 / 12 exclusive fullscreen applications and games!\n\n\n### TL;DR Quick Code Samples\n\n**Screenshot to Memory**\n\n```python\nimport d3dshot\n\nd = d3dshot.create()\nd.screenshot()\n```\n```\nOut[1]: <PIL.Image.Image image mode=RGB size=2560x1440 at 0x1AA7ECB5C88>\n```\n\n**Screenshot to Disk**\n```python\nimport d3dshot\n\nd = d3dshot.create()\nd.screenshot_to_disk()\n```\n```\nOut[1]: \'./1554298682.5632973.png\'\n```\n\n**Screen Capture for 5 Seconds and Grab the Latest Frame**\n```python\nimport d3dshot\nimport time\n\nd = d3dshot.create()\n\nd.capture()\ntime.sleep(5)  # Capture is non-blocking so we wait explicitely\nd.stop()\n\nd.get_latest_frame()\n```\n```\nOut[1]: <PIL.Image.Image image mode=RGB size=2560x1440 at 0x1AA044BCF60>\n```\n\n**Screen Capture the Second Monitor as NumPy Arrays for 3 Seconds and Grab the 4 Latest Frames as a Stack**\n```python\nimport d3dshot\nimport time\n\nd = d3dshot.create(capture_output="numpy")\n\nd.display = d.displays[1]\n\nd.capture()\ntime.sleep(3)  # Capture is non-blocking so we wait explicitely\nd.stop()\n\nframe_stack = d.get_frame_stack((0, 1, 2, 3), stack_dimension="last")\nframe_stack.shape\n```\n```\nOut[1]: (1080, 1920, 3, 4)\n```\n\nThis is barely scratching the surface... Keep reading!\n\n\n## Requirements\n\n* Windows 8.1+ (64-bit)\n* Python 3.6+ (64-bit)\n\n## Installation\n\n```\npip install d3dshot\n```\n\n_D3DShot_ leverages DLLs that are already available on your system so the dependencies are very light. Namely:\n\n* [_comtypes_](https://github.com/enthought/comtypes): Internal use. To preserve developer sanity while working with COM interfaces.\n* [_Pillow_](https://github.com/python-pillow/Pillow): Default Capture Output. Also used to save to disk as PNG and JPG.\n\nThese dependencies will automatically be installed alongside _D3DShot_; No need to worry about them!\n\n##### Extra Step: Laptop Users\n\nWindows has a quirk when using Desktop Duplication on hybrid-GPU systems. Please see the [wiki article](https://github.com/SerpentAI/D3DShot/wiki/Installation-Note:-Laptops) before attempting to use _D3DShot_ on your system.\n\n## Concepts\n\n### Capture Outputs\n\nThe desired _Capture Output_ is defined when creating a _D3DShot_ instance. It defines the type of all captured images. By default, all captures will return PIL.Image objects. This is a good option if you mostly intend to take screenshots.\n\n```python\n# Captures will be PIL.Image in RGB mode\nd = d3dshot.create()\nd = d3dshot.create(capture_output="pil")\n```\n\n_D3DShot_ is however quite flexible! As your environment meets certain optional sets of requirements, more options become available.\n\n\n**If _NumPy_ is available**\n\n```python\n# Captures will be np.ndarray of dtype uint8 with values in range (0, 255)\nd = d3dshot.create(capture_output="numpy")\n\n# Captures will be np.ndarray of dtype float64 with normalized values in range (0.0, 1.0)\nd = d3dshot.create(capture_output="numpy_float")  \n```\n\n**If _NumPy_ and _PyTorch_ are available**\n\n```python\n# Captures will be torch.Tensor of dtype uint8 with values in range (0, 255)\nd = d3dshot.create(capture_output="pytorch")\n\n# Captures will be torch.Tensor of dtype float64 with normalized values in range (0.0, 1.0)\nd = d3dshot.create(capture_output="pytorch_float")\n```\n\n**If _NumPy_ and _PyTorch_ are available + _CUDA_ is installed and _torch.cuda.is_available()_**\n\n```python\n# Captures will be torch.Tensor of dtype uint8 with values in range (0, 255) on device cuda:0\nd = d3dshot.create(capture_output="pytorch_gpu")\n\n# Captures will be torch.Tensor of dtype float64 with normalized values in range (0.0, 1.0) on device cuda:0\nd = d3dshot.create(capture_output="pytorch_float_gpu")\n```\n\nTrying to use a Capture Output for which your environment does not meet the requirements will result in an error.\n\n### Singleton\n\nWindows only allows 1 instance of Desktop Duplication per process. To make sure we fall in line with that limitation to avoid issues, the _D3DShot_ class acts as a singleton. Any subsequent calls to `d3dshot.create()` will always return the existing instance.\n\n```python\nd = d3dshot.create(capture_output="numpy")\n\n# Attempting to create a second instance\nd2 = d3dshot.create(capture_output="pil")\n# Only 1 instance of D3DShot is allowed per process! Returning the existing instance...\n\n# Capture output remains \'numpy\'\nd2.capture_output.backend\n# Out[1]: <d3dshot.capture_outputs.numpy_capture_output.NumpyCaptureOutput at 0x2672be3b8e0>\n\nd == d2\n# Out[2]: True\n```  \n\n\n### Frame Buffer\n\nWhen you create a _D3DShot_ instance, a frame buffer is also initialized. It is meant as a thread-safe, first-in, first-out way to hold a certain quantity of captures and is implemented as a `collections.deque`.\n\nBy default, the size of the frame buffer is set to 60. You can customize it when creating your _D3DShot_ object.\n\n```python\nd = d3dshot.create(frame_buffer_size=100)\n```\n\nBe mindful of RAM usage with larger values; You will be dealing with uncompressed images which use up to 100 MB each depending on the resolution.\n\nThe frame buffer can be accessed directly with `d.frame_buffer` but the usage of the utility methods instead is recommended.\n\nThe buffer is used by the following methods:\n\n* `d.capture()`\n* `d.screenshot_every()`\n\nIt is always automatically cleared before starting one of these operations.\n\n### Displays\n\nWhen you create a _D3DShot_ instance, your available displays will automatically be detected along with all their relevant properties.\n\n```python\nd.displays\n```\n```\nOut[1]: \n[<Display name=BenQ XL2730Z (DisplayPort) adapter=NVIDIA GeForce GTX 1080 Ti resolution=2560x1440 rotation=0 scale_factor=1.0 primary=True>,\n <Display name=BenQ XL2430T (HDMI) adapter=Intel(R) UHD Graphics 630 resolution=1920x1080 rotation=0 scale_factor=1.0 primary=False>]\n```\n\nBy default, your primary display will be selected. At all times you can verify which display is set to be used for capture.\n\n```python\nd.display\n```\n```\nOut[1]: <Display name=BenQ XL2730Z (DisplayPort) adapter=NVIDIA GeForce GTX 1080 Ti resolution=2560x1440 rotation=0 scale_factor=1.0 primary=True>\n```\n\nSelecting another display for capture is as simple as setting `d.display` to another value from `d.displays`\n```python\nd.display = d.displays[1]\nd.display\n```\n```\nOut[1]: <Display name=BenQ XL2430T (HDMI) adapter=Intel(R) UHD Graphics 630 resolution=1080x1920 rotation=90 scale_factor=1.0 primary=False>\n```\n\nDisplay rotation and scaling is detected and handled for you by _D3DShot_:\n\n* Captures on rotated displays will always be in the correct orientation (i.e. matching what you see on your physical displays)\n* Captures on scaled displays will always be in full, non-scaled resolution (e.g. 1280x720 at 200% scaling will yield 2560x1440 captures)\n\n### Regions\n\nAll capture methods (screenshots included) accept an optional `region` kwarg. The expected value is a 4-length tuple of integers that is to be structured like this:\n\n```\n(left, top, right, bottom)  # values represent pixels\n```\n\nFor example, if you want to only capture a 200px by 200px region offset by 100px from both the left and top, you would do:\n\n```python\nd.screenshot(region=(100, 100, 300, 300))\n```\n\nIf you are capturing a scaled display, the region will be computed against the full, non-scaled resolution. \n\nIf you go through the source code, you will notice that the region cropping happens after a full display capture. That might seem sub-optimal but testing has revealed that copying a region of the GPU _D3D11Texture2D_ to the destination CPU _D3D11Texture2D_ using _CopySubresourceRegion_ is only faster when the region is very small. In fact, it doesn\'t take long for larger regions to actually start becoming slower than the full display capture using this method. To make things worse, it adds a lot of complexity by having the surface pitch not match the buffer size and treating rotated displays differently. It was therefore decided that it made more sense to stick to _CopyResource_ in all cases and crop after the fact.\n\n## Usage\n\n**Create a D3DShot instance**\n\n```python\nimport d3dshot\n\nd = d3dshot.create()\n```\n\n`create` accepts 2 optional kwargs:\n\n* `capture_output`: Which capture output to use. See the _Capture Outputs_ section under _Concepts_\n* `frame_buffer_size`: The maximum size the frame buffer can grow to. See the _Frame Buffer_ section under _Concepts_\n\nDo NOT import the _D3DShot_ class directly and attempt to initialize it yourself! The `create` helper function initializes and validates a bunch of things for you behind the scenes.\n\nOnce you have a _D3DShot_ instance in scope, we can start doing stuff with it!\n\n**List the detected displays**\n\n```python\nd.displays\n```\n\n**Select a display for capture**\n\nYour primary display is selected by default but if you have a multi-monitor setup, you can select another entry in `d.displays` \n\n```python\nd.display = d.displays[1]\n```\n\n**Take a screenshot**\n\n```python\nd.screenshot()\n```\n\n`screenshot` accepts 1 optional kwarg:\n\n* `region`: A region tuple. See the _Regions_ section under _Concepts_\n\n_Returns_: A screenshot with a format that matches the capture output you selected when creating your _D3DShot_ object\n\n**Take a screenshot and save it to disk**\n\n```python\nd.screenshot_to_disk()\n```\n\n`screenshot_to_disk` accepts 3 optional kwargs:\n\n* `directory`: The path / directory where to write the file. If omitted, the working directory of the program will be used\n* `file_name`: The file name to use. Permitted extensions are: _.png_, _.jpg_. If omitted, the file name will be `<time.time()>.png` \n* `region`: A region tuple. See the _Regions_ section under _Concepts_\n\n_Returns_: A string representing the full path to the saved image file\n\n**Take a screenshot every X seconds**\n\n```python\nd.screenshot_every(X)  # Where X is a number representing seconds\n```\n\nThis operation is threaded and non-blocking. It will keep running until `d.stop()` is called. Captures are pushed to the frame buffer.\n\n`screenshot_every` accepts 1 optional kwarg:\n\n* `region`: A region tuple. See the _Regions_ section under _Concepts_\n\n_Returns_: A boolean indicating whether or not the capture thread was started\n\n**Take a screenshot every X seconds and save it to disk**\n\n```python\nd.screenshot_to_disk_every(X)  # Where X is a number representing seconds\n```\n\nThis operation is threaded and non-blocking. It will keep running until `d.stop()` is called.\n\n`screenshot_to_disk_every` accepts 2 optional kwargs:\n\n* `directory`: The path / directory where to write the file. If omitted, the working directory of the program will be used\n* `region`: A region tuple. See the _Regions_ section under _Concepts_\n\n_Returns_: A boolean indicating whether or not the capture thread was started\n\n**Start a high-speed screen capture**\n\n```python\nd.capture()\n```\n\nThis operation is threaded and non-blocking. It will keep running until `d.stop()` is called. Captures are pushed to the frame buffer.\n\n`capture` accepts 2 optional kwargs:\n\n* `target_fps`: How many captures per second to aim for. The effective capture rate will go under if the system can\'t keep up but it will never go over this target. It is recommended to set this to a reasonable value for your use case in order not to waste system resources. Default is set to 60.\n* `region`: A region tuple. See the _Regions_ section under _Concepts_\n\n_Returns_: A boolean indicating whether or not the capture thread was started\n\n**Grab the latest frame from the buffer**\n\n```python\nd.get_latest_frame()\n```\n\n_Returns_: A frame with a format that matches the capture output you selected when creating your _D3DShot_ object\n\n**Grab a specific frame from the buffer**\n\n```python\nd.get_frame(X)  # Where X is the index of the desired frame. Needs to be < len(d.frame_buffer)\n```\n\n_Returns_: A frame with a format that matches the capture output you selected when creating your _D3DShot_ object\n\n**Grab specific frames from the buffer**\n\n```python\nd.get_frames([X, Y, Z, ...])  # Where X, Y, Z are valid indices to desired frames\n```\n\n_Returns_: A list of frames with a format that matches the capture output you selected when creating your _D3DShot_ object\n\n**Grab specific frames from the buffer as a stack**\n\n```python\nd.get_frame_stack([X, Y, Z, ...], stack_dimension="first|last")  # Where X, Y, Z are valid indices to desired frames\n```\n\nOnly has an effect on NumPy and PyTorch capture outputs.\n\n`get_frame_stack` accepts 1 optional kwarg:\n\n* `stack_dimension`: One of _first_, _last_. Which axis / dimension to perform the stack on\n\n_Returns_: A single array stacked on the specified dimension with a format that matches the capture output you selected when creating your _D3DShot_ object. If the capture output is not stackable, returns a list of frames.\n\n**Dump the frame buffer to disk**\n\nThe files will be named according to this convention: `<frame buffer index>.png`\n\n```python\nd.frame_buffer_to_disk()\n```\n\n`frame_buffer_to_disk` accepts 1 optional kwarg:\n\n* `directory`: The path / directory where to write the files. If omitted, the working directory of the program will be used\n\n_Returns_: None\n\n## Performance\n\nMeasuring the exact performance of the Windows Desktop Duplication API proves to be a little complicated because it will only return new texture data if the contents of the screen has changed. This is optimal for performance but it makes it difficult to express in terms of frames per second, the measurement people tend to expect for benchmarks. Ultimately the solution ended up being to run a high FPS video game on the display to capture to make sure the screen contents is different at all times while benchmarking.\n\nAs always, remember that benchmarks are inherently flawed and highly depend on your individual hardware configuration and other circumstances. Use the numbers below as a relative indication of what to expect from _D3DShot_, not as some sort of absolute truth.\n\n|                         | 2560x1440 on _NVIDIA GTX 1080 Ti_ | 1920x1080 on _Intel UHD Graphics 630_ | 1080x1920 (vertical) on _Intel UHD Graphics 630_ |\n|-------------------------|-----------------------------------|---------------------------------------|--------------------------------------------------|\n| **"pil"**               | 29.717 FPS                        | 47.75 FPS                             | 35.95 FPS                                        |\n| **"numpy"**             | **57.667 FPS**                    | **58.1 FPS**                          | **58.033 FPS**                                   |\n| **"numpy_float"**       | 18.783 FPS                        | 29.05 FPS                             | 27.517 FPS                                       |\n| **"pytorch"**           | **57.867 FPS**                    | **58.1 FPS**                          | 34.817 FPS                                       |\n| **"pytorch_float"**     | 18.767 FPS                        | 28.367 FPS                            | 27.017 FPS                                       |\n| **"pytorch_gpu"**       | 27.333 FPS                        | 35.767 FPS                            | 34.8 FPS                                         |\n| **"pytorch_float_gpu"** | 27.267 FPS                        | 37.383 FPS                            | 35.033 FPS                                       |\n\nThe absolute fastest capture outputs appear to be _"numpy"_ and unrotated _"pytorch"_; all averaging around 58 FPS. In Python land, this is FAST! \n\n#### How is the "numpy" capture output performance _that_ good?\n\nNumPy arrays have a ctypes interface that can give you their raw memory address (`X.ctypes.data`). If you have the memory address and size of another byte buffer, which is what we end up with by processing what returns from the Desktop Duplication API, you can use `ctypes.memmove` to copy that byte buffer directly to the NumPy structure, effectively bypassing as much Python as possible.\n\nIn practice it ends up looking like this:\n```python\nctypes.memmove(np.empty((size,), dtype=np.uint8).ctypes.data, pointer, size)\n```\n\nThis low-level operation is extremely fast, leaving everything else that would normally compete with NumPy in the dust.\n\n#### Why is the "pytorch" capture output slower on rotated displays?\n\nDon\'t tell anyone but the reason it can compete with NumPy in the first place is only because... _it is_ generated from a NumPy array built from the method above! If you sniff around the code, you will indeed find `torch.from_numpy()` scattered around. This pretty much matches the speed of the "numpy" capture output 1:1, except when dealing with a rotated display. Display rotation is handled by `np.rot90()` calls which yields negative strides on that array. Negative strides are understood and perform well under NumPy but are still unsupported in PyTorch at the time of writing. To address this, an additional copy operation is needed to bring it back to a contiguous array which imposes a performance penalty.\n\n#### Why is the "pil" capture output, being the default, not the fastest?\n\nPIL has no ctypes interface like NumPy so a bytearray needs to be read into Python first and then fed to `PIL.Image.frombytes()`. This is still fast in Python terms, but it just cannot match the speed of the low-level NumPy method.\n\nIt remains the default capture output because:\n\n1) PIL Image objects tend to be familiar to Python users\n2) It\'s a way lighter / simpler dependency for a library compared to NumPy or PyTorch\n\n#### Why are the float versions of capture outputs slower?\n\nThe data of the Direct3D textures made accessible by the Desktop Duplication API is formatted as bytes. To represent this data as normalized floats instead, a type cast and element-wise division needs to be performed on the array holding those bytes. This imposes a major performance penalty. Interestingly, you can see this performance penalty mitigated on GPU PyTorch tensors since the element-wise division can be massively parallelized on the device.\n\n#\n\n_Crafted with ❤ by Serpent.AI 🐍_  \n[Twitter](https://twitter.com/Serpent_AI) - [Twitch](https://www.twitch.tv/serpent_ai)\n',
     'author': 'Nicholas Brochu',
     'author_email': 'nicholas@serpent.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SerpentAI/D3DShot',
```

### Comparing `dedeshot-0.0.1/PKG-INFO` & `dedeshot-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedeshot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extremely Fast and Robust Screen Capture on Windows with the Desktop Duplication API
 Home-page: https://github.com/SerpentAI/D3DShot
 License: MIT
 Keywords: Screen Capture,Screenshot,Computer Vision,Windows
 Author: Nicholas Brochu
 Author-email: nicholas@serpent.ai
 Requires-Python: >=3.6
```

