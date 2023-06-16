# Comparing `tmp/scanoss_winnowing-0.1.0.tar.gz` & `tmp/scanoss_winnowing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanoss_winnowing-0.1.0.tar", last modified: Wed Mar  1 14:27:55 2023, max compression
+gzip compressed data, was "scanoss_winnowing-0.2.0.tar", last modified: Fri Jun 16 13:04:34 2023, max compression
```

## Comparing `scanoss_winnowing-0.1.0.tar` & `scanoss_winnowing-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:27:55.807136 scanoss_winnowing-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-01 14:27:55.807136 scanoss_winnowing-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-01 14:27:55.807136 scanoss_winnowing-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:27:55.803136 scanoss_winnowing-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:27:55.803136 scanoss_winnowing-0.1.0/src/scanoss_winnowing/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing/_winnowing.c
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-03-01 14:27:29.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing/winnowing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:27:55.807136 scanoss_winnowing-0.1.0/src/scanoss_winnowing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-01 14:27:55.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-01 14:27:55.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:27:55.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 14:27:55.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-01 14:27:55.000000 scanoss_winnowing-0.1.0/src/scanoss_winnowing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:34.559440 scanoss_winnowing-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-16 13:04:34.559440 scanoss_winnowing-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 13:04:34.559440 scanoss_winnowing-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:34.555441 scanoss_winnowing-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:34.555441 scanoss_winnowing-0.2.0/src/scanoss_winnowing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing/_winnowing.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-06-16 13:04:07.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing/winnowing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:04:34.559440 scanoss_winnowing-0.2.0/src/scanoss_winnowing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-16 13:04:34.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 13:04:34.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:04:34.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 13:04:34.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 13:04:34.000000 scanoss_winnowing-0.2.0/src/scanoss_winnowing.egg-info/top_level.txt
```

### Comparing `scanoss_winnowing-0.1.0/LICENSE` & `scanoss_winnowing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scanoss_winnowing-0.1.0/PACKAGE.md` & `scanoss_winnowing-0.2.0/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `scanoss_winnowing-0.1.0/PKG-INFO` & `scanoss_winnowing-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss_winnowing
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python Library implementing a C version of the SCANOSS Winnowing algorithm
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss-winnowing.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss-winnowing.py/issues
```

### Comparing `scanoss_winnowing-0.1.0/README.md` & `scanoss_winnowing-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # SCANOSS Winnowing Python Library
 The SCANOSS Winnowing python package provides fast implementation of the winnowing algorithm.
 This is achieved using a C code implementation to generate the snippet IDs.
 
