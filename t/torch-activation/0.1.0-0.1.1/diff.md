# Comparing `tmp/torch_activation-0.1.0.tar.gz` & `tmp/torch_activation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_activation-0.1.0.tar", max compression
+gzip compressed data, was "torch_activation-0.1.1.tar", max compression
```

## Comparing `torch_activation-0.1.0.tar` & `torch_activation-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      466 2023-05-26 05:16:22.044757 torch_activation-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2642 2023-05-26 05:15:36.983248 torch_activation-0.1.0/README.md
--rw-r--r--   0        0        0      546 2023-05-26 05:16:03.785176 torch_activation-0.1.0/torch_activation/__init__.py
--rw-r--r--   0        0        0     2773 2023-05-26 05:12:46.037659 torch_activation-0.1.0/torch_activation/composite.py
--rw-r--r--   0        0        0     3492 2023-05-23 01:10:45.441694 torch_activation-0.1.0/torch_activation/glu_family.py
--rw-r--r--   0        0        0     2613 2023-05-24 04:44:25.674253 torch_activation-0.1.0/torch_activation/lincomb.py
--rw-r--r--   0        0        0     2531 2023-05-24 04:28:43.623528 torch_activation-0.1.0/torch_activation/non_linear.py
--rw-r--r--   0        0        0     4774 2023-05-24 04:44:04.736433 torch_activation-0.1.0/torch_activation/relu_family.py
--rw-r--r--   0        0        0     3681 2023-05-26 05:00:14.812656 torch_activation-0.1.0/torch_activation/trig.py
--rw-r--r--   0        0        0     2877 2023-05-26 04:49:13.643443 torch_activation-0.1.0/torch_activation/utils.py
--rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 torch_activation-0.1.0/setup.py
--rw-r--r--   0        0        0     3298 1970-01-01 00:00:00.000000 torch_activation-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-06-15 08:18:26.113267 torch_activation-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3450 2023-06-15 13:03:48.769903 torch_activation-0.1.1/README.md
+-rw-r--r--   0        0        0      568 2023-06-13 07:56:12.907632 torch_activation-0.1.1/torch_activation/__init__.py
+-rw-r--r--   0        0        0     2773 2023-05-26 05:12:46.037659 torch_activation-0.1.1/torch_activation/composite.py
+-rw-r--r--   0        0        0     3485 2023-06-15 07:47:52.228991 torch_activation-0.1.1/torch_activation/glu_family.py
+-rw-r--r--   0        0        0     2617 2023-06-15 08:19:53.268211 torch_activation-0.1.1/torch_activation/lincomb.py
+-rw-r--r--   0        0        0     2417 2023-06-15 08:18:56.286253 torch_activation-0.1.1/torch_activation/non_linear.py
+-rw-r--r--   0        0        0     6141 2023-06-15 08:32:42.119866 torch_activation-0.1.1/torch_activation/relu_family.py
+-rw-r--r--   0        0        0     3525 2023-06-15 08:35:39.534749 torch_activation-0.1.1/torch_activation/trig.py
+-rw-r--r--   0        0        0     2877 2023-05-26 04:49:13.643443 torch_activation-0.1.1/torch_activation/utils.py
+-rw-r--r--   0        0        0     4197 1970-01-01 00:00:00.000000 torch_activation-0.1.1/setup.py
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 torch_activation-0.1.1/PKG-INFO
```

### Comparing `torch_activation-0.1.0/torch_activation/__init__.py` & `torch_activation-0.1.1/torch_activation/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .composite import DELU, DReLUs
 from .trig import CosLU, GCU, SinLU
 from .lincomb import LinComb, NormLinComb
 from .non_linear import CoLU, ScaledSoftSign
 from .glu_family import ReGLU, GeGLU, SeGLU, SwiGLU
-from .relu_family import ShiLU, CReLU, ReLUN, SquaredReLU
+from .relu_family import ShiLU, CReLU, ReLUN, SquaredReLU, StarReLU
 
 
 __all__ = ["ShiLU", "DELU", "CReLU", "GCU",
            "CosLU", "CoLU", "ReLUN",
            "SquaredReLU", "ScaledSoftSign",
            "ReGLU", "GeGLU", "SeGLU", "SwiGLU"
            "LinComb", "NormLinComb", "SinLU"
-           "DReLUs"]
+           "DReLUs", "StarReLU"]
 
 __version__ = "0.1.0"
