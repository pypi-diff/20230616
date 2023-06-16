# Comparing `tmp/pytorch-complex-0.0.8.tar.gz` & `tmp/pytorch-complex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytorch-complex-0.0.8.tar", last modified: Tue Dec  8 17:15:13 2020, max compression
+gzip compressed data, was "pytorch-complex-0.1.1.tar", last modified: Fri Jun 16 14:49:15 2023, max compression
```

## Comparing `pytorch-complex-0.0.8.tar` & `pytorch-complex-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2020-12-08 17:15:13.679316 pytorch-complex-0.0.8/
--rw-rw-rw-   0        0        0     1771 2020-12-08 17:15:13.678320 pytorch-complex-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      373 2020-11-06 19:54:11.000000 pytorch-complex-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-12-08 17:15:13.651390 pytorch-complex-0.0.8/pytorch_complex.egg-info/
--rw-rw-rw-   0        0        0     1771 2020-12-08 17:15:13.000000 pytorch-complex-0.0.8/pytorch_complex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      669 2020-12-08 17:15:13.000000 pytorch-complex-0.0.8/pytorch_complex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-08 17:15:13.000000 pytorch-complex-0.0.8/pytorch_complex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2020-12-08 17:15:13.000000 pytorch-complex-0.0.8/pytorch_complex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2020-12-08 17:15:13.000000 pytorch-complex-0.0.8/pytorch_complex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-08 17:15:13.679316 pytorch-complex-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1327 2020-12-08 17:14:00.000000 pytorch-complex-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-08 17:15:13.653386 pytorch-complex-0.0.8/torchcomplex/
--rw-rw-rw-   0        0        0        0 2020-11-06 11:17:35.000000 pytorch-complex-0.0.8/torchcomplex/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-08 17:15:13.658372 pytorch-complex-0.0.8/torchcomplex/nn/
--rw-rw-rw-   0        0        0       42 2020-12-08 17:13:31.000000 pytorch-complex-0.0.8/torchcomplex/nn/__init__.py
--rw-rw-rw-   0        0        0    18296 2020-12-08 14:50:55.000000 pytorch-complex-0.0.8/torchcomplex/nn/functional.py
--rw-rw-rw-   0        0        0    20026 2020-12-08 17:12:32.000000 pytorch-complex-0.0.8/torchcomplex/nn/init.py
-drwxrwxrwx   0        0        0        0 2020-12-08 17:15:13.672335 pytorch-complex-0.0.8/torchcomplex/nn/modules/
--rw-rw-rw-   0        0        0     1268 2020-11-18 11:55:03.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/__init__.py
--rw-rw-rw-   0        0        0     5720 2020-12-08 15:05:46.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/activation.py
--rw-rw-rw-   0        0        0    18784 2020-11-06 22:46:48.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/batchnorm.py
--rw-rw-rw-   0        0        0    47004 2020-11-12 11:32:48.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/conv.py
--rw-rw-rw-   0        0        0     8963 2020-11-06 19:35:01.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/dropout.py
--rw-rw-rw-   0        0        0     8877 2020-11-18 11:49:53.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/linear.py
--rw-rw-rw-   0        0        0    51096 2020-11-12 11:32:48.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/pooling.py
--rw-rw-rw-   0        0        0     6974 2020-11-12 11:32:48.000000 pytorch-complex-0.0.8/torchcomplex/nn/modules/upsampling.py
-drwxrwxrwx   0        0        0        0 2020-12-08 17:15:13.676323 pytorch-complex-0.0.8/torchcomplex/utils/
--rw-rw-rw-   0        0        0        0 2020-12-07 21:51:31.000000 pytorch-complex-0.0.8/torchcomplex/utils/__init__.py
--rw-rw-rw-   0        0        0     8880 2020-12-07 21:49:35.000000 pytorch-complex-0.0.8/torchcomplex/utils/signaltools.py
+drwxr-xr-x   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 14:49:15.720881 pytorch-complex-0.1.1/
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     1076 2023-06-16 10:20:33.000000 pytorch-complex-0.1.1/LICENSE
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     3117 2023-06-16 14:49:15.726673 pytorch-complex-0.1.1/PKG-INFO
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     1589 2023-06-16 10:20:33.000000 pytorch-complex-0.1.1/README.md
+drwxr-xr-x   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 14:49:15.362131 pytorch-complex-0.1.1/pytorch_complex.egg-info/
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     3117 2023-06-16 14:49:11.000000 pytorch-complex-0.1.1/pytorch_complex.egg-info/PKG-INFO
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)      649 2023-06-16 14:49:13.000000 pytorch-complex-0.1.1/pytorch_complex.egg-info/SOURCES.txt
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)        1 2023-06-16 14:49:11.000000 pytorch-complex-0.1.1/pytorch_complex.egg-info/dependency_links.txt
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)       13 2023-06-16 14:49:11.000000 pytorch-complex-0.1.1/pytorch_complex.egg-info/top_level.txt
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)       38 2023-06-16 14:49:15.740657 pytorch-complex-0.1.1/setup.cfg
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     1370 2023-06-16 14:41:09.000000 pytorch-complex-0.1.1/setup.py
+drwxr-xr-x   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 14:49:15.386165 pytorch-complex-0.1.1/torchcomplex/
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 10:20:34.000000 pytorch-complex-0.1.1/torchcomplex/__init__.py
+drwxr-xr-x   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 14:49:15.448898 pytorch-complex-0.1.1/torchcomplex/nn/
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)       42 2023-06-16 10:20:34.000000 pytorch-complex-0.1.1/torchcomplex/nn/__init__.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)    21129 2023-06-16 13:59:46.000000 pytorch-complex-0.1.1/torchcomplex/nn/functional.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)    20026 2023-06-16 10:20:34.000000 pytorch-complex-0.1.1/torchcomplex/nn/init.py
+drwxr-xr-x   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 14:49:15.650990 pytorch-complex-0.1.1/torchcomplex/nn/modules/
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     1268 2023-06-16 10:20:34.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/__init__.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     7189 2023-06-16 14:12:50.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/activation.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)    19310 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/batchnorm.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)    46997 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/conv.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     8963 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/dropout.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     8875 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/linear.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)    51096 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/pooling.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     6974 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/nn/modules/upsampling.py
+drwxr-xr-x   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 14:49:15.707300 pytorch-complex-0.1.1/torchcomplex/utils/
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)        0 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/utils/__init__.py
+-rw-r--r--   0 soumick.chatterjee  (6657) glastonbury  (5697)     8880 2023-06-16 10:20:35.000000 pytorch-complex-0.1.1/torchcomplex/utils/signaltools.py
```

### Comparing `pytorch-complex-0.0.8/pytorch_complex.egg-info/SOURCES.txt` & `pytorch-complex-0.1.1/pytorch_complex.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+LICENSE
 README.md
