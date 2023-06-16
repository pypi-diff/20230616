# Comparing `tmp/ivt-0.1.1.tar.gz` & `tmp/ivt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivt-0.1.1.tar", last modified: Mon Jun  5 11:04:25 2023, max compression
+gzip compressed data, was "ivt-0.1.2.tar", last modified: Fri Jun 16 06:48:15 2023, max compression
```

## Comparing `ivt-0.1.1.tar` & `ivt-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1123 2023-06-05 09:53:24.916313 ivt-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2097 2022-12-26 08:46:33.368156 ivt-0.1.1/.gitignore
--rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.1/LICENSE
--rw-r--r--   0        0        0      776 2023-06-05 10:57:06.577472 ivt-0.1.1/README.md
--rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.1/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.1/docs/_templates/page.html
--rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.1/docs/conf.py
--rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.1/docs/core_install.rst
--rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.1/docs/core_intro.rst
--rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.1/docs/forward_intro.rst
--rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.1/docs/index.rst
--rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.1/docs/inverse_intro.rst
--rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.1/docs/plugin_refs.rst
--rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.1/docs/requirements.txt
--rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.1/docs/teaser.png
--rw-r--r--   0        0        0      269 2023-06-05 11:03:32.115809 ivt-0.1.1/ivt/__init__.py
--rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.1/ivt/config.py
--rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.1/ivt/connector.py
--rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.1/ivt/connectors/__init__.py
--rw-r--r--   0        0        0    14092 2023-06-05 09:53:24.918811 ivt-0.1.1/ivt/connectors/psdr_jit_connector.py
--rw-r--r--   0        0        0     3170 2023-06-05 09:53:24.919311 ivt-0.1.1/ivt/io.py
--rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.1/ivt/loss.py
--rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.1/ivt/model.py
--rw-r--r--   0        0        0     2417 2023-06-05 09:53:24.920312 ivt-0.1.1/ivt/parameter.py
--rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.1/ivt/renderer.py
--rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.1/ivt/sampling.py
--rw-r--r--   0        0        0     5729 2023-06-05 09:53:24.921811 ivt-0.1.1/ivt/scene.py
--rw-r--r--   0        0        0     3221 2023-06-05 09:53:24.922311 ivt-0.1.1/ivt/transform.py
--rw-r--r--   0        0        0      440 2023-06-05 10:20:47.334303 ivt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 ivt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-06-05 09:53:24.916313 ivt-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2097 2022-12-26 08:46:33.368156 ivt-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.2/LICENSE
+-rw-r--r--   0        0        0      776 2023-06-05 10:57:06.577472 ivt-0.1.2/README.md
+-rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.2/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.2/docs/_templates/page.html
+-rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.2/docs/core_install.rst
+-rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.2/docs/core_intro.rst
+-rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.2/docs/forward_intro.rst
+-rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.2/docs/index.rst
+-rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.2/docs/inverse_intro.rst
+-rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.2/docs/plugin_refs.rst
+-rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.2/docs/teaser.png
+-rw-r--r--   0        0        0      269 2023-06-16 06:42:43.435704 ivt-0.1.2/ivt/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.2/ivt/config.py
+-rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.2/ivt/connector.py
+-rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.2/ivt/connectors/__init__.py
+-rw-r--r--   0        0        0    14632 2023-06-11 09:51:02.554002 ivt-0.1.2/ivt/connectors/psdr_jit_connector.py
+-rw-r--r--   0        0        0     5051 2023-06-09 21:50:08.990124 ivt-0.1.2/ivt/io.py
+-rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.2/ivt/loss.py
+-rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.2/ivt/model.py
+-rw-r--r--   0        0        0     1908 2023-06-07 05:21:51.299496 ivt-0.1.2/ivt/parameter.py
+-rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.2/ivt/renderer.py
+-rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.2/ivt/sampling.py
+-rw-r--r--   0        0        0     6132 2023-06-11 09:21:37.011237 ivt-0.1.2/ivt/scene.py
+-rw-r--r--   0        0        0     3042 2023-06-07 05:24:56.148994 ivt-0.1.2/ivt/transform.py
+-rw-r--r--   0        0        0      499 2023-06-16 06:40:23.588718 ivt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 ivt-0.1.2/PKG-INFO
```

### Comparing `ivt-0.1.1/.github/workflows/python-publish.yml` & `ivt-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/.gitignore` & `ivt-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/LICENSE` & `ivt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/README.md` & `ivt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/docs/_static/theme_overrides.css` & `ivt-0.1.2/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/docs/conf.py` & `ivt-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/docs/index.rst` & `ivt-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/docs/teaser.png` & `ivt-0.1.2/docs/teaser.png`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/ivt/connector.py` & `ivt-0.1.2/ivt/connector.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/ivt/connectors/psdr_jit_connector.py` & `ivt-0.1.2/ivt/connectors/psdr_jit_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 from ..connector import Connector
 from ..scene import *
 from ..config import *
-from ..io import write_mesh
+from ..io import write_obj
 from collections import OrderedDict
 
 import drjit
 import psdr_jit
 from drjit.scalar import Array3f
 from drjit.cuda import Array3f as Vector3fC, Array3i as Vector3iC
 from drjit.cuda.ad import Array3f as Vector3fD, Float32 as FloatD, Matrix4f as Matrix4fD, Matrix3f as Matrix3fD
 from drjit.cuda.ad import Float32 as FloatD
 import torch
 
+import time
+
+class Timer:
+    def __init__(self, label):
+        self.label = label
+
+    def __enter__(self):
+        self.start_time = time.time()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        elapsed_time = time.time() - self.start_time
+        print(f"[{self.label}] Elapsed time: {elapsed_time} seconds")
+
 class PSDRJITConnector(Connector, connector_name='psdr_jit'):
 
     backend = 'torch'
     device = 'cuda'
     ftype = torch.float32
     itype = torch.long
 
@@ -33,21 +46,24 @@
             cache['scene'].opts.spp = render_options['spp']
             cache['scene'].opts.sppe = render_options['sppe']
             cache['scene'].opts.sppse = render_options['sppse']
             cache['scene'].opts.log_level = render_options['log_level']
 
             cache['name_map'] = {}
             cache['integrators'] = OrderedDict()
+            cache['configured'] = False
 
         drjit_params = []
         for name in scene.components:
             component = scene[name]
             drjit_params += self.extensions[type(component)](name, scene)
 
-        cache['scene'].configure()    
+        if not cache['configured']:
+            cache['scene'].configure() 
+            cache['configured'] = True
         
         return scene.cached['psdr_jit'], drjit_params
 
     def renderC(self, scene, render_options, sensor_ids=[0], integrator_id=0):
         cache, _ = self.update_scene_objects(scene, render_options)
 
         cache['scene'].configure(sensor_ids)
@@ -141,28 +157,26 @@
     sensor = scene[name]
     cache = scene.cached['psdr_jit']
     psdr_scene = cache['scene']
 
     # Create the object if it has not been created
     if name not in cache['name_map']:
         psdr_sensor = psdr_jit.PerspectiveCamera(sensor['fov'], sensor['near'], sensor['far'])
-        # psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
-        psdr_sensor.to_world = Matrix4fD(sensor['to_world'].cpu().numpy())
+        psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
         psdr_scene.add_Sensor(psdr_sensor)
         cache['name_map'][name] = f"Sensor[{psdr_scene.num_sensors - 1}]"
 
     psdr_sensor = psdr_scene.param_map[cache['name_map'][name]]
     
     # Update parameters
     updated = sensor.get_updated()
     if len(updated) > 0:
         for param_name in updated:
             if param_name == "to_world":
-                # psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
-                psdr_sensor.to_world = Matrix4fD(sensor['to_world'].cpu().numpy())
+                psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
             sensor.params[param_name]['updated'] = False
 
     # Enable grad for parameters requiring grad
     drjit_params = []
     requiring_grad = sensor.get_requiring_grad()
     if len(requiring_grad) > 0:
         for param_name in requiring_grad:
@@ -185,17 +199,17 @@
         mat_id = mesh['mat_id']
         if mat_id not in scene:
             raise RuntimeError(f"The material of the mesh {name} doesn't exist: mat_id={mat_id}")
         brdf = scene[mat_id]
         PSDRJITConnector.extensions[type(brdf)](mat_id, scene)
 
         # TODO: Fix this workaround when psdr-jit updates psdr_mesh.load_raw()
-        write_mesh('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'])
-        psdr_emitter = psdr_jit.AreaLight(mesh['radiance'].cpu().numpy()) if mesh['is_emitter'] else None
-        psdr_scene.add_Mesh('__psdr_jit_tmp__.obj', mesh['to_world'].cpu().numpy(), mat_id, psdr_emitter)
+        write_obj('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'], mesh['fuv'])
+        psdr_emitter = psdr_jit.AreaLight(mesh['radiance']) if mesh['is_emitter'] else None
+        psdr_scene.add_Mesh('__psdr_jit_tmp__.obj', mesh['to_world'].reshape(1, 4, 4), mat_id, psdr_emitter)
 
         # psdr_mesh = psdr_jit.Mesh()
         # psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
         # psdr_mesh.use_face_normal = mesh['use_face_normal']
 
         # psdr_emitter = psdr_jit.AreaLight(mesh['radiance'].tolist()) if mesh['is_emitter'] else None
         # psdr_scene.add_Mesh(psdr_mesh, mat_id, psdr_emitter)
@@ -228,15 +242,14 @@
     return drjit_params
 
 def convert_color(color, c, bitmap=True):
     if color.shape == ():
         color = color.tile(c)
     if color.shape == (c,):
         color = color.reshape(1, 1, c)
-    color = color.cpu().numpy()
     h, w, _ = color.shape
     if c == 3:
         color = Vector3fD(color.reshape(-1, c))
         if bitmap:
             color = psdr_jit.Bitmap3fD(w, h, color)
     elif c == 1:
         color = FloatD(color.reshape(-1))
@@ -338,25 +351,29 @@
     
     # Create the object if it has not been created
     if name not in cache['name_map']:
         radiance = convert_color(emitter['radiance'], 3)
 
         psdr_emitter = psdr_jit.EnvironmentMap()
         psdr_emitter.radiance = radiance
+        psdr_emitter.set_transform(Matrix4fD(emitter['to_world'].reshape(1, 4, 4)))
         psdr_scene.add_EnvironmentMap(psdr_emitter)
         cache['name_map'][name] = f"Emitter[{psdr_scene.get_num_emitters() - 1}]"
 
     psdr_emitter = psdr_scene.param_map[cache['name_map'][name]]
 
     # Update parameters
     updated = emitter.get_updated()
     if len(updated) > 0:
         for param_name in updated:
             if param_name == 'radiance':
                 psdr_emitter.radiance = convert_color(emitter['radiance'], 3)
+            elif param_name == 'to_world':
+                psdr_emitter.set_transform(Matrix4fD(emitter['to_world'].reshape(1, 4, 4)))
+            emitter.params[param_name]['updated'] = False
 
     # Enable grad for parameters requiring grad
     drjit_params = []
     
     def enable_grad(drjit_param):
         drjit.enable_grad(drjit_param)
         drjit_params.append(drjit_param)
```