```

### Comparing `torch_activation-0.1.0/torch_activation/composite.py` & `torch_activation-0.1.1/torch_activation/composite.py`

 * *Files identical despite different names*

### Comparing `torch_activation-0.1.0/torch_activation/glu_family.py` & `torch_activation-0.1.1/torch_activation/glu_family.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         return a * F.gelu(b)
 
 
 class SwiGLU(torch.nn.Module):
     r"""
     Applies the SwiGLU activation function, defined as:
 
-    :math:`\text{SwiGLU}(x) =  \text{Swish} (xW + b) \odot (xV + c)`
+    :math:`\sigma(x) =  \text{Swish} (xW + b) \odot (xV + c)`
 
     Args:
         inplace: can optionally do the operation in-place. Default: ``False``
         size: The size of the last dimension of the input tensor.
 
     Shape:
         - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
```

### Comparing `torch_activation-0.1.0/torch_activation/lincomb.py` & `torch_activation-0.1.1/torch_activation/lincomb.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return torch.sum(torch.stack(activations), dim=0)
 
 
 class NormLinComb(nn.Module):
     r"""
     Applies the LinComb activation function:
     
-    :math:`\text{NormLinComb}(x) = \frac{\sum_{i=1}^{n} w_i \cdot F_i(x)}{||W||}`
+    :math:`\text{NormLinComb}(x) = \frac{\sum_{i=1}^{n} w_i \cdot F_i(x)}{\|\|W\|\|}`
     
     Args:
         activation: List of activation functions.
         
     Shape:
         - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
         - Output: :math:`(*)`
```

### Comparing `torch_activation-0.1.0/torch_activation/non_linear.py` & `torch_activation-0.1.1/torch_activation/non_linear.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 from torch import Tensor
 
 
 class CoLU(nn.Module):
     r"""
     Applies the Collapsing Linear Unit activation function:
 
-    :math:`\text{CoLU}(x) = \frac{x}{1-x \mul e^{-(x+e^x)}}`
+    :math:`\text{CoLU}(x) = \frac{x}{1-x \cdot e^{-(x + e^x)}}`
 
     Args:
         inplace: can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
-    .. image:: ../images/activation_images/CoLU.png
-
     Examples::
 
         >>> m = nn.CoLU()
         >>> x = torch.randn(2)
         >>> output = m(x)
 
         >>> m = nn.CoLU(inplace=True)
@@ -42,31 +40,29 @@
             return x / (1 - x * torch.exp(-1 * (x + torch.exp(x))))
 
 
 class ScaledSoftSign(torch.nn.Module):
     r"""
     Applies the ScaledSoftSign activation function:
 
-    :math:`\text{ScaledSoftSign}(x) = \frac{\alpha \mul x}{\beta + |x|}`
+    :math:`\text{ScaledSoftSign}(x) = \frac{\alpha \cdot x}{\beta + \|x\|}`
 
     Args:
         alpha: The initial value of the alpha parameter.
         beta: The initial value of the beta parameter.
         inplace: can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
     Attributes:
         alpha (nn.Parameter): The alpha scaling parameter.
         beta (nn.Parameter): The beta scaling parameter.
 
-    .. image:: ../images/activation_images/ScaledSoftSign.png
-
     Examples:
         >>> m = ScaledSoftSign(alpha=0.5, beta=1.0)
         >>> x = torch.randn(2, 3)
         >>> output = m(x)
 
         >>> m = ScaledSoftSign(inplace=True)
         >>> x = torch.randn(2, 3)
```

### Comparing `torch_activation-0.1.0/torch_activation/relu_family.py` & `torch_activation-0.1.1/torch_activation/relu_family.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from torch import Tensor
 
 
 class ShiLU(nn.Module):
     r"""
     Applies the ShiLU activation function:
 
-    :math:`\text{ShiLU}(x) = \alpha * \max(0,x) + \beta`
+    :math:`\text{ShiLU}(x) = \alpha \cdot \text{ReLU}(x) + \beta`
 
     Args:
         alpha : Scaling factor for the positive part of the input. Default: 1.0.
         beta : Bias term added to the output. Default: 0.0.
         inplace: can optionally do the operation in-place. Default: ``False``
 
     Shape:
@@ -53,26 +53,24 @@
             return self.alpha * F.relu(x) + self.beta
         
 
 class CReLU(nn.Module):
     r"""
     Applies the Concatenated Rectified Linear Unit activation function.
 
