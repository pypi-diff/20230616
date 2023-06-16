# Comparing `tmp/kaldi_io-0.9.5.tar.gz` & `tmp/kaldi_io-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaldi_io-0.9.5.tar", last modified: Tue Dec 20 15:30:10 2022, max compression
+gzip compressed data, was "kaldi_io-0.9.6.tar", last modified: Fri Jun 16 12:30:23 2023, max compression
```

## Comparing `kaldi_io-0.9.5.tar` & `kaldi_io-0.9.6.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 iveselyk   (876) fit        (201)        0 2022-12-20 15:30:10.943603 kaldi_io-0.9.5/
--rw-r--r--   0 iveselyk   (876) fit        (201)    11358 2019-03-12 12:42:30.000000 kaldi_io-0.9.5/LICENSE
--rw-r--r--   0 iveselyk   (876) fit        (201)     2239 2022-12-20 15:30:10.941603 kaldi_io-0.9.5/PKG-INFO
--rw-r--r--   0 iveselyk   (876) fit        (201)     1729 2022-11-29 11:19:03.000000 kaldi_io-0.9.5/README.md
-drwxr-xr-x   0 iveselyk   (876) fit        (201)        0 2022-12-20 15:30:10.808603 kaldi_io-0.9.5/kaldi_io/
--rwxr-xr-x   0 iveselyk   (876) fit        (201)      472 2019-03-12 12:42:30.000000 kaldi_io-0.9.5/kaldi_io/__init__.py
--rwxr-xr-x   0 iveselyk   (876) fit        (201)    30390 2022-12-14 17:08:52.000000 kaldi_io-0.9.5/kaldi_io/kaldi_io.py
-drwxr-xr-x   0 iveselyk   (876) fit        (201)        0 2022-12-20 15:30:10.936603 kaldi_io-0.9.5/kaldi_io.egg-info/
--rw-r--r--   0 iveselyk   (876) fit        (201)     2239 2022-12-20 15:30:10.000000 kaldi_io-0.9.5/kaldi_io.egg-info/PKG-INFO
--rw-r--r--   0 iveselyk   (876) fit        (201)      227 2022-12-20 15:30:10.000000 kaldi_io-0.9.5/kaldi_io.egg-info/SOURCES.txt
--rw-r--r--   0 iveselyk   (876) fit        (201)        1 2022-12-20 15:30:10.000000 kaldi_io-0.9.5/kaldi_io.egg-info/dependency_links.txt
--rw-r--r--   0 iveselyk   (876) fit        (201)       14 2022-12-20 15:30:10.000000 kaldi_io-0.9.5/kaldi_io.egg-info/requires.txt
--rw-r--r--   0 iveselyk   (876) fit        (201)        9 2022-12-20 15:30:10.000000 kaldi_io-0.9.5/kaldi_io.egg-info/top_level.txt
--rw-r--r--   0 iveselyk   (876) fit        (201)       38 2022-12-20 15:30:10.944603 kaldi_io-0.9.5/setup.cfg
--rwxr-xr-x   0 iveselyk   (876) fit        (201)     1203 2022-12-20 15:29:47.000000 kaldi_io-0.9.5/setup.py
+drwxr-xr-x   0 iveselyk   (876) fit        (201)        0 2023-06-16 12:30:23.111493 kaldi_io-0.9.6/
+-rw-r--r--   0 iveselyk   (876) fit        (201)    11358 2019-03-12 12:42:30.000000 kaldi_io-0.9.6/LICENSE
+-rw-r--r--   0 iveselyk   (876) fit        (201)     2407 2023-06-16 12:30:23.109493 kaldi_io-0.9.6/PKG-INFO
+-rw-r--r--   0 iveselyk   (876) fit        (201)     1897 2023-06-16 11:10:21.000000 kaldi_io-0.9.6/README.md
+drwxr-xr-x   0 iveselyk   (876) fit        (201)        0 2023-06-16 12:30:23.053493 kaldi_io-0.9.6/kaldi_io/
+-rwxr-xr-x   0 iveselyk   (876) fit        (201)      472 2019-03-12 12:42:30.000000 kaldi_io-0.9.6/kaldi_io/__init__.py
+-rwxr-xr-x   0 iveselyk   (876) fit        (201)    30668 2023-06-16 11:10:21.000000 kaldi_io-0.9.6/kaldi_io/kaldi_io.py
+drwxr-xr-x   0 iveselyk   (876) fit        (201)        0 2023-06-16 12:30:23.089493 kaldi_io-0.9.6/kaldi_io.egg-info/
+-rw-r--r--   0 iveselyk   (876) fit        (201)     2407 2023-06-16 12:30:22.000000 kaldi_io-0.9.6/kaldi_io.egg-info/PKG-INFO
+-rw-r--r--   0 iveselyk   (876) fit        (201)      329 2023-06-16 12:30:22.000000 kaldi_io-0.9.6/kaldi_io.egg-info/SOURCES.txt
+-rw-r--r--   0 iveselyk   (876) fit        (201)        1 2023-06-16 12:30:22.000000 kaldi_io-0.9.6/kaldi_io.egg-info/dependency_links.txt
+-rw-r--r--   0 iveselyk   (876) fit        (201)       14 2023-06-16 12:30:22.000000 kaldi_io-0.9.6/kaldi_io.egg-info/requires.txt
+-rw-r--r--   0 iveselyk   (876) fit        (201)       15 2023-06-16 12:30:22.000000 kaldi_io-0.9.6/kaldi_io.egg-info/top_level.txt
+-rw-r--r--   0 iveselyk   (876) fit        (201)       38 2023-06-16 12:30:23.112493 kaldi_io-0.9.6/setup.cfg
+-rwxr-xr-x   0 iveselyk   (876) fit        (201)     1203 2023-06-16 11:17:43.000000 kaldi_io-0.9.6/setup.py
+drwxr-xr-x   0 iveselyk   (876) fit        (201)        0 2023-06-16 12:30:23.105493 kaldi_io-0.9.6/tests/
+-rw-r--r--   0 iveselyk   (876) fit        (201)        0 2023-06-16 11:00:37.000000 kaldi_io-0.9.6/tests/__init__.py
+-rw-r--r--   0 iveselyk   (876) fit        (201)      490 2019-03-12 12:42:31.000000 kaldi_io-0.9.6/tests/test_cnet_posteriors.py
+-rw-r--r--   0 iveselyk   (876) fit        (201)      898 2019-03-12 12:42:31.000000 kaldi_io-0.9.6/tests/test_compressed_feats.py
+-rw-r--r--   0 iveselyk   (876) fit        (201)     4760 2020-02-24 15:36:54.000000 kaldi_io-0.9.6/tests/test_kaldi_io.py
```

### Comparing `kaldi_io-0.9.5/LICENSE` & `kaldi_io-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kaldi_io-0.9.5/PKG-INFO` & `kaldi_io-0.9.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaldi_io
-Version: 0.9.5
+Version: 0.9.6
 Summary: Glue code connecting Kaldi data and Python.
 Home-page: https://github.com/vesis84/kaldi-io-for-python
 Author: Karel Vesely
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -57,14 +57,25 @@
   - `python setup.py install` (default python)
 - for local development use: `export PYTHONPATH=${PYTHONPATH}:<kaldi-io-dir>` in `$HOME/.bashrc`
 
 Note: it is recommended to set `$KALDI_ROOT` in your `$HOME/.bashrc` as
 `export KALDI_ROOT=<some_kaldi_dir>`, so you can read/write using
 pipes which contain kaldi binaries.
 
