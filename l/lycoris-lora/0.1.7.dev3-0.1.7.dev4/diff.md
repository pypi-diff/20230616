# Comparing `tmp/lycoris_lora-0.1.7.dev3.tar.gz` & `tmp/lycoris_lora-0.1.7.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.7.dev3.tar", last modified: Fri Jun 16 12:08:57 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.7.dev4.tar", last modified: Fri Jun 16 13:19:06 2023, max compression
```

## Comparing `lycoris_lora-0.1.7.dev3.tar` & `lycoris_lora-0.1.7.dev4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.105215 lycoris_lora-0.1.7.dev3/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev3/Algo.md
--rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev3/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev3/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-06-16 12:08:57.105215 lycoris_lora-0.1.7.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.097702 lycoris_lora-0.1.7.dev3/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev3/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev3/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev3/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev3/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev3/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev3/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev3/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.101208 lycoris_lora-0.1.7.dev3/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/lycoris/__init__.py
--rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev3/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev3/lycoris/ia3.py
--rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev3/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev3/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev3/lycoris/locon.py
--rw-rw-rw-   0        0        0     8481 2023-06-16 12:08:46.000000 lycoris_lora-0.1.7.dev3/lycoris/loha.py
--rw-rw-rw-   0        0        0    10053 2023-06-16 11:30:00.000000 lycoris_lora-0.1.7.dev3/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev3/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.103715 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-06-16 12:08:57.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 12:08:57.105215 lycoris_lora-0.1.7.dev3/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-16 12:08:55.000000 lycoris_lora-0.1.7.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.104715 lycoris_lora-0.1.7.dev3/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev3/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev3/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.955444 lycoris_lora-0.1.7.dev4/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev4/Algo.md
+-rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev4/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev4/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-06-16 13:19:06.954441 lycoris_lora-0.1.7.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.948416 lycoris_lora-0.1.7.dev4/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev4/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev4/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev4/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev4/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev4/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev4/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev4/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.951941 lycoris_lora-0.1.7.dev4/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev4/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev4/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev4/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev4/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev4/lycoris/locon.py
+-rw-rw-rw-   0        0        0     8557 2023-06-16 13:17:19.000000 lycoris_lora-0.1.7.dev4/lycoris/loha.py
+-rw-rw-rw-   0        0        0    10339 2023-06-16 13:18:39.000000 lycoris_lora-0.1.7.dev4/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev4/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.953942 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 13:19:06.955444 lycoris_lora-0.1.7.dev4/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-16 13:19:05.000000 lycoris_lora-0.1.7.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.954441 lycoris_lora-0.1.7.dev4/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev4/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev4/tools/merge.py
```

### Comparing `lycoris_lora-0.1.7.dev3/.gitignore` & `lycoris_lora-0.1.7.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/Algo.md` & `lycoris_lora-0.1.7.dev4/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/Change.md` & `lycoris_lora-0.1.7.dev4/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/Demo.md` & `lycoris_lora-0.1.7.dev4/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/LICENSE.md` & `lycoris_lora-0.1.7.dev4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/README.md` & `lycoris_lora-0.1.7.dev4/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/better_conv.py` & `lycoris_lora-0.1.7.dev4/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/better_conv_extract.py` & `lycoris_lora-0.1.7.dev4/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/concept_neuron.py` & `lycoris_lora-0.1.7.dev4/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/locon_extract_test.py` & `lycoris_lora-0.1.7.dev4/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/locon_merge_test.py` & `lycoris_lora-0.1.7.dev4/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/singular_value_test.py` & `lycoris_lora-0.1.7.dev4/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.7.dev4/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/experiments/time_test.py` & `lycoris_lora-0.1.7.dev4/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/dylora.py` & `lycoris_lora-0.1.7.dev4/lycoris/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/ia3.py` & `lycoris_lora-0.1.7.dev4/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/kohya.py` & `lycoris_lora-0.1.7.dev4/lycoris/kohya.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.7.dev4/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/kohya_utils.py` & `lycoris_lora-0.1.7.dev4/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/locon.py` & `lycoris_lora-0.1.7.dev4/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/loha.py` & `lycoris_lora-0.1.7.dev4/lycoris/loha.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,29 +166,31 @@
         self.multiplier = multiplier
         self.org_module = [org_module] # remove in applying
         self.grad_ckpt = False
 
     def apply_to(self):
         self.org_module[0].forward = self.forward
 
-    def get_weight(self, orig_weight=0):
+    def get_weight(self, orig_weight=None):
         if self.cp:
             weight = make_weight_cp(
-                orig_weight, 
+                0, 
                 self.hada_t1, self.hada_w1_a, self.hada_w1_b,
                 self.hada_t1, self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
         else:
             weight = make_weight(
-                orig_weight, 
+                0, 
                 self.hada_w1_a, self.hada_w1_b,
                 self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
+        if orig_weight is not None:
+            weight = weight.reshape(orig_weight.shape)
         return weight
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.get_weight().norm()
         norm = torch.clamp(orig_norm, max_norm/2)
         desired = torch.clamp(norm, max=max_norm)
```

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/lokr.py` & `lycoris_lora-0.1.7.dev4/lycoris/lokr.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,19 @@
     return rebuild2
 
 
 def make_kron(orig_weight, w1, w2, scale):
     if len(w2.shape) == 4:
         w1 = w1.unsqueeze(2).unsqueeze(2)
     w2 = w2.contiguous()
-    return orig_weight + torch.kron(w1, w2).reshape(orig_weight.shape)*scale
+    rebuild = torch.kron(w1, w2)
+    
+    if isinstance(orig_weight, torch.Tensor):
+        rebuild = rebuild.reshape(orig_weight.shape)
+    return orig_weight + rebuild*scale
 
 
 class LokrModule(nn.Module):
     """
     modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
         and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
         and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
@@ -198,23 +202,25 @@
         assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
 
     # Same as locon.py
     def apply_to(self):
         self.org_forward = self.org_module[0].forward
         self.org_module[0].forward = self.forward
     
-    def get_weight(self):
+    def get_weight(self, orig_weight = None):
         weight = make_kron(
             0, 
             self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
             (self.lokr_w2 if self.use_w2 
              else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
              else self.lokr_w2_a@self.lokr_w2_b),
             torch.tensor(self.scale)
         )
+        if orig_weight is not None:
+            weight = weight.reshape(orig_weight.shape)
         return weight
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.get_weight().norm()
         norm = torch.clamp(orig_norm, max_norm/2)
         desired = torch.clamp(norm, max=max_norm)
@@ -236,15 +242,18 @@
                 self.lokr_w2_b  *= ratio**(1/modules)
             else:
                 self.lokr_w2 *= ratio**(1/modules)
         
         return scaled, orig_norm*ratio
 
     def forward(self, x):
-        weight = self.org_module[0].weight.data + self.get_weight() * self.multiplier
+        weight = (
+            self.org_module[0].weight.data 
+            + self.get_weight(self.org_module[0].weight.data) * self.multiplier
+        )
         bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
         return self.op(
             x, 
             weight.view(self.shape),
             bias,
             **self.extra_args
         )
```

### Comparing `lycoris_lora-0.1.7.dev3/lycoris/utils.py` & `lycoris_lora-0.1.7.dev4/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/setup.py` & `lycoris_lora-0.1.7.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.7.dev3',
+    version='0.1.7.dev4',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.7.dev3/tools/extract_locon.py` & `lycoris_lora-0.1.7.dev4/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev3/tools/merge.py` & `lycoris_lora-0.1.7.dev4/tools/merge.py`

 * *Files identical despite different names*

