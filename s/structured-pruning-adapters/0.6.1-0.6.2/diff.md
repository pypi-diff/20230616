# Comparing `tmp/structured-pruning-adapters-0.6.1.tar.gz` & `tmp/structured-pruning-adapters-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structured-pruning-adapters-0.6.1.tar", last modified: Thu Jun 15 12:49:21 2023, max compression
+gzip compressed data, was "structured-pruning-adapters-0.6.2.tar", last modified: Fri Jun 16 08:57:21 2023, max compression
```

## Comparing `structured-pruning-adapters-0.6.1.tar` & `structured-pruning-adapters-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.202952 structured-pruning-adapters-0.6.1/sp_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/splopa.py
--rw-r--r--   0 runner    (1001) docker     (123)    31876 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/splora.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/torch_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/sp_adapters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 12:49:21.000000 structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:49:21.206952 structured-pruning-adapters-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_lin_as_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_splopa.py
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_splora.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_torchpruning.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 12:47:20.000000 structured-pruning-adapters-0.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.414612 structured-pruning-adapters-0.6.2/sp_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30918 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/torch_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/sp_adapters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.414612 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 08:57:21.000000 structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:57:21.418612 structured-pruning-adapters-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_lin_as_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_torchpruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-16 08:55:19.000000 structured-pruning-adapters-0.6.2/tests/test_utils.py
```

### Comparing `structured-pruning-adapters-0.6.1/LICENSE` & `structured-pruning-adapters-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/PKG-INFO` & `structured-pruning-adapters-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.6.1
+Version: 0.6.2
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.1 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.2 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `structured-pruning-adapters-0.6.1/README.md` & `structured-pruning-adapters-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/setup.py` & `structured-pruning-adapters-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/sp_adapters/lora.py` & `structured-pruning-adapters-0.6.2/sp_adapters/lora.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/sp_adapters/splopa.py` & `structured-pruning-adapters-0.6.2/sp_adapters/splopa.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/sp_adapters/splora.py` & `structured-pruning-adapters-0.6.2/sp_adapters/splora.py`

 * *Files 2% similar despite different names*

```diff
@@ -649,63 +649,39 @@
                     query = key = value = query.transpose(1, 0)
                 else:
                     query, key = [x.transpose(1, 0) for x in (query, key)]
                     value = key
             else:
                 query, key, value = [x.transpose(1, 0) for x in (query, key, value)]
 
-        # if not self._qkv_same_embed_dim:
-        if not self._qkv_same_embed_dim:
-            attn_output, attn_output_weights = F.multi_head_attention_forward(
-                query,
-                key,
-                value,
-                self.embed_dim,
-                self.num_heads,
-                self.in_proj_weight,
-                self.in_proj_bias,
-                self.bias_k,
-                self.bias_v,
-                self.add_zero_attn,
-                self.dropout,
-                self.out_proj.adapted_weight,
-                self.out_proj.bias,
-                training=self.training,
-                key_padding_mask=key_padding_mask,
-                need_weights=need_weights,
-                attn_mask=attn_mask,
-                use_separate_proj_weight=True,
-                q_proj_weight=self.q_proj.adapted_weight,
-                k_proj_weight=self.k_proj.adapted_weight,
-                v_proj_weight=self.v_proj.adapted_weight,
-                average_attn_weights=average_attn_weights,
-                is_causal=is_causal,
-            )
-        else:
-            attn_output, attn_output_weights = F.multi_head_attention_forward(
-                query,
-                key,
-                value,
-                self.embed_dim,
-                self.num_heads,
-                self.in_proj_weight,
-                self.in_proj_bias,
-                self.bias_k,
-                self.bias_v,
-                self.add_zero_attn,
-                self.dropout,
-                self.out_proj.adapted_weight,
-                self.out_proj.bias,
-                training=self.training,
-                key_padding_mask=key_padding_mask,
-                need_weights=need_weights,
-                attn_mask=attn_mask,
-                average_attn_weights=average_attn_weights,
-                is_causal=is_causal,
-            )
+        attn_output, attn_output_weights = F.multi_head_attention_forward(
+            query,
+            key,
+            value,
+            self.embed_dim,
+            self.num_heads,
+            None,  # self.in_proj_weight,
+            self.in_proj_bias,
+            self.bias_k,
+            self.bias_v,
+            self.add_zero_attn,
+            self.dropout,
+            self.out_proj.adapted_weight,
+            self.out_proj.bias,
+            training=self.training,
+            key_padding_mask=key_padding_mask,
+            need_weights=need_weights,
+            attn_mask=attn_mask,
+            use_separate_proj_weight=True,
+            q_proj_weight=self.q_proj.adapted_weight,
+            k_proj_weight=self.k_proj.adapted_weight,
+            v_proj_weight=self.v_proj.adapted_weight,
+            average_attn_weights=average_attn_weights,
+            is_causal=is_causal,
+        )
         if self.batch_first and is_batched:
             return attn_output.transpose(1, 0), attn_output_weights
         else:
             return attn_output, attn_output_weights
 
     @classmethod
     def from_module(
```