### Comparing `ivt-0.1.1/ivt/loss.py` & `ivt-0.1.2/ivt/loss.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/ivt/model.py` & `ivt-0.1.2/ivt/model.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/ivt/parameter.py` & `ivt-0.1.2/ivt/parameter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,36 @@
+from .io import to_torch
 import torch
 from collections import OrderedDict
-from .config import *
 
 class ParamGroup:
 
     def __init__(self):
         self.params = OrderedDict()
 
-        self.ftype = ftype
-        self.itype = itype
-        self.device = device
-
     def __getitem__(self, param_name):
         return self.params[param_name]['value']
     
     def __setitem__(self, param_name, param_value):
         if self.params[param_name]['is_tensor'] and not torch.is_tensor(param_value):
             dtype = self[param_name].dtype
             requires_grad = self[param_name].requires_grad
-            param_value = self.to_tensor(param_value, dtype).requires_grad_(requires_grad)
+            param_value = to_torch(param_value, dtype).requires_grad_(requires_grad)
         self.params[param_name]['value'] = param_value
         self.mark_updated(param_name)
 
     def add_param(self, name, value, is_tensor=False, is_diff=False, help_msg=""):
         self.params[name] = {
             'value': value,
             'is_tensor': is_tensor,
             'is_diff': is_diff,
             'help_msg': help_msg,
             'updated': False
         }
 
