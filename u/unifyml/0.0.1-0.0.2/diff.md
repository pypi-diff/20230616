# Comparing `tmp/unifyml-0.0.1.tar.gz` & `tmp/unifyml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\unifyml-0.0.1.tar", last modified: Sun Jun 11 19:25:00 2023, max compression
+gzip compressed data, was "unifyml-0.0.2.tar", last modified: Fri Jun 16 14:57:10 2023, max compression
```

## Comparing `unifyml-0.0.1.tar` & `unifyml-0.0.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.719773 unifyml-0.0.1/
--rw-rw-rw-   0        0        0      107 2023-06-11 18:52:32.000000 unifyml-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1503 2023-06-11 19:25:00.719773 unifyml-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3193 2023-06-11 13:27:41.000000 unifyml-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-06-11 19:25:00.720773 unifyml-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     7069 2023-06-11 18:59:03.000000 unifyml-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.666725 unifyml-0.0.1/unifyml/
--rw-rw-rw-   0        0        0     1667 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/__init__.py
--rw-rw-rw-   0        0        0     8398 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/_troubleshoot.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.690746 unifyml-0.0.1/unifyml/backend/
--rw-rw-rw-   0        0        0     1106 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/__init__.py
--rw-rw-rw-   0        0        0    66681 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_backend.py
--rw-rw-rw-   0        0        0     6142 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_dtype.py
--rw-rw-rw-   0        0        0    38231 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_linalg.py
--rw-rw-rw-   0        0        0     3101 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_linalg_preconditioner.py
--rw-rw-rw-   0        0        0     9048 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_minimize.py
--rw-rw-rw-   0        0        0    20027 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_numpy_backend.py
--rw-rw-rw-   0        0        0     1296 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_object.py
--rw-rw-rw-   0        0        0    19229 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_partition.py
--rw-rw-rw-   0        0        0    22498 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_profile.py
--rw-rw-rw-   0        0        0      449 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/_triangular_wip.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.692749 unifyml-0.0.1/unifyml/backend/jax/
--rw-rw-rw-   0        0        0      242 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/jax/__init__.py
--rw-rw-rw-   0        0        0    23966 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/jax/_jax_backend.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.694750 unifyml-0.0.1/unifyml/backend/jax/stax/
--rw-rw-rw-   0        0        0        0 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/jax/stax/__init__.py
--rw-rw-rw-   0        0        0    46154 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/jax/stax/nets.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.700756 unifyml-0.0.1/unifyml/backend/tf/
--rw-rw-rw-   0        0        0      954 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/tf/__init__.py
--rw-rw-rw-   0        0        0     4228 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/tf/_compile_cuda.py
--rw-rw-rw-   0        0        0     1950 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/tf/_profiling.py
--rw-rw-rw-   0        0        0    33277 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/tf/_tf_backend.py
--rw-rw-rw-   0        0        0     3280 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/tf/_tf_cuda_resample.py
--rw-rw-rw-   0        0        0    34501 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/tf/nets.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.703759 unifyml-0.0.1/unifyml/backend/torch/
--rw-rw-rw-   0        0        0      264 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/torch/__init__.py
--rw-rw-rw-   0        0        0    59226 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/torch/_torch_backend.py
--rw-rw-rw-   0        0        0    39882 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/backend/torch/nets.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.718771 unifyml-0.0.1/unifyml/math/
--rw-rw-rw-   0        0        0     4877 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/__init__.py
--rw-rw-rw-   0        0        0     3777 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_fit.py
--rw-rw-rw-   0        0        0    56840 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_functional.py
--rw-rw-rw-   0        0        0    37575 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_magic_ops.py
--rw-rw-rw-   0        0        0    32292 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_nd.py
--rw-rw-rw-   0        0        0   125481 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_ops.py
--rw-rw-rw-   0        0        0    42778 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_optimize.py
--rw-rw-rw-   0        0        0    76214 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_shape.py
--rw-rw-rw-   0        0        0    54939 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_sparse.py
--rw-rw-rw-   0        0        0   107641 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_tensors.py
--rw-rw-rw-   0        0        0    18520 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/_trace.py
--rw-rw-rw-   0        0        0    60632 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/extrapolation.py
--rw-rw-rw-   0        0        0    32929 2023-06-11 18:52:32.000000 unifyml-0.0.1/unifyml/math/magic.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:25:00.679736 unifyml-0.0.1/unifyml.egg-info/
--rw-rw-rw-   0        0        0     1503 2023-06-11 19:25:00.000000 unifyml-0.0.1/unifyml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-06-11 19:25:00.000000 unifyml-0.0.1/unifyml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 19:25:00.000000 unifyml-0.0.1/unifyml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-11 19:25:00.000000 unifyml-0.0.1/unifyml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-11 19:25:00.000000 unifyml-0.0.1/unifyml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.539603 unifyml-0.0.2/
+-rw-rw-rw-   0        0        0      111 2023-06-14 08:33:28.000000 unifyml-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4481 2023-06-16 14:57:10.540603 unifyml-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14511 2023-06-16 14:47:41.000000 unifyml-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-16 14:57:10.541605 unifyml-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     6928 2023-06-16 14:52:27.000000 unifyml-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.488558 unifyml-0.0.2/unifyml/
+-rw-rw-rw-   0        0        0        5 2023-06-14 14:39:12.000000 unifyml-0.0.2/unifyml/VERSION
+-rw-rw-rw-   0        0        0     1090 2023-06-14 08:44:57.000000 unifyml-0.0.2/unifyml/__init__.py
+-rw-rw-rw-   0        0        0     8406 2023-06-12 21:40:30.000000 unifyml-0.0.2/unifyml/_troubleshoot.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.514581 unifyml-0.0.2/unifyml/backend/
+-rw-rw-rw-   0        0        0     1140 2023-06-14 08:33:28.000000 unifyml-0.0.2/unifyml/backend/__init__.py
+-rw-rw-rw-   0        0        0    69773 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/_backend.py
+-rw-rw-rw-   0        0        0     6142 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/backend/_dtype.py
+-rw-rw-rw-   0        0        0    38231 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/backend/_linalg.py
+-rw-rw-rw-   0        0        0     3101 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/backend/_linalg_preconditioner.py
+-rw-rw-rw-   0        0        0     9048 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/backend/_minimize.py
+-rw-rw-rw-   0        0        0    20027 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/_numpy_backend.py
+-rw-rw-rw-   0        0        0     1345 2023-06-14 08:33:28.000000 unifyml-0.0.2/unifyml/backend/_object.py
+-rw-rw-rw-   0        0        0    19229 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/backend/_partition.py
+-rw-rw-rw-   0        0        0    22498 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/backend/_profile.py
+-rw-rw-rw-   0        0        0      449 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/backend/_triangular_wip.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.516581 unifyml-0.0.2/unifyml/backend/jax/
+-rw-rw-rw-   0        0        0      163 2023-06-12 21:40:30.000000 unifyml-0.0.2/unifyml/backend/jax/__init__.py
+-rw-rw-rw-   0        0        0    24281 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/jax/_jax_backend.py
+-rw-rw-rw-   0        0        0    40579 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/jax/stax_nets.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.522588 unifyml-0.0.2/unifyml/backend/tensorflow/
+-rw-rw-rw-   0        0        0      909 2023-06-12 21:40:30.000000 unifyml-0.0.2/unifyml/backend/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0     4228 2023-06-12 21:40:30.000000 unifyml-0.0.2/unifyml/backend/tensorflow/_compile_cuda.py
+-rw-rw-rw-   0        0        0     1950 2023-06-12 21:40:30.000000 unifyml-0.0.2/unifyml/backend/tensorflow/_profiling.py
+-rw-rw-rw-   0        0        0    33351 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/tensorflow/_tf_backend.py
+-rw-rw-rw-   0        0        0     3280 2023-06-12 21:40:30.000000 unifyml-0.0.2/unifyml/backend/tensorflow/_tf_cuda_resample.py
+-rw-rw-rw-   0        0        0    24965 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/tensorflow/nets.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.525591 unifyml-0.0.2/unifyml/backend/torch/
+-rw-rw-rw-   0        0        0      224 2023-06-12 21:40:30.000000 unifyml-0.0.2/unifyml/backend/torch/__init__.py
+-rw-rw-rw-   0        0        0    59363 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/torch/_torch_backend.py
+-rw-rw-rw-   0        0        0    29787 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/backend/torch/nets.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.539603 unifyml-0.0.2/unifyml/math/
+-rw-rw-rw-   0        0        0     4809 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/math/__init__.py
+-rw-rw-rw-   0        0        0     3777 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/math/_fit.py
+-rw-rw-rw-   0        0        0    56785 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/math/_functional.py
+-rw-rw-rw-   0        0        0    37575 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/math/_magic_ops.py
+-rw-rw-rw-   0        0        0    32298 2023-06-14 20:31:15.000000 unifyml-0.0.2/unifyml/math/_nd.py
+-rw-rw-rw-   0        0        0   126292 2023-06-16 10:14:59.000000 unifyml-0.0.2/unifyml/math/_ops.py
+-rw-rw-rw-   0        0        0    45293 2023-06-16 11:53:14.000000 unifyml-0.0.2/unifyml/math/_optimize.py
+-rw-rw-rw-   0        0        0    76215 2023-06-14 20:21:24.000000 unifyml-0.0.2/unifyml/math/_shape.py
+-rw-rw-rw-   0        0        0    54939 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/math/_sparse.py
+-rw-rw-rw-   0        0        0   106398 2023-06-14 20:21:24.000000 unifyml-0.0.2/unifyml/math/_tensors.py
+-rw-rw-rw-   0        0        0    18568 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/math/_trace.py
+-rw-rw-rw-   0        0        0    60711 2023-06-14 13:03:12.000000 unifyml-0.0.2/unifyml/math/extrapolation.py
+-rw-rw-rw-   0        0        0    32929 2023-06-11 18:52:32.000000 unifyml-0.0.2/unifyml/math/magic.py
+-rw-rw-rw-   0        0        0    12725 2023-06-16 08:55:17.000000 unifyml-0.0.2/unifyml/nn.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:57:10.503569 unifyml-0.0.2/unifyml.egg-info/
+-rw-rw-rw-   0        0        0     4481 2023-06-16 14:57:10.000000 unifyml-0.0.2/unifyml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1372 2023-06-16 14:57:10.000000 unifyml-0.0.2/unifyml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 14:57:10.000000 unifyml-0.0.2/unifyml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-16 14:57:10.000000 unifyml-0.0.2/unifyml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 14:57:10.000000 unifyml-0.0.2/unifyml.egg-info/top_level.txt
```

### Comparing `unifyml-0.0.1/setup.py` & `unifyml-0.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import distutils.cmd
-import distutils.log
-import subprocess
-import os
-from os.path import join, isfile, abspath, isdir, dirname
-from setuptools import setup
-
-
-def check_tf_cuda_compatibility():
-    import tensorflow
-    build = tensorflow.sysconfig.get_build_info()  # is_rocm_build, cuda_compute_capabilities
-    tf_gcc = build['cpu_compiler']
-    is_cuda_build = build['is_cuda_build']
-    print(f"TensorFlow compiler: {tf_gcc}.")
-    if not is_cuda_build:
-        raise AssertionError("Your TensorFlow build does not support CUDA.")
-    else:
-        cuda_version = build['cuda_version']
-        cudnn_version = build['cudnn_version']
-        print(f"TensorFlow was compiled against CUDA {cuda_version} and cuDNN {cudnn_version}.")
-        return tf_gcc
-
-
-def compile_cuda(file_names, nvcc, source_dir, target_dir, logfile):
-    import tensorflow
-    tf_cflags = tensorflow.sysconfig.get_compile_flags()
-    command = [
-            nvcc,
-            join(source_dir, f'{file_names}.cu.cc'),
-            '-o', join(target_dir, f'{file_names}.cu.o'),
-            '-std=c++11',
-            '-c',
-            '-D GOOGLE_CUDA=1',
-            '-x', 'cu',
-            '-Xcompiler',
-            '-fPIC',
-            '--expt-relaxed-constexpr',
-            '-DNDEBUG',
-            '-O3'
-        ] + tf_cflags
-    print(f"nvcc {file_names}")
-    logfile.writelines(["\n", " ".join(command), "\n"])
-    subprocess.check_call(command, stdout=logfile, stderr=logfile)
-
-
-def compile_gcc(file_names, gcc, source_dir, target_dir, cuda_lib, logfile):
-    import tensorflow
-    from packaging import version
-    if version.parse(tensorflow.__version__) >= version.parse('2.5.0'):
-        cpp_version, gcc_version = '14', '7.5'
-    else:
-        cpp_version, gcc_version = '11', '4.8'
-    tf_cflags = tensorflow.sysconfig.get_compile_flags()
-    tf_lflags = tensorflow.sysconfig.get_link_flags()
-    link_cuda_lib = '-L' + cuda_lib
-    command = [
-                gcc,
-                join(source_dir, f'{file_names}.cc'),
-                join(target_dir, f'{file_names}.cu.o'),
-                '-o', join(target_dir, f'{file_names}.so'),
-                f'-std=c++{cpp_version}',
-                '-shared',
-                '-fPIC',
-                '-lcudart',
-                '-O3',
-                link_cuda_lib
-            ] + tf_cflags + tf_lflags
-    print(f"gcc {file_names}")
-    logfile.writelines(["\n", " ".join(command), "\n"])
-    subprocess.check_call(command, stdout=logfile, stderr=logfile)
-
-
-class CudaCommand(distutils.cmd.Command):
-    description = 'Compile CUDA sources'
-    user_options = [
-        ('gcc=', None, 'Path to the gcc compiler.'),
-        ('nvcc=', None, 'Path to the Nvidia nvcc compiler.'),
-        ('cuda-lib=', None, 'Path to the CUDA libraries.'),
-    ]
-
-    def initialize_options(self):
-        tf_gcc = check_tf_cuda_compatibility()
-        self.gcc = tf_gcc if isfile(tf_gcc) else 'gcc'
-        self.nvcc = '/usr/local/cuda/bin/nvcc' if isfile('/usr/local/cuda/bin/nvcc') else 'nvcc'
-        self.cuda_lib = '/usr/local/cuda/lib64/'
-
-    def finalize_options(self) -> None:
-        pass
-
-    def run(self):
-        src_path = abspath('./unifyml/tf/cuda/src')
-        build_path = abspath('./unifyml/tf/cuda/build')
-        logfile_path = abspath('./unifyml/tf/cuda/log.txt')
-        print("Source Path:\t" + src_path)
-        print("Build Path:\t" + build_path)
-        print("GCC:\t\t" + self.gcc)
-        print("NVCC:\t\t" + self.nvcc)
-        print("CUDA lib:\t" + self.cuda_lib)
-        print("----------------------------")
-        # Remove old build files
-        if isdir(build_path):
-            print('Removing old build files from %s' % build_path)
-            for file in os.listdir(build_path):
-                os.remove(join(build_path, file))
-        else:
-            print('Creating build directory at %s' % build_path)
-            os.mkdir(build_path)
-        print('Compiling CUDA code...')
-        with open(logfile_path, "w") as logfile:
-            try:
-                compile_cuda('resample', self.nvcc, src_path, build_path, logfile=logfile)
-                compile_gcc('resample', self.gcc, src_path, build_path, self.cuda_lib, logfile=logfile)
-                compile_cuda('resample_gradient', self.nvcc, src_path, build_path, logfile=logfile)
-                compile_gcc('resample_gradient', self.gcc, src_path, build_path, self.cuda_lib, logfile=logfile)
-                # compile_cuda('bicgstab_ilu_linear_solve_op', self.nvcc, src_path, build_path, logfile=logfile)
-                # compile_gcc('bicgstab_ilu_linear_solve_op', self.gcc, src_path, build_path, self.cuda_lib, logfile=logfile)
-            except BaseException as err:
-                print(f"Compilation failed. See {logfile_path} for details.")
-                raise err
-        print(f"Compilation complete. See {logfile_path} for details.")
-
-
-try:
-    with open(join(dirname(__file__), 'docs/Package_Info.md'), 'r') as readme:
-        long_description = readme.read()
-except FileNotFoundError:
-    long_description = ""
-    pass
-
-with open(join(dirname(__file__), 'unifyml', 'VERSION'), 'r') as version_file:
-    version = version_file.read()
-
-setup(
-    name='unifyml',
-    version=version,
-    download_url='https://github.com/holl-/UnifyML/archive/%s.tar.gz' % version,
-    packages=['unifyml',
-              'unifyml.math',
-              'unifyml.backend',
-              'unifyml.backend.jax',
-              'unifyml.backend.jax.stax',
-              'unifyml.backend.tf',
-              'unifyml.backend.torch',
-          ],
-    cmdclass={
-        'tf_cuda': CudaCommand,
-    },
-    description='Unified API for machine learning',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    keywords=['Machine Learning', 'Deep Learning', 'Math', 'Linear systems', 'Sparse', 'Tensor', 'Named dimensions'],
-    license='MIT',
-    author='Philipp Holl',
-    author_email='philipp.holl@tum.de',
-    url='https://github.com/holl-/UnifyML',
-    include_package_data=True,
-    install_requires=[
-        'numpy',  # 1.20 causes TensorFlow tracing errors: NotImplementedError: Cannot convert a symbolic Tensor to a numpy array.
-        'scipy>=1.5.4',
-        'packaging',
-    ],
-    # Optional packages:
-    # - torch
-    # - tensorflow
-    # - jax
-    #
-    # unifyml.verify() should detect missing packages.
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-)
+import distutils.cmd
+import distutils.log
+import subprocess
+import os
+from os.path import join, isfile, abspath, isdir, dirname
+from setuptools import setup
+
+
+def check_tf_cuda_compatibility():
+    import tensorflow
+    build = tensorflow.sysconfig.get_build_info()  # is_rocm_build, cuda_compute_capabilities
+    tf_gcc = build['cpu_compiler']
+    is_cuda_build = build['is_cuda_build']
+    print(f"TensorFlow compiler: {tf_gcc}.")
+    if not is_cuda_build:
+        raise AssertionError("Your TensorFlow build does not support CUDA.")
+    else:
+        cuda_version = build['cuda_version']
+        cudnn_version = build['cudnn_version']
+        print(f"TensorFlow was compiled against CUDA {cuda_version} and cuDNN {cudnn_version}.")
+        return tf_gcc
+
+
+def compile_cuda(file_names, nvcc, source_dir, target_dir, logfile):
+    import tensorflow
+    tf_cflags = tensorflow.sysconfig.get_compile_flags()
+    command = [
+            nvcc,
+            join(source_dir, f'{file_names}.cu.cc'),
+            '-o', join(target_dir, f'{file_names}.cu.o'),
+            '-std=c++11',
+            '-c',
+            '-D GOOGLE_CUDA=1',
+            '-x', 'cu',
+            '-Xcompiler',
+            '-fPIC',
+            '--expt-relaxed-constexpr',
+            '-DNDEBUG',
+            '-O3'
+        ] + tf_cflags
+    print(f"nvcc {file_names}")
+    logfile.writelines(["\n", " ".join(command), "\n"])
+    subprocess.check_call(command, stdout=logfile, stderr=logfile)
+
+
+def compile_gcc(file_names, gcc, source_dir, target_dir, cuda_lib, logfile):
+    import tensorflow
+    from packaging import version
+    if version.parse(tensorflow.__version__) >= version.parse('2.5.0'):
+        cpp_version, gcc_version = '14', '7.5'
+    else:
+        cpp_version, gcc_version = '11', '4.8'
+    tf_cflags = tensorflow.sysconfig.get_compile_flags()
+    tf_lflags = tensorflow.sysconfig.get_link_flags()
+    link_cuda_lib = '-L' + cuda_lib
+    command = [
+                gcc,
+                join(source_dir, f'{file_names}.cc'),
+                join(target_dir, f'{file_names}.cu.o'),
+                '-o', join(target_dir, f'{file_names}.so'),
+                f'-std=c++{cpp_version}',
+                '-shared',
+                '-fPIC',
+                '-lcudart',
+                '-O3',
+                link_cuda_lib
+            ] + tf_cflags + tf_lflags
+    print(f"gcc {file_names}")
+    logfile.writelines(["\n", " ".join(command), "\n"])
+    subprocess.check_call(command, stdout=logfile, stderr=logfile)
+
+
+class CudaCommand(distutils.cmd.Command):
+    description = 'Compile CUDA sources'
+    user_options = [
+        ('gcc=', None, 'Path to the gcc compiler.'),
+        ('nvcc=', None, 'Path to the Nvidia nvcc compiler.'),
+        ('cuda-lib=', None, 'Path to the CUDA libraries.'),
+    ]
+
+    def initialize_options(self):
+        tf_gcc = check_tf_cuda_compatibility()
+        self.gcc = tf_gcc if isfile(tf_gcc) else 'gcc'
+        self.nvcc = '/usr/local/cuda/bin/nvcc' if isfile('/usr/local/cuda/bin/nvcc') else 'nvcc'
+        self.cuda_lib = '/usr/local/cuda/lib64/'
+
+    def finalize_options(self) -> None:
+        pass
+
+    def run(self):
+        src_path = abspath('./unifyml/tf/cuda/src')
+        build_path = abspath('./unifyml/tf/cuda/build')
+        logfile_path = abspath('./unifyml/tf/cuda/log.txt')
+        print("Source Path:\t" + src_path)
+        print("Build Path:\t" + build_path)
+        print("GCC:\t\t" + self.gcc)
+        print("NVCC:\t\t" + self.nvcc)
+        print("CUDA lib:\t" + self.cuda_lib)
+        print("----------------------------")
+        # Remove old build files
+        if isdir(build_path):
+            print('Removing old build files from %s' % build_path)
+            for file in os.listdir(build_path):
+                os.remove(join(build_path, file))
+        else:
+            print('Creating build directory at %s' % build_path)
+            os.mkdir(build_path)
+        print('Compiling CUDA code...')
+        with open(logfile_path, "w") as logfile:
+            try:
+                compile_cuda('resample', self.nvcc, src_path, build_path, logfile=logfile)
+                compile_gcc('resample', self.gcc, src_path, build_path, self.cuda_lib, logfile=logfile)
+                compile_cuda('resample_gradient', self.nvcc, src_path, build_path, logfile=logfile)
+                compile_gcc('resample_gradient', self.gcc, src_path, build_path, self.cuda_lib, logfile=logfile)
+                # compile_cuda('bicgstab_ilu_linear_solve_op', self.nvcc, src_path, build_path, logfile=logfile)
+                # compile_gcc('bicgstab_ilu_linear_solve_op', self.gcc, src_path, build_path, self.cuda_lib, logfile=logfile)
+            except BaseException as err:
+                print(f"Compilation failed. See {logfile_path} for details.")
+                raise err
+        print(f"Compilation complete. See {logfile_path} for details.")
+
+
+try:
+    with open(join(dirname(__file__), 'docs/Package_Info.md'), mode='r', encoding='utf-8') as readme:
+        long_description = readme.read()
+except FileNotFoundError:
+    long_description = ""
+    pass
+
+with open(join(dirname(__file__), 'unifyml', 'VERSION'), 'r') as version_file:
+    version = version_file.read()
+
+setup(
+    name='unifyml',
+    version=version,
+    download_url='https://github.com/holl-/UnifyML/archive/%s.tar.gz' % version,
+    packages=['unifyml',
+              'unifyml.math',
+              'unifyml.backend',
+              'unifyml.backend.jax',
+              'unifyml.backend.torch',
+              'unifyml.backend.tensorflow',
+          ],
+    cmdclass={
+        'tf_cuda': CudaCommand,
+    },
+    description='Unified API for machine learning',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    keywords=['Machine Learning', 'Deep Learning', 'Math', 'Linear systems', 'Sparse', 'Tensor', 'Named dimensions'],
+    license='MIT',
+    author='Philipp Holl',
+    author_email='philipp.holl@tum.de',
+    url='https://github.com/holl-/UnifyML',
+    include_package_data=True,
+    install_requires=[
+        'numpy',  # 1.20 causes TensorFlow tracing errors: NotImplementedError: Cannot convert a symbolic Tensor to a numpy array.
+        'scipy>=1.5.4',
+        'packaging',
+    ],
+    # Optional packages:
+    # - torch
+    # - tensorflow
+    # - jax
+    #
+    # unifyml.verify() should detect missing packages.
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+)
```

### Comparing `unifyml-0.0.1/unifyml/_troubleshoot.py` & `unifyml-0.0.2/unifyml/_troubleshoot.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             math.assert_close(math.ones() + math.ones(), 2)
             # TODO cuDNN math.convolve(math.ones(batch=8, x=64), math.ones(x=4))
         except BaseException as err:
             return f"Installed ({tf_version}) but tests failed with error: {err}"
     if gpu_count == 0:
         return f"Installed ({tf_version}), {gpu_count} GPUs available."
     else:
-        from .backend.tf._tf_cuda_resample import librariesLoaded
+        from .backend.tensorflow._tf_cuda_resample import librariesLoaded
         if librariesLoaded:
             cuda_str = 'CUDA kernels available.'
         else:
             import platform
             if platform.system().lower() != 'linux':
                 cuda_str = f"Optional TensorFlow CUDA kernels not available and compilation not recommended on {platform.system()}. GPU will be used nevertheless."
             else:
```

### Comparing `unifyml-0.0.1/unifyml/backend/__init__.py` & `unifyml-0.0.2/unifyml/backend/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     NUMPY = _NumPyBackend()
     """Default backend for NumPy arrays and SciPy objects."""
     BACKENDS.append(NUMPY)
     _DEFAULT.append(NUMPY)
 
 from ._object import ObjectBackend as _ObjectBackend
 OBJECTS = _ObjectBackend()
+"""Backend for Python objects."""
 BACKENDS.append(OBJECTS)
 
 __all__ = [key for key in globals().keys() if not key.startswith('_')]
 
 __pdoc__ = {
     'ComputeDevice.__init__': False,
     'NoBackendFound.__init__': False,
```

### Comparing `unifyml-0.0.1/unifyml/backend/_backend.py` & `unifyml-0.0.2/unifyml/backend/_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import sys
 import warnings
+from builtins import ValueError
 from contextlib import contextmanager
 from dataclasses import dataclass
+from types import ModuleType
 from typing import List, Callable, TypeVar, Tuple, Union, Optional
 
 import numpy
 import numpy as np
 from numpy import ndarray
 
 from ._dtype import DType, combine_types
@@ -77,23 +79,23 @@
         return isinstance(other, ComputeDevice) and other.ref == self.ref
 
     def __hash__(self):
         return hash(self.ref)
 
 
 class Backend:
+    """
+    Backends delegate low-level operations to a ML or numerics library or emulate them.
+    The methods of `Backend` form a comprehensive list of available operations.
+
+    To support a library, subclass `Backend` and register it by adding it to `BACKENDS`.
+    """
 
     def __init__(self, name: str, devices: List[ComputeDevice], default_device: ComputeDevice):
         """
-        Backends delegate low-level operations to a compute library or emulate them.
-
-        The methods of `Backend` form a comprehensive list of available operations.
-
-        To support a compute library, subclass `Backend` and register it by adding it to `BACKENDS`.
-
         Args:
             name: Human-readable string
             default_device: `ComputeDevice` being used by default
         """
         self._name = name
         self._devices = tuple(devices)
         self._default_device = default_device
@@ -150,14 +152,17 @@
     def as_registered(self) -> 'Backend':
         from . import BACKENDS
         for backend in BACKENDS:
             if self.name in backend.name:
                 return backend
         raise RuntimeError(f"Backend '{self}' is not visible.")
 
+    def nn_library(self):
+        raise NotImplementedError(self)
+
     @property
     def complex_type(self) -> DType:
         return DType(complex, max(64, self.precision))
 
     def combine_types(self, *dtypes: DType) -> DType:
         return combine_types(*dtypes, fp_precision=self.precision)
 
@@ -1555,15 +1560,15 @@
         return a << b
 
     def shift_bits_right(self, a, b):
         a, b = self.auto_cast(a, b)
         return a >> b
 
 
-BACKENDS = []
+BACKENDS: List[Backend] = []
 """ Global list of all registered backends. Register a `Backend` by adding it to the list. """
 _DEFAULT = []  # [0] = global default, [1:] from 'with' blocks
 _PRECISION = [32]  # [0] = global precision in bits, [1:] from 'with' blocks
 
 
 def choose_backend(*values, prefer_default=False) -> Backend:
     """
@@ -1582,15 +1587,23 @@
     """
     # --- Default Backend has priority ---
     if _is_applicable(_DEFAULT[-1], values) and (prefer_default or _is_specific(_DEFAULT[-1], values)):
         return _DEFAULT[-1]
     # --- Filter out non-applicable ---
     backends = [backend for backend in BACKENDS if _is_applicable(backend, values)]
     if len(backends) == 0:
-        raise NoBackendFound(f"No backend found for types {[type(v).__name__ for v in values]}; registered backends are {BACKENDS}")
+        unknown_values = [v for v in values if all([not _is_applicable(b, [v]) for b in BACKENDS])]
+        if unknown_values:
+            module_name = type(unknown_values[0]).__module__.partition('.')[0]
+            if init_backend(module_name):
+                return choose_backend(*values, prefer_default)
+            else:
+                raise NoBackendFound(f"Not a native tensor {[type(v).__name__ for v in unknown_values]}")
+        else:
+            raise NoBackendFound(f"Could not resolve backend for native types {[type(v).__name__ for v in values]}")
     # --- Native tensors? ---
     for backend in backends:
         if _is_specific(backend, values):
             return backend
     return backends[0]
 
 
@@ -1599,14 +1612,79 @@
     Thrown by `choose_backend` if no backend can handle the given values.
     """
 
     def __init__(self, msg):
         Exception.__init__(self, msg)
 
 
+def init_installed_backends() -> tuple:
+    """
+    Registers all available backends.
+    This includes only backends for which the minimal requirements are fulfilled.
+
+    Returns:
+        All installed tensor backends as `tuple[Backend]`
+    """
+    try:
+        init_backend('jax')
+    except ImportError:
+        pass
+    try:
+        init_backend('torch')
+    except ImportError:
+        pass
+    try:
+        init_backend('tensorflow')
+    except ImportError:
+        pass
+    return tuple([b for b in BACKENDS if b.name != 'Python'])
+
+
+def init_backend(backend: str):
+    """
+    Args:
+        backend: Module name of the backend or backends as comma-separated string.
+            Pass `'all-imported'` to initialize all backends that are loaded into `sys.modules´.
+    """
+    result = []
+    if backend == 'all-imported':
+        backends = tuple(sys.modules)
+    else:
+        backends = [s.strip() for s in backend.split(',')]
+    if ('jax' in backends or 'jaxlib' in backends) and not is_initialized('jax'):
+        ML_LOGGER.info("Initializing backend 'jax'")
+        from .jax import JAX
+        BACKENDS.append(JAX)
+        result.append(JAX)
+    if 'tensorflow' in backends and not is_initialized('tensorflow'):
+        ML_LOGGER.info("Initializing backend 'tensorflow'")
+        from .tensorflow import TENSORFLOW
+        BACKENDS.append(TENSORFLOW)
+        result.append(TENSORFLOW)
+    if 'torch' in backends and not is_initialized('torch'):
+        ML_LOGGER.info("Initializing backend 'torch'")
+        from .torch import TORCH
+        BACKENDS.append(TORCH)
+        result.append(TORCH)
+    return result
+
+
+def is_initialized(backend: str) -> bool:
+    """
+    Checks whether a specific backend has been successfully initialized and can be used from UnifyML.
+
+    Args:
+        backend: Backend name, such as `'jax'`, `'tensorflow'`, `'torch'` or `'numpy'`.
+
+    Returns:
+        `bool`
+    """
+    return any(b.name == backend for b in BACKENDS)
+
+
 def default_backend() -> Backend:
     """
     The default backend is preferred by `choose_backend()`.
 
     The default backend can be set globally using `set_global_default_backend()` and locally using `with backend:`.
 
     Returns:
@@ -1622,26 +1700,37 @@
 
     Returns:
         `Backend` or `None`
     """
     return _DEFAULT[-1] if len(_DEFAULT) > 1 else None
 
 
-def set_global_default_backend(backend: Backend):
+def set_global_default_backend(backend: Union[str, Backend]):
     """
     Sets the given backend as default.
     This setting can be overridden using `with backend:`.
 
     See `default_backend()`, `choose_backend()`.
 
     Args:
-        backend: `Backend` to set as default
+        backend: `Backend` or backend name to set as default.
+            Possible names are `'torch'`, `'tensorflow'`, `'jax'`, `'numpy'`.
     """
-    assert isinstance(backend, Backend)
-    _DEFAULT[0] = backend
+    if isinstance(backend, ModuleType):
+        backend = str(backend)
+    if isinstance(backend, str):
+        init_backend(backend)
+        matches = [b for b in BACKENDS if b.name == backend.lower()]
+        if not matches:
+            raise ValueError(f"Illegal backend: '{backend}'")
+        backend = matches[0]
+    assert isinstance(backend, Backend), backend
+    if _DEFAULT[0] is not backend:
+        _DEFAULT[0] = backend
+        ML_LOGGER.info(f"UnifyML's default backend is now {backend}")
 
 
 def set_global_precision(floating_point_bits: int):
     """
     Sets the floating point precision of DYNAMIC_BACKEND which affects all registered backends.
 
     If `floating_point_bits` is an integer, all floating point tensors created henceforth will be of the corresponding data type, float16, float32 or float64.
```

### Comparing `unifyml-0.0.1/unifyml/backend/_dtype.py` & `unifyml-0.0.2/unifyml/backend/_dtype.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/_linalg.py` & `unifyml-0.0.2/unifyml/backend/_linalg.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/_linalg_preconditioner.py` & `unifyml-0.0.2/unifyml/backend/_linalg_preconditioner.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/_minimize.py` & `unifyml-0.0.2/unifyml/backend/_minimize.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/_numpy_backend.py` & `unifyml-0.0.2/unifyml/backend/_numpy_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self):
         if sys.platform != "win32" and sys.platform != "darwin":
             mem_bytes = os.sysconf('SC_PAGE_SIZE') * os.sysconf('SC_PHYS_PAGES')
         else:
             mem_bytes = -1
         processors = os.cpu_count()
         cpu = ComputeDevice(self, "CPU", 'CPU', mem_bytes, processors, "", 'CPU')
-        Backend.__init__(self, "NumPy", [cpu], cpu)
+        Backend.__init__(self, "numpy", [cpu], cpu)
 
     def prefers_channels_last(self) -> bool:
         return True
 
     seed = np.random.seed
     clip = staticmethod(np.clip)
     minimum = np.minimum
```

### Comparing `unifyml-0.0.1/unifyml/backend/_object.py` & `unifyml-0.0.2/unifyml/backend/_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import random
 
 from ._backend import Backend, ComputeDevice
 from ._dtype import DType
 
 
 class ObjectBackend(Backend):
+    """
+    Backend for Python objects.
+    """
+
     def __init__(self):
         device = ComputeDevice(self, 'Python', 'CPU', -1, 1, "", None)
         super().__init__('Python', [device], device)
 
     def is_tensor(self, x, only_native=False):
         return isinstance(x, str)
```

### Comparing `unifyml-0.0.1/unifyml/backend/_partition.py` & `unifyml-0.0.2/unifyml/backend/_partition.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/_profile.py` & `unifyml-0.0.2/unifyml/backend/_profile.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/jax/_jax_backend.py` & `unifyml-0.0.2/unifyml/backend/jax/_jax_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import numbers
 import warnings
 from functools import wraps, partial
 from typing import List, Callable, Tuple, Union, Optional
-from packaging import version
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as scipy
 import numpy as np
 from jax import random
 from jax.core import Tracer
+from packaging import version
 
 if version.parse(jax.__version__) >= version.parse('0.2.20'):
     from jax.experimental.sparse import BCOO, COO, CSR, CSC
 
 from .._dtype import DType, to_numpy_dtype, from_numpy_dtype
-from .._backend import Backend, ComputeDevice, combined_dim, SolveResult, ML_LOGGER, TensorType
+from .._backend import Backend, ComputeDevice, combined_dim, ML_LOGGER, TensorType
 
 
 from jax.config import config
 config.update("jax_enable_x64", True)
 
 
 class JaxBackend(Backend):
@@ -28,27 +28,31 @@
         devices = []
         for device_type in ['cpu', 'gpu', 'tpu']:
             try:
                 for jax_dev in jax.devices(device_type):
                     devices.append(ComputeDevice(self, device_type.upper(), jax_dev.platform.upper(), -1, -1, f"id={jax_dev.id}", jax_dev))
             except RuntimeError as err:
                 pass  # this is just Jax not finding anything. jaxlib.xla_client._get_local_backends() could help but isn't currently available on GitHub actions
-        Backend.__init__(self, "Jax", devices, devices[-1])
+        Backend.__init__(self, 'jax', devices, devices[-1])
         try:
             self.rnd_key = jax.random.PRNGKey(seed=0)
         except RuntimeError as err:
             warnings.warn(f"{err}", RuntimeWarning)
             self.rnd_key = None
 
     def prefers_channels_last(self) -> bool:
         return True
 
     def requires_fixed_shapes_when_tracing(self) -> bool:
         return True
 
+    def nn_library(self):
+        from . import stax_nets
+        return stax_nets
+
     def _check_float64(self):
         if self.precision == 64:
             if not jax.config.read('jax_enable_x64'):
                 jax.config.update('jax_enable_x64', True)
             assert jax.config.read('jax_enable_x64'), "FP64 is disabled for Jax."
 
     def seed(self, seed: int):
@@ -216,15 +220,20 @@
                 return (*output_tuple, *grads)
             return unwrap_outputs
         else:
             @wraps(f)
             def nonaux_f(*args):
                 loss, output = f(*args)
                 return loss
-            return jax.grad(nonaux_f, argnums=wrt, has_aux=False)
+            jax_grad = jax.grad(nonaux_f, argnums=wrt, has_aux=False)
+            @wraps(f)
+            def call_jax_grad(*args):
+                args = [self.to_float(arg) if self.dtype(arg).kind in (bool, int) else arg for arg in args]
+                return jax_grad(*args)
+            return call_jax_grad
 
     def custom_gradient(self, f: Callable, gradient: Callable, get_external_cache: Callable = None, on_call_skipped: Callable = None) -> Callable:
         jax_fun = jax.custom_vjp(f)  # custom vector-Jacobian product (reverse-mode differentiation)
 
         def forward(*x):
             y = f(*x)
             return y, (x, y)
```

### Comparing `unifyml-0.0.1/unifyml/backend/jax/stax/nets.py` & `unifyml-0.0.2/unifyml/backend/jax/stax_nets.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 else:
     from jax.experimental import stax
     import jax.experimental.optimizers as optim
     from jax.experimental.optimizers import OptimizerState
 
     warnings.warn(f"Found Jax version {jax.__version__}. Using legacy imports.", FutureWarning)
 
-from .... import math
-from .. import JAX
-from ....math._functional import JitFunction
+from ... import math
+from . import JAX
+from ...math._functional import JitFunction
 
 
 class StaxNet:
 
     def __init__(self, initialize: Callable, apply: Callable, input_shape: tuple):
         self._initialize = initialize
         self._apply = apply
@@ -82,15 +82,15 @@
                 def loss_depending_on_net(params_tracer: tuple, *args, **kwargs):
                     net._tracers = params_tracer
                     loss_function_non_jit = loss_function.f if isinstance(loss_function, JitFunction) else loss_function
                     result = loss_function_non_jit(*args, **kwargs)
                     net._tracers = None
                     return result
 
-                gradient_function = math.functional_gradient(loss_depending_on_net)
+                gradient_function = math.gradient(loss_depending_on_net)
                 current_state = OptimizerState(packed_current_state, self._state.tree_def, self._state.subtree_defs)
                 current_params = self._get_params(current_state)
                 value, grads = gradient_function(current_params, *loss_args, **loss_kwargs)
                 next_state = self._update(self._step_i, grads[0], self._state)
                 return next_state.packed_state, value
 
             if isinstance(loss_function, JitFunction):
@@ -99,27 +99,14 @@
 
         next_packed_state, loss_output = self._update_function_cache[loss_function](self._state.packed_state,
                                                                                     *loss_args, **loss_kwargs)
         self._state = OptimizerState(next_packed_state, self._state.tree_def, self._state.subtree_defs)
         return loss_output
 
 
-def parameter_count(model: StaxNet) -> int:
-    """
-    Counts the number of parameters in a model.
-
-    Args:
-        model: Stax model
-
-    Returns:
-        `int`
-    """
-    return int(_recursive_count_parameters(model.parameters))
-
-
 def _recursive_to_float32(obj):
     if isinstance(obj, (tuple, list)):
         return type(obj)([_recursive_to_float32(i) for i in obj])
     elif isinstance(obj, dict):
         return {k: _recursive_to_float32(v) for k, v in obj.items()}
     else:
         assert isinstance(obj, jax.numpy.ndarray)
@@ -170,138 +157,84 @@
                 uml_tensor = math.wrap(param, math.channel('x,y,z,input,output'))
             else:
                 raise NotImplementedError(rank)
             result[name] = uml_tensor
 
 
 def save_state(obj: Union[StaxNet, JaxOptimizer], path: str):
-    """
-    Write the state of a module or optimizer to a file.
-
-    See Also:
-        `load_state()`
-
-    Args:
-        obj: `torch.nn.Module or torch.optim.Optimizer`
-        path: File path as `str`.
-    """
     if not path.endswith('.npy'):
         path += '.npy'
     if isinstance(obj, StaxNet):
         numpy.save(path, obj.parameters)
     else:
         raise NotImplementedError  # ToDo
         # numpy.save(path, obj._state)
 
 
 def load_state(obj: Union[StaxNet, JaxOptimizer], path: str):
-    """
-    Read the state of a module or optimizer from a file.
-
-    See Also:
-        `save_state()`
-
-    Args:
-        obj: `torch.nn.Module or torch.optim.Optimizer`
-        path: File path as `str`.
-    """
     if not path.endswith('.npy'):
         path += '.npy'
     if isinstance(obj, StaxNet):
         state = numpy.load(path, allow_pickle=True)
         obj.parameters = tuple([tuple(layer) for layer in state])
     else:
         raise NotImplementedError  # ToDo
 
 
 def update_weights(net: StaxNet, optimizer: JaxOptimizer, loss_function: Callable, *loss_args, **loss_kwargs):
-    """
-    Computes the gradients of `loss_function` w.r.t. the parameters of `net` and updates its weights using `optimizer`.
-
-    This is the Jax version. Analogue functions exist for other learning frameworks.
-
-    Args:
-        net: Learning model.
-        optimizer: Optimizer.
-        loss_function: Loss function, called as `loss_function(*loss_args, **loss_kwargs)`.
-        *loss_args: Arguments given to `loss_function`.
-        **loss_kwargs: Keyword arguments given to `loss_function`.
-
-    Returns:
-        Output of `loss_function`.
-    """
     loss_output = optimizer.update(net, loss_function, net.parameters, loss_args, loss_kwargs)
     net.parameters = optimizer.get_network_parameters()
     return loss_output
 
 
 def adam(net: StaxNet, learning_rate: float = 1e-3, betas=(0.9, 0.999), epsilon=1e-07):
-    """
-    Creates an Adam optimizer for `net`, alias for [`jax.example_libraries.optimizers.adam`](https://jax.readthedocs.io/en/latest/jax.example_libraries.optimizers.html).
-    Analogous functions exist for other learning frameworks.
-    """
     opt = JaxOptimizer(*optim.adam(learning_rate, betas[0], betas[1], epsilon))
     opt.initialize(net.parameters)
     return opt
 
 
 def sgd(net: StaxNet, learning_rate: float = 1e-3, momentum=0, dampening=0, weight_decay=0, nesterov=False):
-    """
-    Creates an SGD optimizer for `net`, alias for [`jax.example_libraries.optimizers.SGD`](https://jax.readthedocs.io/en/latest/jax.example_libraries.optimizers.html).
-    Analogous functions exist for other learning frameworks.
-    """
+    assert dampening == 0
+    assert weight_decay == 0
+    assert not nesterov
     if momentum == 0:
         opt = JaxOptimizer(*optim.sgd(learning_rate))
     else:
         opt = JaxOptimizer(*optim.momentum(learning_rate, momentum))
     opt.initialize(net.parameters)
     return opt
 
 
 def adagrad(net: StaxNet, learning_rate: float = 1e-3, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
-    """
-    Creates an Adagrad optimizer for `net`, alias for [`jax.example_libraries.optimizers.adagrad`](https://jax.readthedocs.io/en/latest/jax.example_libraries.optimizers.html).
-    Analogue functions exist for other learning frameworks.
-    """
+    assert lr_decay == 0
+    assert weight_decay == 0
+    assert initial_accumulator_value == 0
+    assert eps == 1e-10
     opt = JaxOptimizer(*optim.adagrad(learning_rate))
     opt.initialize(net.parameters)
     return opt
 
 
 def rmsprop(net: StaxNet, learning_rate: float = 1e-3, alpha=0.99, eps=1e-08, weight_decay=0, momentum=0, centered=False):
-    """
-    Creates an RMSprop optimizer for `net`, alias for [`jax.example_libraries.optimizers.rmsprop`](https://jax.readthedocs.io/en/latest/jax.example_libraries.optimizers.html).
-    Analogue functions exist for other learning frameworks.
-    """
+    assert weight_decay == 0
+    assert not centered
     if momentum == 0:
         opt = JaxOptimizer(*optim.rmsprop(learning_rate, alpha, eps))
     else:
         opt = JaxOptimizer(*optim.rmsprop_momentum(learning_rate, alpha, eps, momentum))
     opt.initialize(net.parameters)
     return opt
 
 
-def dense_net(in_channels: int,
+def mlp(in_channels: int,
               out_channels: int,
               layers: Sequence[int],
               batch_norm=False,
               activation='ReLU',
               softmax=False) -> StaxNet:
-    """
-    Fully-connected neural networks are available in ΦFlow via dense_net().
-    Arguments:
-        in_channels : size of input layer, int
-        out_channels = size of output layer, int
-        layers : tuple of linear layers between input and output neurons, list or tuple
-        activation : activation function used within the layers, string
-        batch_norm : use of batch norm after each linear layer, bool
-
-    Returns:
-        Dense net model as specified by input arguments
-    """
     activation = {'ReLU': stax.Relu, 'Sigmoid': stax.Sigmoid, 'tanh': stax.Tanh}[activation]
     stax_layers = []
     for neuron_count in layers:
         stax_layers.append(stax.Dense(neuron_count))
         stax_layers.append(activation)
         if batch_norm:
             stax_layers.append(stax.BatchNorm(axis=(0,)))
@@ -319,33 +252,14 @@
           levels: int = 4,
           filters: Union[int, tuple, list] = 16,
           batch_norm: bool = True,
           activation='ReLU',
           in_spatial: Union[tuple, int] = 2,
           periodic=False,
           use_res_blocks: bool = False) -> StaxNet:
-    """
-     ΦFlow provides a built-in U-net architecture, classically popular for Semantic Segmentation in Computer Vision, composed of downsampling and upsampling layers.
-
-     Arguments:
-
-         in_channels: input channels of the feature map, dtype : int
-         out_channels : output channels of the feature map, dtype : int
-         levels : number of levels of down-sampling and upsampling, dtype : int
-         filters : filter sizes at each down/up sampling convolutional layer, if the input is integer all conv layers have the same filter size,
-         dtype : int or tuple
-         activation : activation function used within the layers, dtype : string
-         batch_norm : use of batchnorm after each conv layer, dtype : bool
-         in_spatial : spatial dimensions of the input feature map, dtype : int
-         use_res_blocks : use convolutional blocks with skip connections instead of regular convolutional blocks, dtype : bool
-
-     Returns:
-
-         U-net model as specified by input arguments
-     """
     if isinstance(filters, (tuple, list)):
         assert len(filters) == levels, f"List of filters has length {len(filters)} but u-net has {levels} levels."
     else:
         filters = (filters,) * levels
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     if isinstance(in_spatial, int):
         d = in_spatial
@@ -408,30 +322,17 @@
     return net
 
 
 ACTIVATIONS = {'ReLU': stax.Relu, 'Sigmoid': stax.Sigmoid, 'tanh': stax.Tanh, 'SiLU': stax.Selu}
 CONV = [None,
         functools.partial(stax.GeneralConv, ('NWC', 'WIO', 'NWC')),
         functools.partial(stax.GeneralConv, ('NWHC', 'WHIO', 'NWHC')),
-        functools.partial(stax.GeneralConv, ('NWHDC', 'WHDIO', 'NWHDC')), ]
-
-'''
-def create_double_conv(d: int, out_channels: int, mid_channels: int, batch_norm: bool, activation: Callable):
-    
-    return stax.serial(
-        CONV[d](out_channels, (3,) * d, padding='same'),
-        stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
-        activation,
-        CONV[d](out_channels, (3,) * d, padding='same'),
-        stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
-        activation)
-'''
+        functools.partial(stax.GeneralConv, ('NWHDC', 'WHDIO', 'NWHDC'))]
 
 
-# Periodic Implementation
 def create_double_conv(d: int, out_channels: int, mid_channels: int, batch_norm: bool, activation: Callable, periodic: bool):
     init_fn, apply_fn = {}, {}
     init_fn['conv1'], apply_fn['conv1'] = stax.serial(CONV[d](mid_channels, (3,) * d, padding='valid'), stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity, activation)
     init_fn['conv2'], apply_fn['conv2'] = stax.serial(CONV[d](mid_channels, (3,) * d, padding='valid'), stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity, activation)
 
     def net_init(rng, input_shape):
         params = {}
@@ -457,22 +358,22 @@
     # def upsample_init(rng, input_shape):
     #     return shape, []
     def upsample_apply(params, inputs, **kwargs):
         x = math.wrap(inputs, math.batch('batch'), *[math.spatial(f'{i}') for i in range(len(inputs.shape) - 2)],
                       math.channel('vector'))
         x = math.upsample2x(x)
         return x.native(x.shape)
-
     return NotImplemented, upsample_apply
 
 
 def conv_classifier(in_features: int,
                     in_spatial: Union[tuple, list],
                     num_classes: int,
                     blocks=(64, 128, 256, 256, 512, 512),
+                    block_sizes=(2, 2, 3, 3, 3),
                     dense_layers=(4096, 4096, 100),
                     batch_norm=True,
                     activation='ReLU',
                     softmax=True,
                     periodic=False):
     """
     Based on VGG16.
@@ -482,25 +383,19 @@
         in_spatial = (1,) * d
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     stax_dense_layers = []
     init_fn, apply_fn = {}, {}
-
     net_list = []
-    for i, (prev, next) in enumerate(zip((in_features,) + tuple(blocks[:-1]), blocks)):
-        if i in (0, 1):
-            net_list.append(f'conv{i+1}')
-            init_fn[net_list[-1]], apply_fn[net_list[-1]] = create_double_conv(d, next, next, batch_norm, activation, periodic)
-        else:
-            net_list.append(f'conv{i+1}_1')
-            init_fn[net_list[-1]], apply_fn[net_list[-1]] = create_double_conv(d, 256, 256, batch_norm, activation, periodic)
-            net_list.append(f'conv{i+1}_2')
-            init_fn[net_list[-1]], apply_fn[net_list[-1]] = stax.serial(CONV[d](256, (3,) * d, padding='valid'),
+    for i, (prev, next, block_size) in enumerate(zip((in_features,) + tuple(blocks[:-1]), blocks, block_sizes)):
+        for j in range(block_size):
+            net_list.append(f'conv{i+1}_{j}')
+            init_fn[net_list[-1]], apply_fn[net_list[-1]] = stax.serial(CONV[d](next, (3,) * d, padding='valid'),
                                                                         stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
                                                                         activation)
         net_list.append(f'max_pool{i+1}')
         init_fn[net_list[-1]], apply_fn[net_list[-1]] = stax.MaxPool((2,) * d, padding='valid', strides=(2,) * d)
     init_fn['flatten'], apply_fn['flatten'] = stax.Flatten
     for i, neuron_count in enumerate(dense_layers):
         stax_dense_layers.append(stax.Dense(neuron_count))
@@ -513,26 +408,26 @@
     dense_init, dense_apply = stax.serial(*stax_dense_layers)
 
     def net_init(rng, input_shape):
         params = {}
         rngs = random.split(rng, 2)
         shape = input_shape
         N = len(net_list)
-        for i in range(N):
-            shape, params[f'{net_list[i]}'] = init_fn[f'{net_list[i]}'](rngs[i], shape)
+        for i, layer in enumerate(net_list):
+            shape, params[layer] = init_fn[layer](rngs[i], shape)
         shape, params['flatten'] = init_fn['flatten'](rngs[N], shape)
         flat_size = int(np.prod(in_spatial) * blocks[-1] / (2**d) ** len(blocks))
         shape, params['dense'] = dense_init(rngs[N + 1], (1,) + (flat_size,))
         return shape, params
 
     def net_apply(params, inputs, **kwargs):
         x = inputs
         pad_tuple = [[0, 0]] + [[1, 1]] * d + [[0, 0]]
         for i in range(len(net_list)):
-            if net_list[i] in ['conv3_2', 'conv4_2', 'conv5_2']:
+            if net_list[i].startswith('conv'):
                 x = jnp.pad(x, pad_width=pad_tuple, mode='wrap' if periodic else 'constant')
             x = apply_fn[f'{net_list[i]}'](params[f'{net_list[i]}'], x)
         x = apply_fn['flatten'](params['flatten'], x)
         out = dense_apply(params['dense'], x, **kwargs)
         return out
 
     net = StaxNet(net_init, net_apply, (1,) + in_spatial + (in_features,))
@@ -642,18 +537,16 @@
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     stax_layers = []
     if len(layers) > 0:
         stax_layers.append(resnet_block(in_channels, layers[0], periodic, batch_norm, activation, d))
-
         for i in range(1, len(layers)):
             stax_layers.append(resnet_block(layers[i - 1], layers[i], periodic, batch_norm, activation, d))
-
         stax_layers.append(resnet_block(layers[len(layers) - 1], out_channels, periodic, batch_norm, activation, d))
     else:
         stax_layers.append(resnet_block(in_channels, out_channels, periodic, batch_norm, activation, d))
     net_init, net_apply = stax.serial(*stax_layers)
     net = StaxNet(net_init, net_apply, (1,) + in_spatial + (in_channels,))
     net.initialize()
     return net
@@ -671,39 +564,35 @@
         CONV[d](out_channels, (3,) * d, padding='valid'),
         stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
         activation)
     init_fn['conv2'], apply_fn['conv2'] = stax.serial(
         CONV[d](out_channels, (3,) * d, padding='valid'),
         stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
         activation)
-
     init_activation, apply_activation = activation
     if in_channels != out_channels:
         init_fn['sample_conv'], apply_fn['sample_conv'] = stax.serial(
             CONV[d](out_channels, (1,) * d, padding='VALID'),
             stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity)
     else:
         init_fn['sample_conv'], apply_fn['sample_conv'] = stax.Identity
 
     def net_init(rng, input_shape):
         params = {}
         rngs = random.split(rng, 2)
-
         # Preparing a list of shapes and dictionary of parameters to return
         shape, params['conv1'] = init_fn['conv1'](rngs[0], input_shape)
         shape, params['conv2'] = init_fn['conv2'](rngs[1], shape)
         shape, params['sample_conv'] = init_fn['sample_conv'](rngs[2], input_shape)
         shape, params['activation'] = init_activation(rngs[3], shape)
         return shape, params
 
     def net_apply(params, inputs, **kwargs):
         x = inputs
-
         pad_tuple = [[0, 0]] + [[1, 1] for i in range(d)] + [[0, 0]]
-
         out = jnp.pad(x, pad_width=pad_tuple, mode='wrap' if periodic else 'constant')
         out = apply_fn['conv1'](params['conv1'], out)
         out = jnp.pad(out, pad_width=pad_tuple, mode='wrap' if periodic else 'constant')
         out = apply_fn['conv2'](params['conv2'], out)
         skip_x = apply_fn['sample_conv'](params['sample_conv'], x, **kwargs)
         out = jnp.add(out, skip_x)
         # out = apply_activation(params['activation'], out)
@@ -719,76 +608,57 @@
         N = shape[-1]
         range_n = jnp.arange(0, N)
         even_ind = range_n % 2
         checker = jnp.reshape(even_ind, (-1, N))
     elif len(shape) == 4:
         H = shape[2] if data_format == 'NCHW' else shape[1]
         W = shape[3] if data_format == 'NCHW' else shape[2]
-
         range_h = jnp.arange(0, H) % 2
         range_w = jnp.arange(0, W) % 2
-
         even_ind_h = range_h.astype(bool)
         even_ind_w = range_w.astype(bool)
-
         ind_h = jnp.tile(jnp.expand_dims(even_ind_h, -1), [1, W])
         ind_w = jnp.tile(jnp.expand_dims(even_ind_w, 0), [H, 1])
         # ind_h = even_ind_h.unsqueeze(-1).repeat(1, W)
         # ind_w = even_ind_w.unsqueeze( 0).repeat(H, 1)
-
         checker = jnp.logical_xor(ind_h, ind_w)
-
         reshape = [-1, 1, H, W] if data_format == 'NCHW' else [-1, H, W, 1]
         checker = jnp.reshape(checker, reshape)
         checker = checker.astype(jnp.float32)
-
     else:
-        raise ValueError('Invalid tensor shape. Dimension of the tensor shape must be '
-                         '2 (NxD) or 4 (NxCxHxW or NxHxWxC), got {}.'.format(inputs.get_shape().as_list()))
-
+        raise ValueError('Invalid tensor shape. Dimension of the tensor shape must be 2 (NxD) or 4 (NxCxHxW or NxHxWxC), got {}.'.format(inputs.get_shape().as_list()))
     if reverse_mask:
         checker = 1 - checker
-
     return checker
 
 
 def Dense_resnet_block(in_channels: int,
                        mid_channels: int,
                        batch_norm: bool = False,
                        activation: Union[str, Callable] = 'ReLU'):
     inputs = keras.Input(shape=(in_channels,))
-    x_1 = inputs
-
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     init_fn, apply_fn = {}, {}
-    init_fn['dense1'], apply_fn['dense1'] = stax.serial(stax.Dense(mid_channels),
-                                                        stax.BatchNorm(axis=(0,)),
-                                                        activation)
-    init_fn['dense2'], apply_fn['dense2'] = stax.serial(stax.Dense(in_channels),
-                                                        stax.BatchNorm(axis=(0,)),
-                                                        activation)
+    init_fn['dense1'], apply_fn['dense1'] = stax.serial(stax.Dense(mid_channels), stax.BatchNorm(axis=(0,)), activation)
+    init_fn['dense2'], apply_fn['dense2'] = stax.serial(stax.Dense(in_channels), stax.BatchNorm(axis=(0,)), activation)
     init_activation, apply_activation = activation
 
     def net_init(rng, input_shape):
         params = {}
         rngs = random.split(rng, 2)
-
         shape, params['dense1'] = init_fn['dense1'](rngs[0], input_shape)
         shape, params['dense2'] = init_fn['dense2'](rngs[1], shape)
         shape, params['activation'] = init_activation(rngs[2], shape)
         return shape, params
 
     def net_apply(params, inputs, **kwargs):
         x = inputs
-
         out = apply_fn['dense1'](params['dense1'], x)
         out = apply_fn['dense2'](params['dense2'], out)
-
         out = jnp.add(out, x)
-
         return out
 
     return net_init, net_apply
 
 
 def conv_net_unit(in_channels: int,
                   out_channels: int,
@@ -801,61 +671,49 @@
     if isinstance(in_spatial, int):
         d = in_spatial
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
     if isinstance(activation, str):
         activation = ACTIVATIONS[activation]
-
     init_fn, apply_fn = {}, {}
     if len(layers) < 1:
         layers.append(out_channels)
     init_fn['conv_in'], apply_fn['conv_in'] = stax.serial(
         CONV[d](layers[0], (3,) * d, padding='valid'),
         stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
         activation)
     for i in range(1, len(layers)):
         init_fn[f'conv{i}'], apply_fn[f'conv{i}'] = stax.serial(
             CONV[d](layers[i], (3,) * d, padding='valid'),
             stax.BatchNorm(axis=tuple(range(d + 1))) if batch_norm else stax.Identity,
             activation)
-
     init_fn['conv_out'], apply_fn['conv_out'] = CONV[d](out_channels, (1,) * d)
 
     def net_init(rng, input_shape):
         params = {}
         rngs = random.split(rng, 2)
-
         shape, params['conv_in'] = init_fn['conv_in'](rngs[0], input_shape)
-
         for i in range(1, len(layers)):
             shape, params[f'conv{i + 1}'] = init_fn[f'conv{i + 1}'](rngs[i], shape)
-
         shape, params['conv_out'] = init_fn['conv_out'](rngs[len(layers)], shape)
-
         return shape, params
 
     def net_apply(params, inputs):
         x = inputs
-
         pad_tuple = [(0, 0)]
         for i in range(d):
             pad_tuple.append((1, 1))
         pad_tuple.append((0, 0))
-
         out = jnp.pad(x, pad_width=pad_tuple, mode='wrap' if periodic else 'constant')
-
         out = apply_fn['conv_in'](params['conv_in'], out)
-
         for i in range(1, len(layers)):
             out = jnp.pad(out, pad_width=pad_tuple, mode='wrap' if periodic else 'constant')
             out = apply_fn[f'conv{i + 1}'](params[f'conv{i + 1}'], out)
-
         out = apply_fn['conv_out'](params['conv_out'], out)
-
         return out
 
     return net_init, net_apply
 
 
 def u_net_unit(in_channels: int,
                out_channels: int,
@@ -987,115 +845,86 @@
         init_fn['t1'], apply_fn['t1'] = NET[net](in_channels=in_channels, out_channels=in_channels, layers=[], batch_norm=batch_norm, activation=activation, in_spatial=in_spatial, **kwargs)
         init_fn['s2'], apply_fn['s2'] = NET[net](in_channels=in_channels, out_channels=in_channels, layers=[], batch_norm=batch_norm, activation=activation, in_spatial=in_spatial, **kwargs)
         init_fn['t2'], apply_fn['t2'] = NET[net](in_channels=in_channels, out_channels=in_channels, layers=[], batch_norm=batch_norm, activation=activation, in_spatial=in_spatial, **kwargs)
 
     def net_init(rng, input_shape):
         params = {}
         rngs = random.split(rng, 2)
-
         shape, params['s1'] = init_fn['s1'](rngs[0], input_shape)
         shape, params['t1'] = init_fn['t1'](rngs[1], input_shape)
         shape, params['s2'] = init_fn['s2'](rngs[2], input_shape)
         shape, params['t2'] = init_fn['t2'](rngs[3], input_shape)
-
         return shape, params
 
     def net_apply(params, inputs, invert=False):
         x = inputs
-
         mask = get_mask(x, reverse_mask, 'NCHW')
-
         if invert:
             v1 = x * mask
             v2 = x * (1 - mask)
-
             s1 = apply_fn['s1'](params['s1'], v1)
             t1 = apply_fn['t1'](params['t1'], v1)
-
             u2 = (1 - mask) * (v2 - t1) * jnp.exp(-jnp.tanh(s1))
-
             s2 = apply_fn['s2'](params['s2'], u2)
             t2 = apply_fn['t2'](params['t2'], u2)
-
             u1 = mask * (v1 - t2) * jnp.exp(-jnp.tanh(s2))
-
             return u1 + u2
         else:
             u1 = x * mask
             u2 = x * (1 - mask)
-
             s2 = apply_fn['s2'](params['s2'], u2)
             t2 = apply_fn['t2'](params['t2'], u2)
-
             v1 = mask * (u1 * jnp.exp(jnp.tanh(s2)) + t2)
-
             s1 = apply_fn['s1'](params['s1'], v1)
             t1 = apply_fn['t1'](params['t1'], v1)
-
             v2 = (1 - mask) * (u2 * jnp.exp(jnp.tanh(s1)) + t1)
-
             return v1 + v2
-
     return net_init, net_apply
 
 
-def invertible_net(in_channels: int,
-                   num_blocks: int,
-                   batch_norm: bool = False,
-                   net: str = 'u_net',
-                   activation: Union[str, type] = 'ReLU',
-                   in_spatial: Union[tuple, int] = 2, **kwargs):
-    """
-    ΦFlow also provides invertible neural networks that are capable of inverting the output tensor back to the input tensor initially passed.\ These networks have far reaching applications in predicting input parameters of a problem given its observations.\ Invertible nets are composed of multiple concatenated coupling blocks wherein each such block consists of arbitrary neural networks.
-
-    Currently, these arbitrary neural networks could be set to u_net(default), conv_net, res_net or dense_net blocks with in_channels = out_channels.
-    The architecture used is popularized by ["Real NVP"](https://arxiv.org/abs/1605.08803).
-
-    Arguments:
-
-        in_channels : input channels of the feature map, dtype : int
-        num_blocks : number of coupling blocks inside the invertible net, dtype : int
-        activation : activation function used within the layers, dtype : string
-        batch_norm : use of batchnorm after each layer, dtype : bool
-        in_spatial : spatial dimensions of the input feature map, dtype : int
-        net : type of neural network blocks used in coupling layers, dtype : str
-        **kwargs : placeholder for arguments not supported by the function
-
-    Returns:
-
-        Invertible Net model as specified by input arguments
-
-    Note: Currently supported values for net are 'u_net'(default), 'conv_net' and 'res_net'.
-    For choosing 'dense_net' as the network block in coupling layers in_spatial must be set to zero.
-    """
-    if isinstance(in_spatial, int):
-        d = in_spatial
-    else:
-        assert isinstance(in_spatial, tuple)
-        d = len(in_spatial)
-    init_fn, apply_fn = {}, {}
-    for i in range(num_blocks):
-        init_fn[f'CouplingLayer{i + 1}'], apply_fn[f'CouplingLayer{i + 1}'] = coupling_layer(in_channels, activation, batch_norm, d, net, (i % 2 == 0), **kwargs)
-
-    def net_init(rng, input_shape):
-        params = {}
-        rngs = random.split(rng, 2)
-        for i in range(num_blocks):
-            shape, params[f'CouplingLayer{i + 1}'] = init_fn[f'CouplingLayer{i + 1}'](rngs[i], input_shape)
-        return shape, params
-
-    def net_apply(params, inputs, invert=False):
-        out = inputs
-        if invert:
-            for i in range(num_blocks, 0, -1):
-                out = apply_fn[f'CouplingLayer{i}'](params[f'CouplingLayer{i}'], out, invert)
-        else:
-            for i in range(1, num_blocks + 1):
-                out = apply_fn[f'CouplingLayer{i}'](params[f'CouplingLayer{i}'], out)
-        return out
-
-    if d == 0:
-        net = StaxNet(net_init, net_apply, (1,) + (in_channels,))
-    else:
-        net = StaxNet(net_init, net_apply, (1,) + (1,) * d + (in_channels,))
-    net.initialize()
-    return net
+def invertible_net(num_blocks: int,
+                   construct_net: Union[str, Callable],
+                   **construct_kwargs):  # mlp, u_net, res_net, conv_net
+    raise NotImplementedError("invertible_net is not implemented for Jax")
+    # if construct_net == 'mlp':
+    #     construct_net = '_inv_net_dense_resnet_block'
+    # if isinstance(construct_net, str):
+    #     construct_net = globals()[construct_net]
+    # if 'in_channels' in construct_kwargs and 'out_channels' not in construct_kwargs:
+    #     construct_kwargs['out_channels'] = construct_kwargs['in_channels']
+    # init_fn, apply_fn = {}, {}
+    # for i in range(num_blocks):
+    #     init_fn[f'CouplingLayer{i + 1}'], apply_fn[f'CouplingLayer{i + 1}'] = coupling_layer(in_channels, activation, batch_norm, d, net, (i % 2 == 0), **kwargs)
+    #
+    # def net_init(rng, input_shape):
+    #     params = {}
+    #     rngs = random.split(rng, 2)
+    #     for i in range(num_blocks):
+    #         shape, params[f'CouplingLayer{i + 1}'] = init_fn[f'CouplingLayer{i + 1}'](rngs[i], input_shape)
+    #     return shape, params
+    #
+    # def net_apply(params, inputs, invert=False):
+    #     out = inputs
+    #     if invert:
+    #         for i in range(num_blocks, 0, -1):
+    #             out = apply_fn[f'CouplingLayer{i}'](params[f'CouplingLayer{i}'], out, invert)
+    #     else:
+    #         for i in range(1, num_blocks + 1):
+    #             out = apply_fn[f'CouplingLayer{i}'](params[f'CouplingLayer{i}'], out)
+    #     return out
+    #
+    # if d == 0:
+    #     net = StaxNet(net_init, net_apply, (1,) + (in_channels,))
+    # else:
+    #     net = StaxNet(net_init, net_apply, (1,) + (1,) * d + (in_channels,))
+    # net.initialize()
+    # return net
+
+
+def fno(in_channels: int,
+        out_channels: int,
+        mid_channels: int,
+        modes: Sequence[int],
+        activation: Union[str, type] = 'ReLU',
+        batch_norm: bool = False,
+        in_spatial: int = 2):
+    raise NotImplementedError("fno is not implemented for Jax")
```

### Comparing `unifyml-0.0.1/unifyml/backend/tf/__init__.py` & `unifyml-0.0.2/unifyml/backend/tensorflow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,10 +20,8 @@
 from ._compile_cuda import compile_cuda_ops
 
 from ._tf_backend import TFBackend as _TFBackend
 
 TENSORFLOW = _TFBackend()
 """Backend for TensorFlow operations."""
 
-# _math.backend.BACKENDS.append(TENSORFLOW)
-
 __all__ = [key for key in globals().keys() if not key.startswith('_')]
```

### Comparing `unifyml-0.0.1/unifyml/backend/tf/_compile_cuda.py` & `unifyml-0.0.2/unifyml/backend/tensorflow/_compile_cuda.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/tf/_profiling.py` & `unifyml-0.0.2/unifyml/backend/tensorflow/_profiling.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/tf/_tf_backend.py` & `unifyml-0.0.2/unifyml/backend/tensorflow/_tf_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,28 +22,32 @@
         # Example refs: '/device:CPU:0'
         default_device_ref = '/' + os.path.basename(tf.zeros(()).device)
         default_device = None
         for device in devices:
             if device.ref == default_device_ref:
                 default_device = device
         assert default_device is not None
-        Backend.__init__(self, "TensorFlow", devices, default_device)
+        Backend.__init__(self, 'tensorflow', devices, default_device)
 
     def prefers_channels_last(self) -> bool:
         return True
 
     def _device_for(self, *values):
         devices = set(v.device for v in values if hasattr(v, 'device'))
         if len(devices) == 0:
             return tf.device(self._default_device.ref)
         elif len(devices) == 1:
             return tf.device(next(iter(devices)))
         else:
             return tf.device(self._default_device.ref)
 
+    def nn_library(self):
+        from . import nets
+        return nets
+
     def seed(self, seed: int):
         tf.random.set_seed(seed)
 
     def is_module(self, obj):
         return isinstance(obj, keras.Model)
 
     def is_tensor(self, x, only_native=False):
```

### Comparing `unifyml-0.0.1/unifyml/backend/tf/_tf_cuda_resample.py` & `unifyml-0.0.2/unifyml/backend/tensorflow/_tf_cuda_resample.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/backend/tf/nets.py` & `unifyml-0.0.2/unifyml/backend/torch/nets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,803 +1,662 @@
 """
-Jax implementation of the unified machine learning API.
+PyTorch implementation of the unified machine learning API.
 Equivalent functions also exist for the other frameworks.
 
-For API documentation, see https://holl-.github.io/UnifyML/Network_API .
+For API documentation, see `unifyml.nn`.
 """
-import pickle
-from typing import Callable
-from typing import Union, Sequence
+from typing import Callable, Union, Sequence
 
-import numpy
 import numpy as np
-import tensorflow as tf
-from tensorflow import Tensor
-from tensorflow import keras
-from tensorflow.keras import layers as kl
+import torch
+import torch.nn as nn
+from torch import optim
+
+from . import TORCH
+from ._torch_backend import register_module_call
+from ... import math
 
-from .. import math
 
+def get_parameters(net: nn.Module, wrap=True) -> dict:
+    if not wrap:
+        return {name: param for name, param in net.named_parameters()}
+    result = {}
+    for name, param in net.named_parameters():
+        if name.endswith('.weight'):
+            order = [
+                None,
+                'output',
+                'input,output',
+                'x,input,output',
+                'x,y,input,output',
+                'x,y,z,input,output'
+            ][param.ndim]
+            uml_tensor = math.wrap(param, math.channel(order))
+        elif name.endswith('.bias'):
+            uml_tensor = math.wrap(param, math.channel('output'))
+        else:
+            raise NotImplementedError
+        result[name] = uml_tensor
+    return result
 
-def parameter_count(model: keras.Model):
-    """
-    Counts the number of parameters in a model.
 
-    Args:
-        model: Keras model
+def save_state(obj: Union[nn.Module, optim.Optimizer], path: str):
+    if not path.endswith('.pth'):
+        path += '.pth'
+    torch.save(obj.state_dict(), path)
+
+
+def load_state(obj: Union[nn.Module, optim.Optimizer], path: str):
+    if not path.endswith('.pth'):
+        path += '.pth'
+    obj.load_state_dict(torch.load(path))
+
+
+def update_weights(net: nn.Module, optimizer: optim.Optimizer, loss_function: Callable, *loss_args, check_nan=False, **loss_kwargs):
+    optimizer.zero_grad()
+    output = loss_function(*loss_args, **loss_kwargs)
+    loss = output[0] if isinstance(output, tuple) else output
+    loss.sum.backward()
+    if isinstance(optimizer, optim.LBFGS):
+        def closure():
+            result = loss_function(*loss_args, **loss_kwargs)
+            loss_val = result[0] if isinstance(result, tuple) else result
+            return loss_val.sum
+        optimizer.step(closure=closure)
+    else:
+        if check_nan:
+            for p in net.parameters():
+                if not torch.all(torch.isfinite(p.grad)):
+                    raise RuntimeError(f"NaN in network gradient detected. Parameter: {p}")
+        optimizer.step()
+    return output
 
-    Returns:
-        `int`
-    """
-    total = 0
-    for parameter in model.trainable_weights:
-        total += numpy.prod(parameter.shape)
-    return int(total)
 
+def adam(net: nn.Module, learning_rate: float = 1e-3, betas=(0.9, 0.999), epsilon=1e-07):
+    return optim.Adam(net.parameters(), learning_rate, betas, epsilon)
 
-def get_parameters(model: keras.Model, wrap=True) -> dict:
-    result = {}
-    for var in model.trainable_weights:
-        name: str = var.name
-        layer = name[:name.index('/')].replace('_', '').replace('dense', 'linear')
-        try:
-            int(layer[-1:])
-        except ValueError:
-            layer += '0'
-        prop = name[name.index('/') + 1:].replace('kernel', 'weight')
-        if prop.endswith(':0'):
-            prop = prop[:-2]
-        name = f"{layer}.{prop}"
-        var = var.numpy()
-        if not wrap:
-            result[name] = var
-        else:
-            if name.endswith('.weight'):
-                if var.ndim == 2:
-                    uml_tensor = math.wrap(var, math.channel('input,output'))
-                elif var.ndim == 3:
-                    uml_tensor = math.wrap(var, math.channel('x,input,output'))
-                elif var.ndim == 4:
-                    uml_tensor = math.wrap(var, math.channel('x,y,input,output'))
-                elif var.ndim == 5:
-                    uml_tensor = math.wrap(var, math.channel('x,y,z,input,output'))
-            elif name.endswith('.bias'):
-                uml_tensor = math.wrap(var, math.channel('output'))
-            elif var.ndim == 1:
-                uml_tensor = math.wrap(var, math.channel('output'))
-            else:
-                raise NotImplementedError(name, var)
-            result[name] = uml_tensor
-    return result
 
+def sgd(net: nn.Module, learning_rate: float = 1e-3, momentum=0, dampening=0, weight_decay=0, nesterov=False):
+    return optim.SGD(net.parameters(), learning_rate, momentum, dampening, weight_decay, nesterov)
 
-def save_state(obj: Union[keras.models.Model, keras.optimizers.Optimizer], path: str):
-    """
-    Write the state of a module or optimizer to a file.
-
-    See Also:
-        `load_state()`
-
-    Args:
-        obj: `keras.models.Model or keras.optimizers.Optimizer`
-        path: File path as `str`.
-    """
-    if isinstance(obj, keras.models.Model):
-        if not path.endswith('.h5'):
-            path += '.h5'
-        obj.save_weights(path)
-    elif isinstance(obj, keras.optimizers.Optimizer):
-        if not path.endswith('.pkl'):
-            path += '.pkl'
-        weights = obj.get_weights()
-        with open(path, 'wb') as f:
-            pickle.dump(weights, f)
-    else:
-        raise ValueError("obj must be a Keras model or optimizer")
 
+def adagrad(net: nn.Module, learning_rate: float = 1e-3, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
+    return optim.Adagrad(net.parameters(), learning_rate, lr_decay, weight_decay, initial_accumulator_value, eps)
 
-def load_state(obj: Union[keras.models.Model, keras.optimizers.Optimizer], path: str):
-    """
-    Read the state of a module or optimizer from a file.
-
-    See Also:
-        `save_state()`
-
-    Args:
-        obj: `keras.models.Model or keras.optimizers.Optimizer`
-        path: File path as `str`.
-    """
-    if isinstance(obj, keras.models.Model):
-        if not path.endswith('.h5'):
-            path += '.h5'
-        obj.load_weights(path)
-    elif isinstance(obj, keras.optimizers.Optimizer):
-        if not path.endswith('.pkl'):
-            path += '.pkl'
-        with open(path, 'rb') as f:
-            weights = pickle.load(f)
-        obj.set_weights(weights)
-    else:
-        raise ValueError("obj must be a Keras model or optimizer")
 
+def rmsprop(net: nn.Module, learning_rate: float = 1e-3, alpha=0.99, eps=1e-08, weight_decay=0, momentum=0, centered=False):
+    return optim.RMSprop(net.parameters(), learning_rate, alpha, eps, weight_decay, momentum, centered)
 
-def update_weights(net: keras.Model, optimizer: keras.optimizers.Optimizer, loss_function: Callable, *loss_args, **loss_kwargs):
-    """
-    Computes the gradients of `loss_function` w.r.t. the parameters of `net` and updates its weights using `optimizer`.
-
-    This is the TensorFlow/Keras version. Analogue functions exist for other learning frameworks.
-
-    Args:
-        net: Learning model.
-        optimizer: Optimizer.
-        loss_function: Loss function, called as `loss_function(*loss_args, **loss_kwargs)`.
-        *loss_args: Arguments given to `loss_function`.
-        **loss_kwargs: Keyword arguments given to `loss_function`.
-
-    Returns:
-        Output of `loss_function`.
-    """
-    with tf.GradientTape() as tape:
-        output = loss_function(*loss_args, **loss_kwargs)
-        loss = output[0] if isinstance(output, tuple) else output
-        gradients = tape.gradient(loss.sum, net.trainable_variables)
-    optimizer.apply_gradients(zip(gradients, net.trainable_variables))
-    return output
+
+def _bias0(conv):
+    def initialize(*args, **kwargs):
+        module = conv(*args, **kwargs)
+        module.bias.data.fill_(0)
+        return module
+    return initialize
 
 
-def adam(net: keras.Model, learning_rate: float = 1e-3, betas=(0.9, 0.999), epsilon=1e-07):
-    """
-    Creates an Adam optimizer for `net`, alias for [`keras.optimizers.Adam`](https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Adam).
-    Analogous functions exist for other learning frameworks.
-    """
-    return keras.optimizers.Adam(learning_rate, betas[0], betas[1], epsilon)
-
-
-def sgd(net: keras.Model, learning_rate: float = 1e-3, momentum=0, dampening=0, weight_decay=0, nesterov=False):
-    """
-    Creates an SGD optimizer for 'net', alias for ['keras.optimizers.SGD'](https://keras.io/api/optimizers/sgd/)
-    Analogous functions exist for other learning frameworks.
-    """
-    return keras.optimizers.SGD(learning_rate, momentum, nesterov)
-
-
-def adagrad(net: keras.Model, learning_rate: float = 1e-3, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
-    """
-    Creates an Adagrad optimizer for 'net', alias for ['keras.optimizers.Adagrad'](https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Adagrad)
-    Analogous functions exist for other learning frameworks.
-    """
-    return keras.optimizers.Adagrad(learning_rate, initial_accumulator_value, eps)
-
-
-def rmsprop(net: keras.Model, learning_rate: float = 1e-3, alpha=0.99, eps=1e-08, weight_decay=0, momentum=0, centered=False):
-    """
-    Creates an RMSProp optimizer for 'net', alias for ['keras.optimizers.RMSprop'](https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/RMSprop)
-    Analogous functions exist for other learning frameworks.
-    """
-    return keras.optimizers.RMSprop(learning_rate, alpha, momentum, eps, centered)
+CONV = [None, _bias0(nn.Conv1d), _bias0(nn.Conv2d), _bias0(nn.Conv3d)]
+NORM = [None, nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d]
+ACTIVATIONS = {'ReLU': nn.ReLU, 'Sigmoid': nn.Sigmoid, 'tanh': nn.Tanh, 'SiLU': nn.SiLU, 'GeLU': nn.GELU}
 
 
-def dense_net(in_channels: int,
+def mlp(in_channels: int,
               out_channels: int,
               layers: Sequence[int],
               batch_norm=False,
-              activation='ReLU',
-              softmax=False) -> keras.Model:
-    """
-    Fully-connected neural networks are available in ΦFlow via dense_net().
-    Arguments:
-        in_channels : size of input layer, int
-        out_channels = size of output layer, int
-        layers : tuple of linear layers between input and output neurons, list or tuple
-        activation : activation function used within the layers, string
-        batch_norm : use of batch norm after each linear layer, bool
-
-    Returns:
-        Dense net model as specified by input arguments
-    """
+              activation: Union[str, Callable] = 'ReLU',
+              softmax=False) -> nn.Module:
+    layers = [in_channels, *layers, out_channels]
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
-    keras_layers = []
-    for neuron_count in layers:
-        keras_layers.append(kl.Dense(neuron_count, activation=activation))
-        if batch_norm:
-            keras_layers.append(kl.BatchNormalization())
-    return keras.models.Sequential([kl.InputLayer(input_shape=(in_channels,)),
-                                    *keras_layers,
-                                    kl.Dense(out_channels, activation='linear'),
-                                    *([kl.Softmax()] if softmax else [])])
+    net = DenseNet(layers, activation, batch_norm, softmax)
+    return net.to(TORCH.get_default_device().ref)
+
+
+class DenseNet(nn.Module):
+
+    def __init__(self,
+                 layers: list,
+                 activation: type,
+                 batch_norm: bool,
+                 use_softmax: bool):
+        super(DenseNet, self).__init__()
+        self._layers = layers
+        self._activation = activation
+        self._batch_norm = batch_norm
+        for i, (s1, s2) in enumerate(zip(layers[:-2], layers[1:-1])):
+            self.add_module(f'linear{i}', _bias0(nn.Linear)(s1, s2, bias=True))
+            if batch_norm:
+                self.add_module(f'norm{i}', nn.BatchNorm1d(s2))
+        self.add_module(f'linear_out', _bias0(nn.Linear)(layers[-2], layers[-1], bias=True))
+        self.softmax = nn.Softmax() if use_softmax else None
+
+    def forward(self, x):
+        register_module_call(self)
+        x = TORCH.as_tensor(x)
+        for i in range(len(self._layers) - 2):
+            x = self._activation()(getattr(self, f'linear{i}')(x))
+            if self._batch_norm:
+                x = getattr(self, f'norm{i}')(x)
+        x = getattr(self, f'linear_out')(x)
+        if self.softmax:
+            x = self.softmax(x)
+        return x
+
+
+class DenseResNetBlock(nn.Module):
+
+    def __init__(self, layers, batch_norm, activation):
+        super(DenseResNetBlock, self).__init__()
+        self._layers = layers
+        self._activation = activation
+        self._batch_norm = batch_norm
+        for i, (s1, s2) in enumerate(zip(layers[:-1], layers[1:])):
+            self.add_module(f'linear{i}', _bias0(nn.Linear)(s1, s2, bias=True))
+            if batch_norm:
+                self.add_module(f'norm{i}', nn.BatchNorm1d(s2))
+
+    def forward(self, x):
+        x0 = x
+        for i in range(len(self._layers) - 1):
+            x = self._activation()(getattr(self, f'linear{i}')(x))
+            if self._batch_norm:
+                x = getattr(self, f'norm{i}')(x)
+        return x + x0
 
 
 def u_net(in_channels: int,
           out_channels: int,
           levels: int = 4,
           filters: Union[int, tuple, list] = 16,
           batch_norm: bool = True,
-          activation: Union[str, Callable] = 'ReLU',
+          activation: Union[str, type] = 'ReLU',
           in_spatial: Union[tuple, int] = 2,
           periodic=False,
-          use_res_blocks: bool = False, **kwargs) -> keras.Model:
-    """
-    ΦFlow provides a built-in U-net architecture, classically popular for Semantic Segmentation in Computer Vision, composed of downsampling and upsampling layers.
-
-    Arguments:
-
-        in_channels: input channels of the feature map, dtype : int
-        out_channels : output channels of the feature map, dtype : int
-        levels : number of levels of down-sampling and upsampling, dtype : int
-        filters : filter sizes at each down/up sampling convolutional layer, if the input is integer all conv layers have the same filter size,
-        dtype : int or tuple
-        activation : activation function used within the layers, dtype : string
-        batch_norm : use of batchnorm after each conv layer, dtype : bool
-        in_spatial : spatial dimensions of the input feature map, dtype : int
-        use_res_blocks : use convolutional blocks with skip connections instead of regular convolutional blocks, dtype : bool
-
-    Returns:
-
-        U-net model as specified by input arguments
-    """
+          use_res_blocks: bool = False) -> nn.Module:
+    if isinstance(filters, (tuple, list)):
+        assert len(filters) == levels, f"List of filters has length {len(filters)} but u-net has {levels} levels."
+    else:
+        filters = (filters,) * levels
+    activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
     if isinstance(in_spatial, int):
         d = in_spatial
-        in_spatial = (None,) * d
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
-    activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
-    if isinstance(filters, (tuple, list)):
-        assert len(filters) == levels, f"List of filters has length {len(filters)} but u-net has {levels} levels."
-    else:
-        filters = (filters,) * levels
-    # --- Construct the U-Net ---
-    x = inputs = keras.Input(shape=in_spatial + (in_channels,))
-    x = resnet_block(x.shape[-1], filters[0], periodic, batch_norm, activation, d)(x) if use_res_blocks else double_conv(x, d, filters[0], filters[0], batch_norm, activation, periodic)
-    xs = [x]
-    for i in range(1, levels):
-        x = MAX_POOL[d](2, padding="same")(x)
-        x = resnet_block(x.shape[-1], filters[i], periodic, batch_norm, activation, d)(x) if use_res_blocks else double_conv(x, d, filters[i], filters[i], batch_norm, activation, periodic)
-        xs.insert(0, x)
-    for i in range(1, levels):
-        x = UPSAMPLE[d](2)(x)
-        x = kl.Concatenate()([x, xs[i]])
-        x = resnet_block(x.shape[-1], filters[i - 1], periodic, batch_norm, activation, d)(x) if use_res_blocks else double_conv(x, d, filters[i - 1], filters[i - 1], batch_norm, activation, periodic)
-    x = CONV[d](out_channels, 1)(x)
-    return keras.Model(inputs, x)
-
-
-CONV = [None, kl.Conv1D, kl.Conv2D, kl.Conv3D]
-MAX_POOL = [None, kl.MaxPool1D, kl.MaxPool2D, kl.MaxPool3D]
-UPSAMPLE = [None, kl.UpSampling1D, kl.UpSampling2D, kl.UpSampling3D]
-ACTIVATIONS = {'tanh': keras.activations.tanh, 'ReLU': keras.activations.relu, 'Sigmoid': keras.activations.sigmoid, 'SiLU': keras.activations.selu}
-
-
-def pad_periodic(x: Tensor):
-    d = len(x.shape) - 2
-    if d >= 1:
-        x = tf.concat([tf.expand_dims(x[:, -1, ...], axis=1), x, tf.expand_dims(x[:, 0, ...], axis=1)], axis=1)
-    if d >= 2:
-        x = tf.concat([tf.expand_dims(x[:, :, -1, ...], axis=2), x, tf.expand_dims(x[:, :, 0, ...], axis=2)], axis=2)
-    if d >= 3:
-        x = tf.concat([tf.expand_dims(x[:, :, :, -1, ...], axis=3), x, tf.expand_dims(x[:, :, :, 0, ...], axis=3)],
-                      axis=3)
-    return x
-
-
-def double_conv(x, d: int, out_channels: int, mid_channels: int, batch_norm: bool, activation: Callable, periodic: bool):
-    x = CONV[d](mid_channels, 3, padding='valid')(pad_periodic(x)) if periodic else CONV[d](mid_channels, 3, padding='same')(x)
-    if batch_norm:
-        x = kl.BatchNormalization()(x)
-    x = activation(x)
-    x = CONV[d](out_channels, 3, padding='valid')(pad_periodic(x)) if periodic else CONV[d](out_channels, 3, padding='same')(x)
-    if batch_norm:
-        x = kl.BatchNormalization()(x)
-    x = activation(x)
-    return x
+    net = UNet(d, in_channels, out_channels, filters, batch_norm, activation, periodic, use_res_blocks)
+    return net.to(TORCH.get_default_device().ref)
+
+
+class UNet(nn.Module):
+
+    def __init__(self, d: int, in_channels: int, out_channels: int, filters: tuple, batch_norm: bool, activation: type, periodic: bool, use_res_blocks: bool):
+        super(UNet, self).__init__()
+        self._levels = len(filters)
+        self._spatial_rank = d
+        if use_res_blocks:
+            self.add_module('inc', ResNetBlock(d, in_channels, filters[0], batch_norm, activation, periodic))
+        else:
+            self.add_module('inc', DoubleConv(d, in_channels, filters[0], filters[0], batch_norm, activation, periodic))
+        for i in range(1, self._levels):
+            self.add_module(f'down{i}', Down(d, filters[i - 1], filters[i], batch_norm, activation, periodic, use_res_blocks))
+            self.add_module(f'up{i}', Up(d, filters[i] + filters[i - 1], filters[i - 1], batch_norm, activation, periodic, use_res_blocks))
+        self.add_module('outc', CONV[d](filters[0], out_channels, kernel_size=1))
+
+    def forward(self, x):
+        register_module_call(self)
+        x = TORCH.as_tensor(x)
+        x = self.inc(x)
+        xs = [x]
+        for i in range(1, self._levels):
+            x = getattr(self, f'down{i}')(x)
+            xs.insert(0, x)
+        for i in range(1, self._levels):
+            x = getattr(self, f'up{i}')(x, xs[i])
+        x = self.outc(x)
+        return x
+
+
+class DoubleConv(nn.Module):
+    """(convolution => [BN] => ReLU) * 2"""
+
+    def __init__(self, d: int, in_channels: int, out_channels: int, mid_channels: int, batch_norm: bool, activation: type, periodic: bool):
+        super().__init__()
+        self.add_module('double_conv', nn.Sequential(
+            CONV[d](in_channels, mid_channels, kernel_size=3, padding=1, padding_mode='circular' if periodic else 'zeros'),
+            NORM[d](mid_channels) if batch_norm else nn.Identity(),
+            activation(),
+            CONV[d](mid_channels, out_channels, kernel_size=3, padding=1, padding_mode='circular' if periodic else 'zeros'),
+            NORM[d](out_channels) if batch_norm else nn.Identity(),
+            nn.ReLU(inplace=True)
+        ))
+
+    def forward(self, x):
+        return self.double_conv(x)
+
+
+MAX_POOL = [None, nn.MaxPool1d, nn.MaxPool2d, nn.MaxPool3d]
+
+
+class Down(nn.Module):
+    """Downscaling with maxpool then double conv or resnet_block"""
+
+    def __init__(self, d: int, in_channels: int, out_channels: int, batch_norm: bool, activation: Union[str, type], use_res_blocks: bool, periodic):
+        super().__init__()
+        self.add_module('maxpool', MAX_POOL[d](2))
+        if use_res_blocks:
+            self.add_module('conv', ResNetBlock(d, in_channels, out_channels, batch_norm, activation, periodic))
+        else:
+            self.add_module('conv', DoubleConv(d, in_channels, out_channels, out_channels, batch_norm, activation, periodic))
+
+    def forward(self, x):
+        x = self.maxpool(x)
+        return self.conv(x)
+
+
+class Up(nn.Module):
+    """Upscaling then double conv"""
+
+    _MODES = [None, 'linear', 'bilinear', 'trilinear']
+
+    def __init__(self, d: int, in_channels: int, out_channels: int, batch_norm: bool, activation: type, periodic: bool, use_res_blocks: bool):
+        super().__init__()
+        up = nn.Upsample(scale_factor=2, mode=Up._MODES[d])
+        if use_res_blocks:
+            conv = ResNetBlock(d, in_channels, out_channels, batch_norm, activation, periodic)
+        else:
+            conv = DoubleConv(d, in_channels, out_channels, in_channels // 2, batch_norm, activation, periodic)
+        self.add_module('up', up)
+        self.add_module('conv', conv)
+
+    def forward(self, x1, x2):
+        x1 = self.up(x1)
+        # input is CHW
+        # diff = [x2.size()[i] - x1.size()[i] for i in range(2, len(x1.shape))]
+        # x1 = F.pad(x1, [diffX // 2, diffX - diffX // 2,
+        #                 diffY // 2, diffY - diffY // 2])
+        # if you have padding issues, see
+        # https://github.com/HaiyongJiang/U-Net-Pytorch-Unstructured-Buggy/commit/0e854509c2cea854e247a9c615f175f76fbb2e3a
+        # https://github.com/xiaopeng-liao/Pytorch-UNet/commit/8ebac70e633bac59fc22bb5195e513d5832fb3bd
+        x = torch.cat([x2, x1], dim=1)
+        return self.conv(x)
+
+
+class ConvNet(nn.Module):
+
+    def __init__(self, in_spatial, in_channels, out_channels, layers, batch_norm, activation, periodic: bool):
+        super(ConvNet, self).__init__()
+        activation = ACTIVATIONS[activation]
+        if len(layers) < 1:
+            layers.append(out_channels)
+        self.layers = layers
+        self.add_module(f'Conv_in', nn.Sequential(
+            CONV[in_spatial](in_channels, layers[0], kernel_size=3, padding=1, padding_mode='circular' if periodic else 'zeros'),
+            NORM[in_spatial](layers[0]) if batch_norm else nn.Identity(),
+            activation()))
+        for i in range(1, len(layers)):
+            self.add_module(f'Conv{i}', nn.Sequential(
+                CONV[in_spatial](layers[i - 1], layers[i], kernel_size=3, padding=1, padding_mode='circular' if periodic else 'zeros'),
+                NORM[in_spatial](layers[i]) if batch_norm else nn.Identity(),
+                activation()))
+        self.add_module(f'Conv_out', CONV[in_spatial](layers[len(layers) - 1], out_channels, kernel_size=1))
+
+    def forward(self, x):
+        x = getattr(self, f'Conv_in')(x)
+        for i in range(1, len(self.layers)):
+            x = getattr(self, f'Conv{i}')(x)
+        x = getattr(self, f'Conv_out')(x)
+        return x
 
 
 def conv_net(in_channels: int,
              out_channels: int,
              layers: Sequence[int],
              batch_norm: bool = False,
-             activation: Union[str, Callable] = 'ReLU',
-             periodic=False,
-             in_spatial: Union[int, tuple] = 2, **kwargs) -> keras.Model:
-    """
-    Built in Conv-Nets are also provided. Contrary to the classical convolutional neural networks, the feature map spatial size remains the same throughout the layers. Each layer of the network is essentially a convolutional block comprising of two conv layers. A filter size of 3 is used in the convolutional layers.
-    Arguments:
-
-        in_channels : input channels of the feature map, dtype : int
-        out_channels : output channels of the feature map, dtype : int
-        layers : list or tuple of output channels for each intermediate layer between the input and final output channels, dtype : list or tuple
-        activation : activation function used within the layers, dtype : string
-        batch_norm : use of batchnorm after each conv layer, dtype : bool
-        in_spatial : spatial dimensions of the input feature map, dtype : int
-
-    Returns:
-
-        Conv-net model as specified by input arguments
-    """
+             activation: Union[str, type] = 'ReLU',
+             in_spatial: Union[int, tuple] = 2,
+             periodic=False) -> nn.Module:
     if isinstance(in_spatial, int):
         d = in_spatial
-        in_spatial = (None,) * d
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
-    activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
-    x = inputs = keras.Input(shape=in_spatial + (in_channels,))
-    if len(layers) < 1:
-        layers.append(out_channels)
-    for i in range(len(layers)):
-        x = CONV[d](layers[i], 3, padding='valid')(pad_periodic(x)) if periodic else CONV[d](layers[i], 3, padding='same')(x)
-        if batch_norm:
-            x = kl.BatchNormalization()(x)
-        x = activation(x)
-    x = CONV[d](out_channels, 1)(x)
-    return keras.Model(inputs, x)
-
-
-def resnet_block(in_channels: int,
-                 out_channels: int,
-                 periodic: bool,
-                 batch_norm: bool = False,
-                 activation: Union[str, Callable] = 'ReLU',
-                 in_spatial: Union[int, tuple] = 2):
-    activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
-    if isinstance(in_spatial, int):
-        d = in_spatial
+    net = ConvNet(d, in_channels, out_channels, layers, batch_norm, activation, periodic)
+    net = net.to(TORCH.get_default_device().ref)
+    return net
+
+
+class ResNetBlock(nn.Module):
+
+    def __init__(self, in_spatial, in_channels, out_channels, batch_norm, activation, periodic: bool):
+        # Since in_channels and out_channels might be different, we need a sampling layer for up/down sampling input in order to add it as a skip connection
+        super(ResNetBlock, self).__init__()
+        if in_channels != out_channels:
+            self.sample_input = CONV[in_spatial](in_channels, out_channels, kernel_size=1, padding=0)
+            self.bn_sample = NORM[in_spatial](out_channels) if batch_norm else nn.Identity()
+        else:
+            self.sample_input = nn.Identity()
+            self.bn_sample = nn.Identity()
+        self.activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
+        self.bn1 = NORM[in_spatial](out_channels) if batch_norm else nn.Identity()
+        self.conv1 = CONV[in_spatial](in_channels, out_channels, kernel_size=3, padding=1, padding_mode='circular' if periodic else 'zeros')
+        self.bn2 = NORM[in_spatial](out_channels) if batch_norm else nn.Identity()
+        self.conv2 = CONV[in_spatial](out_channels, out_channels, kernel_size=3, padding=1, padding_mode='circular' if periodic else 'zeros')
+
+    def forward(self, x):
+        x = TORCH.as_tensor(x)
+        out = self.activation()(self.bn1(self.conv1(x)))
+        out = self.activation()(self.bn2(self.conv2(out)))
+        out = (out + self.bn_sample(self.sample_input(x)))
+        return out
+
+
+def get_mask(inputs, reverse_mask, data_format='NHWC'):
+    """ Compute mask for slicing input feature map for Invertible Nets """
+    shape = inputs.shape
+    if len(shape) == 2:
+        N = shape[-1]
+        range_n = torch.arange(0, N)
+        even_ind = range_n % 2
+        checker = torch.reshape(even_ind, (-1, N))
+    elif len(shape) == 4:
+        H = shape[2] if data_format == 'NCHW' else shape[1]
+        W = shape[3] if data_format == 'NCHW' else shape[2]
+        range_h = torch.arange(0, H)
+        range_w = torch.arange(0, W)
+        even_ind_h = range_h % 2
+        even_ind_w = range_w % 2
+        ind_h = even_ind_h.unsqueeze(-1).repeat(1, W)
+        ind_w = even_ind_w.unsqueeze(0).repeat(H, 1)
+        checker = torch.logical_xor(ind_h, ind_w)
+        checker = checker.reshape(1, 1, H, W) if data_format == 'NCHW' else checker.reshape(1, H, W, 1)
+        checker = checker.long()
     else:
-        assert isinstance(in_spatial, tuple)
-        d = len(in_spatial)
-    x = x_1 = inputs = keras.Input(shape=(None,) * d + (in_channels,))
-    x = CONV[d](out_channels, 3, padding='valid')(pad_periodic(x)) if periodic else CONV[d](out_channels, 3, padding='same')(x)
-    if batch_norm:
-        x = kl.BatchNormalization()(x)
-    x = activation(x)
-    x = CONV[d](out_channels, 3, padding='valid')(pad_periodic(x)) if periodic else CONV[d](out_channels, 3, padding='same')(x)
-    if batch_norm:
-        x = kl.BatchNormalization()(x)
-    x = activation(x)
-    if in_channels != out_channels:
-        x_1 = CONV[d](out_channels, 1)(x_1)
-        if batch_norm:
-            x_1 = kl.BatchNormalization()(x_1)
-    x = kl.Add()([x, x_1])
-    return keras.Model(inputs, x)
+        raise ValueError('Invalid tensor shape. Dimension of the tensor shape must be 2 (NxD) or 4 (NxCxHxW or NxHxWxC), got {}.'.format(inputs.get_shape().as_list()))
+    if reverse_mask:
+        checker = 1 - checker
+    return checker.to(TORCH.get_default_device().ref)
+
+
+class ResNet(nn.Module):
+
+    def __init__(self, in_spatial, in_channels, out_channels, layers, batch_norm, activation, periodic: bool):
+        super(ResNet, self).__init__()
+        self.layers = layers
+        if len(self.layers) < 1:
+            layers.append(out_channels)
+        self.add_module('Res_in', ResNetBlock(in_spatial, in_channels, layers[0], batch_norm, activation, periodic))
+        for i in range(1, len(layers)):
+            self.add_module(f'Res{i}', ResNetBlock(in_spatial, layers[i - 1], layers[i], batch_norm, activation, periodic))
+        self.add_module('Res_out', CONV[in_spatial](layers[len(layers) - 1], out_channels, kernel_size=1))
+
+    def forward(self, x):
+        x = TORCH.as_tensor(x)
+        x = getattr(self, 'Res_in')(x)
+        for i in range(1, len(self.layers)):
+            x = getattr(self, f'Res{i}')(x)
+        x = getattr(self, 'Res_out')(x)
+        return x
 
 
 def res_net(in_channels: int,
             out_channels: int,
             layers: Sequence[int],
             batch_norm: bool = False,
-            activation: Union[str, Callable] = 'ReLU',
-            periodic=False,
-            in_spatial: Union[int, tuple] = 2, **kwargs):
-    """
-    Built in Res-Nets are provided in the ΦFlow framework. Similar to the conv-net, the feature map spatial size remains the same throughout the layers.
-    These networks use residual blocks composed of two conv layers with a skip connection added from the input to the output feature map.
-    A default filter size of 3 is used in the convolutional layers.
-
-    Arguments:
-
-        in_channels : input channels of the feature map, dtype : int
-        out_channels : output channels of the feature map, dtype : int
-        layers : list or tuple of output channels for each intermediate layer between the input and final output channels, dtype : list or tuple
-        activation : activation function used within the layers, dtype : string
-        batch_norm : use of batchnorm after each conv layer, dtype : bool
-        in_spatial : spatial dimensions of the input feature map, dtype : int
-
-    Returns:
-
-        Res-net model as specified by input arguments
-    """
+            activation: Union[str, type] = 'ReLU',
+            in_spatial: Union[int, tuple] = 2,
+            periodic=False) -> nn.Module:
     if isinstance(in_spatial, int):
         d = in_spatial
-        in_spatial = (None,) * d
     else:
         assert isinstance(in_spatial, tuple)
         d = len(in_spatial)
-
-    x = inputs = keras.Input(shape=in_spatial + (in_channels,))
-    if len(layers) < 1:
-        layers.append(out_channels)
-    out = resnet_block(in_channels, layers[0], periodic, batch_norm, activation, d)(x)
-    for i in range(1, len(layers)):
-        out = resnet_block(layers[i - 1], layers[i], periodic, batch_norm, activation, d)(out)
-    out = CONV[d](out_channels, 1)(out)
-    return keras.Model(inputs, out)
+    activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
+    net = ResNet(d, in_channels, out_channels, layers, batch_norm, activation, periodic)
+    net = net.to(TORCH.get_default_device().ref)
+    return net
 
 
 def conv_classifier(in_features: int,
                     in_spatial: Union[tuple, list],
                     num_classes: int,
                     blocks=(64, 128, 256, 256, 512, 512),
                     block_sizes=(2, 2, 3, 3, 3),
                     dense_layers=(4096, 4096, 100),
                     batch_norm=True,
                     activation='ReLU',
                     softmax=True,
                     periodic=False):
-    """
-    Based on VGG16.
-    """
     assert isinstance(in_spatial, (tuple, list))
     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
-    d = len(in_spatial)
-    x = inputs = keras.Input(shape=in_spatial + (in_features,))
-    for i, (next, block_size) in enumerate(zip(blocks, block_sizes)):
-        for j in range(block_size):
-            x = CONV[d](next, 3, padding='valid')(pad_periodic(x)) if periodic else CONV[d](next, 3, padding='same')(x)
-            if batch_norm:
-                x = kl.BatchNormalization()(x)
-            x = activation(x)
-        x = MAX_POOL[d](2)(x)
-    x = kl.Flatten()(x)
-    flat_size = int(np.prod(in_spatial) * blocks[-1] / (2**d) ** len(blocks))
-    x = dense_net(flat_size, num_classes, dense_layers, batch_norm, activation, softmax)(x)
-    return keras.Model(inputs, x)
-
+    net = ConvClassifier(in_features, in_spatial, num_classes, batch_norm, softmax, blocks, block_sizes, dense_layers, periodic, activation)
+    return net.to(TORCH.get_default_device().ref)
 
-def get_mask(inputs, reverse_mask, data_format='NHWC'):
-    """ Compute mask for slicing input feature map for Invertible Nets """
-    shape = inputs.shape
-    if len(shape) == 2:
-        N = shape[-1]
-        range_n = tf.range(0, N)
-        even_ind = range_n % 2
-        checker = tf.reshape(even_ind, (-1, N))
-    elif len(shape) == 4:
-        H = shape[2] if data_format == 'NCHW' else shape[1]
-        W = shape[3] if data_format == 'NCHW' else shape[2]
 
-        range_h = tf.range(0, H)
-        range_w = tf.range(0, W)
+class ConvClassifier(nn.Module):
 
-        even_ind_h = tf.cast(range_h % 2, dtype=tf.bool)
-        even_ind_w = tf.cast(range_w % 2, dtype=tf.bool)
-
-        ind_h = tf.tile(tf.expand_dims(even_ind_h, -1), [1, W])
-        ind_w = tf.tile(tf.expand_dims(even_ind_w, 0), [H, 1])
-        # ind_h = even_ind_h.unsqueeze(-1).repeat(1, W)
-        # ind_w = even_ind_w.unsqueeze( 0).repeat(H, 1)
-
-        checker = tf.math.logical_xor(ind_h, ind_w)
-
-        reshape = [-1, 1, H, W] if data_format == 'NCHW' else [-1, H, W, 1]
-        checker = tf.reshape(checker, reshape)
-        checker = tf.cast(checker, dtype=tf.float32)
-
-    else:
-        raise ValueError('Invalid tensor shape. Dimension of the tensor shape must be '
-                         '2 (NxD) or 4 (NxCxHxW or NxHxWxC), got {}.'.format(inputs.get_shape().as_list()))
-
-    if reverse_mask:
-        checker = 1 - checker
-
-    return checker
-
-
-def Dense_resnet_block(in_channels: int,
-                       mid_channels: int,
-                       batch_norm: bool = False,
-                       activation: Union[str, Callable] = 'ReLU'):
-    inputs = keras.Input(shape=(in_channels,))
-    x_1 = inputs
-    activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
-
-    x = kl.Dense(mid_channels)(inputs)
-    if batch_norm:
-        x = kl.BatchNormalization()(x)
-    x = activation(x)
-
-    x = kl.Dense(in_channels)(x)
-    if batch_norm:
-        x = kl.BatchNormalization()(x)
-    x = activation(x)
-
-    x = kl.Add()([x, x_1])
-
-    return keras.Model(inputs, x)
+    def __init__(self, in_features, in_spatial: list, num_classes: int, batch_norm: bool, use_softmax: bool, blocks: tuple, block_sizes: tuple, dense_layers: tuple, periodic: bool, activation):
+        super(ConvClassifier, self).__init__()
+        d = len(in_spatial)
+        self.in_spatial = in_spatial
+        self._blocks = blocks
+        self.add_module('maxpool', MAX_POOL[d](2))
+        for i, (prev, next) in enumerate(zip((in_features,) + tuple(blocks[:-1]), blocks)):
+            block_size = block_sizes[i]
+            layers = []
+            for j in range(block_size):
+                layers.append(CONV[d](prev if j == 0 else next, next, kernel_size=3, padding=1, padding_mode='circular' if periodic else 'zeros'))
+                layers.append(NORM[d](next) if batch_norm else nn.Identity())
+                layers.append(activation())
+            self.add_module(f'conv{i+1}', nn.Sequential(*layers))
+        flat_size = int(np.prod(in_spatial) * blocks[-1] / (2**d) ** len(blocks))
+        self.mlp = mlp(flat_size, num_classes, dense_layers, batch_norm, activation, use_softmax)
+        self.flatten = nn.Flatten()
+
+    def forward(self, x):
+        for i in range(len(self._blocks)):
+            x = getattr(self, f'conv{i+1}')(x)
+            x = self.maxpool(x)
+        x = self.flatten(x)
+        x = self.mlp(x)
+        return x
 
 
 NET = {'u_net': u_net, 'res_net': res_net, 'conv_net': conv_net}
 
 
-class CouplingLayer(keras.Model):
+class CouplingLayer(nn.Module):
 
-    def __init__(self, in_channels, activation, batch_norm, in_spatial, net, reverse_mask):
+    def __init__(self, construct_net: Callable, construction_kwargs: dict, reverse_mask):
         super(CouplingLayer, self).__init__()
-
-        self.activation = activation
-        self.batch_norm = batch_norm
         self.reverse_mask = reverse_mask
+        self.s1 = construct_net(**construction_kwargs)
+        self.t1 = construct_net(**construction_kwargs)
+        self.s2 = construct_net(**construction_kwargs)
+        self.t2 = construct_net(**construction_kwargs)
 
-        if in_spatial == 0:  # for in_spatial = 0, use dense layers
-            self.s1 = Dense_resnet_block(in_channels, in_channels, batch_norm, activation)
-            self.t1 = Dense_resnet_block(in_channels, in_channels, batch_norm, activation)
-
-            self.s2 = Dense_resnet_block(in_channels, in_channels, batch_norm, activation)
-            self.t2 = Dense_resnet_block(in_channels, in_channels, batch_norm, activation)
-        else:
-            self.s1 = NET[net](in_channels=in_channels, out_channels=in_channels, layers=[],
-                               batch_norm=batch_norm, activation=activation,
-                               in_spatial=in_spatial)
-            self.t1 = NET[net](in_channels=in_channels, out_channels=in_channels, layers=[],
-                               batch_norm=batch_norm, activation=activation,
-                               in_spatial=in_spatial)
-
-            self.s2 = NET[net](in_channels=in_channels, out_channels=in_channels, layers=[],
-                               batch_norm=batch_norm, activation=activation,
-                               in_spatial=in_spatial)
-            self.t2 = NET[net](in_channels=in_channels, out_channels=in_channels, layers=[],
-                               batch_norm=batch_norm, activation=activation,
-                               in_spatial=in_spatial)
-
-    def call(self, x, invert=False):
+    def forward(self, x, invert=False):
+        x = TORCH.as_tensor(x)
         mask = get_mask(x, self.reverse_mask, 'NCHW')
-
         if invert:
             v1 = x * mask
             v2 = x * (1 - mask)
-
-            u2 = (1 - mask) * (v2 - self.t1(v1)) * tf.math.exp(tf.tanh(-self.s1(v1)))
-            u1 = mask * (v1 - self.t2(u2)) * tf.math.exp(tf.tanh(-self.s2(u2)))
-
+            u2 = (1 - mask) * (v2 - self.t1(v1)) * torch.exp(-self.s1(v1))
+            u1 = mask * (v1 - self.t2(u2)) * torch.exp(-self.s2(u2))
             return u1 + u2
         else:
             u1 = x * mask
             u2 = x * (1 - mask)
-
-            v1 = mask * (u1 * tf.math.exp(tf.tanh(self.s2(u2))) + self.t2(u2))
-            v2 = (1 - mask) * (u2 * tf.math.exp(tf.tanh(self.s1(v1))) + self.t1(v1))
-
+            v1 = mask * (u1 * torch.exp(self.s2(u2)) + self.t2(u2))
+            v2 = (1 - mask) * (u2 * torch.exp(self.s1(v1)) + self.t1(v1))
             return v1 + v2
 
 
-class InvertibleNet(keras.Model):
-    def __init__(self, in_channels, num_blocks, activation, batch_norm, in_spatial, net):
+class InvertibleNet(nn.Module):
+    def __init__(self, num_blocks: int, construct_net, construction_kwargs: dict):
         super(InvertibleNet, self).__init__()
         self.num_blocks = num_blocks
-
-        self.layer_dict = {}
         for i in range(num_blocks):
-            self.layer_dict[f'coupling_block{i + 1}'] = \
-                CouplingLayer(in_channels,
-                              activation, batch_norm,
-                              in_spatial, net, (i % 2 == 0))
+            self.add_module(f'coupling_block{i + 1}', CouplingLayer(construct_net, construction_kwargs, (i % 2 == 0)))
 
-    def call(self, x, backward=False):
+    def forward(self, x, backward=False):
         if backward:
             for i in range(self.num_blocks, 0, -1):
-                x = self.layer_dict[f'coupling_block{i}'](x, backward)
+                x = getattr(self, f'coupling_block{i}')(x, backward)
         else:
             for i in range(1, self.num_blocks + 1):
-                x = self.layer_dict[f'coupling_block{i}'](x)
+                x = getattr(self, f'coupling_block{i}')(x, backward)
         return x
 
 
-def invertible_net(in_channels: int,
-                   num_blocks: int,
-                   batch_norm: bool = False,
-                   net: str = 'u_net',
+def invertible_net(num_blocks: int,
+                   construct_net: Union[str, Callable],
+                   **construct_kwargs):  # mlp, u_net, res_net, conv_net
+    if construct_net == 'mlp':
+        def construct_net(in_channels: int, layers: Sequence[int], batch_norm=False, activation='ReLU', softmax=False, out_channels: int = None):
+            assert not softmax, "Softmax not supported inside invertible net"
+            assert out_channels is None or out_channels == in_channels, "out_channels must match in_channels or be unspecified"
+            activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
+            layers = [in_channels, *layers, in_channels]
+            return DenseResNetBlock(layers, batch_norm=batch_norm, activation=activation)
+    if isinstance(construct_net, str):
+        construct_net = globals()[construct_net]
+    if 'in_channels' in construct_kwargs and 'out_channels' not in construct_kwargs:
+        construct_kwargs['out_channels'] = construct_kwargs['in_channels']
+    return InvertibleNet(num_blocks, construct_net, construct_kwargs).to(TORCH.get_default_device().ref)
+
+
+def coupling_layer(in_channels: int,
                    activation: Union[str, type] = 'ReLU',
-                   in_spatial: Union[tuple, int] = 2, **kwargs):
-    """
-    ΦFlow also provides invertible neural networks that are capable of inverting the output tensor back to the input tensor initially passed.\ These networks have far reaching applications in predicting input parameters of a problem given its observations.\ Invertible nets are composed of multiple concatenated coupling blocks wherein each such block consists of arbitrary neural networks.
-
-    Currently, these arbitrary neural networks could be set to u_net(default), conv_net, res_net or dense_net blocks with in_channels = out_channels.
-    The architecture used is popularized by ["Real NVP"](https://arxiv.org/abs/1605.08803).
-
-    Arguments:
-
-        in_channels : input channels of the feature map, dtype : int
-        num_blocks : number of coupling blocks inside the invertible net, dtype : int
-        activation : activation function used within the layers, dtype : string
-        batch_norm : use of batchnorm after each layer, dtype : bool
-        in_spatial : spatial dimensions of the input feature map, dtype : int
-        net : type of neural network blocks used in coupling layers, dtype : str
-        **kwargs : placeholder for arguments not supported by the function
-
-    Returns:
-
-        Invertible Net model as specified by input arguments
-
-    Note: Currently supported values for net are 'u_net'(default), 'conv_net' and 'res_net'.
-    For choosing 'dense_net' as the network block in coupling layers in_spatial must be set to zero.
-    """
+                   batch_norm=False,
+                   reverse_mask=False,
+                   in_spatial: Union[tuple, int] = 2):
     if isinstance(in_spatial, tuple):
         in_spatial = len(in_spatial)
-
-    return InvertibleNet(in_channels, num_blocks, activation,
-                         batch_norm, in_spatial, net)
-
-
-##################################################################################################################
-#  Fourier Neural Operators
-#  source: https://github.com/zongyi-li/fourier_neural_operator
-###################################################################################################################
-RFFT = [None, tf.signal.rfft, tf.signal.rfft2d, tf.signal.rfft3d]
-FFT = [None, tf.signal.fft, tf.signal.fft2d, tf.signal.fft3d]
-IRFFT = [None, tf.signal.irfft, tf.signal.irfft2d, tf.signal.irfft3d]
-
-class SpectralConv(keras.Model):
-
-    def __init__(self, in_channels, out_channels, modes, in_spatial):
-
-        super(SpectralConv, self).__init__()
-
-        self.in_channels = in_channels
-        self.out_channels = out_channels
-        self.in_spatial = in_spatial
-        assert in_spatial >= 1 and in_spatial <= 3
-        if isinstance(modes, int):
-            mode = modes
-            modes = [mode for i in range(in_spatial)]
-
-        self.scale = 1 / (in_channels * out_channels)
-
-        self.modes = {i + 1: modes[i] for i in range(len(modes))}
-        self.weights_ = {}
-
-        rand_shape = [in_channels, out_channels]
-        rand_shape += [self.modes[i] for i in range(1, in_spatial + 1)]
-
-        for i in range(2 ** (in_spatial - 1)):
-            self.weights_[f'w{i + 1}'] = tf.complex(tf.Variable(self.scale * tf.random.normal(shape=rand_shape, dtype=tf.dtypes.float32), trainable=True),
-                                                tf.Variable(self.scale * tf.random.normal(shape=rand_shape, dtype=tf.dtypes.float32), trainable=True))
-
-    def complex_mul(self, input, weights):
-
-        if self.in_spatial == 1:
-            return tf.einsum("bix,iox->box", input, weights)
-        elif self.in_spatial == 2:
-            return tf.einsum("bixy,ioxy->boxy", input, weights)
-        elif self.in_spatial == 3:
-            return tf.einsum("bixyz,ioxyz->boxyz", input, weights)
-
-
-    def call(self, x):
-        batch_size = x.shape[0]
-
-        x_ft = RFFT[self.in_spatial](x)
-
-        outft_dims = [batch_size, self.out_channels] + \
-                     [x.shape[-i] for i in range(self.in_spatial, 1, -1)] + [x.shape[-1] // 2 + 1]
-        out_ft0 = tf.complex(tf.Variable(tf.zeros(outft_dims, dtype=tf.dtypes.float32)),
-                            tf.Variable(tf.zeros(outft_dims, dtype=tf.dtypes.float32)))
-
-        if self.in_spatial == 1:
-            out_ft1 = self.complex_mul(x_ft[:, :, :self.modes[1]],
-                                      self.weights_['w1'])
-            out_ft = tf.concat([out_ft1, out_ft0[:, :, self.modes[1]:]], axis=-1)
-        elif self.in_spatial == 2:
-            out_ft1 = self.complex_mul(x_ft[:, :, :self.modes[1], :self.modes[2]],
-                                 self.weights_['w1'])
-            out_ft2 = self.complex_mul(x_ft[:, :, -self.modes[1]:, :self.modes[2]],
-                                 self.weights_['w2'])
-            out_ft3 = tf.concat([out_ft1, out_ft0[:, :, self.modes[1]:-self.modes[1],
-                                         :self.modes[2]], out_ft2], axis=-2)
-            out_ft = tf.concat([out_ft3, out_ft0[:, :, :, self.modes[2]:]], axis=-1)
-        elif self.in_spatial == 3:
-            out_ft1 = self.complex_mul(x_ft[:, :, :self.modes[1], :self.modes[2], :self.modes[3]],
-                                 self.weights_['w1'])
-            out_ft2 = self.complex_mul(x_ft[:, :, -self.modes[1]:, :self.modes[2], :self.modes[3]],
-                                 self.weights_['w2'])
-            out_ft3 = self.complex_mul(x_ft[:, :, :self.modes[1], -self.modes[2]:, :self.modes[3]],
-                                 self.weights_['w3'])
-            out_ft4 = self.complex_mul(x_ft[:, :, -self.modes[1]:, -self.modes[2]:, :self.modes[3]],
-                                 self.weights_['w4'])
-
-            out_ft5 = tf.concat([out_ft1, out_ft0[:, :, self.modes[1]:-self.modes[1], :self.modes[2], :self.modes[3]]
-                                    , out_ft2], axis=-3)
-            out_ft6 = tf.concat([out_ft3, out_ft0[:, :, self.modes[1]:-self.modes[1], -self.modes[2]:, :self.modes[3]]
-                                    , out_ft4], axis=-3)
-            out_ft7 = tf.concat([out_ft5, out_ft0[:, :, :, self.modes[2]:-self.modes[2], :self.modes[3]], out_ft6],
-                                axis=-2)
-            out_ft = tf.concat([out_ft7, out_ft0[:, :, :, :, self.modes[3]:]], axis=-1)
-
-        ##Return to Physical Space
-        x = IRFFT[self.in_spatial](out_ft)
-
-        return x
-
-
-class FNO(keras.Model):
-
-    def __init__(self, in_channels, out_channels, width, modes, activation, batch_norm, in_spatial):
-        super(FNO, self).__init__()
-
-        """
-        The overall network. It contains 4 layers of the Fourier layer.
-        1. Lift the input to the desire channel dimension by self.fc0 .
-        2. 4 layers of the integral operators u' = (W + K)(u).
-            W defined by self.w; K defined by self.conv .
-        3. Project from the channel space to the output space by self.fc1 and self.fc2.
-
-        input shape and output shape: (batchsize b, channels c, *spatial)
-        """
-
-        self.activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
-        self.width = width
-        self.in_spatial = in_spatial
-
-        self.fc0 = kl.Dense(self.width)
-
-        self.model_dict = {}
-        for i in range(4):
-            self.model_dict[f'conv{i}'] = SpectralConv(self.width, self.width, modes, in_spatial)
-            self.model_dict[f'w{i}'] = CONV[self.in_spatial](self.width, kernel_size=1)
-            self.model_dict[f'bn{i}'] = kl.BatchNormalization()
-
-        self.fc1 = kl.Dense(128)
-        self.fc2 = kl.Dense(out_channels)
-
-    # Adding extra spatial channels eg. x, y, z, .... to input x
-    def get_grid(self, shape, device):
-        batch_size = shape[0]
-        grid_channel_sizes = shape[1:-1]  # shape =  (batch_size, *spatial, channels)
-        self.grid_channels = {}
-        for i in range(self.in_spatial):
-            self.grid_channels[f'dim{i}'] = tf.cast(tf.linspace(0, 1,
-                                        grid_channel_sizes[i]), dtype=tf.dtypes.float32)  #tf.tensor(tf.linspace(0, 1, grid_channel_sizes[i]), dtype=tf.dtypes.float32)
-            reshape_dim_tuple = [1,] + [1 if i != j else grid_channel_sizes[j]
-                                        for j in range(self.in_spatial)] + [1,]
-            repeat_dim_tuple = [batch_size,] + [1 if i == j else grid_channel_sizes[j]
-                                                for j in range(self.in_spatial)] + [1,]
-
-            self.grid_channels[f'dim{i}'] = tf.tile(tf.reshape(self.grid_channels[f'dim{i}'], reshape_dim_tuple), repeat_dim_tuple)
-
-        return tf.concat([self.grid_channels[f'dim{i}'] for i in range(self.in_spatial)], axis=-1)
-
-    def call(self, x):
-        grid = self.get_grid(x.shape, x.device)
-        x = tf.concat([x, grid], axis=-1)
-
-        permute_tuple= [0] + [self.in_spatial + 1] + [i + 1 for i in range(self.in_spatial)]
-        permute_tuple_reverse = [0] + [2 + i for i in range(self.in_spatial)] + [1]
-
-        # No need to Transpose x such that channels shape lies
-        # at the end to pass it through linear layers as it's the default in tf
-        #x = tf.transpose(x, permute_tuple)
-
-        x = self.fc0(x)
-
-        for i in range(4):
-            x1 = self.model_dict[f'w{i}'](x)
-            # Spectral conv expects a shape : [batch, channel, *spatial]
-            # hence the transpose:
-            x2 = self.model_dict[f'conv{i}'](tf.transpose(x, permute_tuple))
-            x2 = tf.transpose(x2, permute_tuple_reverse)
-            x = self.model_dict[f'bn{i}'](x1) + self.model_dict[f'bn{i}'](x2)
-            x = self.activation(x)
-
-        x = self.activation(self.fc1(x))
-        x = self.fc2(x)
-
-        return x
-
-
-def fno(in_channels: int,
-        out_channels: int,
-        mid_channels: int,
-        modes: Sequence[int],
-        activation: Union[str, type] = 'ReLU',
-        batch_norm: bool = False,
-        in_spatial: int = 2):
-    """
-    ["Fourier Neural Operator"](https://github.com/zongyi-li/fourier_neural_operator) network contains 4 layers of the Fourier layer.
-    1. Lift the input to the desire channel dimension by self.fc0 .
-    2. 4 layers of the integral operators u' = (W + K)(u). W defined by self.w; K defined by self.conv .
-    3. Project from the channel space to the output space by self.fc1 and self.fc2.
-
-    Arguments:
-
-        in_channels : input channels of the feature map, dtype : int
-        out_channels : output channels of the feature map, dtype : int
-        mid_channels : channels used in Spectral Convolution Layers, dtype : int
-        modes : Fourier modes for each spatial channel, dtype : List[int] or int (in case all number modes are to be the same for each spatial channel)
-        activation : activation function used within the layers, dtype : string
-        batch_norm : use of batchnorm after each conv layer, dtype : bool
-        in_spatial : spatial dimensions of the input feature map, dtype : int
-
-    Returns:
-
-        Fourier Neural Operator model as specified by input arguments.
-    """
-    net = FNO(in_channels, out_channels, mid_channels, modes, activation, batch_norm, in_spatial)
-    return net
+    activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
+    net = CouplingLayer(in_channels, activation, batch_norm, in_spatial, reverse_mask)
+    net = net.to(TORCH.get_default_device().ref)
+    return net
+
+
+# class SpectralConv(nn.Module):
+#
+#     def __init__(self, in_channels, out_channels, modes, in_spatial):
+#         super(SpectralConv, self).__init__()
+#         self.in_channels = in_channels
+#         self.out_channels = out_channels
+#         self.in_spatial = in_spatial
+#         assert in_spatial >= 1 and in_spatial <= 3
+#         if isinstance(modes, int):
+#             mode = modes
+#             modes = [mode for i in range(in_spatial)]
+#         self.scale = 1 / (in_channels * out_channels)
+#         self.modes = {i + 1: modes[i] for i in range(len(modes))}
+#         self.weights = {}
+#         rand_shape = [in_channels, out_channels]
+#         rand_shape += [self.modes[i] for i in range(1, in_spatial + 1)]
+#         for i in range(2 ** (in_spatial - 1)):
+#             self.weights[f'w{i + 1}'] = nn.Parameter(self.scale * torch.randn(rand_shape, dtype=torch.cfloat))
+#
+#     def complex_mul(self, input, weights):
+#         if self.in_spatial == 1:
+#             return torch.einsum("bix,iox->box", input, weights)
+#         elif self.in_spatial == 2:
+#             return torch.einsum("bixy,ioxy->boxy", input, weights)
+#         elif self.in_spatial == 3:
+#             return torch.einsum("bixyz,ioxyz->boxyz", input, weights)
+#
+#     def forward(self, x):
+#         batch_size = x.shape[0]
+#         # --- Convert to Fourier space ---
+#         dims = [-i for i in range(self.in_spatial, 0, -1)]
+#         x_ft = torch.fft.rfftn(x, dim=dims)
+#         outft_dims = [batch_size, self.out_channels] + [x.size(-i) for i in range(self.in_spatial, 1, -1)] + [x.size(-1) // 2 + 1]
+#         out_ft = torch.zeros(outft_dims, dtype=torch.cfloat, device=x.device)
+#         # --- Multiply relevant fourier modes ---
+#         if self.in_spatial == 1:
+#             out_ft[:, :, :self.modes[1]] = self.complex_mul(x_ft[:, :, :self.modes[1]], self.weights['w1'].to(x_ft.device))
+#         elif self.in_spatial == 2:
+#             out_ft[:, :, :self.modes[1], :self.modes[2]] = self.complex_mul(x_ft[:, :, :self.modes[1], :self.modes[2]], self.weights['w1'].to(x_ft.device))
+#             out_ft[:, :, -self.modes[1]:, :self.modes[2]] = self.complex_mul(x_ft[:, :, -self.modes[1]:, :self.modes[2]], self.weights['w2'].to(x_ft.device))
+#         elif self.in_spatial == 3:
+#             out_ft[:, :, :self.modes[1], :self.modes[2], :self.modes[3]] = self.complex_mul(x_ft[:, :, :self.modes[1], :self.modes[2], :self.modes[3]], self.weights['w1'].to(x_ft.device))
+#             out_ft[:, :, -self.modes[1]:, :self.modes[2], :self.modes[3]] = self.complex_mul(x_ft[:, :, -self.modes[1]:, :self.modes[2], :self.modes[3]], self.weights['w2'].to(x_ft.device))
+#             out_ft[:, :, :self.modes[1], -self.modes[2]:, :self.modes[3]] = self.complex_mul(x_ft[:, :, :self.modes[1], -self.modes[2]:, :self.modes[3]], self.weights['w3'].to(x_ft.device))
+#             out_ft[:, :, -self.modes[1]:, -self.modes[2]:, :self.modes[3]] = self.complex_mul(x_ft[:, :, -self.modes[1]:, -self.modes[2]:, :self.modes[3]], self.weights['w4'].to(x_ft.device))
+#         # --- Return to Physical Space ---
+#         x = torch.fft.irfftn(out_ft, s=[x.size(-i) for i in range(self.in_spatial, 0, -1)])
+#         return x
+#
+#
+# class FNO(nn.Module):
+#     """
+#     Fourier Neural Operators
+#     source: https://github.com/zongyi-li/fourier_neural_operator
+#
+#     The overall network contains 4 layers of the ["Fourier layer"](https://github.com/zongyi-li/fourier_neural_operator).
+#     1. Lift the input to the desire channel dimension by self.fc0 .
+#     2. 4 layers of the integral operators u' = (W + K)(u).
+#         W defined by self.w; K defined by self.conv .
+#     3. Project from the channel space to the output space by self.fc1 and self.fc2.
+#
+#     input shape and output shape: (batchsize b, channels c, *spatial)
+#     """
+#
+#     def __init__(self, in_channels, out_channels, width, modes, activation, batch_norm, in_spatial):
+#         super(FNO, self).__init__()
+#         self.activation = activation
+#         self.width = width
+#         self.in_spatial = in_spatial
+#         self.fc0 = _bias0(nn.Linear)(in_channels + in_spatial, self.width)
+#         for i in range(4):
+#             self.add_module(f'conv{i}', SpectralConv(self.width, self.width, modes, in_spatial))
+#             self.add_module(f'w{i}', CONV[in_spatial](self.width, self.width, kernel_size=1))
+#             self.add_module(f'bn{i}', NORM[in_spatial](self.width) if batch_norm else nn.Identity())
+#         self.fc1 = _bias0(nn.Linear)(self.width, 128)
+#         self.fc2 = _bias0(nn.Linear)(128, out_channels)
+#
+#     # Adding extra spatial channels eg. x, y, z, .... to input x
+#     def get_grid(self, shape, device):
+#         batch_size = shape[0]
+#         grid_channel_sizes = shape[2:]  # shape =  (batch_size, channels, *spatial)
+#         self.grid_channels = {}
+#         for i in range(self.in_spatial):
+#             self.grid_channels[f'dim{i}'] = torch.tensor(torch.linspace(0, 1, grid_channel_sizes[i]), dtype=torch.float)
+#             reshape_dim_tuple = [1, 1] + [1 if i != j else grid_channel_sizes[j] for j in range(self.in_spatial)]
+#             repeat_dim_tuple = [batch_size, 1] + [1 if i == j else grid_channel_sizes[j] for j in range(self.in_spatial)]
+#             self.grid_channels[f'dim{i}'] = self.grid_channels[f'dim{i}'].reshape(reshape_dim_tuple).repeat(repeat_dim_tuple)
+#         return torch.cat([self.grid_channels[f'dim{i}'] for i in range(self.in_spatial)], dim=1).to(device)
+#
+#     def forward(self, x):
+#         grid = self.get_grid(x.shape, x.device)
+#         x = torch.cat([x, grid], dim=1)
+#         permute_tuple = [0] + [2 + i for i in range(self.in_spatial)] + [1]
+#         permute_tuple_reverse = [0] + [self.in_spatial + 1] + [i + 1 for i in range(self.in_spatial)]
+#         # Transpose x such that channels shape lies at the end to pass it through linear layers
+#         x = x.permute(permute_tuple)
+#         x = self.fc0(x)
+#         # Transpose x back to its original shape to pass it through convolutional layers
+#         x = x.permute(permute_tuple_reverse)
+#         for i in range(4):
+#             x1 = getattr(self, f'w{i}')(x)
+#             x2 = getattr(self, f'conv{i}')(x)
+#             x = getattr(self, f'bn{i}')(x1) + getattr(self, f'bn{i}')(x2)
+#             x = self.activation()(x)
+#         x = x.permute(permute_tuple)
+#         x = self.activation()(self.fc1(x))
+#         x = self.fc2(x)
+#         x = x.permute(permute_tuple_reverse)
+#         return x
+#
+#
+# def fno(in_channels: int,
+#         out_channels: int,
+#         mid_channels: int,
+#         modes: Sequence[int],
+#         activation: Union[str, type] = 'ReLU',
+#         batch_norm: bool = False,
+#         in_spatial: int = 2):
+#     activation = ACTIVATIONS[activation] if isinstance(activation, str) else activation
+#     net = FNO(in_channels, out_channels, mid_channels, modes, activation, batch_norm, in_spatial)
+#     net = net.to(TORCH.get_default_device().ref)
+#     return net
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `unifyml-0.0.1/unifyml/backend/torch/_torch_backend.py` & `unifyml-0.0.2/unifyml/backend/torch/_torch_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,22 +18,26 @@
 
     def __init__(self):
         cpu = NUMPY.get_default_device()
         devices = [ComputeDevice(self, "CPU", 'CPU', cpu.memory, cpu.processor_count, cpu.description, ref='cpu')]
         for index in range(torch.cuda.device_count()):
             properties = torch.cuda.get_device_properties(index)
             devices.append(ComputeDevice(self, properties.name, 'GPU', properties.total_memory, properties.multi_processor_count, f"compute capability {properties.major}.{properties.minor}", f'cuda:{index}'))
-        Backend.__init__(self, 'PyTorch', devices, devices[1 if len(devices) > 1 else 0])
+        Backend.__init__(self, 'torch', devices, devices[1 if len(devices) > 1 else 0])
 
     def prefers_channels_last(self) -> bool:
         return False
 
     def is_module(self, obj):
         return isinstance(obj, (JITFunction, torch.nn.Module))
 
+    def nn_library(self):
+        from . import nets
+        return nets
+
     def is_tensor(self, x, only_native=False):
         if isinstance(x, torch.Tensor):
             return True
         if only_native:
             return False
         if isinstance(x, numbers.Number):
             return True
@@ -137,18 +141,17 @@
         return self.get_device_by_ref(str(tensor.device))
 
     def allocate_on_device(self, tensor: TensorType, device: ComputeDevice) -> TensorType:
         return self.as_tensor(tensor).to(device.ref)
 
     def multi_slice(self, tensor, slices: tuple):
         neg_slices = [i for i, s in enumerate(slices) if isinstance(s, slice) and s.step is not None and s.step < 0]
-        if neg_slices:
-            tensor = torch.flip(tensor, neg_slices)
-        pos_slices = [slice(s.start, s.stop, -s.step) if i in neg_slices else s for i, s in enumerate(slices)]
-        return tensor[tuple(pos_slices)]
+        pos_slices = [slice(0 if s.stop is None else s.stop+1, None if s.start is None else s.start+1 or None, -s.step) if i in neg_slices else s for i, s in enumerate(slices)]
+        sliced = tensor[tuple(pos_slices)]
+        return torch.flip(sliced, neg_slices) if neg_slices else sliced
 
     sqrt = torch.sqrt
     exp = torch.exp
     sin = torch.sin
     arcsin = torch.arcsin
     cos = torch.cos
     arccos = torch.arccos
```

### Comparing `unifyml-0.0.1/unifyml/math/__init__.py` & `unifyml-0.0.2/unifyml/math/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Instead, they delegate the actual computation to either NumPy, TensorFlow or PyTorch, depending on the configuration.
 This allows the user to write simulation code once and have it run with various computation backends.
 
 See the documentation at https://holl-.github.io/UnifyML/Math.html
 """
 
 from ..backend._dtype import DType
-from ..backend import NUMPY, precision, set_global_precision, get_precision
+from ..backend import NUMPY, precision, set_global_precision, get_precision, set_global_default_backend as use
 
 from ._shape import (
     shape, Shape, EMPTY_SHAPE, DimFilter,
     spatial, channel, batch, instance, dual,
     non_batch, non_spatial, non_instance, non_channel, non_dual, non_primal, primal,
     merge_shapes, concat_shapes, IncompatibleShapes,
     enable_debug_checks,
@@ -43,52 +43,52 @@
     native, numpy, reshaped_native, reshaped_tensor, reshaped_numpy, copy, native_call,
     print_ as print,
     map_ as map,
     zeros, ones, fftfreq, random_normal, random_uniform, meshgrid, linspace, arange as range, range_tensor,  # creation operators (use default backend)
     zeros_like, ones_like,
     pad,
     transpose,  # reshape operations
-    safe_div, safe_div as divide_no_nan,
+    safe_div,
     where, nonzero,
     sum_ as sum, finite_sum, mean, finite_mean, std, prod, max_ as max, finite_max, min_ as min, finite_min, any_ as any, all_ as all, quantile, median,  # reduce
     dot,
     abs_ as abs, sign,
     round_ as round, ceil, floor,
     maximum, minimum, clip,
     sqrt, exp, log, log2, log10, sigmoid, soft_plus,
     sin, cos, tan, sinh, cosh, tanh, arcsin, arccos, arctan, arcsinh, arccosh, arctanh, log_gamma, factorial,
     to_float, to_int32, to_int64, to_complex, imag, real, conjugate,
     degrees,
     boolean_mask,
-    is_finite, is_finite as isfinite, is_nan, is_inf,
+    is_finite, is_nan, is_inf,
     closest_grid_values, grid_sample, scatter, gather,
     histogram,
     fft, ifft, convolve, cumulative_sum,
     dtype, cast,
     close, assert_close,
     stop_gradient,
     pairwise_distances, map_pairs,
 )
 
 from ._nd import (
     shift,
-    vec, const_vec, vec_abs, vec_abs as vec_length, vec_squared, vec_normalize, cross_product, rotate_vector, dim_mask,
+    vec, const_vec, vec_length, vec_squared, vec_normalize, cross_product, rotate_vector, dim_mask,
     normalize_to,
     l1_loss, l2_loss, frequency_loss,
     spatial_gradient, laplace,
     fourier_laplace, fourier_poisson, abs_square,
     downsample2x, upsample2x, sample_subgrid,
     masked_fill, finite_fill
 )
 
 from ._trace import matrix_from_function
 
 from ._functional import (
     LinearFunction, jit_compile_linear, jit_compile,
-    jacobian, jacobian as gradient, functional_gradient, custom_gradient, print_gradient,
+    jacobian, gradient, custom_gradient, print_gradient,
     map_types, map_s2b, map_i2b, map_c2b,
     broadcast,
     iterate,
     identity,
     trace_check,
 )
```

### Comparing `unifyml-0.0.1/unifyml/math/_fit.py` & `unifyml-0.0.2/unifyml/math/_fit.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/math/_functional.py` & `unifyml-0.0.2/unifyml/math/_functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
             wrt_natives.extend([i] * len(value._natives()))
         return [n_i for n_i, t_i in enumerate(wrt_natives) if t_i in wrt_tensors]
 
 
 def jacobian(f: Callable, wrt: str = None, get_output=True) -> Callable:
     """
     Creates a function which computes the Jacobian matrix of `f`.
-    For scalar functions, consider using `functional_gradient()` instead.
+    For scalar functions, consider using `gradient()` instead.
 
     Example:
     ```python
     def f(x, y):
         prediction = f(x)
         loss = math.l2_loss(prediction - y)
         return loss, prediction
@@ -552,28 +552,28 @@
     Returns:
         Function with the same arguments as `f` that returns the value of `f`, auxiliary data and Jacobian of `f` if `get_output=True`, else just the Jacobian of `f`.
     """
     f_params, wrt = simplify_wrt(f, wrt)
     return GradientFunction(f, f_params, wrt, get_output, is_f_scalar=False)
 
 
-def functional_gradient(f: Callable, wrt: str = None, get_output=True) -> Callable:
+def gradient(f: Callable, wrt: str = None, get_output=True) -> Callable:
     """
     Creates a function which computes the gradient of `f`.
 
     Example:
     ```python
     def loss_function(x, y):
         prediction = f(x)
         loss = math.l2_loss(prediction - y)
         return loss, prediction
 
-    dx = functional_gradient(loss_function, 'x', get_output=False)(x, y)
+    dx = gradient(loss_function, 'x', get_output=False)(x, y)
 
-    (loss, prediction), (dx, dy) = functional_gradient(loss_function,
+    (loss, prediction), (dx, dy) = gradient(loss_function,
                                             'x,y', get_output=True)(x, y)
     ```
 
     Functional gradients are implemented for the following backends:
 
     * PyTorch: [`torch.autograd.grad`](https://pytorch.org/docs/stable/autograd.html#torch.autograd.grad) / [`torch.autograd.backward`](https://pytorch.org/docs/stable/autograd.html#torch.autograd.backward)
     * TensorFlow: [`tf.GradientTape`](https://www.tensorflow.org/api_docs/python/tf/GradientTape)
@@ -926,15 +926,15 @@
         reason: Message giving hints as to why `f` needs to be re-traced given `args` and `kwargs`.
     """
     if isinstance(f, (JitFunction, GradientFunction, HessianFunction, CustomGradientFunction)):
         keys = f.traces.keys()
     elif isinstance(f, LinearFunction):
         keys = f.matrices_and_biases.keys()
     else:
-        raise ValueError(f"{f_name(f)} is not a traceable function. Only supports jit_compile, jit_compile_linear, functional_gradient, custom_gradient, jacobian, hessian")
+        raise ValueError(f"{f_name(f)} is not a traceable function. Only supports jit_compile, jit_compile_linear, gradient, custom_gradient, jacobian, hessian")
     key, *_ = key_from_args(args, kwargs, f.f_params, aux=f.auxiliary_args)
     if not keys:
         return False, "Function has not yet been traced"
     if key in keys:
         return True, ""
     traced_key = next(iter(keys))  # ToDo compare against all
     cond_equal = key.auxiliary_kwargs == traced_key.auxiliary_kwargs
```

### Comparing `unifyml-0.0.1/unifyml/math/_magic_ops.py` & `unifyml-0.0.2/unifyml/math/_magic_ops.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/math/_nd.py` & `unifyml-0.0.2/unifyml/math/_nd.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             shape = dim
     else:
         dims = parse_dim_order(dim)
         shape = channel(vector=dims)
     return wrap([value] * shape.size, shape)
 
 
-def vec_abs(vec: Tensor, vec_dim: DimFilter = channel, eps: Union[float, Tensor] = None):
+def vec_length(vec: Tensor, vec_dim: DimFilter = channel, eps: Union[float, Tensor] = None):
     """
     Computes the vector length of `vec`.
 
     Args:
         eps: Minimum vector length. Use to avoid `inf` gradients for zero-length vectors.
     """
     if vec.dtype.kind == complex:
@@ -107,15 +107,15 @@
 def vec_squared(vec: Tensor, vec_dim: DimFilter = channel):
     """ Computes the squared length of `vec`. If `vec_dim` is None, the combined channel dimensions of `vec` are interpreted as a vector. """
     return math.sum_(vec ** 2, dim=vec_dim)
 
 
 def vec_normalize(vec: Tensor, vec_dim: DimFilter = channel):
     """ Normalizes the vectors in `vec`. If `vec_dim` is None, the combined channel dimensions of `vec` are interpreted as a vector. """
-    return vec / vec_abs(vec, vec_dim=vec_dim)
+    return vec / vec_length(vec, vec_dim=vec_dim)
 
 
 def cross_product(vec1: Tensor, vec2: Tensor) -> Tensor:
     """
     Computes the cross product of two vectors in 2D.
 
     Args:
```

### Comparing `unifyml-0.0.1/unifyml/math/_ops.py` & `unifyml-0.0.2/unifyml/math/_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -818,15 +818,15 @@
             broadcast_shape = broadcast_shape.with_dim_size(dim, sum([v.shape.get_size(dim) for v in values]))
         return NativeTensor(concatenated, broadcast_shape)
 
     result = broadcast_op(inner_concat, values)
     return result
 
 
-def pad(value: Tensor, widths: dict, mode: Union['e_.Extrapolation', Tensor, Number], **kwargs) -> Tensor:
+def pad(value: Tensor, widths: Union[dict, tuple], mode: Union['e_.Extrapolation', Tensor, Number] = 0, **kwargs) -> Tensor:
     """
     Pads a tensor along the specified dimensions, determining the added values using the given extrapolation.
     Unlike `Extrapolation.pad()`, this function can handle negative widths which slice off outer values.
 
     Args:
         value: `Tensor` to be padded
         widths: `dict` mapping dimension name (`str`) to `(lower, upper)`
@@ -842,14 +842,22 @@
     Examples:
         >>> math.pad(math.ones(spatial(x=10, y=10)), {'x': (1, 1), 'y': (2, 1)}, 0)
         (xˢ=12, yˢ=13) 0.641 ± 0.480 (0e+00...1e+00)
 
         >>> math.pad(math.ones(spatial(x=10, y=10)), {'x': (1, -1)}, 0)
         (xˢ=10, yˢ=10) 0.900 ± 0.300 (0e+00...1e+00)
     """
+    if isinstance(widths, (tuple, list)):
+        if len(widths) == 2 and isinstance(widths[0], int) and isinstance(widths[1], int):  # (lower, upper)
+            assert non_batch(value).rank == 1, f"Can only pad 1D tensors (excluding batch dims) when widths=(lower, upper) but got {shape(value)} and widths={widths}"
+            widths = {non_batch(value).name: widths}
+        else:  # ((lo0, up0), (lo1, up1), ...)
+            assert len(widths) == non_batch(value), f"Cannot pad tensor with non-batch dims {non_batch(value)} by widths {widths}. Sizes must match."
+            warnings.warn("Padding by sequence of (lower, upper) is not recommended. Please use a dict instead.", SyntaxWarning, stacklevel=2)
+            widths = {dim: w for dim, w in zip(non_batch(value).names, widths)}
     mode = mode if isinstance(mode, e_.Extrapolation) else e_.ConstantExtrapolation(mode)
     has_negative_widths = any(w0 < 0 or w1 < 0 for w0, w1 in widths.values())
     has_positive_widths = any(w0 > 0 or w1 > 0 for w0, w1 in widths.values())
     slices = None
     if has_negative_widths:
         slices = {dim: slice(max(0, -w[0]), min(0, w[1]) or None) for dim, w in widths.items()}
         widths = {dim: (max(0, w[0]), max(0, w[1])) for dim, w in widths.items()}
@@ -993,15 +1001,15 @@
         dim = next(iter(iter_dims))
         dim_type = None
         size = None
         item_names = None
         unstacked = []
         for tensor in tensors:
             if dim in tensor.shape.names:
-                unstacked_tensor = tensor.unstack(dim)
+                unstacked_tensor = tensor._unstack(dim)
                 unstacked.append(unstacked_tensor)
                 if size is None:
                     size = len(unstacked_tensor)
                     dim_type = tensor.shape.get_type(dim)
                 else:
                     assert size == len(unstacked_tensor)
                     assert dim_type == tensor.shape.get_type(dim)
@@ -1285,15 +1293,15 @@
 def _std(value: Tensor, dims: Shape) -> Tensor:
     if value.shape.is_uniform:
         result = value.default_backend.std(value.native(value.shape), value.shape.indices(dims))
         return NativeTensor(result, value.shape.without(dims))
     else:
         non_uniform_dim = value.shape.shape.without('dims')
         assert non_uniform_dim.only(dims).is_empty, f"Cannot compute std along non-uniform dims {dims}. shape={value.shape}"
-        return stack([_std(t, dims) for t in value.unstack(non_uniform_dim.name)], non_uniform_dim)
+        return stack([_std(t, dims) for t in value._unstack(non_uniform_dim.name)], non_uniform_dim)
 
 
 def any_(boolean_tensor: Union[Tensor, list, tuple], dim: DimFilter = non_batch) -> Tensor:
     """
     Tests whether any entry of `boolean_tensor` is `True` along the specified dimensions.
 
     Args:
```

### Comparing `unifyml-0.0.1/unifyml/math/_optimize.py` & `unifyml-0.0.2/unifyml/math/_optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import warnings
 from typing import Callable, Generic, List, TypeVar, Any, Tuple, Union, Optional
 
 import numpy
 import numpy as np
 
 from ..backend import get_precision, NUMPY, Backend
-from ..backend._backend import SolveResult, ML_LOGGER, default_backend, convert, Preconditioner
+from ..backend._backend import SolveResult, ML_LOGGER, default_backend, convert, Preconditioner, choose_backend
 from ..backend._linalg import IncompleteLU, incomplete_lu_dense, incomplete_lu_coo, coarse_explicit_preconditioner_coo
 from ._shape import EMPTY_SHAPE, Shape, merge_shapes, batch, non_batch, shape, dual, channel, non_dual, instance, spatial
 from ._magic_ops import stack, copy_with, rename_dims, unpack_dim
 from ._sparse import native_matrix, SparseCoordinateTensor, CompressedSparseMatrix, stored_values, is_sparse
 from ._tensors import Tensor, disassemble_tree, assemble_tree, wrap, cached, NativeTensor, layout
 from . import _ops as math
 from ._ops import choose_backend_t, zeros_like, all_available, reshaped_native, reshaped_tensor, to_float, reshaped_numpy
@@ -527,14 +527,49 @@
     f_kwargs.update(f_kwargs_)
     f_args = f_args[0] if len(f_args) == 1 and isinstance(f_args[0], tuple) else f_args
     # --- Get input and output tensors ---
     y_tree, y_tensors = disassemble_tree(y)
     x0_tree, x0_tensors = disassemble_tree(solve.x0)
     assert solve.x0 is not None, "Please specify the initial guess as Solve(..., x0=initial_guess)"
     assert len(x0_tensors) == len(y_tensors) == 1, "Only single-tensor linear solves are currently supported"
+    if y_tree == 'native' and x0_tree == 'native':
+        if callable(f):  # assume batch + 1 dim
+            rank = y_tensors[0].rank
+            assert x0_tensors[0].rank == rank, f"y and x0 must have the same rank but got {y_tensors[0].shape.sizes} for y and {x0_tensors[0].shape.sizes} for x0"
+            y = wrap(y, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
+            x0 = wrap(solve.x0, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
+            solve = copy_with(solve, x0=x0)
+            solution = solve_linear(f, y, solve, *f_args, grad_for_f=grad_for_f, f_kwargs=f_kwargs, **f_kwargs_)
+            return solution.native(','.join([f'batch{i}' for i in range(rank - 1)]) + ',vector')
+        else:
+            b = choose_backend(y, solve.x0, f)
+            f_dims = b.staticshape(f)
+            y_dims = b.staticshape(y)
+            x_dims = b.staticshape(solve.x0)
+            rank = len(f_dims) - 2
+            assert rank >= 0, f"f must be a matrix but got shape {f_dims}"
+            f = wrap(f, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'), dual('vector'))
+            if len(x_dims) == len(f_dims):  # matrix solve
+                assert len(x_dims) == len(f_dims)
+                assert x_dims[-2] == f_dims[-1]
+                assert y_dims[-2] == f_dims[-2]
+                y = wrap(y, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'), batch('extra_batch'))
+                x0 = wrap(solve.x0, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'), batch('extra_batch'))
+                solve = copy_with(solve, x0=x0)
+                solution = solve_linear(f, y, solve, *f_args, grad_for_f=grad_for_f, f_kwargs=f_kwargs, **f_kwargs_)
+                return solution.native(','.join([f'batch{i}' for i in range(rank - 1)]) + ',vector,extra_batch')
+            else:
+                assert len(x_dims) == len(f_dims) - 1
+                assert x_dims[-1] == f_dims[-1]
+                assert y_dims[-1] == f_dims[-2]
+                y = wrap(y, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
+                x0 = wrap(solve.x0, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
+                solve = copy_with(solve, x0=x0)
+                solution = solve_linear(f, y, solve, *f_args, grad_for_f=grad_for_f, f_kwargs=f_kwargs, **f_kwargs_)
+                return solution.native(','.join([f'batch{i}' for i in range(rank - 1)]) + ',vector')
     backend = choose_backend_t(*y_tensors, *x0_tensors)
     prefer_explicit = backend.supports(Backend.sparse_coo_tensor) or backend.supports(Backend.csr_matrix) or grad_for_f
 
     if isinstance(f, Tensor) or (isinstance(f, LinearFunction) and prefer_explicit):  # Matrix solve
         if isinstance(f, LinearFunction):
             matrix, bias = f.sparse_matrix_and_bias(solve.x0, *f_args, **f_kwargs)
         else:
```

### Comparing `unifyml-0.0.1/unifyml/math/_shape.py` & `unifyml-0.0.2/unifyml/math/_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,15 +507,15 @@
             dim_size = self.get_size(dim)
         else:
             inner = self
             dim_size = self.shape.get_size(dim)
         sizes = []
         for size in inner.sizes:
             if isinstance(size, Tensor) and dim in size.shape:
-                sizes.append(size.unstack(dim))
+                sizes.append(size._unstack(dim))
                 dim_size = size.shape.get_size(dim)
             else:
                 sizes.append(size)
         assert isinstance(dim_size, int)
         shapes = tuple(Shape(tuple([int(size[i]) if isinstance(size, tuple) else size for size in sizes]), inner.names, inner.types, inner.item_names) for i in range(dim_size))
         return shapes
```

### Comparing `unifyml-0.0.1/unifyml/math/_sparse.py` & `unifyml-0.0.2/unifyml/math/_sparse.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml/math/_tensors.py` & `unifyml-0.0.2/unifyml/math/_tensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,33 +441,21 @@
 
         """
         raise NotImplementedError()
 
     def __setitem__(self, key, value):
         raise SyntaxError("Tensors are not editable to preserve the autodiff chain. This feature might be added in the future. To update part of a tensor, use math.where() or math.scatter()")
 
-    def flip(self, *dims: str) -> 'Tensor':
-        """
-        Reverses the order of elements along one or multiple dimensions.
-
-        Args:
-            *dims: dimensions to flip
-
-        Returns:
-            `Tensor` of the same `Shape`
-        """
-        raise NotImplementedError()
-
     def __unstack__(self, dims: Tuple[str, ...]) -> Tuple['Tensor', ...]:  # from unifyml.math.magic.Sliceable
         if len(dims) == 1:
-            return self.unstack(dims[0])
+            return self._unstack(dims[0])
         else:
             return NotImplemented
 
-    def unstack(self, dim: str):
+    def _unstack(self, dim: str):
         """
         Splits this tensor along the specified dimension.
         The returned tensors have the same dimensions as this tensor save the unstacked dimension.
 
         Raises an error if the dimension is not part of the `Shape` of this `Tensor`.
 
         See Also:
@@ -851,19 +839,14 @@
         new_shape = Shape(shape.sizes, tuple(new_names), tuple(new_types), shape.item_names)
         return self.tensor._with_shape_replaced(new_shape)
 
     @property
     def index(self):
         return self.tensor.shape.index(self.name)
 
-    def flip(self):
-        """ Flips the element order along this dimension and returns the result as a `Tensor`. """
-        warnings.warn("dim.flip() is deprecated. Use dim[::-1] instead", DeprecationWarning, stacklevel=2)
-        return self.tensor.flip(self.name)
-
     def split(self, split_dimensions: Shape):
         """ See `unifyml.math.unpack_dim()` """
         warnings.warn("dim.split() is deprecated. Use math.split_dims() instead.", stacklevel=2)
         from ._magic_ops import unpack_dim
         return unpack_dim(self.tensor, self.name, split_dimensions)
 
     def __mul__(self, other):
@@ -953,15 +936,15 @@
         return repr(self._obj)
 
     def __format__(self, format_spec):
         if BROADCAST_FORMATTER.values is not None:
             return BROADCAST_FORMATTER.register_formatted(self, format_spec)
         return repr(self._obj)
 
-    def unstack(self, dimension: str):
+    def _unstack(self, dimension: str):
         if dimension == self._shape.names[0]:
             native = tuple(self._obj.values()) if isinstance(self._obj, dict) else self._obj
             inner_shape = self._shape[1:]
             return tuple([Layout(n, inner_shape) for n in native])
         else:
             raise NotImplementedError()
 
@@ -1244,20 +1227,15 @@
             elif name not in self._shape:
                 assert isinstance(sel, int), f"Attempting slice missing dimension {name} with {selection}"
         gathered = self.default_backend.multi_slice(self._native, tuple(selections)) if selections else self._native
         new_native_shape = self._native_shape.after_gather(selection)
         new_shape = self._shape.after_gather(selection)
         return NativeTensor(gathered, new_native_shape, new_shape)
 
-    def flip(self, *dims: str) -> 'Tensor':
-        native_dims = [dim for dim in dims if dim in self._native_shape]
-        native = self.default_backend.flip(self._native, self._native_shape.indices(native_dims))
-        return NativeTensor(native, self._native_shape.flipped(native_dims), self._shape.flipped(dims))
-
-    def unstack(self, dim):
+    def _unstack(self, dim):
         new_shape = self._shape.without(dim)
         new_native_shape = self._native_shape.without(dim)
         if dim in self._native_shape:
             tensors = self.default_backend.unstack(self._native, axis=self._native_shape.index(dim))
             return tuple([NativeTensor(t, new_native_shape, new_shape) for t in tensors])
         else:
             assert dim in self._shape, f"Cannot unstack tensor {self._shape} along non-existant dimension '{dim}'"
@@ -1346,15 +1324,15 @@
                 natives = [t.native(order=self._shape.names) for t in self._tensors]
                 native = choose_backend(*natives).concat(natives, axis=self.shape.index(self._stack_dim.name))
                 self._cached = NativeTensor(native, self._shape)
             else:  # cache stack_dim on inner tensors
                 non_uniform_dim = self._tensors[0].shape.shape.without('dims')
                 if len(non_uniform_dim) > 1:
                     raise NotImplementedError
-                unstacked = [t.unstack(non_uniform_dim.name) for t in self._tensors]
+                unstacked = [t._unstack(non_uniform_dim.name) for t in self._tensors]
                 stacked = []
                 for to_stack in zip(*unstacked):
                     tensor = TensorStack(to_stack, self._stack_dim)._cache()
                     stacked.append(tensor)
                 self._cached = TensorStack(stacked, non_uniform_dim)
         return self._cached
 
@@ -1411,47 +1389,38 @@
             elif isinstance(selection, slice):
                 return TensorStack(tensors[selection], self._stack_dim)
             else:
                 raise NotImplementedError(f"{type(selection)} not supported. Only (int, slice) allwoed")
         else:
             return TensorStack(tensors, self._stack_dim)
 
-    def flip(self, *dims: str) -> 'Tensor':
-        if self._cached is not None:
-            return self._cached.flip(*dims)
-        else:
-            tensors = [t.flip(*dims) for t in self._tensors]
-            if self._stack_dim.name in dims:
-                tensors = tensors[::-1]
-            return TensorStack(tensors, self._stack_dim)
-
-    def unstack(self, dimension):
+    def _unstack(self, dim):
         if self._cached is not None:
-            return self._cached.unstack(dimension)
-        if dimension == self._stack_dim.name:
+            return self._cached._unstack(dim)
+        if dim == self._stack_dim.name:
             return self._tensors
         else:
             if self.requires_broadcast:
-                unstacked = [t.unstack(dimension) for t in self._tensors]
+                unstacked = [t._unstack(dim) for t in self._tensors]
                 return tuple([TensorStack(items, self._stack_dim) for items in zip(*unstacked)])
             else:
-                return self._cache().unstack(dimension)
+                return self._cache()._unstack(dim)
 
     def _op1(self, native_function):
         if self.requires_broadcast:
             tensors = [t._op1(native_function) for t in self._tensors]
             return TensorStack(tensors, self._stack_dim)
         else:
             return self._cache()._op1(native_function)
 
     def _op2(self, other, operator, native_function, op_name: str = 'unknown', op_symbol: str = '?'):
         other = self._tensor(other)
         if self.requires_broadcast:
             if self._stack_dim.name in other.shape:
-                other = other.unstack(self._stack_dim.name)
+                other = other._unstack(self._stack_dim.name)
                 tensors = [operator(t1, t2) for t1, t2 in zip(self._tensors, other)]
             else:
                 tensors = [operator(t, other) for t in self._tensors]
             return TensorStack(tensors, self._stack_dim)
         elif isinstance(other, NativeTensor) or (isinstance(other, TensorStack) and not other.requires_broadcast):
             new_shape, (native1, native2) = broadcastable_native_tensors(self, other)  # ToDo we don't have to expand all
             result_tensor = native_function(native1, native2)
```

### Comparing `unifyml-0.0.1/unifyml/math/_trace.py` & `unifyml-0.0.2/unifyml/math/_trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                     values = math.expand(values, self._shape.only(dim))  # dim order may be scrambled
                 if delta:
                     shift = shift._replace_single_size(dim, shift.get_size(dim) + delta) if dim in shift else shift._expand(spatial(**{dim: delta}))
             val[shift.only(sorted(shift.names), reorder=True)] = val_fun(values)
         bias = bias_fun(self.bias)
         return ShiftLinTracer(self.source, val, new_shape, bias)
 
-    def unstack(self, dimension):
+    def _unstack(self, dimension):
         raise NotImplementedError()
 
     def __neg__(self):
         return ShiftLinTracer(self.source, {shift: -values for shift, values in self.val.items()}, self._shape, -self.bias)
 
     def _op1(self, native_function):
         # __neg__ is the only proper linear op1 and is implemented above.
@@ -281,15 +281,15 @@
             sparsify_batch = not target_backend.supports(Backend.csr_matrix_batched)
         else:
             sparsify_batch = not target_backend.supports(Backend.sparse_coo_tensor_batched)
     matrix, bias = tracer_to_coo(tracer, sparsify_batch, separate_independent)
     # --- Compress ---
     if not auto_compress:
         return matrix, bias
-    if matrix.default_backend.supports(Backend.mul_csr_dense) and target_backend.supports(Backend.mul_csr_dense):
+    if matrix.default_backend.supports(Backend.mul_csr_dense) and target_backend.supports(Backend.mul_csr_dense) and isinstance(matrix, SparseCoordinateTensor):
         return matrix.compress_rows(), bias
     # elif backend.supports(Backend.mul_csc_dense):
     #     return matrix.compress_cols(), tracer.bias
     else:
         return matrix, bias
```

### Comparing `unifyml-0.0.1/unifyml/math/extrapolation.py` & `unifyml-0.0.2/unifyml/math/extrapolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,18 @@
     def to_dict(self) -> dict:
         return {'type': repr(self)}
 
     @property
     def backend_pad_mode(self) -> Optional[str]:
         return repr(self)
 
+    @property
+    def native_grid_sample_mode(self) -> Union[str, None]:
+        return str(self)
+
     def __value_attrs__(self):
         return ()
 
     def valid_outer_faces(self, dim) -> Tuple[bool, bool]:
         return True, True
 
     @property
@@ -426,18 +430,14 @@
             return self._pad_linear_tracer(value, widths)
         else:
             raise NotImplementedError(f'{type(value)} not supported')
 
     def _pad_linear_tracer(self, value, widths: dict):
         raise NotImplementedError()
 
-    @property
-    def native_grid_sample_mode(self) -> Union[str, None]:
-        return str(self)
-
     def __eq__(self, other):
         return type(other) == type(self)
 
     def __hash__(self):
         return hash(self.__class__)
 
     def _op(self, other, op):
@@ -495,14 +495,18 @@
     def __repr__(self):
         return 'zero-gradient'
 
     @property
     def backend_pad_mode(self) -> Optional[str]:
         return 'boundary'
 
+    @property
+    def native_grid_sample_mode(self) -> Union[str, None]:
+        return 'boundary'
+
     def spatial_gradient(self):
         return ZERO
 
     @property
     def is_flexible(self) -> bool:
         return True
 
@@ -633,17 +637,17 @@
 
     def transform_coordinates(self, coordinates: Tensor, shape: Shape, **kwargs) -> Tensor:
         coordinates = coordinates % (2 * shape)
         return ((2 * shape - 1) - abs((2 * shape - 1) - 2 * coordinates)) // 2
 
     def pad_values(self, value: Tensor, width: int, dim: str, upper_edge: bool, **kwargs) -> Tensor:
         if upper_edge:
-            return value[{dim: slice(-width, None)}].flip(dim)
+            return value[{dim: slice(-1, -width-1, -1)}]
         else:
-            return value[{dim: slice(0, width)}].flip(dim)
+            return value[{dim: slice(width-1, None, -1)}]
 
     def _pad_linear_tracer(self, value: 'ShiftLinTracer', widths: dict) -> 'ShiftLinTracer':
         """
         *Warning*:
         This implementation discards corners, i.e. values that lie outside the original tensor in more than one dimension.
         These are typically sliced off in differential operators. Corners are instead assigned the value 0.
         To take corners into account, call pad() for each axis individually. This is inefficient with ShiftLinTracer.
@@ -749,17 +753,17 @@
 
     @property
     def is_flexible(self) -> bool:
         return True
 
     def pad_values(self, value: Tensor, width: int, dim: str, upper_edge: bool, **kwargs) -> Tensor:
         if upper_edge:
-            return value[{dim: slice(-1-width, -1)}].flip(dim)
+            return value[{dim: slice(-2, -2-width, -1)}]
         else:
-            return value[{dim: slice(1, width+1)}].flip(dim)
+            return value[{dim: slice(width, 0, -1)}]
 
     def transform_coordinates(self, coordinates: Tensor, shape: Shape, **kwargs) -> Tensor:
         coordinates = coordinates % (2 * shape - 2)
         return (shape - 1) - math.abs_((shape - 1) - coordinates)
 
     def _pad_linear_tracer(self, value: 'ShiftLinTracer', widths: dict) -> 'ShiftLinTracer':
         """
```

### Comparing `unifyml-0.0.1/unifyml/math/magic.py` & `unifyml-0.0.2/unifyml/math/magic.py`

 * *Files identical despite different names*

### Comparing `unifyml-0.0.1/unifyml.egg-info/SOURCES.txt` & `unifyml-0.0.2/unifyml.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+unifyml/VERSION
 unifyml/__init__.py
 unifyml/_troubleshoot.py
+unifyml/nn.py
 unifyml.egg-info/PKG-INFO
 unifyml.egg-info/SOURCES.txt
 unifyml.egg-info/dependency_links.txt
 unifyml.egg-info/requires.txt
 unifyml.egg-info/top_level.txt
 unifyml/backend/__init__.py
 unifyml/backend/_backend.py
@@ -18,22 +20,21 @@
 unifyml/backend/_numpy_backend.py
 unifyml/backend/_object.py
 unifyml/backend/_partition.py
 unifyml/backend/_profile.py
 unifyml/backend/_triangular_wip.py
 unifyml/backend/jax/__init__.py
 unifyml/backend/jax/_jax_backend.py
-unifyml/backend/jax/stax/__init__.py
-unifyml/backend/jax/stax/nets.py
-unifyml/backend/tf/__init__.py
-unifyml/backend/tf/_compile_cuda.py
-unifyml/backend/tf/_profiling.py
-unifyml/backend/tf/_tf_backend.py
-unifyml/backend/tf/_tf_cuda_resample.py
-unifyml/backend/tf/nets.py
+unifyml/backend/jax/stax_nets.py
+unifyml/backend/tensorflow/__init__.py
+unifyml/backend/tensorflow/_compile_cuda.py
+unifyml/backend/tensorflow/_profiling.py
+unifyml/backend/tensorflow/_tf_backend.py
+unifyml/backend/tensorflow/_tf_cuda_resample.py
+unifyml/backend/tensorflow/nets.py
 unifyml/backend/torch/__init__.py
 unifyml/backend/torch/_torch_backend.py
 unifyml/backend/torch/nets.py
 unifyml/math/__init__.py
 unifyml/math/_fit.py
 unifyml/math/_functional.py
 unifyml/math/_magic_ops.py
```