+[![Local Build/Test](https://github.com/scanoss/scanoss-winnowing.py/actions/workflows/python-local-test.yml/badge.svg)](https://github.com/scanoss/scanoss-winnowing.py/actions/workflows/python-local-test.yml)
+[![Publish Python Package - PyPI](https://github.com/scanoss/scanoss-winnowing.py/actions/workflows/python-publish-pypi.yml/badge.svg)](https://github.com/scanoss/scanoss-winnowing.py/actions/workflows/python-publish-pypi.yml)
+
 ## Installation
 To install (from [pypi.org](https://pypi.org/project/scanoss_winnowing)), please run:
 ```bash
 pip3 install scanoss_winnowing
 ```
 
 ## Usage
```

### Comparing `scanoss_winnowing-0.1.0/setup.cfg` & `scanoss_winnowing-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scanoss_winnowing-0.1.0/src/scanoss_winnowing/__init__.py` & `scanoss_winnowing-0.2.0/src/scanoss_winnowing/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,8 +18,8 @@
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

### Comparing `scanoss_winnowing-0.1.0/src/scanoss_winnowing/_winnowing.c` & `scanoss_winnowing-0.2.0/src/scanoss_winnowing/_winnowing.c`

 * *Files identical despite different names*

### Comparing `scanoss_winnowing-0.1.0/src/scanoss_winnowing/winnowing.py` & `scanoss_winnowing-0.2.0/src/scanoss_winnowing/winnowing.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     ".exe", ".zip", ".tar", ".tgz", ".gz", ".7z", ".rar", ".jar", ".war", ".ear", ".class", ".pyc",
     ".o", ".a", ".so", ".obj", ".dll", ".lib", ".out", ".app", ".bin",
     ".lst", ".dat", ".json", ".htm", ".html", ".xml", ".md", ".txt",
     ".doc", ".docx", ".xls", ".xlsx", ".ppt", ".pptx", ".odt", ".ods", ".odp", ".pages", ".key", ".numbers",
     ".pdf", ".min.js", ".mf", ".sum"
 }
 
+CRC8_MAXIM_DOW_TABLE_SIZE = 0x100
+CRC8_MAXIM_DOW_POLYNOMIAL = 0x8C # 0x31 reflected
+CRC8_MAXIM_DOW_INITIAL = 0x00 # 0x00 reflected
+CRC8_MAXIM_DOW_FINAL = 0x00 # 0x00 reflected
 
 class Winnowing:
     """
     Winnowing Algorithm implementation for SCANOSS.
 
     This module implements an adaptation of the original winnowing algorithm by
     S. Schleimer, D. S. Wilkerson and A. Aiken as described in their seminal article which can be found here:
@@ -101,15 +105,15 @@
     Where component is the MD5 hash and path of the component container (could be a path to a compressed file or URL).
     file is the MD5 hash, file length and file path being fingerprinted, followed by
     a list of WFP fingerprints with their corresponding line numbers.
     """
 
     def __init__(self, size_limit: bool = True, debug: bool = False, trace: bool = False, quiet: bool = False,
                  skip_snippets: bool = False, post_size: int = 64, all_extensions: bool = False,
-                 obfuscate: bool = False, c_accelerated: bool = True
+                 obfuscate: bool = False, hpsm: bool = False, c_accelerated: bool = True
                  ):
         """
         Instantiate Winnowing class
         :param size_limit: Limit the size of a fingerprint to 64k (post size) - default True
         :param debug: Enable debug - default False
         :param trace: Enable trace - default False
         :param quiet: Force quiet mode - default False
@@ -126,14 +130,17 @@
         self.skip_snippets = skip_snippets
         self.max_post_size = post_size * 1024 if post_size > 0 else MAX_POST_SIZE
         self.all_extensions = all_extensions
         self.c_accelerated = c_accelerated
         self.obfuscate = obfuscate
         self.ob_count = 1
         self.file_map = {} if obfuscate else None
+        self.hpsm = hpsm
+        if hpsm:
+            self.crc8_maxim_dow_table = []
 
     @staticmethod
     def _normalize(byte):
         """
         Normalise a given byte as an ASCII character
         :param byte: The byte to normalise
         :return: integer
@@ -226,14 +233,18 @@
             self.file_map[wfp_filename] = file  # Save the file name map for later (reverse lookup)
 
         wfp = 'file={0},{1},{2}\n'.format(file_md5, content_length, wfp_filename)
         # We don't process snippets for binaries, or other uninteresting files, or if we're requested to skip
         if bin_file or self.skip_snippets or\
                 (not self.all_extensions and self.__skip_snippets(file, contents.decode('utf-8', 'ignore'))):
             return wfp
+        # Add HPSM
+        if self.hpsm:
+            hpsm = self.calc_hpsm(contents)
+            wfp += 'hpsm={0}\n'.format(hpsm)
         # Run the C implementation of the winnowing algorithm
         if self.c_accelerated:
             import _winnowing
             self.print_trace(f'Using C code...')
             res = _winnowing.compute_wfd(contents, crc32c)
             wfp = wfp + str.lstrip(b''.join(res).decode('ascii'))
             wfp_len = len(wfp.encode("utf-8"))
@@ -303,14 +314,64 @@
             else:
                 self.print_debug(f'Warning: skipping output in WFP for {file} - "{output}"')
 
         if wfp is None or wfp == '':
             self.print_stderr(f'Warning: No WFP content data for {file}')
         return wfp
 
+    def calc_hpsm(self, content):
+        list_normalized = []    #Array of numbers
+        crc_lines = []  #Array of numbers that represent the crc8_maxim for each line of the file
+        last_line = 0
+        self.crc8_generate_table()
+        for i, byte in enumerate(content):
+            c = byte
+            if c == ASCII_LF:   #When there is a new line
+                if len(list_normalized): 
+                    crc_lines.append(self.crc8_buffer(list_normalized))
+                    list_normalized=[]
+                elif last_line+1 == i:
+                    crc_lines.append(0xFF)
+                elif i-last_line  > 1:
+                    crc_lines.append(0x00)
+                last_line = i
+            else:
+                c_normalized = self._normalize(c)
+                if c_normalized != 0:
+                    list_normalized.append(c_normalized)
+        crc_lines_hex = []
+        for x in crc_lines:
+            crc_lines_hex.append(hex(x))
+        hpsm = ''.join('{:02x}'.format(x) for x in crc_lines)
+        return hpsm
+
+    def crc8_generate_table(self):
+        for i in range(CRC8_MAXIM_DOW_TABLE_SIZE):
+            self.crc8_maxim_dow_table.append(self.crc8_byte_checksum(0, i))
+        
+    def crc8_byte_checksum(self, crc, byte):
+        crc ^= byte
+        for count in range(8):
+            isSet = crc & 0x01
+            crc >>= 1
+            if isSet:
+                crc ^= CRC8_MAXIM_DOW_POLYNOMIAL
+        return crc
+
+    def crc8_byte(self, crc, byte):
+        index = byte ^ crc
+        return self.crc8_maxim_dow_table[ index ] ^ ( crc >> 8 )
+
+    def crc8_buffer(self, buffer):
+        crc = CRC8_MAXIM_DOW_INITIAL
+        for index in range(len(buffer)):
+            crc = self.crc8_byte(crc, buffer[index])
+        crc ^= CRC8_MAXIM_DOW_FINAL
+        return crc
+
     def print_msg(self, *args, **kwargs):
         """
         Print message if quite mode is not enabled
         """
         if not self.quiet:
             self.print_stderr(*args, **kwargs)
```

### Comparing `scanoss_winnowing-0.1.0/src/scanoss_winnowing.egg-info/PKG-INFO` & `scanoss_winnowing-0.2.0/src/scanoss_winnowing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss-winnowing
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python Library implementing a C version of the SCANOSS Winnowing algorithm
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss-winnowing.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss-winnowing.py/issues
```