+#### Unit tests
+
+Unit tests are started this way:
+
+`./run_tests.sh`
+
+or by:
+
+`python3 -m unittest discover -s tests -t .`
+`python2 -m unittest discover -s tests -t .`
+
 
 #### License
 Apache License, Version 2.0 ('LICENSE-2.0.txt')
 
 #### Contact
 - If you have an extension to share, please create a pull request.
 - For feedback and suggestions, please create a GitHub 'Issue' in the project.
```

### Comparing `kaldi_io-0.9.5/README.md` & `kaldi_io-0.9.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -43,14 +43,25 @@
   - `python setup.py install` (default python)
 - for local development use: `export PYTHONPATH=${PYTHONPATH}:<kaldi-io-dir>` in `$HOME/.bashrc`
 
 Note: it is recommended to set `$KALDI_ROOT` in your `$HOME/.bashrc` as
 `export KALDI_ROOT=<some_kaldi_dir>`, so you can read/write using
 pipes which contain kaldi binaries.
 
+#### Unit tests
+
+Unit tests are started this way:
+
+`./run_tests.sh`
+
+or by:
+
+`python3 -m unittest discover -s tests -t .`
+`python2 -m unittest discover -s tests -t .`
+
 
 #### License
 Apache License, Version 2.0 ('LICENSE-2.0.txt')
 
 #### Contact
 - If you have an extension to share, please create a pull request.
 - For feedback and suggestions, please create a GitHub 'Issue' in the project.