-    def to_tensor(self, array, dtype):
-        if torch.is_tensor(array):
-            array = array.to(dtype).to(self.device)
-        else:
-            array = torch.tensor(array, dtype=dtype, device=self.device)
-        return array
-    
-    def to_ftensor(self, array):
-        return self.to_tensor(array, self.ftype)
-
-    def to_itensor(self, array):
-        return self.to_tensor(array, self.itype)
-
     def get_requiring_grad(self):
         return [name for name in self.params if self.params[name]['is_diff'] and self[name].requires_grad]
     
     def get_updated(self):
         return [name for name in self.params if self.params[name]['updated']]
     
     def mark_updated(self, param_name):
```

### Comparing `ivt-0.1.1/ivt/renderer.py` & `ivt-0.1.2/ivt/renderer.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/ivt/sampling.py` & `ivt-0.1.2/ivt/sampling.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.1/ivt/scene.py` & `ivt-0.1.2/ivt/scene.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .parameter import ParamGroup
 from .transform import lookat
-from .io import read_image, read_mesh
+from .io import read_image, read_obj, to_torch_f, to_torch_i
 
 from collections import OrderedDict
 
 import torch
 
 class Scene:
 
@@ -33,28 +33,31 @@
             item = item[c]
         return True
 
     def configure(self):
         requiring_grad = []
         for cname in self.components:
             requiring_grad += [f'{cname}.{pname}' for pname in self.components[cname].get_requiring_grad()]
