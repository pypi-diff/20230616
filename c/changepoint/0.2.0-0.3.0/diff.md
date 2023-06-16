# Comparing `tmp/changepoint-0.2.0-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.whl.zip` & `tmp/changepoint-0.3.0-cp38-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1265652 bytes, number of entries: 5
--rw-r--r--  4.6 unx     2708 b- defN 23-Mar-01 04:06 changepoint-0.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx      128 b- defN 23-Mar-01 04:06 changepoint-0.2.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      135 b- defN 23-Mar-01 04:06 pychangepoint/__init__.py
--rwxr-xr-x  4.6 unx  4433216 b- defN 23-Mar-01 04:06 pychangepoint/pychangepoint.pypy39-pp73-x86-linux-gnu.so
--rw-r--r--  4.6 unx      416 b- defN 23-Mar-01 04:06 changepoint-0.2.0.dist-info/RECORD
-5 files, 4436603 bytes uncompressed, 1264882 bytes compressed:  71.5%
+Zip file size: 278134 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     3029 b- defN 23-Jun-16 02:46 changepoint-0.3.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-16 02:46 changepoint-0.3.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      127 b- defN 23-Jun-16 02:46 changepoint/__init__.py
+-rwxr-xr-x  4.6 unx   652800 b- defN 23-Jun-16 02:46 changepoint/changepoint.cp38-win_amd64.pyd
+-rw-r--r--  4.6 unx      398 b- defN 23-Jun-16 02:46 changepoint-0.3.0.dist-info/RECORD
+5 files, 656450 bytes uncompressed, 277396 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: changepoint-0.2.0.dist-info/METADATA
+Filename: changepoint-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: changepoint-0.2.0.dist-info/WHEEL
+Filename: changepoint-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: pychangepoint/__init__.py
+Filename: changepoint/__init__.py
 Comment: 
 
-Filename: pychangepoint/pychangepoint.pypy39-pp73-x86-linux-gnu.so
+Filename: changepoint/changepoint.cp38-win_amd64.pyd
 Comment: 
 