-    :math:`\text{CReLU}(x) = \max(0,x) \oplus \max(0,-x)`
+    :math:`\text{CReLU}(x) = \text{ReLU}(x) \oplus \text{ReLU}(-x)`
 
     Args:
         dim: Dimension along which to concatenate in the output tensor. Default: 1
         inplace: can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*, C, *)` where :math:`*` means any number of additional dimensions
         - Output: :math:`(*, 2C, *)`
 
-    .. image:: ../images/activation_images/CReLU.png
-
     Examples::
 
         >>> m = nn.CReLU()
         >>> x = torch.randn(2, 3)
         >>> output = m(x)
         
         >>> m = CReLU(inplace=True)
@@ -88,29 +86,27 @@
     def forward(self, x) -> Tensor:
         return F.relu(torch.cat((x, -x), dim=self.dim))
         
         
 class ReLUN(nn.Module):
     r"""Applies the element-wise function:
 
-    :math:`\text{ReLUN}(x) = \min(\max(0,x), n)`
+    :math:`\text{ReLUN}(x) = \min(\text{ReLU}(x), n)`
 
     Args:
         n: Upper bound for the function's output. Default is 1.0.
         inplace: can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
         
     Attributes:
         n: Upper bound for the function's output. Default is 1.0.
         
-    .. image:: ../images/activation_images/ReLUN.png
-
     Examples::
 
         >>> m = nn.ReLUN(n=6.0) # ReLU6
         >>> x = torch.randn(2)
         >>> output = m(x)
         
         >>> m = nn.ReLUN(inplace=True)
@@ -140,16 +136,14 @@
 
     Args:
         inplace: can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
-        
-    .. image:: ../images/activation_images/SquaredReLU.png
 
     Examples::
 
         >>> m = nn.SquaredReLU()
         >>> x = torch.randn(2)
         >>> output = m(x)
 
@@ -164,11 +158,59 @@
         self.inplace = inplace
 
     def forward(self, x) -> Tensor:
         if self.inplace:
             return F.relu_(x).pow_(2)
         else:
             return F.relu(x).pow(2)
+        
+class StarReLU(nn.Module):
+    r"""
+    Applies the element-wise function:
+
+    :math:`\text{StarReLU}(x) = s \cdot \text{ReLU}(x)^2 + b`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+        s: Scaled factor for StarReLU, shared across channel. Default: 0.8944
+        b: Bias term for StarReLU, shared across channel. Default: -0.4472
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    .. image:: ../images/activation_images/SquaredReLU.png
+
+    Examples::
+
+        >>> m = nn.StarReLU(s=1.0, b=0.0)
+        >>> x = torch.randn(3, 384, 384)
+        >>> output = m(x)
+
+        >>> m = nn.StarReLU(learnable=True, inplace=True)
+        >>> x = torch.randn(3, 384, 384)
+        >>> m(x)
+    """
+    
+    
+    def __init__(self, s=0.8944, b=-0.4472, learnable=True, inplace=False):
+        super().__init__()
+        self.inplace = inplace
+        if learnable:
+            self.s = nn.Parameter(torch.tensor(s))
+            self.b = nn.Parameter(torch.tensor(b))
+        else:
+            self.s = torch.tensor(s)
+            self.b = torch.tensor(b)
+        
+
+    def forward(self, x) -> Tensor:
+        if self.inplace:
+            return F.relu_(x).pow_(2) \
+                             .mul_(self.s) \
+                             .add_(self.b)
+        else:
+            return self.s * F.relu(x).pow(2) + self.b
     
     
 if __name__ == '__main__':
     pass
```

### Comparing `torch_activation-0.1.0/torch_activation/trig.py` & `torch_activation-0.1.1/torch_activation/trig.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
     Args:
         inplace: can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
-
-    .. image:: ../images/activation_images/GCU.png
-
+        
     Examples::
 
         >>> m = nn.GCU()
         >>> x = torch.randn(2)
         >>> output = m(x)
 
         >>> m = nn.GCU(inplace=True)
@@ -59,16 +57,14 @@
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
     Attributes:
         alpha: Scaling factor for the cosine term. Default is 1.0.
         beta: Frequency factor for the cosine term. Default is 1.0.
 
-    .. image:: ../images/activation_images/CosLU.png
-
     Examples::
 
         >>> m = CosLU(alpha=2.0, beta=1.0)
         >>> x = torch.randn(2)
         >>> output = m(x)
 
         >>> m = CosLU(inplace=True)
@@ -108,16 +104,14 @@
         a: Initial value for sine function magnitude. Default: 1.0.
         b: Initial value for sine function period. Default: 1.0.
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
-    .. image:: ../images/activation_images/GCU.png
-
     Examples::
 
         >>> m = nn.SinLU(a=5.0, b=6.0)
         >>> x = torch.randn(2)
         >>> output = m(x)
     """
     def __init__(self, a=1.0, b=1.0):
```

### Comparing `torch_activation-0.1.0/torch_activation/utils.py` & `torch_activation-0.1.1/torch_activation/utils.py`

 * *Files identical despite different names*