-        self.requiring_grad = set(requiring_grad)
+        self.requiring_grad = tuple(requiring_grad)
 
     def __str__(self):
         lines = []
 
         for name in self.components:
             lines.append(f"{name}:")
             lines.append(str(self.components[name]))
             lines.append("\n")
 
         return '\n'.join(lines)
     
     def clear_cache(self):
         self.cached = {}
+        # Detach the tensors requiring grad
+        for param_name in self.requiring_grad:
+            self[param_name] = self[param_name].detach()
 
 class Integrator(ParamGroup):
 
     def __init__(self, type, config):
         super().__init__()
         
         self.add_param('type', type, help_msg='integrator type')
@@ -72,81 +75,83 @@
     
     def __init__(self, fov, to_world, near=1e-6, far=1e7):
         super().__init__()
 
         self.add_param('fov', fov, help_msg='sensor fov')
         self.add_param('near', near, help_msg='sensor near clip')
         self.add_param('far', far, help_msg='sensor far clip')
-        self.add_param('to_world', self.to_ftensor(to_world), is_tensor=True, is_diff=True, help_msg='sensor to_world matrix')
+        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, is_diff=True, help_msg='sensor to_world matrix')
 
     @classmethod
     def from_lookat(cls, fov, origin, target, up, near=1e-6, far=1e7):
         sensor = cls(fov, torch.eye(4), near, far)