```

### Comparing `kaldi_io-0.9.5/kaldi_io/kaldi_io.py` & `kaldi_io-0.9.6/kaldi_io/kaldi_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,17 +203,17 @@
 
      Example of writing arkfile:
      with open(ark_file,'w') as f:
          for key,vec in dict.iteritems():
              kaldi_io.write_vec_flt(f, vec, key=key)
     """
     assert(isinstance(v, np.ndarray))
-    assert(v.dtype == np.int32)
+    assert(v.dtype == np.int32), v.dtype
     fd = open_or_fd(file_or_fd, mode='wb')
-    if sys.version_info[0] == 3: assert(fd.mode == 'wb')
+    if sys.version_info[0] == 3: assert(fd.mode == 'wb'), fd.mode
     try:
         if key != '' : fd.write((key+' ').encode("latin1")) # ark-files have keys (utterance-id),
         fd.write('\0B'.encode()) # we write binary!
         # dim,
         fd.write('\4'.encode()) # int32 type,
         fd.write(struct.pack(np.dtype('int32').char, v.shape[0]))
         # data,
@@ -286,15 +286,15 @@
     return ans
 
 def _read_vec_flt_binary(fd):
     header = fd.read(3).decode()
     if header == 'FV ' : sample_size = 4 # floats
     elif header == 'DV ' : sample_size = 8 # doubles
     else : raise UnknownVectorHeader("The header contained '%s'" % header)
-    assert (sample_size > 0)
+    assert (sample_size > 0), sample_size
     # Dimension,
     assert (fd.read(1).decode() == '\4'); # int-size
     vec_size = np.frombuffer(fd.read(4), dtype='int32', count=1)[0] # vector dim
     if vec_size == 0:
         return np.array([], dtype='float32')
     # Read whole vector,
     buf = fd.read(vec_size * sample_size)
@@ -317,17 +317,17 @@
      kaldi_io.write_vec_flt(filename, vec)
 
      Example of writing arkfile:
      with open(ark_file,'w') as f:
          for key,vec in dict.iteritems():
              kaldi_io.write_vec_flt(f, vec, key=key)
     """
-    assert(isinstance(v, np.ndarray))
+    assert(isinstance(v, np.ndarray)), (type(v), v)
     fd = open_or_fd(file_or_fd, mode='wb')
-    if sys.version_info[0] == 3: assert(fd.mode == 'wb')
+    if sys.version_info[0] == 3: assert(fd.mode == 'wb'), fd.mode
     try:
         if key != '' : fd.write((key+' ').encode("latin1")) # ark-files have keys (utterance-id),
         fd.write('\0B'.encode()) # we write binary!
         # Data-type,
         if v.dtype == 'float32': fd.write('FV '.encode())
         elif v.dtype == 'float64': fd.write('DV '.encode())
         else: raise UnsupportedDataType("'%s', please use 'float32' or 'float64'" % v.dtype)
@@ -340,41 +340,43 @@
         if fd is not file_or_fd : fd.close()
 
 
 #################################################
 # Float matrices (features, transformations, ...),
 
 # Reading,
+
 def read_mat_scp(file_or_fd):
     """ generator(key,mat) = read_mat_scp(file_or_fd)
      Returns generator of (key,matrix) tuples, read according to kaldi scp.
      file_or_fd : scp, gzipped scp, pipe or opened file descriptor.
 
      Iterate the scp:
      for key,mat in kaldi_io.read_mat_scp(file):
          ...
 
      Read scp to a 'dictionary':
      d = { key:mat for key,mat in kaldi_io.read_mat_scp(file) }
     """
     fd = open_or_fd(file_or_fd)
-    try:
-        for line in fd:
+
+    for line in fd:
+        try:
             (key, rxfile) = line.decode().split(' ')
             (rxfile, range_slice) = _strip_mat_range(rxfile)
 
             # TODO, this reads whole file, and then selects the range.
             # A faster solution would be to change API of read_mat() and load just the frames we need...
             mat = read_mat(rxfile)
             if range_slice is not None: mat = (mat[range_slice]).copy() # apply the range_slice,
-            #
-
             yield key, mat