-Filename: changepoint-0.2.0.dist-info/RECORD
+Filename: changepoint-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `changepoint-0.2.0.dist-info/METADATA` & `changepoint-0.3.0.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,103 @@
 Metadata-Version: 2.1
 Name: changepoint
-Version: 0.2.0
+Version: 0.3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Summary: A Bayesian change point library
 Keywords: changepoint
 Author: Redpoll <info@redpoll.ai>
 Author-email: Redpoll <info@redpoll.ai>
 License: MIT
 Requires-Python: >=3.7, < 4
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/promised-ai/changepoint
 
-# changepoint
-
-Python bindings for important functionality of the rust library [changepoint](https://crates.io/crates/changepoint), a library for doing change point detection for steams of data.
-
-## Installation
-
-Install via pip with
-```bash
-$ python3 -m pip install "changepoint"
-```
-
-__Note__: If there is no binary distribution for your OS, architecture, and Python version, you will need the Rust compiler to build the package and install a Python tool called Maturin:
-```bash
-curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
-python3 -m pip install maturin
-```
-
-See [rustup.rs](https://rustup.rs/) for instructions on installing Rust.
-
-## Quick Docs
-By convention in these docs and examples, 
-```python
-import changepoint as chp
-```
-
-### Models
-#### Bocpd
-
-The Bayesian change point detector, `Bocpd`, takes a prior distribution, aka one of
-```python
-chp.BetaBernoulli
-chp.NormalGamma
-chp.NormalInvChiSquared
-chp.NormalInvGamma
-chp.NormalInvWishart
-chp.PoissonGamma
-```
-
-Then, a `Bocpd` may be created:
-```python
-cpd = chp.Bocpd(
-    prior=chp.NormalGamma(),
-    lam=12,
-)
-```
-where the prior is a `NormalGamma` and the characteristic run length is `12`.
-
-Each step of the data stream, `data`, can be processed by
-```python
-n = len(data)
-change_point_history = np.zeros((n, n))
-for i, x in enumerate(data):
-    change_point_history[i, : i + 1] = cpd.step(x)
-```
-
-
-#### ArgpCpd
-
-`ArgpCpd` has an implicit prior as it is a Gaussian Process of the form `X_{i+1} = c X_{i-l-1, ..., i-1} + ε`
-where `c` is the scale, `X_{i-l-1, ..., i-1}` is the previous vales in the sequence (`l` is the max-lag parameter), and `ε` is a white noise parameter.
-It behaves similarity to the `Bocpd` class; for example,
-
-```python
-argp = chp.ArgpCpd(logistic_hazard_h=-2, scale=3, noise_level=0.01)
-n = len(data)
-change_point_history = np.zeros((n + 1, n + 1))
-xs = []
-ys = []
-for i, x in enumerate(data):
-    cps = argp.step(x)
-    change_point_history[i, : len(cps)] = cps
-```
-
-## Example
-
-An example IPython notebook can be found [here](https://gitlab.com/Redpoll/changepoint/-/blob/master/changepoint-py/ChangePointExample.ipynb).
+# changepoint
+
+Python bindings for important functionality of the rust library [changepoint](https://crates.io/crates/changepoint), a library for doing change point detection for steams of data.
+
+## Installation
+
+Install via pip with
+```bash
+$ python3 -m pip install "changepoint"
+```
+
+__Note__: If there is no binary distribution for your OS, architecture, and Python version, you will need the Rust compiler to build the package and install a Python tool called Maturin:
+```bash
+curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
+python3 -m pip install maturin
+```
+
+See [rustup.rs](https://rustup.rs/) for instructions on installing Rust.
+
+## Quick Docs
+By convention in these docs and examples, 
+```python
+import changepoint as chp
+```
+
+### Models
+#### Bocpd
+
+The Bayesian change point detector, `Bocpd`, takes a prior distribution, aka one of
+```python,ignore
+chp.BetaBernoulli
+chp.NormalGamma
+chp.NormalInvChiSquared
+chp.NormalInvGamma
+chp.NormalInvWishart
+chp.PoissonGamma
+```
+
+Then, a `Bocpd` may be created:
+```python
+cpd = chp.Bocpd(
+    prior=chp.NormalGamma(),
+    lam=12,
+)
+```
+where the prior is a `NormalGamma` and the characteristic run length is `12`.
+
+Each step of the data stream, `data`, can be processed by
+```python
+import random
+import numpy as np
+
+data = [random.gauss() for _ in range(30)] \
+    + [random.gauss(1, 2) for _ in range(30)]
+
+n = len(data)
+change_point_history = np.zeros((n, n))
+for i, x in enumerate(data):
+    change_point_history[i, : i + 1] = cpd.step(x)
+
+print(chp.map_changepoints(change_point_history))
+```
+
+
+#### ArgpCpd
+
+`ArgpCpd` has an implicit prior as it is a Gaussian Process of the form `X_{i+1} = c X_{i-l-1, ..., i-1} + ε`
+where `c` is the scale, `X_{i-l-1, ..., i-1}` is the previous vales in the sequence (`l` is the max-lag parameter), and `ε` is a white noise parameter.
+It behaves similarity to the `Bocpd` class; for example,
+
+```python
+argp = chp.ArgpCpd(logistic_hazard_h=-2, scale=3, noise_level=0.01)
+n = len(data)
+change_point_history = np.zeros((n + 1, n + 1))
+xs = []
+ys = []
+for i, x in enumerate(data):
+    cps = argp.step(x)
+    change_point_history[i, : len(cps)] = cps
+
+print(chp.map_changepoints(change_point_history))
+```
+
+## Example
+
+An example IPython notebook can be found [here](https://gitlab.com/Redpoll/changepoint/-/blob/master/changepoint-py/ChangePointExample.ipynb).
```