### Comparing `structured-pruning-adapters-0.6.1/sp_adapters/torch_pruning.py` & `structured-pruning-adapters-0.6.2/sp_adapters/torch_pruning.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,24 +107,26 @@
         return layer.in_channels
 
 
 splora_conv_pruner = SPLoRAConvPruner()
 
 
 class SPLoRAMultiheadAttentionPruner(function.BasePruningFunc):
-    TARGET_MODULES = nn.MultiheadAttention
+    TARGET_MODULES = SPLoRAMultiheadAttention
 
     def check(self, layer, idxs, to_output):
         super().check(layer, idxs, to_output)
         assert (layer.embed_dim - len(idxs)) % layer.num_heads == 0, (
             "embed_dim (%d) of MultiheadAttention after pruning must divide evenly by `num_heads` (%d)"
             % (layer.embed_dim, layer.num_heads)
         )
 
-    def prune_out_channels(self, layer, idxs: list) -> nn.Module:
+    def prune_out_channels(
+        self, layer: SPLoRAMultiheadAttention, idxs: Sequence[int]
+    ) -> nn.Module:
         """
         Note: The `torch_pruning.pruning.function.MultiheadAttentionPruner`
         implementation is fundamentally flawed.
 
         There is no good reason to prune other parameters than `out_proj` besides to
         satisfy that `embed_dim` is consistent across all its uses.
         Currently, however, the PyTorch implementation of nn.MultiheadAttention and
@@ -142,14 +144,15 @@
             idxs
             + [i + layer.embed_dim for i in idxs]
             + [i + 2 * layer.embed_dim for i in idxs]
         )
         keep_idxs_3x_repeated = list(
             set(range(3 * layer.embed_dim)) - set(pruning_idxs_repeated)
         )
+        keep_idxs_3x_repeated.sort()
 
         layer.q_proj = splora_linear_pruner.prune_out_channels(layer.q_proj, idxs)
         layer.q_proj = splora_linear_pruner.prune_in_channels(layer.q_proj, idxs)
 
         layer.k_proj = splora_linear_pruner.prune_out_channels(layer.k_proj, idxs)
         layer.k_proj = splora_linear_pruner.prune_in_channels(layer.k_proj, idxs)
 
@@ -170,21 +173,19 @@
 
         layer.embed_dim = layer.embed_dim - len(idxs)
         layer.head_dim = layer.embed_dim // layer.num_heads
         layer.kdim = layer.embed_dim
         layer.vdim = layer.embed_dim
         return layer
 
-    prune_in_channels = prune_out_channels
-
-    def get_out_channels(self, layer):
+    def get_out_channels(self, layer: SPLoRAMultiheadAttention):
         return layer.embed_dim
 
-    def get_in_channels(self, layer):
-        return self.get_out_channels(layer)
+    prune_in_channels = prune_out_channels
+    get_in_channels = get_out_channels
 
 
 splora_mha_pruner = SPLoRAMultiheadAttentionPruner()
 
 # Pass this dict to the "customized_pruners" argument of pruners in the Torch Pruning lib
 customized_pruners = {
     SPLoRALinear: splora_linear_pruner,
```

### Comparing `structured-pruning-adapters-0.6.1/sp_adapters/utils.py` & `structured-pruning-adapters-0.6.2/sp_adapters/utils.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/PKG-INFO` & `structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.6.1
+Version: 0.6.2
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.1 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.2 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `structured-pruning-adapters-0.6.1/structured_pruning_adapters.egg-info/SOURCES.txt` & `structured-pruning-adapters-0.6.2/structured_pruning_adapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/tests/test_lin_as_conv.py` & `structured-pruning-adapters-0.6.2/tests/test_lin_as_conv.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/tests/test_splopa.py` & `structured-pruning-adapters-0.6.2/tests/test_splopa.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.6.1/tests/test_splora.py` & `structured-pruning-adapters-0.6.2/tests/test_splora.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,22 +175,21 @@
     x = torch.randn(seq_len, embed_dim)
     y = torch.randn(seq_len, embed_dim)
 
     mha = nn.MultiheadAttention(
         embed_dim,
         num_heads,
         dropout=0.0,
-        bias=True,
+        bias=False,
         add_bias_kv=False,
         add_zero_attn=False,
         kdim=None,
         vdim=None,
         batch_first=False,
     )
-    mha.in_proj_bias = torch.nn.Parameter(torch.rand_like(mha.in_proj_bias))
 
     # Transfer
     spmha = SPLoRA(mha, rank)
 
     # Weights are all close, biases are equal
     assert torch.equal(
         mha.in_proj_weight,
@@ -201,19 +200,17 @@
                 spmha.v_proj.weight,
             )
         ),
     )
     assert torch.allclose(  # in_proj_weight property uses adapted_weights
         mha.in_proj_weight, spmha.in_proj_weight, atol=_DEFAULT_INIT_RANGE
     )
-    assert torch.equal(mha.in_proj_bias, spmha.in_proj_bias)
     assert torch.allclose(
         mha.out_proj.weight, spmha.out_proj.adapted_weight, atol=_DEFAULT_INIT_RANGE
     )
-    assert torch.equal(mha.out_proj.bias, spmha.out_proj.bias)
 
     # Prepare optim
     optimizer = torch.optim.Adam(spmha.parameters())
     optimizer.zero_grad()
 
     # Save for later comparison
     prev_q_proj_cols = torch.clone(spmha.q_proj.adapter.cols)
@@ -248,18 +245,14 @@
         ),
     )
     assert torch.equal(
         mha.out_proj.weight,
         spmha.out_proj.weight,
     )
 
-    # Biases changed
-    assert not torch.equal(mha.in_proj_bias, spmha.in_proj_bias)
-    assert not torch.equal(mha.out_proj.bias, spmha.out_proj.bias)
-
     # Adapter params changed
     assert not torch.equal(prev_q_proj_cols, spmha.q_proj.adapter.cols)
     assert not torch.equal(prev_q_proj_rows, spmha.q_proj.adapter.rows)
     assert not torch.equal(prev_k_proj_cols, spmha.k_proj.adapter.cols)
     assert not torch.equal(prev_k_proj_rows, spmha.k_proj.adapter.rows)
     assert not torch.equal(prev_v_proj_cols, spmha.v_proj.adapter.cols)
     assert not torch.equal(prev_v_proj_rows, spmha.v_proj.adapter.rows)
@@ -269,17 +262,15 @@
     # Export to mha
     mha2 = spmha.to_module()
 
     # Weights and biases are equal
     assert torch.equal(  # in_proj_weight property uses adapted_weights
         mha2.in_proj_weight, spmha.in_proj_weight
     )
-    assert torch.equal(mha2.in_proj_bias, spmha.in_proj_bias)
     assert torch.equal(mha2.out_proj.weight, spmha.out_proj.adapted_weight)
-    assert torch.equal(mha2.out_proj.bias, spmha.out_proj.bias)
 
 
 def test_splora_mha_diff_qkv_dim():
     rank = 2
     embed_dim = 16
     kdim = vdim = 24
     num_heads = 4
```

### Comparing `structured-pruning-adapters-0.6.1/tests/test_torchpruning.py` & `structured-pruning-adapters-0.6.2/tests/test_torchpruning.py`

 * *Files 6% similar despite different names*

```diff
@@ -306,10 +306,59 @@
     assert model.customized_layer.adapter.out_features == 2 * d_hidden - len(prune_idxs)
     assert model.c2.in_channels == 2 * d_hidden - len(prune_idxs)
 
     # print("The pruned model:\n", model)
     assert model(torch.randn(1, d_in, seq_len)).shape == (1, num_classes, 1)
 
 
+def test_SPLoRAMultiheadAttention_pruning():
+    class MhaNet(nn.Module):
+        def __init__(self, input_size, num_classes, hidden_units):
+            super().__init__()
+            self.fc1 = nn.Linear(input_size, hidden_units)
+            # self.mha = nn.MultiheadAttention(hidden_units, num_heads=4)
+            self.mha = spa.SPLoRAMultiheadAttention(hidden_units, num_heads=4, rank=2)
+            self.fc2 = nn.Linear(hidden_units, num_classes)
+
+        def forward(self, x):
+            x = F.relu(self.fc1(x))
+            x, _ = self.mha(x, x, x)
+            y_hat = self.fc2(x)
+            return y_hat
+
+    num_classes = 3
+    d_in = 8
+    d_hidden = 16
+    seq_len = 10
+    model = MhaNet(d_in, num_classes, d_hidden)
+    example_input = torch.randn(seq_len, d_in)
+
+    DG = tp.DependencyGraph()
+
+    DG.build_dependency(
+        model,
+        example_inputs=example_input,
+        customized_pruners=spa.torch_pruning.customized_pruners,
+    )
+    # Get a pruning group according to the dependency graph.
+    # idxs is the indices of pruned filters.
+    # Prune out channels
+    prune_idxs = [0, 1, 3, 6]
+    pruning_group = DG.get_pruning_group(
+        model.fc1, tp.prune_linear_out_channels, idxs=prune_idxs
+    )
+    print(pruning_group)
+
+    # Execute this group (prune the model)
+    pruning_group.prune()
+
+    # Check shapes
+    embed_dim = d_hidden - len(prune_idxs)
+    assert model.mha.q_proj.adapted_weight.shape == (embed_dim, embed_dim)
+    assert model.mha.k_proj.adapted_weight.shape == (embed_dim, embed_dim)
+    assert model.mha.v_proj.adapted_weight.shape == (embed_dim, embed_dim)
+    assert model.mha.out_proj.adapted_weight.shape == (embed_dim, embed_dim)
+
+
 if __name__ == "__main__":
     # test_SPLoRALinear_pruning()
     test_SPLoRALinear_magpruner()
```