-    finally:
-        if fd is not file_or_fd : fd.close()
+        except:
+            print("WARNING: error reading matrix, key: %s, (it is skipped)" % key)
+
+    if fd is not file_or_fd: fd.close()
 
 def read_mat_ark(file_or_fd):
     """ generator(key,mat) = read_mat_ark(file_or_fd)
      Returns generator of (key,matrix) tuples, read from ark file/stream.
      file_or_fd : scp, gzipped scp, pipe or opened file descriptor.
 
      Iterate the ark:
@@ -438,29 +440,29 @@
     """
     fd = open_or_fd(file_or_fd)
     try:
         binary = fd.read(2).decode()
         if binary == '\0B' :
             mat = _read_mat_binary(fd)
         else:
-            assert(binary == ' [')
+            assert(binary == ' ['), binary
             mat = _read_mat_ascii(fd)
     finally:
         if fd is not file_or_fd: fd.close()
     return mat
 
 def _read_mat_binary(fd):
     # Data type
     header = fd.read(3).decode()
     # 'CM', 'CM2', 'CM3' are possible values,
     if header.startswith('CM'): return _read_compressed_mat(fd, header)
     elif header == 'FM ': sample_size = 4 # floats
     elif header == 'DM ': sample_size = 8 # doubles
     else: raise UnknownMatrixHeader("The header contained '%s'" % header)
-    assert(sample_size > 0)
+    assert(sample_size > 0), sample_size
     # Dimensions
     s1, rows, s2, cols = np.frombuffer(fd.read(10), dtype='int8,int32,int8,int32', count=1)[0]
     # Read whole matrix
     buf = fd.read(rows * cols * sample_size)
     if sample_size == 4 : vec = np.frombuffer(buf, dtype='float32')
     elif sample_size == 8 : vec = np.frombuffer(buf, dtype='float64')
     else : raise BadSampleSize
@@ -483,15 +485,15 @@
 
 
 def _read_compressed_mat(fd, format):
     """ Read a compressed matrix,
         see: https://github.com/kaldi-asr/kaldi/blob/master/src/matrix/compressed-matrix.h
         methods: CompressedMatrix::Read(...), CompressedMatrix::CopyToMat(...),
     """
-    assert(format == 'CM ') # The formats CM2, CM3 are not supported...
+    assert(format == 'CM '), format # The formats CM2, CM3 are not supported...
 
     # Format of header 'struct',
     global_header = np.dtype([('minvalue','float32'),('range','float32'),('num_rows','int32'),('num_cols','int32')]) # member '.format' is not written,
     per_col_header = np.dtype([('percentile_0','uint16'),('percentile_25','uint16'),('percentile_75','uint16'),('percentile_100','uint16')])
 
     # Read global header,
     globmin, globrange, rows, cols = np.frombuffer(fd.read(16), dtype=global_header, count=1)[0]
@@ -531,18 +533,18 @@
      kaldi_io.write_mat(filename, mat)
 
      Example of writing arkfile:
      with open(ark_file,'w') as f:
          for key,mat in dict.iteritems():
              kaldi_io.write_mat(f, mat, key=key)
     """
-    assert(isinstance(m, np.ndarray))
+    assert(isinstance(m, np.ndarray)), type(m)
     assert(len(m.shape) == 2), "'m' has to be 2d matrix!"
     fd = open_or_fd(file_or_fd, mode='wb')
-    if sys.version_info[0] == 3: assert(fd.mode == 'wb')
+    if sys.version_info[0] == 3: assert(fd.mode == 'wb'), fd.mode
     try:
         if key != '' : fd.write((key+' ').encode("latin1")) # ark-files have keys (utterance-id),
         fd.write('\0B'.encode()) # we write binary!
         # Data-type,
         if m.dtype == 'float32': fd.write('FM '.encode())
         elif m.dtype == 'float64': fd.write('DM '.encode())
         else: raise UnsupportedDataType("'%s', please use 'float32' or 'float64'" % m.dtype)
@@ -634,25 +636,25 @@
      and a 'float-value'. The 'float-value' can represent a probability
      or any other numeric value.
 
      Returns vector of vectors of tuples.
     """
     fd = open_or_fd(file_or_fd)
     ans=[]
-    binary = fd.read(2).decode(); assert(binary == '\0B'); # binary flag
+    binary = fd.read(2).decode(); assert(binary == '\0B'), binary # binary flag
     assert(fd.read(1).decode() == '\4'); # int-size
     outer_vec_size = np.frombuffer(fd.read(4), dtype='int32', count=1)[0] # number of frames (or bins)
 
     # Loop over 'outer-vector',
     for i in range(outer_vec_size):
         assert(fd.read(1).decode() == '\4'); # int-size
         inner_vec_size = np.frombuffer(fd.read(4), dtype='int32', count=1)[0] # number of records for frame (or bin)
         data = np.frombuffer(fd.read(inner_vec_size*10), dtype=[('size_idx','int8'),('idx','int32'),('size_post','int8'),('post','float32')], count=inner_vec_size)