-        origin = sensor.to_ftensor(origin)
-        target = sensor.to_ftensor(target)
-        up = sensor.to_ftensor(up)
+        origin = to_torch_f(origin)
+        target = to_torch_f(target)
+        up = to_torch_f(up)
         sensor['to_world'] = lookat(origin, target, up)
         return sensor
         
 class Mesh(ParamGroup):
 
-    def __init__(self, v, f, uv, mat_id, to_world=torch.eye(4), use_face_normal=True, radiance=torch.zeros(3)):
+    def __init__(self, v, f, uv, fuv, mat_id, to_world=torch.eye(4), use_face_normal=True, radiance=torch.zeros(3)):
         super().__init__()
         
-        self.add_param('v', self.to_ftensor(v), is_tensor=True, is_diff=True, help_msg='mesh vertex positions')
-        self.add_param('f', self.to_itensor(f), is_tensor=True, help_msg='mesh face indices')
-        self.add_param('uv', self.to_ftensor(uv), is_tensor=True, help_msg='mesh uv coordinates')
+        self.add_param('v', to_torch_f(v), is_tensor=True, is_diff=True, help_msg='mesh vertex positions')
+        self.add_param('f', to_torch_i(f), is_tensor=True, help_msg='mesh face indices')
+        self.add_param('uv', to_torch_f(uv), is_tensor=True, help_msg='mesh uv coordinates')
+        self.add_param('fuv', to_torch_i(fuv), is_tensor=True, help_msg='mesh uv face indices')
         self.add_param('mat_id', mat_id, help_msg='name of the material of the mesh')
-        self.add_param('to_world', self.to_ftensor(to_world), is_tensor=True, help_msg='mesh to world matrix')
+        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, help_msg='mesh to world matrix')
         self.add_param('use_face_normal', use_face_normal, help_msg='whether to use face normal')
 
-        radiance = self.to_itensor(radiance)
+        radiance = to_torch_f(radiance)
         is_emitter = radiance.sum() > 0
         self.add_param('is_emitter', is_emitter, help_msg='whether it is used as an emitter')
         self.add_param('radiance', radiance, is_tensor=True, is_diff=True, help_msg='radiance if it is used as an emitter')
 
     @classmethod
     def from_file(cls, filename, mat_id, to_world=torch.eye(4), use_face_normal=True, radiance=torch.zeros(3)):
-        v, f, uv = read_mesh(filename)
-        return cls(v, f, uv, mat_id, to_world, use_face_normal, radiance)
+        v, tc, n, f, ftc, fn = read_obj(filename)
+        return cls(v, f, tc, ftc, mat_id, to_world, use_face_normal, radiance)
     
 class DiffuseBRDF(ParamGroup):
 
     def __init__(self, d):
         super().__init__()
         
