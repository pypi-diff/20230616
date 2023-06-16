# Comparing `tmp/lycoris_lora-0.1.7.dev2.tar.gz` & `tmp/lycoris_lora-0.1.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.7.dev2.tar", last modified: Fri Jun 16 11:30:37 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.7.dev3.tar", last modified: Fri Jun 16 12:08:57 2023, max compression
```

## Comparing `lycoris_lora-0.1.7.dev2.tar` & `lycoris_lora-0.1.7.dev3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:37.854219 lycoris_lora-0.1.7.dev2/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev2/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev2/Algo.md
--rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev2/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev2/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev2/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-06-16 11:30:37.854219 lycoris_lora-0.1.7.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:37.847704 lycoris_lora-0.1.7.dev2/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev2/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev2/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev2/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev2/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev2/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev2/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev2/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev2/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:37.851217 lycoris_lora-0.1.7.dev2/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev2/lycoris/__init__.py
--rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev2/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev2/lycoris/ia3.py
--rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev2/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev2/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev2/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev2/lycoris/locon.py
--rw-rw-rw-   0        0        0     8376 2023-06-16 11:29:33.000000 lycoris_lora-0.1.7.dev2/lycoris/loha.py
--rw-rw-rw-   0        0        0    10053 2023-06-16 11:30:00.000000 lycoris_lora-0.1.7.dev2/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev2/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:37.853217 lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-16 11:30:37.000000 lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-06-16 11:30:37.000000 lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:30:37.000000 lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-16 11:30:37.000000 lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 11:30:37.000000 lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 11:30:37.854722 lycoris_lora-0.1.7.dev2/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-16 11:30:36.000000 lycoris_lora-0.1.7.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:30:37.853217 lycoris_lora-0.1.7.dev2/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev2/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev2/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.105215 lycoris_lora-0.1.7.dev3/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev3/Algo.md
+-rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev3/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev3/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-06-16 12:08:57.105215 lycoris_lora-0.1.7.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.097702 lycoris_lora-0.1.7.dev3/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev3/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev3/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev3/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev3/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev3/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev3/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev3/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.101208 lycoris_lora-0.1.7.dev3/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev3/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev3/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev3/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev3/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev3/lycoris/locon.py
+-rw-rw-rw-   0        0        0     8481 2023-06-16 12:08:46.000000 lycoris_lora-0.1.7.dev3/lycoris/loha.py
+-rw-rw-rw-   0        0        0    10053 2023-06-16 11:30:00.000000 lycoris_lora-0.1.7.dev3/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev3/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.103715 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-06-16 12:08:57.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 12:08:56.000000 lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 12:08:57.105215 lycoris_lora-0.1.7.dev3/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-16 12:08:55.000000 lycoris_lora-0.1.7.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:08:57.104715 lycoris_lora-0.1.7.dev3/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev3/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev3/tools/merge.py
```

### Comparing `lycoris_lora-0.1.7.dev2/.gitignore` & `lycoris_lora-0.1.7.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/Algo.md` & `lycoris_lora-0.1.7.dev3/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/Change.md` & `lycoris_lora-0.1.7.dev3/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/Demo.md` & `lycoris_lora-0.1.7.dev3/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/LICENSE.md` & `lycoris_lora-0.1.7.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/README.md` & `lycoris_lora-0.1.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/better_conv.py` & `lycoris_lora-0.1.7.dev3/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/better_conv_extract.py` & `lycoris_lora-0.1.7.dev3/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/concept_neuron.py` & `lycoris_lora-0.1.7.dev3/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/locon_extract_test.py` & `lycoris_lora-0.1.7.dev3/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/locon_merge_test.py` & `lycoris_lora-0.1.7.dev3/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/singular_value_test.py` & `lycoris_lora-0.1.7.dev3/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.7.dev3/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/experiments/time_test.py` & `lycoris_lora-0.1.7.dev3/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/dylora.py` & `lycoris_lora-0.1.7.dev3/lycoris/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/ia3.py` & `lycoris_lora-0.1.7.dev3/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/kohya.py` & `lycoris_lora-0.1.7.dev3/lycoris/kohya.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.7.dev3/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/kohya_utils.py` & `lycoris_lora-0.1.7.dev3/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/locon.py` & `lycoris_lora-0.1.7.dev3/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/loha.py` & `lycoris_lora-0.1.7.dev3/lycoris/loha.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,25 +166,25 @@
         self.multiplier = multiplier
         self.org_module = [org_module] # remove in applying
         self.grad_ckpt = False
 
     def apply_to(self):
         self.org_module[0].forward = self.forward
 
-    def get_weight(self):
+    def get_weight(self, orig_weight=0):
         if self.cp:
             weight = make_weight_cp(
-                0, 
+                orig_weight, 
                 self.hada_t1, self.hada_w1_a, self.hada_w1_b,
                 self.hada_t1, self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
         else:
             weight = make_weight(
-                0, 
+                orig_weight, 
                 self.hada_w1_a, self.hada_w1_b,
                 self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
         return weight
 
     @torch.no_grad()
@@ -207,15 +207,18 @@
                 self.hada_t2 *= ratio**(1/modules)
         
         return scaled, orig_norm*ratio
 
     @torch.enable_grad()
     def forward(self, x):
         # print(torch.mean(torch.abs(self.orig_w1a.to(x.device) - self.hada_w1_a)), end='\r')
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

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/lokr.py` & `lycoris_lora-0.1.7.dev3/lycoris/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris/utils.py` & `lycoris_lora-0.1.7.dev3/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.7.dev3/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/setup.py` & `lycoris_lora-0.1.7.dev3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.7.dev2',
+    version='0.1.7.dev3',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.7.dev2/tools/extract_locon.py` & `lycoris_lora-0.1.7.dev3/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev2/tools/merge.py` & `lycoris_lora-0.1.7.dev3/tools/merge.py`

 * *Files identical despite different names*