-        assert(data[0]['size_idx'] == 4)
-        assert(data[0]['size_post'] == 4)
+        assert(data[0]['size_idx'] == 4), data[0]['size_idx']
+        assert(data[0]['size_post'] == 4), data[0]['size_post']
         ans.append(data[['idx','post']].tolist())
 
     if fd is not file_or_fd: fd.close()
     return ans
 
 def write_post(file_or_fd, p, key=''):
     """ write_post(f, p, key='')
@@ -678,15 +680,15 @@
      and a 'float-value'. The 'float-value' can represent a probability
      or any other numeric value.
 
     """
     assert(isinstance(p, list)), str(type(p))
     fd = open_or_fd(file_or_fd, mode='wb')
     if sys.version_info[0] == 3:
-        assert(fd.mode == 'wb')
+        assert(fd.mode == 'wb'), fd.mode
     try:
         if key != '':
             fd.write((key+' ').encode("latin1"))  # ark-files have keys (utterance-id),
         fd.write('\0B'.encode())  # we write binary!
         fd.write('\4'.encode())  # int32 type,
         fd.write(struct.pack(np.dtype('int32').char, len(p)))  # outer vec size
         inner_vec_size = None
@@ -741,22 +743,22 @@
      Binary layout is '<num-bins> <beg1> <end1> <beg2> <end2> ...'
 
      file_or_fd : file, gzipped file, pipe or opened file descriptor.
 
      Returns vector of tuples.
     """
     fd = open_or_fd(file_or_fd)
-    binary = fd.read(2).decode(); assert(binary == '\0B'); # assuming it's binary
+    binary = fd.read(2).decode(); assert(binary == '\0B'), binary # assuming it's binary
 
     assert(fd.read(1).decode() == '\4'); # int-size
     vec_size = np.frombuffer(fd.read(4), dtype='int32', count=1)[0] # number of frames (or bins)
 
     data = np.frombuffer(fd.read(vec_size*10), dtype=[('size_beg','int8'),('t_beg','float32'),('size_end','int8'),('t_end','float32')], count=vec_size)
-    assert(data[0]['size_beg'] == 4)
-    assert(data[0]['size_end'] == 4)
+    assert(data[0]['size_beg'] == 4), data[0]['size_beg']
+    assert(data[0]['size_end'] == 4), data[0]['size_end']
     ans = data[['t_beg','t_end']].tolist() # Return vector of tuples (t_beg,t_end),
 
     if fd is not file_or_fd : fd.close()
     return ans
 
 
 #################################################
```

### Comparing `kaldi_io-0.9.5/kaldi_io.egg-info/PKG-INFO` & `kaldi_io-0.9.6/kaldi_io.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaldi-io
-Version: 0.9.5
+Version: 0.9.6
 Summary: Glue code connecting Kaldi data and Python.
 Home-page: https://github.com/vesis84/kaldi-io-for-python
 Author: Karel Vesely
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -57,14 +57,25 @@
   - `python setup.py install` (default python)
 - for local development use: `export PYTHONPATH=${PYTHONPATH}:<kaldi-io-dir>` in `$HOME/.bashrc`
 
 Note: it is recommended to set `$KALDI_ROOT` in your `$HOME/.bashrc` as
 `export KALDI_ROOT=<some_kaldi_dir>`, so you can read/write using
 pipes which contain kaldi binaries.
 
+#### Unit tests
+
+Unit tests are started this way:
+
+`./run_tests.sh`
+
+or by:
+
+`python3 -m unittest discover -s tests -t .`
+`python2 -m unittest discover -s tests -t .`
+
 
 #### License
 Apache License, Version 2.0 ('LICENSE-2.0.txt')
 
 #### Contact
 - If you have an extension to share, please create a pull request.
 - For feedback and suggestions, please create a GitHub 'Issue' in the project.
```

### Comparing `kaldi_io-0.9.5/setup.py` & `kaldi_io-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Python 2 (override)
 import sys
 if sys.version_info[0] < 3: long_description = "" # avoid syntax errors (markdown is broken in python2)
 
 setuptools.setup(
     name='kaldi_io',
-    version='0.9.5',
+    version='0.9.6',
     author='Karel Vesely',
     description='Glue code connecting Kaldi data and Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/vesis84/kaldi-io-for-python',
     install_requires=[ 'numpy>=1.15.3', ],
     packages=setuptools.find_packages(),
```