-        self.add_param('d', self.to_ftensor(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
+        self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
 
     @classmethod
     def from_file(cls, filename, is_srgb=None):
         texture = read_image(filename, is_srgb)
         return cls(texture)
     
 class MicrofacetBRDF(ParamGroup):
 
     def __init__(self, d, s, r):
         super().__init__()
         
-        self.add_param('d', self.to_ftensor(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
-        self.add_param('s', self.to_ftensor(s), is_tensor=True, is_diff=True, help_msg='specular reflectance')
-        self.add_param('r', self.to_ftensor(r), is_tensor=True, is_diff=True, help_msg='roughness')
+        self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
+        self.add_param('s', to_torch_f(s), is_tensor=True, is_diff=True, help_msg='specular reflectance')
+        self.add_param('r', to_torch_f(r), is_tensor=True, is_diff=True, help_msg='roughness')
 
     @classmethod
     def from_file(cls, d_filename, s_filename, r_filename, d_is_srgb=None, s_is_srgb=None, r_is_srgb=None):
         d_texture = read_image(d_filename, d_is_srgb)
         s_texture = read_image(s_filename, s_is_srgb)
         r_texture = read_image(r_filename, r_is_srgb)[..., 0:1]
 
         return cls(d_texture, s_texture, r_texture)
     
 class EnvironmentLight(ParamGroup):
 
-    def __init__(self, radiance):
+    def __init__(self, radiance, to_world=torch.eye(4)):
         super().__init__()
         
-        self.add_param('radiance', self.to_ftensor(radiance), is_tensor=True, is_diff=True, help_msg='environment light radiance')
+        self.add_param('radiance', to_torch_f(radiance), is_tensor=True, is_diff=True, help_msg='environment light radiance')
+        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, is_diff=False, help_msg='environment to_world matrix')
 
     @classmethod
-    def from_file(cls, radiance_filename, radiance_is_srgb=None):
+    def from_file(cls, radiance_filename, radiance_is_srgb=None, to_world=torch.eye(4)):
         radiance_texture = read_image(radiance_filename, radiance_is_srgb)
 
-        return cls(radiance_texture)
+        return cls(radiance_texture, to_world)
```

### Comparing `ivt-0.1.1/ivt/transform.py` & `ivt-0.1.2/ivt/transform.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,132 +1,126 @@
+from .io import to_torch_f
 import torch 
 import torch.nn.functional as F
-from .config import ftype, device
-
-def to_ftensor(data):
-    if torch.is_tensor(data):
-        return data.to(ftype).to(device)
-    else:
-        return torch.tensor(data, dtype=ftype, device=device)
 
 def lookat(origin, target, up):
-    origin = to_ftensor(origin)
-    target = to_ftensor(target)
-    up = to_ftensor(up)
+    origin = to_torch_f(origin)
+    target = to_torch_f(target)
+    up = to_torch_f(up)
 
     dir = F.normalize(target - origin, dim=0)
     left = F.normalize(torch.cross(up, dir), dim=0)
     new_up = F.normalize(torch.cross(dir, left), dim=0)
 
-    to_world = to_ftensor(torch.eye(4))
+    to_world = to_torch_f(torch.eye(4))
     to_world[:3, 0] = left
     to_world[:3, 1] = new_up
     to_world[:3, 2] = dir
     to_world[:3, 3] = origin
 
     return to_world
 
 def perspective(fov, near=1e-6, far=1e7):
     recip = 1 / (far - near)
-    tan = torch.tan(torch.deg2rad(to_ftensor(fov * 0.5)))
+    tan = torch.tan(torch.deg2rad(to_torch_f(fov * 0.5)))
     cot = 1 / tan
 
-    mat = torch.diag(to_ftensor([cot, cot, far * recip, 0]))
+    mat = torch.diag(to_torch_f([cot, cot, far * recip, 0]))
     mat[2, 3] = -near * far * recip
     mat[3, 2] = 1
 
     return mat
 
 def translate(t_vec):
-    t_vec = to_ftensor(t_vec)
+    t_vec = to_torch_f(t_vec)
 
-    to_world = to_ftensor(torch.eye(4))
+    to_world = to_torch_f(torch.eye(4))
     to_world[:3, 3] = t_vec
 
     return to_world
 
 def rotate(axis, angle, use_degree=True):
-    axis = to_ftensor(axis)
-    angle = to_ftensor(angle)
+    axis = to_torch_f(axis)
+    angle = to_torch_f(angle)
 
-    to_world = to_ftensor(torch.eye(4))
+    to_world = to_torch_f(torch.eye(4))
     axis = F.normalize(axis, dim=0).reshape(3, 1)
 
     if use_degree:
         angle = torch.deg2rad(angle)
 
     sin_theta = torch.sin(angle)
     cos_theta = torch.cos(angle)
 
-    cpm = to_ftensor(torch.zeros((3, 3)))
+    cpm = to_torch_f(torch.zeros((3, 3)))
     cpm[0, 1] = -axis[2]
     cpm[0, 2] =  axis[1]
     cpm[1, 0] =  axis[2]
     cpm[1, 2] = -axis[0]
     cpm[2, 0] = -axis[1]
     cpm[2, 1] =  axis[0]
 
-    R = cos_theta * to_ftensor(torch.eye(3))
+    R = cos_theta * to_torch_f(torch.eye(3))
     R += sin_theta * cpm
     R += (1 - cos_theta) * (axis @ axis.T)
 
     to_world[:3, :3] = R
 
     return to_world
 
 def scale(size):
-    size = to_ftensor(size)
+    size = to_torch_f(size)
 
-    to_world = to_ftensor(torch.eye(4))
+    to_world = to_torch_f(torch.eye(4))
 
     if size.size() == () or size.size(dim=0) == 1:
-        to_world[:3, :3] = to_ftensor(torch.eye(3)) * size
+        to_world[:3, :3] = to_torch_f(torch.eye(3)) * size
     elif size.size(dim=0) == 3:
         to_world[:3, :3] = torch.diag(size)
     else:
         print(f"unrecognized shape for size: {size.shape}")
         exit()
 
     return to_world
 
 # texture map transform (2d)
 def translate2D(t_vec):
-    t_vec = to_ftensor(t_vec)
+    t_vec = to_torch_f(t_vec)
 
-    to_world = to_ftensor(torch.eye(3))
+    to_world = to_torch_f(torch.eye(3))
     to_world[:2, 2] = t_vec
 
     return to_world
 
 def rotate2D(angle, use_degree=True):
-    angle = to_ftensor(angle)
+    angle = to_torch_f(angle)
 
-    to_world = to_ftensor(torch.eye(3))
+    to_world = to_torch_f(torch.eye(3))
 
     if use_degree:
         angle = torch.deg2rad(angle)
 
     sin_theta = torch.sin(angle)
     cos_theta = torch.cos(angle)
 
-    R = cos_theta * to_ftensor(torch.eye(2))
+    R = cos_theta * to_torch_f(torch.eye(2))
 
     R[0 ,1] = -sin_theta
     R[1 ,0] = sin_theta
 
     to_world[:2, :2] = R
 
     return to_world
 
 def scale2D(size):
-    size = to_ftensor(size)
-    to_world = to_ftensor(torch.eye(3))
+    size = to_torch_f(size)
+    to_world = to_torch_f(torch.eye(3))
 
     if size.size(dim=0) == 1:
-        to_world[:2, :2] = torch.diag(size) * to_ftensor(torch.eye(2))
+        to_world[:2, :2] = torch.diag(size) * to_torch_f(torch.eye(2))
     elif size.size(dim=0) == 2:
         to_world[:2, :2] = torch.diag(size)
     else:
         print(f"unrecognized shape for size: {size.shape}")
         exit()
 
     return to_world
```

### Comparing `ivt-0.1.1/PKG-INFO` & `ivt-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ivt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Inverse-Rendering Toolkit
 Author-email: Guangyan Cai <gcai3@uci.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: imageio >= 2.27.0
 Requires-Dist: numpy
 Requires-Dist: gin-config
 Requires-Dist: trimesh
+Requires-Dist: libigl
 Project-URL: Home, https://github.com/uci-rendering/inv-render-toolkit
 
 # ivt
 `ivt` stands for Inverse-Rendering Toolkit. It is a simple framework for conducting inverse rendering experiments. Since there are a lot differentiable renderers in development, mastering them all and migrating between them can be a headache. `ivt` provides a simple scene representation based on `pytorch` that can be rendered by **connectors** that connect to different differentiable renderers and get the graident of the scene parameters. Migrating between renderers is just a matter of changing the connector. 
 
 ## Installation
 `ivt` depends on `pytorch`. Since it is widely used and some projects might have specific requirements to it, we leave its installation to the user.
```