+setup.cfg
 setup.py
 pytorch_complex.egg-info/PKG-INFO
 pytorch_complex.egg-info/SOURCES.txt
 pytorch_complex.egg-info/dependency_links.txt
-pytorch_complex.egg-info/requires.txt
 pytorch_complex.egg-info/top_level.txt
 torchcomplex/__init__.py
 torchcomplex/nn/__init__.py
 torchcomplex/nn/functional.py
 torchcomplex/nn/init.py
 torchcomplex/nn/modules/__init__.py
 torchcomplex/nn/modules/activation.py
```

### Comparing `pytorch-complex-0.0.8/setup.py` & `pytorch-complex-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import setuptools
-
-with open("README.md", "r", encoding='utf8') as fh:
-    readme = fh.read()
-
-with open('HISTORY.rst', "r", encoding='utf8') as history_file:
-    history = history_file.read()
-
-requirements = [
-    'torch>=1.7'
-]
-
-setup_requirements = [
-]
-
-tests_requirements = [
-]
-
-setuptools.setup(
-    name="pytorch-complex", 
-    version="0.0.8",
-    author="Soumick Chatterjee",
-    author_email="soumick.chatterjee@ovgu.de",
-    description="Complex Modules for PyTorch",
-    long_description=readme + '\n\n' + history,
-    long_description_content_type="text/markdown",
-    url="https://github.com/soumickmj/pytorch-complex",
-    packages=setuptools.find_packages(include=['torchcomplex', 'torchcomplex.*']),
-    classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires=requirements,
-    setup_requires=setup_requirements,
-    tests_require=tests_requirements,
-    license='MIT license',
-    include_package_data=True,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import setuptools
+
+with open("README.md", "r", encoding='utf8') as fh:
+    readme = fh.read()
+
+with open('HISTORY.rst', "r", encoding='utf8') as history_file:
+    history = history_file.read()
+
+requirements = [
+    
+]
+
+setup_requirements = [
+]
+
+tests_requirements = [
+]
+
+setuptools.setup(
+    name="pytorch-complex", 
+    version="0.1.1",
+    author="Soumick Chatterjee",
+    author_email="soumick.chatterjee@ovgu.de",
+    description="Complex Modules for PyTorch",
+    long_description=readme + '\n\n' + history,
+    long_description_content_type="text/markdown",
+    url="https://github.com/soumickmj/pytorch-complex",
+    packages=setuptools.find_packages(include=['torchcomplex', 'torchcomplex.*']),
+    classifiers=[
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+    install_requires=requirements,
+    setup_requires=setup_requirements,
+    tests_require=tests_requirements,
+    license='MIT license',
+    include_package_data=True,
+)
```

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/functional.py` & `pytorch-complex-0.1.1/torchcomplex/nn/functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         MiKr = funtinal_handle(inp_i, w_r, b_r, *args[3:]) #Imaginary Feature Maps * Real Kernels
     real = MrKr - MiKi
     imag = MrKi + MiKr
     out = torch.view_as_complex(torch.stack((real,imag),dim=-1))
     
     return out
 
+#Convolutions
+
 def conv1d(input, weight, bias=None, stride=1, padding=0, dilation=1, groups=1) -> Tensor:
     return _fcaller(F.conv1d, input, weight, bias, stride, padding, dilation, groups)
 
 def conv2d(input, weight, bias=None, stride=1, padding=0, dilation=1, groups=1) -> Tensor:
     return _fcaller(F.conv2d, input, weight, bias, stride, padding, dilation, groups)
 
 def conv3d(input, weight, bias=None, stride=1, padding=0, dilation=1, groups=1) -> Tensor:
@@ -94,14 +96,33 @@
 
 def conv_transpose2d(input, weight, bias=None, stride=1, padding=0, output_padding=0, groups=1, dilation=1) -> Tensor:
     return _fcaller(F.conv_transpose2d, input, weight, bias, stride, padding, output_padding, groups, dilation)
 
 def conv_transpose3d(input, weight, bias=None, stride=1, padding=0, output_padding=0, groups=1, dilation=1) -> Tensor:
     return _fcaller(F.conv_transpose3d, input, weight, bias, stride, padding, output_padding, groups, dilation)
 
+#Poolings
+def max_pool1d(input, kernel_size, stride=None, padding=0, dilation=1, ceil_mode=False, return_indices=False) -> Tensor:
+    return complex_fcaller(F.max_pool1d, input, kernel_size, stride, padding, dilation, ceil_mode, return_indices)
+
+def max_pool2d(input, kernel_size, stride=None, padding=0, dilation=1, ceil_mode=False, return_indices=False) -> Tensor: 
+    return complex_fcaller(F.max_pool2d, input, kernel_size, stride, padding, dilation, ceil_mode, return_indices)
+
+def max_pool3d(input, kernel_size, stride=None, padding=0, dilation=1, ceil_mode=False, return_indices=False) -> Tensor:
+    return complex_fcaller(F.max_pool3d, input, kernel_size, stride, padding, dilation, ceil_mode, return_indices)
+
+def avg_pool1d(input, kernel_size, stride=None, padding=0, ceil_mode=False, count_include_pad=True, divisor_override=None) -> Tensor:
+    return complex_fcaller(F.avg_pool1d, input, kernel_size, stride, padding, ceil_mode, count_include_pad, divisor_override)
+
+def avg_pool2d(input, kernel_size, stride=None, padding=0, ceil_mode=False, count_include_pad=True, divisor_override=None) -> Tensor:
+    return complex_fcaller(F.avg_pool2d, input, kernel_size, stride, padding, ceil_mode, count_include_pad, divisor_override)
+
+def avg_pool3d(input, kernel_size, stride=None, padding=0, ceil_mode=False, count_include_pad=True, divisor_override=None) -> Tensor:
+    return complex_fcaller(F.avg_pool3d, input, kernel_size, stride, padding, ceil_mode, count_include_pad, divisor_override)
+
 # Linear
 def linear(input, weight, bias=None):
     return _fcaller(F.linear, input, weight, bias)
 
 def bilinear(input1, input2, weight, bias=None):
     return _fcaller(F.bilinear, (input1, input2), weight, bias)
 
@@ -212,23 +233,24 @@
 
 def batch_norm(input, running_mean, running_var, weight=None, bias=None,
                training=False, momentum=0.1, eps=1e-5, naive=False):
 
     """
     Source: Source: https://github.com/ivannz/cplxmodule/blob/master/cplxmodule/nn/modules/batchnorm.py
     """
+    complex_weight = not(type(weight) == torch.nn.ParameterList)
     if naive:
         real = F.batch_norm(input.real,
                             running_mean[0] if running_mean is not None else None,
                             running_var[0] if running_var is not None else None,
-                            weight[0], bias[0], training, momentum, eps)
+                            weight.real if complex_weight else weight[0], bias.real if complex_weight else bias[0], training, momentum, eps)
         imag = F.batch_norm(input.imag,
                             running_mean[1] if running_mean is not None else None,
                             running_var[1] if running_var is not None else None,
-                            weight[1], bias[1], training, momentum, eps)
+                            weight.imag if complex_weight else weight[1], bias.imag if complex_weight else bias[1], training, momentum, eps)
         return torch.view_as_complex(torch.stack((real, imag),dim=-1))
     else:
         # stack along the first axis
         x = torch.stack([input.real, input.imag], dim=0)
 
         # whiten and apply affine transformation
         z = _whiten2x2(x, training=training, running_mean=running_mean,
@@ -265,33 +287,35 @@
     https://arxiv.org/pdf/1705.09792.pdf
     '''
     if input.is_complex():
         return input * ((0 < input.angle()) * (input.angle() < math.pi/2)).float()
     else:
         return F.relu(input, inplace=inplace)
 
-def modrelu(input: Tensor, bias: int, inplace: bool = False) -> Tensor:
+def modrelu(input: Tensor, bias: Tensor, inplace: bool = False) -> Tensor:
     '''
     Martin Arjovsky, Amar Shah, and Yoshua Bengio. Unitary evolution recurrent neural networks. arXiv preprint arXiv:1511.06464, 2015.
     Notice that |z| (z.magnitude) is always positive, so if b > 0  then |z| + b > = 0 always.
     In order to have any non-linearity effect, b must be smaller than 0 (b<0).
+    Update: The implementation has been updated following: \\operatorname{ReLU}(|z|+b) \\frac{z}{|z|}
     '''
     if input.is_complex():
         z_mag = torch.abs(input)
-        return input * ((z_mag + bias) >= 0).float() * (1 + bias / z_mag)
+        return F.relu(z_mag + bias) * (input / z_mag)
     else:
         return F.relu(input, inplace=inplace)
 
 def cmodrelu(input: Tensor, threshold: int, inplace: bool = False):
     r"""Compute the Complex modulus relu of the complex tensor in re-im pair.
     As proposed in : https://arxiv.org/pdf/1802.08026.pdf
     Source: https://github.com/ivannz/cplxmodule"""
     if input.is_complex():
         modulus = torch.clamp(torch.abs(input), min=1e-5)
-        return input * F.relu(1. - threshold / modulus)
+        _tmp_newshape = (1,len(threshold)) + (1,)*len(input.shape[2:])
+        return input * F.relu(1. - threshold.view(_tmp_newshape) / modulus)
     else:
         return F.relu(input, inplace=inplace)
 
 def softmax(input, dim=None, _stacklevel=3, dtype=None):
     '''
     Complex-valued Neural Networks with Non-parametric Activation Functions
     (Eq. 36)
@@ -307,14 +331,31 @@
         a, b = input.real, input.imag
         denominator = torch.cosh(2*a) + torch.cos(2*b)
         real = torch.sinh(2 * a) / denominator
         imag = torch.sin(2 * a) / denominator
         return torch.view_as_complex(torch.stack((real, imag),dim=-1))
     else:
         return F.tanh(input)
+    
+def hirose(input: Tensor, m_sqaure: float = 1):
+    '''
+    A. Hirose. Complex-valued neural networks: Advances and applications. John Wiley & Sons, 2013. 
+    and
+    Wolter and Yao. Complex Gated Recurrent Neural Networks. NeurIPS 2018. (Eq. 5) https://papers.nips.cc/paper_files/paper/2018/file/652cf38361a209088302ba2b8b7f51e0-Paper.pdf
+    '''
+    mag_input = torch.abs(input)
+    return F.tanh(mag_input/m_sqaure) * (input / mag_input)
+
+def modsigmoid(input: Tensor, alpha: float = 0.5):
+    '''
+    Wolter and Yao. Complex Gated Recurrent Neural Networks. NeurIPS 2018. (Eq. 13) https://papers.nips.cc/paper_files/paper/2018/file/652cf38361a209088302ba2b8b7f51e0-Paper.pdf
+    and
+    Xie et al. Complex Recurrent Variational Autoencoder with Application to Speech Enhancement. 2023. arXiv:2204.02195v2
+    '''
+    return torch.sigmoid(alpha * input.real + (1 - alpha) * input.imag)
 
 def sigmoid(input: Tensor):
     if input.is_complex():
         a, b = input.real, input.imag
         denominator = 1 + 2 * torch.exp(-a) * torch.cos(b) + torch.exp(-2 * a)
         real = 1 + torch.exp(-a) * torch.cos(b) / denominator
         imag = torch.exp(-a) * torch.sin(b) / denominator
```

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/init.py` & `pytorch-complex-0.1.1/torchcomplex/nn/init.py`

 * *Files identical despite different names*

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/modules/__init__.py` & `pytorch-complex-0.1.1/torchcomplex/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/modules/batchnorm.py` & `pytorch-complex-0.1.1/torchcomplex/nn/modules/batchnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,33 @@
     def __init__(
         self,
         num_features: int,
         eps: float = 1e-5,
         momentum: float = 0.1,
         affine: bool = True,
         track_running_stats: bool = True,
-        naive = False
+        naive = False,
+        complex_weights = True
     ) -> None:
         super(_NormBase, self).__init__()
         self.num_features = num_features
         self.eps = eps
         self.momentum = momentum
         self.affine = affine
         self.track_running_stats = track_running_stats
         self.naive = naive
+        self.complex_weights = complex_weights
         if naive:
             if self.affine:
-                self.weight = ParameterList([Parameter(torch.Tensor(num_features)), Parameter(torch.Tensor(num_features))])
-                self.bias = ParameterList([Parameter(torch.Tensor(num_features)), Parameter(torch.Tensor(num_features))])
+                if complex_weights:
+                    self.weight = Parameter(torch.Tensor(num_features).to(torch.cfloat))
+                    self.bias = Parameter(torch.Tensor(num_features).to(torch.cfloat))
+                else:
+                    self.weight = ParameterList([Parameter(torch.Tensor(num_features)), Parameter(torch.Tensor(num_features))])
+                    self.bias = ParameterList([Parameter(torch.Tensor(num_features)), Parameter(torch.Tensor(num_features))])
             else:
                 self.register_parameter('weight', None)
                 self.register_parameter('bias', None)
             if self.track_running_stats:
                 self.register_buffer('running_mean', torch.zeros(2, num_features))
                 self.register_buffer('running_var', torch.ones(2, num_features))
                 self.register_buffer('num_batches_tracked', torch.tensor(0, dtype=torch.long))
@@ -87,18 +93,22 @@
                 self.running_var[1, 1].fill_(1)
                 self.num_batches_tracked.zero_()  # type: ignore[operator]
 
     def reset_parameters(self) -> None:
         self.reset_running_stats()
         if self.naive:
             if self.affine:
-                init.ones_(self.weight[0])
-                init.zeros_(self.bias[0])
-                init.ones_(self.weight[1])
-                init.zeros_(self.bias[1])
+                if self.complex_weights:
+                    init.ones_(self.weight)
+                    init.zeros_(self.bias)
+                else:
+                    init.ones_(self.weight[0])
+                    init.zeros_(self.bias[0])
+                    init.ones_(self.weight[1])
+                    init.zeros_(self.bias[1])
         else:
             if self.affine:
                 init.ones_(self.weight[0, 0])
                 init.zeros_(self.weight[1, 0])
                 init.zeros_(self.weight[0, 1])
                 init.ones_(self.weight[1, 1])
                 init.zeros_(self.bias)
@@ -125,17 +135,17 @@
             state_dict, prefix, local_metadata, strict,
             missing_keys, unexpected_keys, error_msgs)
 
 
 class _BatchNorm(_NormBase):
 
     def __init__(self, num_features, eps=1e-5, momentum=0.1, affine=True,
-                 track_running_stats=True, naive=False):
+                 track_running_stats=True, naive=False, complex_weights=True):
         super(_BatchNorm, self).__init__(
-            num_features, eps, momentum, affine, track_running_stats, naive)
+            num_features, eps, momentum, affine, track_running_stats, naive, complex_weights)
 
     def forward(self, input: Tensor) -> Tensor:
         self._check_input_dim(input)
 
         # exponential_average_factor is set to self.momentum
         # (when it is available) only so that it gets updated
         # in ONNX graph when this node is exported to ONNX.
```

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/modules/conv.py` & `pytorch-complex-0.1.1/torchcomplex/nn/modules/conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                  padding: _size_1_t,
                  dilation: _size_1_t,
                  transposed: bool,
                  output_padding: _size_1_t,
                  groups: int,
                  bias: bool,
                  padding_mode: str,
-                 complex_weights=False) -> None:
+                 complex_weights=True) -> None:
         super(_ConvNd, self).__init__()
         if in_channels % groups != 0:
             raise ValueError('in_channels must be divisible by groups')
         if out_channels % groups != 0:
             raise ValueError('out_channels must be divisible by groups')
         valid_padding_modes = {'zeros', 'reflect', 'replicate', 'circular'}
         if padding_mode not in valid_padding_modes:
@@ -264,15 +264,15 @@
         kernel_size: _size_1_t,
         stride: _size_1_t = 1,
         padding: _size_1_t = 0,
         dilation: _size_1_t = 1,
         groups: int = 1,
         bias: bool = True,
         padding_mode: str = 'zeros',
-        complex_weights = False
+        complex_weights = True
     ):
         kernel_size = _single(kernel_size)
         stride = _single(stride)
         padding = _single(padding)
         dilation = _single(dilation)
         super(Conv1d, self).__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
@@ -401,15 +401,15 @@
         kernel_size: _size_2_t,
         stride: _size_2_t = 1,
         padding: _size_2_t = 0,
         dilation: _size_2_t = 1,
         groups: int = 1,
         bias: bool = True,
         padding_mode: str = 'zeros',
-        complex_weights = False
+        complex_weights = True
     ):
         kernel_size = _pair(kernel_size)
         stride = _pair(stride)
         padding = _pair(padding)
         dilation = _pair(dilation)
         super(Conv2d, self).__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
@@ -527,15 +527,15 @@
         kernel_size: _size_3_t,
         stride: _size_3_t = 1,
         padding: _size_3_t = 0,
         dilation: _size_3_t = 1,
         groups: int = 1,
         bias: bool = True,
         padding_mode: str = 'zeros',
-        complex_weights = False
+        complex_weights = True
     ):
         kernel_size = _triple(kernel_size)
         stride = _triple(stride)
         padding = _triple(padding)
         dilation = _triple(dilation)
         super(Conv3d, self).__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
@@ -698,15 +698,15 @@
         stride: _size_1_t = 1,
         padding: _size_1_t = 0,
         output_padding: _size_1_t = 0,
         groups: int = 1,
         bias: bool = True,
         dilation: _size_1_t = 1,
         padding_mode: str = 'zeros',
-        complex_weights = False
+        complex_weights = True
     ):
         kernel_size = _single(kernel_size)
         stride = _single(stride)
         padding = _single(padding)
         dilation = _single(dilation)
         output_padding = _single(output_padding)
         super(ConvTranspose1d, self).__init__(
@@ -841,15 +841,15 @@
         stride: _size_2_t = 1,
         padding: _size_2_t = 0,
         output_padding: _size_2_t = 0,
         groups: int = 1,
         bias: bool = True,
         dilation: int = 1,
         padding_mode: str = 'zeros',
-        complex_weights = False
+        complex_weights = True
     ):
         kernel_size = _pair(kernel_size)
         stride = _pair(stride)
         padding = _pair(padding)
         dilation = _pair(dilation)
         output_padding = _pair(output_padding)
         super(ConvTranspose2d, self).__init__(
@@ -981,15 +981,15 @@
         stride: _size_3_t = 1,
         padding: _size_3_t = 0,
         output_padding: _size_3_t = 0,
         groups: int = 1,
         bias: bool = True,
         dilation: _size_3_t = 1,
         padding_mode: str = 'zeros',
-        complex_weights = False
+        complex_weights = True
     ):
         kernel_size = _triple(kernel_size)
         stride = _triple(stride)
         padding = _triple(padding)
         dilation = _triple(dilation)
         output_padding = _triple(output_padding)
         super(ConvTranspose3d, self).__init__(
```

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/modules/dropout.py` & `pytorch-complex-0.1.1/torchcomplex/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/modules/linear.py` & `pytorch-complex-0.1.1/torchcomplex/nn/modules/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     __constants__ = ['in_features', 'out_features']
     in_features: int
     out_features: int
     complex_weights: bool
     weight: Union[Tensor, Tuple[Tensor, Tensor]]
     bias: Optional[Union[Tensor, Tuple[Tensor, Tensor]]]
 
-    def __init__(self, in_features: int, out_features: int, bias: bool = True, complex_weights: bool = False) -> None:
+    def __init__(self, in_features: int, out_features: int, bias: bool = True, complex_weights: bool = True) -> None:
         super(Linear, self).__init__()
         self.in_features = in_features
         self.out_features = out_features
         self.complex_weights = complex_weights
 
         if complex_weights:
             self.weight = Parameter(torch.Tensor(out_features, in_features).to(torch.cfloat))
@@ -153,15 +153,15 @@
     in1_features: int
     in2_features: int
     out_features: int
     complex_weights: bool
     weight: Union[Tensor, Tuple[Tensor, Tensor]]
     bias: Optional[Union[Tensor, Tuple[Tensor, Tensor]]]
 
-    def __init__(self, in1_features: int, in2_features: int, out_features: int, bias: bool = True, complex_weights: bool = False) -> None:
+    def __init__(self, in1_features: int, in2_features: int, out_features: int, bias: bool = True, complex_weights: bool = True) -> None:
         super(Bilinear, self).__init__()
         self.in1_features = in1_features
         self.in2_features = in2_features
         self.out_features = out_features
         self.complex_weights = complex_weights
 
         if complex_weights:
```

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/modules/pooling.py` & `pytorch-complex-0.1.1/torchcomplex/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `pytorch-complex-0.0.8/torchcomplex/nn/modules/upsampling.py` & `pytorch-complex-0.1.1/torchcomplex/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `pytorch-complex-0.0.8/torchcomplex/utils/signaltools.py` & `pytorch-complex-0.1.1/torchcomplex/utils/signaltools.py`

 * *Files identical despite different names*

