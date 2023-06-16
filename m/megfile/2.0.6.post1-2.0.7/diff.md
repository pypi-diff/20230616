# Comparing `tmp/megfile-2.0.6.post1-py3-none-any.whl.zip` & `tmp/megfile-2.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,47 +1,47 @@
-Zip file size: 108077 bytes, number of entries: 45
+Zip file size: 107875 bytes, number of entries: 45
 -rw-rw-r--  2.0 unx     5434 b- defN 23-May-25 06:42 megfile/__init__.py
 -rw-rw-r--  2.0 unx    10033 b- defN 23-May-25 06:42 megfile/cli.py
--rw-rw-r--  2.0 unx    11686 b- defN 23-Jun-16 08:51 megfile/errors.py
--rw-rw-r--  2.0 unx    11621 b- defN 23-Jun-15 07:50 megfile/fs.py
+-rw-rw-r--  2.0 unx    11349 b- defN 23-Jun-16 11:38 megfile/errors.py
+-rw-rw-r--  2.0 unx    11621 b- defN 23-Jun-16 11:26 megfile/fs.py
 -rw-rw-r--  2.0 unx    38552 b- defN 23-Jun-16 02:18 megfile/fs_path.py
--rw-rw-r--  2.0 unx     1852 b- defN 23-Jun-15 07:50 megfile/http.py
+-rw-rw-r--  2.0 unx     1852 b- defN 23-Jun-16 11:26 megfile/http.py
 -rw-rw-r--  2.0 unx     4487 b- defN 23-Jun-16 02:18 megfile/http_path.py
 -rw-rw-r--  2.0 unx     6219 b- defN 23-May-25 06:42 megfile/interfaces.py
 -rw-rw-r--  2.0 unx    29307 b- defN 23-Jun-13 05:49 megfile/pathlike.py
--rw-rw-r--  2.0 unx    12456 b- defN 23-Jun-15 07:50 megfile/s3.py
--rw-rw-r--  2.0 unx    85102 b- defN 23-Jun-16 02:18 megfile/s3_path.py
--rw-rw-r--  2.0 unx    11943 b- defN 23-Jun-15 07:50 megfile/sftp.py
--rw-rw-r--  2.0 unx    44039 b- defN 23-Jun-16 07:57 megfile/sftp_path.py
+-rw-rw-r--  2.0 unx    12456 b- defN 23-Jun-16 11:26 megfile/s3.py
+-rw-rw-r--  2.0 unx    84902 b- defN 23-Jun-16 11:38 megfile/s3_path.py
+-rw-rw-r--  2.0 unx    11943 b- defN 23-Jun-16 11:26 megfile/sftp.py
+-rw-rw-r--  2.0 unx    44133 b- defN 23-Jun-16 11:38 megfile/sftp_path.py
 -rw-rw-r--  2.0 unx    31952 b- defN 23-Jun-13 05:49 megfile/smart.py
 -rw-rw-r--  2.0 unx     6708 b- defN 23-Jun-16 02:18 megfile/smart_path.py
--rw-rw-r--  2.0 unx      559 b- defN 23-Jun-15 07:50 megfile/stdio.py
+-rw-rw-r--  2.0 unx      559 b- defN 23-Jun-16 11:26 megfile/stdio.py
 -rw-rw-r--  2.0 unx     2682 b- defN 23-Jun-16 02:18 megfile/stdio_path.py
--rw-rw-r--  2.0 unx       25 b- defN 23-Jun-16 10:24 megfile/version.py
+-rw-rw-r--  2.0 unx       19 b- defN 23-Jun-16 11:55 megfile/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-25 06:42 megfile/lib/__init__.py
--rw-rw-r--  2.0 unx     4580 b- defN 23-Jun-15 07:50 megfile/lib/combine_reader.py
+-rw-rw-r--  2.0 unx     4580 b- defN 23-Jun-16 11:26 megfile/lib/combine_reader.py
 -rw-rw-r--  2.0 unx     2233 b- defN 23-Jun-13 05:49 megfile/lib/compare.py
 -rw-rw-r--  2.0 unx     3053 b- defN 23-Jun-13 05:49 megfile/lib/compat.py
 -rw-rw-r--  2.0 unx     4054 b- defN 23-May-25 06:42 megfile/lib/fnmatch.py
 -rw-rw-r--  2.0 unx     9514 b- defN 23-Jun-15 06:20 megfile/lib/glob.py
 -rw-rw-r--  2.0 unx      929 b- defN 23-May-25 06:42 megfile/lib/joinpath.py
 -rw-rw-r--  2.0 unx     1915 b- defN 23-May-25 06:42 megfile/lib/lazy_handler.py
 -rw-rw-r--  2.0 unx     6934 b- defN 23-May-25 06:42 megfile/lib/s3_buffered_writer.py
 -rw-rw-r--  2.0 unx     1322 b- defN 23-May-25 06:42 megfile/lib/s3_cached_handler.py
 -rw-rw-r--  2.0 unx     6057 b- defN 23-May-25 06:42 megfile/lib/s3_limited_seekable_writer.py
 -rw-rw-r--  2.0 unx     3725 b- defN 23-May-25 06:42 megfile/lib/s3_memory_handler.py
 -rw-rw-r--  2.0 unx     3404 b- defN 23-May-25 06:42 megfile/lib/s3_pipe_handler.py
 -rw-rw-r--  2.0 unx    15053 b- defN 23-May-25 06:42 megfile/lib/s3_prefetch_reader.py
--rw-rw-r--  2.0 unx     3791 b- defN 23-Jun-15 07:50 megfile/lib/s3_share_cache_reader.py
+-rw-rw-r--  2.0 unx     3791 b- defN 23-Jun-16 11:26 megfile/lib/s3_share_cache_reader.py
 -rw-rw-r--  2.0 unx     2683 b- defN 23-May-25 06:42 megfile/lib/shadow_handler.py
 -rw-rw-r--  2.0 unx     2044 b- defN 23-May-25 06:42 megfile/lib/stdio_handler.py
 -rw-rw-r--  2.0 unx      103 b- defN 23-Jun-16 02:18 megfile/lib/url.py
 -rw-rw-r--  2.0 unx     9025 b- defN 23-May-25 06:42 megfile/utils/__init__.py
 -rw-rw-r--  2.0 unx     2461 b- defN 23-May-25 06:42 megfile/utils/mutex.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-16 10:25 megfile-2.0.6.post1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1080 b- defN 23-Jun-16 10:25 megfile-2.0.6.post1.dist-info/LICENSE.pyre
--rw-rw-r--  2.0 unx    10160 b- defN 23-Jun-16 10:25 megfile-2.0.6.post1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 10:25 megfile-2.0.6.post1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       49 b- defN 23-Jun-16 10:25 megfile-2.0.6.post1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jun-16 10:25 megfile-2.0.6.post1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3645 b- defN 23-Jun-16 10:25 megfile-2.0.6.post1.dist-info/RECORD
-45 files, 423928 bytes uncompressed, 102363 bytes compressed:  75.9%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-16 11:56 megfile-2.0.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1080 b- defN 23-Jun-16 11:56 megfile-2.0.7.dist-info/LICENSE.pyre
+-rw-rw-r--  2.0 unx    10154 b- defN 23-Jun-16 11:56 megfile-2.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 11:56 megfile-2.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       49 b- defN 23-Jun-16 11:56 megfile-2.0.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jun-16 11:56 megfile-2.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3603 b- defN 23-Jun-16 11:56 megfile-2.0.7.dist-info/RECORD
+45 files, 423431 bytes uncompressed, 102245 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -108,29 +108,29 @@
 
 Filename: megfile/utils/__init__.py
 Comment: 
 
 Filename: megfile/utils/mutex.py
 Comment: 
 
-Filename: megfile-2.0.6.post1.dist-info/LICENSE
+Filename: megfile-2.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: megfile-2.0.6.post1.dist-info/LICENSE.pyre
+Filename: megfile-2.0.7.dist-info/LICENSE.pyre
 Comment: 
 
-Filename: megfile-2.0.6.post1.dist-info/METADATA
+Filename: megfile-2.0.7.dist-info/METADATA
 Comment: 
 
-Filename: megfile-2.0.6.post1.dist-info/WHEEL
+Filename: megfile-2.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: megfile-2.0.6.post1.dist-info/entry_points.txt
+Filename: megfile-2.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: megfile-2.0.6.post1.dist-info/top_level.txt
+Filename: megfile-2.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: megfile-2.0.6.post1.dist-info/RECORD
+Filename: megfile-2.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## megfile/errors.py

```diff
@@ -1,12 +1,12 @@
 import time
 from contextlib import contextmanager
 from functools import wraps
 from logging import getLogger
-from typing import Callable, Optional
+from typing import Callable, List, Optional
 
 import botocore.exceptions
 import requests.exceptions
 import urllib3.exceptions
 from botocore.exceptions import ClientError, NoCredentialsError, ParamValidationError
 from requests.exceptions import HTTPError
 
@@ -130,32 +130,26 @@
         retry_callback: Optional[Callable] = None):
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         if before_callback is not None:
             before_callback(*args, **kwargs)
 
-        error = None
         for retries in range(1, max_retries + 1):
             try:
                 result = func(*args, **kwargs)
                 if after_callback is not None:
                     result = after_callback(result, *args, **kwargs)
-                if error is not None:
-                    _logger.debug(  # pragma: no cover
-                        'unknown error resolved: %s, with %d tries' %
-                        (full_error_message(error), retries))
                 return result
-            except EOFError as eof_exception:
-                raise eof_exception  # pragma: no cover
-            except Exception as exception:
+            except Exception as error:
+                if not should_retry(error):
+                    raise
                 if retry_callback is not None:
                     retry_callback(error, *args, **kwargs)
-                error = exception
-                if retries == max_retries or not should_retry(error):
+                if retries == max_retries:
                     raise
                 retry_interval = min(0.1 * 2**retries, 30)
                 _logger.debug(
                     'unknown error encountered: %s, retry in %0.1f seconds after %d tries'
                     % (full_error_message(error), retry_interval, retries))
                 time.sleep(retry_interval)
```

## megfile/s3_path.py

```diff
@@ -219,5101 +219,5089 @@
 00000da0: 6572 6174 696f 6e5f 6e61 6d65 290a 2020  eration_name).  
 00000db0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
 00000dc0: 756c 740a 0a20 2020 2064 6566 2072 6574  ult..    def ret
 00000dd0: 7279 5f63 616c 6c62 6163 6b28 6572 726f  ry_callback(erro
 00000de0: 722c 206f 7065 7261 7469 6f6e 5f6d 6f64  r, operation_mod
 00000df0: 656c 2c20 7265 7175 6573 745f 6469 6374  el, request_dict
 00000e00: 2c20 7265 7175 6573 745f 636f 6e74 6578  , request_contex
-00000e10: 7429 3a0a 2020 2020 2020 2020 6966 2065  t):.        if e
-00000e20: 7272 6f72 2069 7320 4e6f 6e65 3a20 2023  rror is None:  #
-00000e30: 2072 6574 7279 2066 6f72 2074 6865 2066   retry for the f
-00000e40: 6972 7374 2074 696d 650a 2020 2020 2020  irst time.      
-00000e50: 2020 2020 2020 6572 726f 725f 6c6f 6767        error_logg
-00000e60: 6572 2e64 6562 7567 280a 2020 2020 2020  er.debug(.      
-00000e70: 2020 2020 2020 2020 2020 2766 6169 6c65            'faile
-00000e80: 6420 746f 2070 726f 6365 7373 3a20 2572  d to process: %r
-00000e90: 2c20 7769 7468 2070 6172 616d 6574 6572  , with parameter
-00000ea0: 733a 2025 7327 2c0a 2020 2020 2020 2020  s: %s',.        
-00000eb0: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-00000ec0: 6e5f 6d6f 6465 6c2e 6e61 6d65 2c20 7265  n_model.name, re
-00000ed0: 7175 6573 745f 6469 6374 290a 2020 2020  quest_dict).    
-00000ee0: 2020 2020 6966 2069 735f 7265 6164 6162      if is_readab
-00000ef0: 6c65 2872 6571 7565 7374 5f64 6963 745b  le(request_dict[
-00000f00: 2762 6f64 7927 5d29 3a0a 2020 2020 2020  'body']):.      
-00000f10: 2020 2020 2020 7265 7175 6573 745f 6469        request_di
-00000f20: 6374 5b27 626f 6479 275d 2e73 6565 6b28  ct['body'].seek(
-00000f30: 3029 0a0a 2020 2020 6465 6620 6265 666f  0)..    def befo
-00000f40: 7265 5f63 616c 6c62 6163 6b28 6f70 6572  re_callback(oper
-00000f50: 6174 696f 6e5f 6d6f 6465 6c2c 2072 6571  ation_model, req
-00000f60: 7565 7374 5f64 6963 742c 2072 6571 7565  uest_dict, reque
-00000f70: 7374 5f63 6f6e 7465 7874 293a 0a20 2020  st_context):.   
-00000f80: 2020 2020 205f 6c6f 6767 6572 2e64 6562       _logger.deb
-00000f90: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
-00000fa0: 2773 656e 6420 7333 2072 6571 7565 7374  'send s3 request
-00000fb0: 3a20 2572 2c20 7769 7468 2070 6172 616d  : %r, with param
-00000fc0: 6574 6572 733a 2025 7327 2c20 6f70 6572  eters: %s', oper
-00000fd0: 6174 696f 6e5f 6d6f 6465 6c2e 6e61 6d65  ation_model.name
-00000fe0: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-00000ff0: 7175 6573 745f 6469 6374 290a 0a20 2020  quest_dict)..   
-00001000: 2063 6c69 656e 742e 5f6d 616b 655f 7265   client._make_re
-00001010: 7175 6573 7420 3d20 7061 7463 685f 6d65  quest = patch_me
-00001020: 7468 6f64 280a 2020 2020 2020 2020 636c  thod(.        cl
-00001030: 6965 6e74 2e5f 6d61 6b65 5f72 6571 7565  ient._make_reque
-00001040: 7374 2c0a 2020 2020 2020 2020 6d61 785f  st,.        max_
-00001050: 7265 7472 6965 733d 6d61 785f 7265 7472  retries=max_retr
-00001060: 6965 732c 0a20 2020 2020 2020 2073 686f  ies,.        sho
-00001070: 756c 645f 7265 7472 793d 7333 5f73 686f  uld_retry=s3_sho
-00001080: 756c 645f 7265 7472 792c 0a20 2020 2020  uld_retry,.     
-00001090: 2020 2061 6674 6572 5f63 616c 6c62 6163     after_callbac
-000010a0: 6b3d 6166 7465 725f 6361 6c6c 6261 636b  k=after_callback
-000010b0: 2c0a 2020 2020 2020 2020 6265 666f 7265  ,.        before
-000010c0: 5f63 616c 6c62 6163 6b3d 6265 666f 7265  _callback=before
-000010d0: 5f63 616c 6c62 6163 6b2c 0a20 2020 2020  _callback,.     
-000010e0: 2020 2072 6574 7279 5f63 616c 6c62 6163     retry_callbac
-000010f0: 6b3d 7265 7472 795f 6361 6c6c 6261 636b  k=retry_callback
-00001100: 290a 2020 2020 7265 7475 726e 2063 6c69  ).    return cli
-00001110: 656e 740a 0a0a 6465 6620 7061 7273 655f  ent...def parse_
-00001120: 7333 5f75 726c 2873 335f 7572 6c3a 2050  s3_url(s3_url: P
-00001130: 6174 684c 696b 6529 202d 3e20 5475 706c  athLike) -> Tupl
-00001140: 655b 7374 722c 2073 7472 5d3a 0a20 2020  e[str, str]:.   
-00001150: 2073 335f 7572 6c20 3d20 6673 7061 7468   s3_url = fspath
-00001160: 2873 335f 7572 6c29 0a20 2020 2069 6620  (s3_url).    if 
-00001170: 6e6f 7420 6973 5f73 3328 7333 5f75 726c  not is_s3(s3_url
-00001180: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00001190: 2056 616c 7565 4572 726f 7228 274e 6f74   ValueError('Not
-000011a0: 2061 2073 3320 7572 6c3a 2025 7227 2025   a s3 url: %r' %
-000011b0: 2073 335f 7572 6c29 0a20 2020 2072 6967   s3_url).    rig
-000011c0: 6874 7061 7274 203d 2073 335f 7572 6c2e  htpart = s3_url.
-000011d0: 7370 6c69 7428 273a 2f2f 272c 206d 6178  split('://', max
-000011e0: 7370 6c69 743d 3129 5b31 5d0a 2020 2020  split=1)[1].    
-000011f0: 6275 636b 6574 6d61 7463 6820 3d20 7265  bucketmatch = re
-00001200: 2e6d 6174 6368 2827 282e 2a3f 292f 272c  .match('(.*?)/',
-00001210: 2072 6967 6874 7061 7274 290a 2020 2020   rightpart).    
-00001220: 6966 2062 7563 6b65 746d 6174 6368 2069  if bucketmatch i
-00001230: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00001240: 6275 636b 6574 203d 2072 6967 6874 7061  bucket = rightpa
-00001250: 7274 0a20 2020 2020 2020 2070 6174 6820  rt.        path 
-00001260: 3d20 2727 0a20 2020 2065 6c73 653a 0a20  = ''.    else:. 
-00001270: 2020 2020 2020 2062 7563 6b65 7420 3d20         bucket = 
-00001280: 6275 636b 6574 6d61 7463 682e 6772 6f75  bucketmatch.grou
-00001290: 7028 3129 0a20 2020 2020 2020 2070 6174  p(1).        pat
-000012a0: 6820 3d20 7269 6768 7470 6172 745b 6c65  h = rightpart[le
-000012b0: 6e28 6275 636b 6574 2920 2b20 313a 5d0a  n(bucket) + 1:].
-000012c0: 2020 2020 7265 7475 726e 2062 7563 6b65      return bucke
-000012d0: 742c 2070 6174 680a 0a0a 6465 6620 6765  t, path...def ge
-000012e0: 745f 7363 6f70 6564 5f63 6f6e 6669 6728  t_scoped_config(
-000012f0: 7072 6f66 696c 655f 6e61 6d65 3a20 4f70  profile_name: Op
-00001300: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00001310: 6e65 2920 2d3e 2044 6963 743a 0a20 2020  ne) -> Dict:.   
-00001320: 2072 6574 7572 6e20 6765 745f 7333 5f73   return get_s3_s
-00001330: 6573 7369 6f6e 280a 2020 2020 2020 2020  ession(.        
-00001340: 7072 6f66 696c 655f 6e61 6d65 3d70 726f  profile_name=pro
-00001350: 6669 6c65 5f6e 616d 6529 2e5f 7365 7373  file_name)._sess
-00001360: 696f 6e2e 6765 745f 7363 6f70 6564 5f63  ion.get_scoped_c
-00001370: 6f6e 6669 6728 290a 0a0a 406c 7275 5f63  onfig()...@lru_c
-00001380: 6163 6865 2829 0a64 6566 2077 6172 6e69  ache().def warni
-00001390: 6e67 5f65 6e64 706f 696e 745f 7572 6c28  ng_endpoint_url(
-000013a0: 6b65 793a 2073 7472 2c20 656e 6470 6f69  key: str, endpoi
-000013b0: 6e74 5f75 726c 3a20 7374 7229 3a0a 2020  nt_url: str):.  
-000013c0: 2020 5f6c 6f67 6765 722e 696e 666f 2822    _logger.info("
-000013d0: 7573 696e 6720 2573 3a20 2573 2220 2520  using %s: %s" % 
-000013e0: 286b 6579 2c20 656e 6470 6f69 6e74 5f75  (key, endpoint_u
-000013f0: 726c 2929 0a0a 0a64 6566 2067 6574 5f65  rl))...def get_e
-00001400: 6e64 706f 696e 745f 7572 6c28 7072 6f66  ndpoint_url(prof
-00001410: 696c 655f 6e61 6d65 3a20 4f70 7469 6f6e  ile_name: Option
-00001420: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2920  al[str] = None) 
-00001430: 2d3e 2073 7472 3a0a 2020 2020 2727 2747  -> str:.    '''G
-00001440: 6574 2074 6865 2065 6e64 706f 696e 7420  et the endpoint 
-00001450: 7572 6c20 6f66 2053 330a 0a20 2020 203a  url of S3..    :
-00001460: 7265 7475 726e 733a 2053 3320 656e 6470  returns: S3 endp
-00001470: 6f69 6e74 2075 726c 0a20 2020 2027 2727  oint url.    '''
-00001480: 0a20 2020 2065 6e76 6972 6f6e 5f6b 6579  .    environ_key
-00001490: 203d 2066 277b 7072 6f66 696c 655f 6e61   = f'{profile_na
-000014a0: 6d65 7d5f 5f4f 5353 5f45 4e44 504f 494e  me}__OSS_ENDPOIN
-000014b0: 5427 2e75 7070 6572 280a 2020 2020 2920  T'.upper(.    ) 
-000014c0: 6966 2070 726f 6669 6c65 5f6e 616d 6520  if profile_name 
-000014d0: 656c 7365 2027 4f53 535f 454e 4450 4f49  else 'OSS_ENDPOI
-000014e0: 4e54 270a 2020 2020 656e 7669 726f 6e5f  NT'.    environ_
-000014f0: 656e 6470 6f69 6e74 5f75 726c 203d 206f  endpoint_url = o
-00001500: 732e 656e 7669 726f 6e2e 6765 7428 656e  s.environ.get(en
-00001510: 7669 726f 6e5f 6b65 7929 0a20 2020 2069  viron_key).    i
-00001520: 6620 656e 7669 726f 6e5f 656e 6470 6f69  f environ_endpoi
-00001530: 6e74 5f75 726c 3a0a 2020 2020 2020 2020  nt_url:.        
-00001540: 7761 726e 696e 675f 656e 6470 6f69 6e74  warning_endpoint
-00001550: 5f75 726c 2865 6e76 6972 6f6e 5f6b 6579  _url(environ_key
-00001560: 2c20 656e 7669 726f 6e5f 656e 6470 6f69  , environ_endpoi
-00001570: 6e74 5f75 726c 290a 2020 2020 2020 2020  nt_url).        
-00001580: 7265 7475 726e 2065 6e76 6972 6f6e 5f65  return environ_e
-00001590: 6e64 706f 696e 745f 7572 6c0a 2020 2020  ndpoint_url.    
-000015a0: 7472 793a 0a20 2020 2020 2020 2063 6f6e  try:.        con
-000015b0: 6669 675f 656e 6470 6f69 6e74 5f75 726c  fig_endpoint_url
-000015c0: 203d 2067 6574 5f73 636f 7065 645f 636f   = get_scoped_co
-000015d0: 6e66 6967 2870 726f 6669 6c65 5f6e 616d  nfig(profile_nam
-000015e0: 653d 7072 6f66 696c 655f 6e61 6d65 292e  e=profile_name).
-000015f0: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-00001600: 2027 7333 272c 207b 7d29 2e67 6574 2827   's3', {}).get('
-00001610: 656e 6470 6f69 6e74 5f75 726c 2729 0a20  endpoint_url'). 
-00001620: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-00001630: 5f65 6e64 706f 696e 745f 7572 6c3a 0a20  _endpoint_url:. 
-00001640: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-00001650: 6e67 5f65 6e64 706f 696e 745f 7572 6c28  ng_endpoint_url(
-00001660: 277e 2f2e 6177 732f 636f 6e66 6967 272c  '~/.aws/config',
-00001670: 2063 6f6e 6669 675f 656e 6470 6f69 6e74   config_endpoint
-00001680: 5f75 726c 290a 2020 2020 2020 2020 2020  _url).          
-00001690: 2020 7265 7475 726e 2063 6f6e 6669 675f    return config_
-000016a0: 656e 6470 6f69 6e74 5f75 726c 0a20 2020  endpoint_url.   
-000016b0: 2065 7863 6570 7420 626f 746f 636f 7265   except botocore
-000016c0: 2e65 7863 6570 7469 6f6e 732e 5072 6f66  .exceptions.Prof
-000016d0: 696c 654e 6f74 466f 756e 643a 2020 2320  ileNotFound:  # 
-000016e0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-000016f0: 0a20 2020 2020 2020 2070 6173 730a 2020  .        pass.  
-00001700: 2020 7265 7475 726e 2065 6e64 706f 696e    return endpoin
-00001710: 745f 7572 6c0a 0a0a 6465 6620 6765 745f  t_url...def get_
-00001720: 7333 5f73 6573 7369 6f6e 2870 726f 6669  s3_session(profi
-00001730: 6c65 5f6e 616d 653d 4e6f 6e65 293a 0a20  le_name=None):. 
-00001740: 2020 2027 2727 4765 7420 5333 2073 6573     '''Get S3 ses
-00001750: 7369 6f6e 0a0a 2020 2020 3a72 6574 7572  sion..    :retur
-00001760: 6e73 3a20 5333 2073 6573 7369 6f6e 0a20  ns: S3 session. 
-00001770: 2020 2027 2727 0a20 2020 2072 6574 7572     '''.    retur
-00001780: 6e20 7468 7265 6164 5f6c 6f63 616c 280a  n thread_local(.
-00001790: 2020 2020 2020 2020 6627 7333 5f73 6573          f's3_ses
-000017a0: 7369 6f6e 3a7b 7072 6f66 696c 655f 6e61  sion:{profile_na
-000017b0: 6d65 7d27 2c20 626f 746f 332e 5365 7373  me}', boto3.Sess
-000017c0: 696f 6e2c 2070 726f 6669 6c65 5f6e 616d  ion, profile_nam
-000017d0: 653d 7072 6f66 696c 655f 6e61 6d65 290a  e=profile_name).
-000017e0: 0a0a 6465 6620 6765 745f 6163 6365 7373  ..def get_access
-000017f0: 5f74 6f6b 656e 2870 726f 6669 6c65 5f6e  _token(profile_n
-00001800: 616d 653d 4e6f 6e65 293a 0a20 2020 2061  ame=None):.    a
-00001810: 6363 6573 735f 6b65 795f 656e 765f 6e61  ccess_key_env_na
-00001820: 6d65 203d 2066 227b 7072 6f66 696c 655f  me = f"{profile_
-00001830: 6e61 6d65 7d5f 5f41 5753 5f41 4343 4553  name}__AWS_ACCES
-00001840: 535f 4b45 595f 4944 222e 7570 7065 7228  S_KEY_ID".upper(
-00001850: 0a20 2020 2029 2069 6620 7072 6f66 696c  .    ) if profil
-00001860: 655f 6e61 6d65 2065 6c73 6520 2241 5753  e_name else "AWS
-00001870: 5f41 4343 4553 535f 4b45 595f 4944 220a  _ACCESS_KEY_ID".
-00001880: 2020 2020 7365 6372 6574 5f6b 6579 5f65      secret_key_e
-00001890: 6e76 5f6e 616d 6520 3d20 6622 7b70 726f  nv_name = f"{pro
-000018a0: 6669 6c65 5f6e 616d 657d 5f5f 4157 535f  file_name}__AWS_
-000018b0: 5345 4352 4554 5f41 4343 4553 535f 4b45  SECRET_ACCESS_KE
-000018c0: 5922 2e75 7070 6572 280a 2020 2020 2920  Y".upper(.    ) 
-000018d0: 6966 2070 726f 6669 6c65 5f6e 616d 6520  if profile_name 
-000018e0: 656c 7365 2022 4157 535f 5345 4352 4554  else "AWS_SECRET
-000018f0: 5f41 4343 4553 535f 4b45 5922 0a20 2020  _ACCESS_KEY".   
-00001900: 2061 6363 6573 735f 6b65 7920 3d20 6f73   access_key = os
-00001910: 2e67 6574 656e 7628 6163 6365 7373 5f6b  .getenv(access_k
-00001920: 6579 5f65 6e76 5f6e 616d 6529 0a20 2020  ey_env_name).   
-00001930: 2073 6563 7265 745f 6b65 7920 3d20 6f73   secret_key = os
-00001940: 2e67 6574 656e 7628 7365 6372 6574 5f6b  .getenv(secret_k
-00001950: 6579 5f65 6e76 5f6e 616d 6529 0a20 2020  ey_env_name).   
-00001960: 2069 6620 6163 6365 7373 5f6b 6579 2061   if access_key a
-00001970: 6e64 2073 6563 7265 745f 6b65 793a 0a20  nd secret_key:. 
-00001980: 2020 2020 2020 2072 6574 7572 6e20 6163         return ac
-00001990: 6365 7373 5f6b 6579 2c20 7365 6372 6574  cess_key, secret
-000019a0: 5f6b 6579 0a0a 2020 2020 6372 6564 656e  _key..    creden
-000019b0: 7469 616c 7320 3d20 6765 745f 7333 5f73  tials = get_s3_s
-000019c0: 6573 7369 6f6e 2870 726f 6669 6c65 5f6e  ession(profile_n
-000019d0: 616d 653d 7072 6f66 696c 655f 6e61 6d65  ame=profile_name
-000019e0: 292e 6765 745f 6372 6564 656e 7469 616c  ).get_credential
-000019f0: 7328 290a 2020 2020 6966 2063 7265 6465  s().    if crede
-00001a00: 6e74 6961 6c73 3a0a 2020 2020 2020 2020  ntials:.        
-00001a10: 6966 206e 6f74 2061 6363 6573 735f 6b65  if not access_ke
-00001a20: 793a 0a20 2020 2020 2020 2020 2020 2061  y:.            a
-00001a30: 6363 6573 735f 6b65 7920 3d20 6372 6564  ccess_key = cred
-00001a40: 656e 7469 616c 732e 6163 6365 7373 5f6b  entials.access_k
-00001a50: 6579 0a20 2020 2020 2020 2069 6620 6e6f  ey.        if no
-00001a60: 7420 7365 6372 6574 5f6b 6579 3a0a 2020  t secret_key:.  
-00001a70: 2020 2020 2020 2020 2020 7365 6372 6574            secret
-00001a80: 5f6b 6579 203d 2063 7265 6465 6e74 6961  _key = credentia
-00001a90: 6c73 2e73 6563 7265 745f 6b65 790a 2020  ls.secret_key.  
-00001aa0: 2020 7265 7475 726e 2061 6363 6573 735f    return access_
-00001ab0: 6b65 792c 2073 6563 7265 745f 6b65 790a  key, secret_key.
-00001ac0: 0a0a 6465 6620 6765 745f 7333 5f63 6c69  ..def get_s3_cli
-00001ad0: 656e 7428 0a20 2020 2020 2020 2063 6f6e  ent(.        con
-00001ae0: 6669 673a 204f 7074 696f 6e61 6c5b 626f  fig: Optional[bo
-00001af0: 746f 636f 7265 2e63 6f6e 6669 672e 436f  tocore.config.Co
-00001b00: 6e66 6967 5d20 3d20 4e6f 6e65 2c0a 2020  nfig] = None,.  
-00001b10: 2020 2020 2020 6361 6368 655f 6b65 793a        cache_key:
-00001b20: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00001b30: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
-00001b40: 726f 6669 6c65 5f6e 616d 653a 204f 7074  rofile_name: Opt
-00001b50: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00001b60: 6529 3a0a 2020 2020 2727 2747 6574 2053  e):.    '''Get S
-00001b70: 3320 636c 6965 6e74 0a0a 2020 2020 3a72  3 client..    :r
-00001b80: 6574 7572 6e73 3a20 5333 2063 6c69 656e  eturns: S3 clien
-00001b90: 740a 2020 2020 2727 270a 2020 2020 6966  t.    '''.    if
-00001ba0: 2063 6163 6865 5f6b 6579 2069 7320 6e6f   cache_key is no
-00001bb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00001bc0: 7265 7475 726e 2074 6872 6561 645f 6c6f  return thread_lo
-00001bd0: 6361 6c28 0a20 2020 2020 2020 2020 2020  cal(.           
-00001be0: 2063 6163 6865 5f6b 6579 2c20 6765 745f   cache_key, get_
-00001bf0: 7333 5f63 6c69 656e 742c 2063 6f6e 6669  s3_client, confi
-00001c00: 673d 636f 6e66 6967 2c20 7072 6f66 696c  g=config, profil
-00001c10: 655f 6e61 6d65 3d70 726f 6669 6c65 5f6e  e_name=profile_n
-00001c20: 616d 6529 0a0a 2020 2020 6163 6365 7373  ame)..    access
-00001c30: 5f6b 6579 2c20 7365 6372 6574 5f6b 6579  _key, secret_key
-00001c40: 203d 2067 6574 5f61 6363 6573 735f 746f   = get_access_to
-00001c50: 6b65 6e28 7072 6f66 696c 655f 6e61 6d65  ken(profile_name
-00001c60: 290a 2020 2020 636c 6965 6e74 203d 2067  ).    client = g
-00001c70: 6574 5f73 335f 7365 7373 696f 6e28 292e  et_s3_session().
-00001c80: 636c 6965 6e74 280a 2020 2020 2020 2020  client(.        
-00001c90: 2773 3327 2c0a 2020 2020 2020 2020 656e  's3',.        en
-00001ca0: 6470 6f69 6e74 5f75 726c 3d67 6574 5f65  dpoint_url=get_e
-00001cb0: 6e64 706f 696e 745f 7572 6c28 7072 6f66  ndpoint_url(prof
-00001cc0: 696c 655f 6e61 6d65 3d70 726f 6669 6c65  ile_name=profile
-00001cd0: 5f6e 616d 6529 2c0a 2020 2020 2020 2020  _name),.        
-00001ce0: 636f 6e66 6967 3d63 6f6e 6669 672c 0a20  config=config,. 
-00001cf0: 2020 2020 2020 2061 7773 5f61 6363 6573         aws_acces
-00001d00: 735f 6b65 795f 6964 3d61 6363 6573 735f  s_key_id=access_
-00001d10: 6b65 792c 0a20 2020 2020 2020 2061 7773  key,.        aws
-00001d20: 5f73 6563 7265 745f 6163 6365 7373 5f6b  _secret_access_k
-00001d30: 6579 3d73 6563 7265 745f 6b65 792c 0a20  ey=secret_key,. 
-00001d40: 2020 2029 0a20 2020 2063 6c69 656e 7420     ).    client 
-00001d50: 3d20 5f70 6174 6368 5f6d 616b 655f 7265  = _patch_make_re
-00001d60: 7175 6573 7428 636c 6965 6e74 290a 2020  quest(client).  
-00001d70: 2020 7265 7475 726e 2063 6c69 656e 740a    return client.
-00001d80: 0a0a 6465 6620 7333 5f70 6174 685f 6a6f  ..def s3_path_jo
-00001d90: 696e 2870 6174 683a 2050 6174 684c 696b  in(path: PathLik
-00001da0: 652c 202a 6f74 6865 725f 7061 7468 733a  e, *other_paths:
-00001db0: 2050 6174 684c 696b 6529 202d 3e20 7374   PathLike) -> st
-00001dc0: 723a 0a20 2020 2027 2727 0a20 2020 2043  r:.    '''.    C
-00001dd0: 6f6e 6361 7420 3220 6f72 206d 6f72 6520  oncat 2 or more 
-00001de0: 7061 7468 2074 6f20 6120 636f 6d70 6c65  path to a comple
-00001df0: 7465 2070 6174 680a 0a20 2020 203a 7061  te path..    :pa
-00001e00: 7261 6d20 7061 7468 3a20 4769 7665 6e20  ram path: Given 
-00001e10: 7061 7468 0a20 2020 203a 7061 7261 6d20  path.    :param 
-00001e20: 6f74 6865 725f 7061 7468 733a 2050 6174  other_paths: Pat
-00001e30: 6873 2074 6f20 6265 2063 6f6e 6361 7465  hs to be concate
-00001e40: 6e61 7465 640a 2020 2020 3a72 6574 7572  nated.    :retur
-00001e50: 6e73 3a20 436f 6e63 6174 656e 6174 6564  ns: Concatenated
-00001e60: 2063 6f6d 706c 6574 6520 7061 7468 0a0a   complete path..
-00001e70: 2020 2020 2e2e 206e 6f74 6520 3a3a 0a0a      .. note ::..
-00001e80: 2020 2020 2020 2020 5468 6520 6469 6666          The diff
-00001e90: 6572 656e 6365 2062 6574 7765 656e 2074  erence between t
-00001ea0: 6869 7320 6675 6e63 7469 6f6e 2061 6e64  his function and
-00001eb0: 2060 606f 732e 7061 7468 2e6a 6f69 6e60   ``os.path.join`
-00001ec0: 6020 6973 2074 6861 7420 7468 6973 2066  ` is that this f
-00001ed0: 756e 6374 696f 6e20 6967 6e6f 7265 7320  unction ignores 
-00001ee0: 6c65 6674 2073 6964 6520 736c 6173 6820  left side slash 
-00001ef0: 2877 6869 6368 2069 6e64 6963 6174 6573  (which indicates
-00001f00: 2061 6273 6f6c 7574 6520 7061 7468 2920   absolute path) 
-00001f10: 696e 2060 606f 7468 6572 5f70 6174 6873  in ``other_paths
-00001f20: 6060 2061 6e64 2077 696c 6c20 6469 7265  `` and will dire
-00001f30: 6374 6c79 2063 6f6e 6361 742e 0a20 2020  ctly concat..   
-00001f40: 2020 2020 2065 2e67 2e20 6f73 2e70 6174       e.g. os.pat
-00001f50: 682e 6a6f 696e 2827 2f70 6174 6827 2c20  h.join('/path', 
-00001f60: 2774 6f27 2c20 272f 6669 6c65 2729 203d  'to', '/file') =
-00001f70: 3e20 272f 6669 6c65 272c 2062 7574 2073  > '/file', but s
-00001f80: 335f 7061 7468 5f6a 6f69 6e28 272f 7061  3_path_join('/pa
-00001f90: 7468 272c 2027 746f 272c 2027 2f66 696c  th', 'to', '/fil
-00001fa0: 6527 2920 3d3e 2027 2f70 6174 682f 746f  e') => '/path/to
-00001fb0: 2f66 696c 6527 0a20 2020 2027 2727 0a20  /file'.    '''. 
-00001fc0: 2020 2072 6574 7572 6e20 7572 695f 6a6f     return uri_jo
-00001fd0: 696e 2866 7370 6174 6828 7061 7468 292c  in(fspath(path),
-00001fe0: 202a 6d61 7028 6673 7061 7468 2c20 6f74   *map(fspath, ot
-00001ff0: 6865 725f 7061 7468 7329 290a 0a0a 6465  her_paths))...de
-00002000: 6620 5f6c 6973 745f 616c 6c5f 6275 636b  f _list_all_buck
-00002010: 6574 7328 7072 6f66 696c 655f 6e61 6d65  ets(profile_name
-00002020: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00002030: 3d20 4e6f 6e65 2920 2d3e 204c 6973 745b  = None) -> List[
-00002040: 7374 725d 3a0a 2020 2020 636c 6965 6e74  str]:.    client
-00002050: 203d 2067 6574 5f73 335f 636c 6965 6e74   = get_s3_client
-00002060: 2870 726f 6669 6c65 5f6e 616d 653d 7072  (profile_name=pr
-00002070: 6f66 696c 655f 6e61 6d65 290a 2020 2020  ofile_name).    
-00002080: 7265 7370 6f6e 7365 203d 2063 6c69 656e  response = clien
-00002090: 742e 6c69 7374 5f62 7563 6b65 7473 2829  t.list_buckets()
-000020a0: 0a20 2020 2072 6574 7572 6e20 5b63 6f6e  .    return [con
-000020b0: 7465 6e74 5b27 4e61 6d65 275d 2066 6f72  tent['Name'] for
-000020c0: 2063 6f6e 7465 6e74 2069 6e20 7265 7370   content in resp
-000020d0: 6f6e 7365 5b27 4275 636b 6574 7327 5d5d  onse['Buckets']]
-000020e0: 0a0a 0a64 6566 205f 7061 7273 655f 7333  ...def _parse_s3
-000020f0: 5f75 726c 5f69 676e 6f72 655f 6272 6163  _url_ignore_brac
-00002100: 6528 7333 5f75 726c 3a20 7374 7229 202d  e(s3_url: str) -
-00002110: 3e20 5475 706c 655b 7374 722c 2073 7472  > Tuple[str, str
-00002120: 5d3a 0a20 2020 2073 335f 7572 6c20 3d20  ]:.    s3_url = 
-00002130: 6673 7061 7468 2873 335f 7572 6c29 0a20  fspath(s3_url). 
-00002140: 2020 2073 335f 7363 6865 6d65 2c20 7269     s3_scheme, ri
-00002150: 6768 7470 6172 7420 3d20 7333 5f75 726c  ghtpart = s3_url
-00002160: 5b3a 355d 2c20 7333 5f75 726c 5b35 3a5d  [:5], s3_url[5:]
-00002170: 0a20 2020 2069 6620 7333 5f73 6368 656d  .    if s3_schem
-00002180: 6520 213d 2027 7333 3a2f 2f27 3a0a 2020  e != 's3://':.  
-00002190: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000021a0: 6545 7272 6f72 2827 4e6f 7420 6120 7333  eError('Not a s3
-000021b0: 2075 726c 3a20 2572 2720 2520 7333 5f75   url: %r' % s3_u
-000021c0: 726c 290a 2020 2020 6c65 6674 5f62 7261  rl).    left_bra
-000021d0: 6365 203d 2046 616c 7365 0a20 2020 2066  ce = False.    f
-000021e0: 6f72 2063 7572 7265 6e74 5f69 6e64 6578  or current_index
-000021f0: 2c20 6375 7272 656e 745f 6368 6172 6163  , current_charac
-00002200: 7465 7220 696e 2065 6e75 6d65 7261 7465  ter in enumerate
-00002210: 2872 6967 6874 7061 7274 293a 0a20 2020  (rightpart):.   
-00002220: 2020 2020 2069 6620 6375 7272 656e 745f       if current_
-00002230: 6368 6172 6163 7465 7220 3d3d 2022 2f22  character == "/"
-00002240: 2061 6e64 206c 6566 745f 6272 6163 6520   and left_brace 
-00002250: 6973 2046 616c 7365 3a0a 2020 2020 2020  is False:.      
-00002260: 2020 2020 2020 7265 7475 726e 2072 6967        return rig
-00002270: 6874 7061 7274 5b3a 6375 7272 656e 745f  htpart[:current_
-00002280: 696e 6465 785d 2c20 7269 6768 7470 6172  index], rightpar
-00002290: 745b 6375 7272 656e 745f 696e 6465 7820  t[current_index 
-000022a0: 2b20 313a 5d0a 2020 2020 2020 2020 656c  + 1:].        el
-000022b0: 6966 2063 7572 7265 6e74 5f63 6861 7261  if current_chara
-000022c0: 6374 6572 203d 3d20 227b 223a 0a20 2020  cter == "{":.   
-000022d0: 2020 2020 2020 2020 206c 6566 745f 6272           left_br
-000022e0: 6163 6520 3d20 5472 7565 0a20 2020 2020  ace = True.     
-000022f0: 2020 2065 6c69 6620 6375 7272 656e 745f     elif current_
-00002300: 6368 6172 6163 7465 7220 3d3d 2022 7d22  character == "}"
-00002310: 3a0a 2020 2020 2020 2020 2020 2020 6c65  :.            le
-00002320: 6674 5f62 7261 6365 203d 2046 616c 7365  ft_brace = False
-00002330: 0a20 2020 2072 6574 7572 6e20 7269 6768  .    return righ
-00002340: 7470 6172 742c 2022 220a 0a0a 6465 6620  tpart, ""...def 
-00002350: 5f67 726f 7570 5f73 3370 6174 685f 6279  _group_s3path_by
-00002360: 5f62 7563 6b65 7428 0a20 2020 2020 2020  _bucket(.       
-00002370: 2073 335f 7061 7468 6e61 6d65 3a20 7374   s3_pathname: st
-00002380: 722c 2070 726f 6669 6c65 5f6e 616d 653a  r, profile_name:
-00002390: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-000023a0: 204e 6f6e 6529 202d 3e20 4c69 7374 5b73   None) -> List[s
-000023b0: 7472 5d3a 0a20 2020 2062 7563 6b65 742c  tr]:.    bucket,
-000023c0: 206b 6579 203d 205f 7061 7273 655f 7333   key = _parse_s3
-000023d0: 5f75 726c 5f69 676e 6f72 655f 6272 6163  _url_ignore_brac
-000023e0: 6528 7333 5f70 6174 686e 616d 6529 0a20  e(s3_pathname). 
-000023f0: 2020 2069 6620 6e6f 7420 6275 636b 6574     if not bucket
-00002400: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00002410: 206b 6579 3a0a 2020 2020 2020 2020 2020   key:.          
-00002420: 2020 7261 6973 6520 556e 7375 7070 6f72    raise Unsuppor
-00002430: 7465 6445 7272 6f72 2827 476c 6f62 2077  tedError('Glob w
-00002440: 686f 6c65 2073 3327 2c20 7333 5f70 6174  hole s3', s3_pat
-00002450: 686e 616d 6529 0a20 2020 2020 2020 2072  hname).        r
-00002460: 6169 7365 2053 3342 7563 6b65 744e 6f74  aise S3BucketNot
-00002470: 466f 756e 6445 7272 6f72 2827 456d 7074  FoundError('Empt
-00002480: 7920 6275 636b 6574 206e 616d 653a 2025  y bucket name: %
-00002490: 7227 2025 2073 335f 7061 7468 6e61 6d65  r' % s3_pathname
-000024a0: 290a 0a20 2020 2067 726f 7570 6564 5f70  )..    grouped_p
-000024b0: 6174 6820 3d20 5b5d 0a0a 2020 2020 6465  ath = []..    de
-000024c0: 6620 6765 6e65 7261 7465 5f73 335f 7061  f generate_s3_pa
-000024d0: 7468 2862 7563 6b65 743a 2073 7472 2c20  th(bucket: str, 
-000024e0: 6b65 793a 2073 7472 2920 2d3e 2073 7472  key: str) -> str
-000024f0: 3a0a 2020 2020 2020 2020 6966 206b 6579  :.        if key
-00002500: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00002510: 7475 726e 2022 7333 3a2f 2f25 732f 2573  turn "s3://%s/%s
-00002520: 2220 2520 2862 7563 6b65 742c 206b 6579  " % (bucket, key
-00002530: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00002540: 2022 7333 3a2f 2f25 7325 7322 2025 2028   "s3://%s%s" % (
-00002550: 6275 636b 6574 2c20 222f 2220 6966 2073  bucket, "/" if s
-00002560: 335f 7061 7468 6e61 6d65 2e65 6e64 7377  3_pathname.endsw
-00002570: 6974 6828 222f 2229 2065 6c73 6520 2222  ith("/") else ""
-00002580: 290a 0a20 2020 2061 6c6c 5f62 7563 6b65  )..    all_bucke
-00002590: 7420 3d20 6c72 755f 6361 6368 6528 6d61  t = lru_cache(ma
-000025a0: 7873 697a 653d 3129 285f 6c69 7374 5f61  xsize=1)(_list_a
-000025b0: 6c6c 5f62 7563 6b65 7473 290a 2020 2020  ll_buckets).    
-000025c0: 666f 7220 6275 636b 6574 6e61 6d65 2069  for bucketname i
-000025d0: 6e20 756e 676c 6f62 6c69 7a65 2862 7563  n ungloblize(buc
-000025e0: 6b65 7429 3a0a 2020 2020 2020 2020 6966  ket):.        if
-000025f0: 2068 6173 5f6d 6167 6963 2862 7563 6b65   has_magic(bucke
-00002600: 746e 616d 6529 3a0a 2020 2020 2020 2020  tname):.        
-00002610: 2020 2020 7370 6c69 745f 6275 636b 6574      split_bucket
-00002620: 6e61 6d65 203d 2062 7563 6b65 746e 616d  name = bucketnam
-00002630: 652e 7370 6c69 7428 222f 222c 2031 290a  e.split("/", 1).
-00002640: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00002650: 5f70 6172 7420 3d20 4e6f 6e65 0a20 2020  _part = None.   
-00002660: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00002670: 7370 6c69 745f 6275 636b 6574 6e61 6d65  split_bucketname
-00002680: 2920 3d3d 2032 3a0a 2020 2020 2020 2020  ) == 2:.        
-00002690: 2020 2020 2020 2020 6275 636b 6574 6e61          bucketna
-000026a0: 6d65 2c20 7061 7468 5f70 6172 7420 3d20  me, path_part = 
-000026b0: 7370 6c69 745f 6275 636b 6574 6e61 6d65  split_bucketname
-000026c0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-000026d0: 7465 726e 203d 2072 652e 636f 6d70 696c  tern = re.compil
-000026e0: 6528 7472 616e 736c 6174 6528 7265 2e73  e(translate(re.s
-000026f0: 7562 2872 275c 2a7b 322c 7d27 2c20 272a  ub(r'\*{2,}', '*
-00002700: 272c 2062 7563 6b65 746e 616d 6529 2929  ', bucketname)))
-00002710: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00002720: 7220 6275 636b 6574 2069 6e20 616c 6c5f  r bucket in all_
-00002730: 6275 636b 6574 2870 726f 6669 6c65 5f6e  bucket(profile_n
-00002740: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
-00002750: 2020 2020 2020 6966 2070 6174 7465 726e        if pattern
-00002760: 2e66 756c 6c6d 6174 6368 2862 7563 6b65  .fullmatch(bucke
-00002770: 7429 2069 7320 6e6f 7420 4e6f 6e65 3a0a  t) is not None:.
-00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 2020 2020 6966 2070 6174 685f 7061 7274      if path_part
-000027a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2020 2020 6275 636b 6574 203d 2022        bucket = "
-000027d0: 2573 2f25 7322 2025 2028 0a20 2020 2020  %s/%s" % (.     
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027f0: 2020 2020 2020 2062 7563 6b65 742c 2070         bucket, p
-00002800: 6174 685f 7061 7274 2920 2023 2070 7261  ath_part)  # pra
-00002810: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 6772 6f75 7065 645f 7061 7468 2e61    grouped_path.a
-00002840: 7070 656e 6428 6765 6e65 7261 7465 5f73  ppend(generate_s
-00002850: 335f 7061 7468 2862 7563 6b65 742c 206b  3_path(bucket, k
-00002860: 6579 2929 0a20 2020 2020 2020 2065 6c73  ey)).        els
-00002870: 653a 0a20 2020 2020 2020 2020 2020 2067  e:.            g
-00002880: 726f 7570 6564 5f70 6174 682e 6170 7065  rouped_path.appe
-00002890: 6e64 2867 656e 6572 6174 655f 7333 5f70  nd(generate_s3_p
-000028a0: 6174 6828 6275 636b 6574 6e61 6d65 2c20  ath(bucketname, 
-000028b0: 6b65 7929 290a 0a20 2020 2072 6574 7572  key))..    retur
-000028c0: 6e20 6772 6f75 7065 645f 7061 7468 0a0a  n grouped_path..
-000028d0: 0a64 6566 205f 7333 5f73 706c 6974 5f6d  .def _s3_split_m
-000028e0: 6167 6963 5f69 676e 6f72 655f 6272 6163  agic_ignore_brac
-000028f0: 6528 7333 5f70 6174 686e 616d 653a 2073  e(s3_pathname: s
-00002900: 7472 2920 2d3e 2054 7570 6c65 5b73 7472  tr) -> Tuple[str
-00002910: 2c20 7374 725d 3a0a 2020 2020 6966 206e  , str]:.    if n
-00002920: 6f74 2073 335f 7061 7468 6e61 6d65 3a0a  ot s3_pathname:.
-00002930: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00002940: 6c75 6545 7272 6f72 2822 7333 5f70 6174  lueError("s3_pat
-00002950: 686e 616d 653a 2025 7322 2c20 7333 5f70  hname: %s", s3_p
-00002960: 6174 686e 616d 6529 0a0a 2020 2020 6861  athname)..    ha
-00002970: 735f 7072 6f74 6f63 6f6c 203d 2046 616c  s_protocol = Fal
-00002980: 7365 0a20 2020 2069 6620 7333 5f70 6174  se.    if s3_pat
-00002990: 686e 616d 652e 7374 6172 7473 7769 7468  hname.startswith
-000029a0: 2822 7333 3a2f 2f22 293a 0a20 2020 2020  ("s3://"):.     
-000029b0: 2020 2068 6173 5f70 726f 746f 636f 6c20     has_protocol 
-000029c0: 3d20 5472 7565 0a20 2020 2020 2020 2073  = True.        s
-000029d0: 335f 7061 7468 6e61 6d65 203d 2073 335f  3_pathname = s3_
-000029e0: 7061 7468 6e61 6d65 5b35 3a5d 0a0a 2020  pathname[5:]..  
-000029f0: 2020 6861 735f 6465 6c69 6d69 7465 7220    has_delimiter 
-00002a00: 3d20 4661 6c73 650a 2020 2020 6966 2073  = False.    if s
-00002a10: 335f 7061 7468 6e61 6d65 2e65 6e64 7377  3_pathname.endsw
-00002a20: 6974 6828 222f 2229 3a0a 2020 2020 2020  ith("/"):.      
-00002a30: 2020 6861 735f 6465 6c69 6d69 7465 7220    has_delimiter 
-00002a40: 3d20 5472 7565 0a20 2020 2020 2020 2073  = True.        s
-00002a50: 335f 7061 7468 6e61 6d65 203d 2073 335f  3_pathname = s3_
-00002a60: 7061 7468 6e61 6d65 5b3a 2d31 5d0a 0a20  pathname[:-1].. 
-00002a70: 2020 206e 6f72 6d61 6c5f 7061 7274 7320     normal_parts 
-00002a80: 3d20 5b5d 0a20 2020 206d 6167 6963 5f70  = [].    magic_p
-00002a90: 6172 7473 203d 205b 5d0a 2020 2020 6c65  arts = [].    le
-00002aa0: 6674 5f62 7261 6365 203d 2046 616c 7365  ft_brace = False
-00002ab0: 0a20 2020 206c 6566 745f 696e 6465 7820  .    left_index 
-00002ac0: 3d20 300a 2020 2020 666f 7220 6375 7272  = 0.    for curr
-00002ad0: 656e 745f 696e 6465 782c 2063 7572 7265  ent_index, curre
-00002ae0: 6e74 5f63 6861 7261 6374 6572 2069 6e20  nt_character in 
-00002af0: 656e 756d 6572 6174 6528 7333 5f70 6174  enumerate(s3_pat
-00002b00: 686e 616d 6529 3a0a 2020 2020 2020 2020  hname):.        
-00002b10: 6966 2063 7572 7265 6e74 5f63 6861 7261  if current_chara
-00002b20: 6374 6572 203d 3d20 222f 2220 616e 6420  cter == "/" and 
-00002b30: 6c65 6674 5f62 7261 6365 2069 7320 4661  left_brace is Fa
-00002b40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00002b50: 2069 6620 6861 735f 6d61 6769 635f 6967   if has_magic_ig
-00002b60: 6e6f 7265 5f62 7261 6365 2873 335f 7061  nore_brace(s3_pa
-00002b70: 7468 6e61 6d65 5b6c 6566 745f 696e 6465  thname[left_inde
-00002b80: 783a 6375 7272 656e 745f 696e 6465 785d  x:current_index]
-00002b90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00002ba0: 2020 206d 6167 6963 5f70 6172 7473 2e61     magic_parts.a
-00002bb0: 7070 656e 6428 7333 5f70 6174 686e 616d  ppend(s3_pathnam
-00002bc0: 655b 6c65 6674 5f69 6e64 6578 3a63 7572  e[left_index:cur
-00002bd0: 7265 6e74 5f69 6e64 6578 5d29 0a20 2020  rent_index]).   
-00002be0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00002bf0: 7333 5f70 6174 686e 616d 655b 6375 7272  s3_pathname[curr
-00002c00: 656e 745f 696e 6465 7820 2b20 313a 5d3a  ent_index + 1:]:
-00002c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c20: 2020 2020 206d 6167 6963 5f70 6172 7473       magic_parts
-00002c30: 2e61 7070 656e 6428 7333 5f70 6174 686e  .append(s3_pathn
-00002c40: 616d 655b 6375 7272 656e 745f 696e 6465  ame[current_inde
-00002c50: 7820 2b20 313a 5d29 0a20 2020 2020 2020  x + 1:]).       
-00002c60: 2020 2020 2020 2020 2020 2020 206c 6566               lef
-00002c70: 745f 696e 6465 7820 3d20 6c65 6e28 7333  t_index = len(s3
-00002c80: 5f70 6174 686e 616d 6529 0a20 2020 2020  _pathname).     
-00002c90: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00002ca0: 0a20 2020 2020 2020 2020 2020 206e 6f72  .            nor
-00002cb0: 6d61 6c5f 7061 7274 732e 6170 7065 6e64  mal_parts.append
-00002cc0: 2873 335f 7061 7468 6e61 6d65 5b6c 6566  (s3_pathname[lef
-00002cd0: 745f 696e 6465 783a 6375 7272 656e 745f  t_index:current_
-00002ce0: 696e 6465 785d 290a 2020 2020 2020 2020  index]).        
-00002cf0: 2020 2020 6c65 6674 5f69 6e64 6578 203d      left_index =
-00002d00: 2063 7572 7265 6e74 5f69 6e64 6578 202b   current_index +
-00002d10: 2031 0a20 2020 2020 2020 2065 6c69 6620   1.        elif 
-00002d20: 6375 7272 656e 745f 6368 6172 6163 7465  current_characte
-00002d30: 7220 3d3d 2022 7b22 3a0a 2020 2020 2020  r == "{":.      
-00002d40: 2020 2020 2020 6c65 6674 5f62 7261 6365        left_brace
-00002d50: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00002d60: 656c 6966 2063 7572 7265 6e74 5f63 6861  elif current_cha
-00002d70: 7261 6374 6572 203d 3d20 227d 223a 0a20  racter == "}":. 
-00002d80: 2020 2020 2020 2020 2020 206c 6566 745f             left_
-00002d90: 6272 6163 6520 3d20 4661 6c73 650a 2020  brace = False.  
-00002da0: 2020 6966 2073 335f 7061 7468 6e61 6d65    if s3_pathname
-00002db0: 5b6c 6566 745f 696e 6465 783a 5d3a 0a20  [left_index:]:. 
-00002dc0: 2020 2020 2020 2069 6620 6861 735f 6d61         if has_ma
-00002dd0: 6769 635f 6967 6e6f 7265 5f62 7261 6365  gic_ignore_brace
-00002de0: 2873 335f 7061 7468 6e61 6d65 5b6c 6566  (s3_pathname[lef
-00002df0: 745f 696e 6465 783a 5d29 3a0a 2020 2020  t_index:]):.    
-00002e00: 2020 2020 2020 2020 6d61 6769 635f 7061          magic_pa
-00002e10: 7274 732e 6170 7065 6e64 2873 335f 7061  rts.append(s3_pa
-00002e20: 7468 6e61 6d65 5b6c 6566 745f 696e 6465  thname[left_inde
-00002e30: 783a 5d29 0a20 2020 2020 2020 2065 6c73  x:]).        els
-00002e40: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
-00002e50: 6f72 6d61 6c5f 7061 7274 732e 6170 7065  ormal_parts.appe
-00002e60: 6e64 2873 335f 7061 7468 6e61 6d65 5b6c  nd(s3_pathname[l
-00002e70: 6566 745f 696e 6465 783a 5d29 0a0a 2020  eft_index:])..  
-00002e80: 2020 6966 2068 6173 5f70 726f 746f 636f    if has_protoco
-00002e90: 6c20 616e 6420 6e6f 726d 616c 5f70 6172  l and normal_par
-00002ea0: 7473 3a0a 2020 2020 2020 2020 6e6f 726d  ts:.        norm
-00002eb0: 616c 5f70 6172 7473 2e69 6e73 6572 7428  al_parts.insert(
-00002ec0: 302c 2022 7333 3a2f 2229 0a20 2020 2065  0, "s3:/").    e
-00002ed0: 6c69 6620 6861 735f 7072 6f74 6f63 6f6c  lif has_protocol
-00002ee0: 3a0a 2020 2020 2020 2020 6d61 6769 635f  :.        magic_
-00002ef0: 7061 7274 732e 696e 7365 7274 2830 2c20  parts.insert(0, 
-00002f00: 2273 333a 2f22 290a 0a20 2020 2069 6620  "s3:/")..    if 
-00002f10: 6861 735f 6465 6c69 6d69 7465 7220 616e  has_delimiter an
-00002f20: 6420 6d61 6769 635f 7061 7274 733a 0a20  d magic_parts:. 
-00002f30: 2020 2020 2020 206d 6167 6963 5f70 6172         magic_par
-00002f40: 7473 2e61 7070 656e 6428 2222 290a 2020  ts.append("").  
-00002f50: 2020 656c 6966 2068 6173 5f64 656c 696d    elif has_delim
-00002f60: 6974 6572 3a0a 2020 2020 2020 2020 6e6f  iter:.        no
-00002f70: 726d 616c 5f70 6172 7473 2e61 7070 656e  rmal_parts.appen
-00002f80: 6428 2222 290a 0a20 2020 2072 6574 7572  d("")..    retur
-00002f90: 6e20 222f 222e 6a6f 696e 286e 6f72 6d61  n "/".join(norma
-00002fa0: 6c5f 7061 7274 7329 2c20 222f 222e 6a6f  l_parts), "/".jo
-00002fb0: 696e 286d 6167 6963 5f70 6172 7473 290a  in(magic_parts).
-00002fc0: 0a0a 6465 6620 5f67 726f 7570 5f73 3370  ..def _group_s3p
-00002fd0: 6174 685f 6279 5f70 7265 6669 7828 7333  ath_by_prefix(s3
-00002fe0: 5f70 6174 686e 616d 653a 2073 7472 2920  _pathname: str) 
-00002ff0: 2d3e 204c 6973 745b 7374 725d 3a0a 0a20  -> List[str]:.. 
-00003000: 2020 205f 2c20 6b65 7920 3d20 7061 7273     _, key = pars
-00003010: 655f 7333 5f75 726c 2873 335f 7061 7468  e_s3_url(s3_path
-00003020: 6e61 6d65 290a 2020 2020 6966 206e 6f74  name).    if not
-00003030: 206b 6579 3a0a 2020 2020 2020 2020 7265   key:.        re
-00003040: 7475 726e 2075 6e67 6c6f 626c 697a 6528  turn ungloblize(
-00003050: 7333 5f70 6174 686e 616d 6529 0a0a 2020  s3_pathname)..  
-00003060: 2020 746f 705f 6469 722c 206d 6167 6963    top_dir, magic
-00003070: 5f70 6172 7420 3d20 5f73 335f 7370 6c69  _part = _s3_spli
-00003080: 745f 6d61 6769 635f 6967 6e6f 7265 5f62  t_magic_ignore_b
-00003090: 7261 6365 2873 335f 7061 7468 6e61 6d65  race(s3_pathname
-000030a0: 290a 2020 2020 6966 206e 6f74 2074 6f70  ).    if not top
-000030b0: 5f64 6972 3a0a 2020 2020 2020 2020 7265  _dir:.        re
-000030c0: 7475 726e 205b 6d61 6769 635f 7061 7274  turn [magic_part
-000030d0: 5d0a 2020 2020 6772 6f75 7065 645f 7061  ].    grouped_pa
-000030e0: 7468 203d 205b 5d0a 2020 2020 666f 7220  th = [].    for 
-000030f0: 7061 7468 6e61 6d65 2069 6e20 756e 676c  pathname in ungl
-00003100: 6f62 6c69 7a65 2874 6f70 5f64 6972 293a  oblize(top_dir):
-00003110: 0a20 2020 2020 2020 2069 6620 6d61 6769  .        if magi
-00003120: 635f 7061 7274 3a0a 2020 2020 2020 2020  c_part:.        
-00003130: 2020 2020 7061 7468 6e61 6d65 203d 2022      pathname = "
-00003140: 2f22 2e6a 6f69 6e28 5b70 6174 686e 616d  /".join([pathnam
-00003150: 652c 206d 6167 6963 5f70 6172 745d 290a  e, magic_part]).
-00003160: 2020 2020 2020 2020 6772 6f75 7065 645f          grouped_
-00003170: 7061 7468 2e61 7070 656e 6428 7061 7468  path.append(path
-00003180: 6e61 6d65 290a 2020 2020 7265 7475 726e  name).    return
-00003190: 2067 726f 7570 6564 5f70 6174 680a 0a0a   grouped_path...
-000031a0: 6465 6620 5f62 6563 6f6d 655f 7072 6566  def _become_pref
-000031b0: 6978 2870 7265 6669 783a 2073 7472 2920  ix(prefix: str) 
-000031c0: 2d3e 2073 7472 3a0a 2020 2020 6966 2070  -> str:.    if p
-000031d0: 7265 6669 7820 213d 2027 2720 616e 6420  refix != '' and 
-000031e0: 6e6f 7420 7072 6566 6978 2e65 6e64 7377  not prefix.endsw
-000031f0: 6974 6828 272f 2729 3a0a 2020 2020 2020  ith('/'):.      
-00003200: 2020 7072 6566 6978 202b 3d20 272f 270a    prefix += '/'.
-00003210: 2020 2020 7265 7475 726e 2070 7265 6669      return prefi
-00003220: 780a 0a0a 6465 6620 5f73 335f 7370 6c69  x...def _s3_spli
-00003230: 745f 6d61 6769 6328 7333 5f70 6174 686e  t_magic(s3_pathn
-00003240: 616d 653a 2073 7472 2920 2d3e 2054 7570  ame: str) -> Tup
-00003250: 6c65 5b73 7472 2c20 7374 725d 3a0a 2020  le[str, str]:.  
-00003260: 2020 6966 206e 6f74 2068 6173 5f6d 6167    if not has_mag
-00003270: 6963 2873 335f 7061 7468 6e61 6d65 293a  ic(s3_pathname):
-00003280: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003290: 7333 5f70 6174 686e 616d 652c 2027 270a  s3_pathname, ''.
-000032a0: 2020 2020 6465 6c69 6d69 7465 7220 3d20      delimiter = 
-000032b0: 272f 270a 2020 2020 6e6f 726d 616c 5f70  '/'.    normal_p
-000032c0: 6172 7473 203d 205b 5d0a 2020 2020 6d61  arts = [].    ma
-000032d0: 6769 635f 7061 7274 7320 3d20 5b5d 0a20  gic_parts = []. 
-000032e0: 2020 2061 6c6c 5f70 6172 7473 203d 2073     all_parts = s
-000032f0: 335f 7061 7468 6e61 6d65 2e73 706c 6974  3_pathname.split
-00003300: 2864 656c 696d 6974 6572 290a 2020 2020  (delimiter).    
-00003310: 666f 7220 692c 2070 6172 7420 696e 2065  for i, part in e
-00003320: 6e75 6d65 7261 7465 2861 6c6c 5f70 6172  numerate(all_par
-00003330: 7473 293a 0a20 2020 2020 2020 2069 6620  ts):.        if 
-00003340: 6e6f 7420 6861 735f 6d61 6769 6328 7061  not has_magic(pa
-00003350: 7274 293a 0a20 2020 2020 2020 2020 2020  rt):.           
-00003360: 206e 6f72 6d61 6c5f 7061 7274 732e 6170   normal_parts.ap
-00003370: 7065 6e64 2870 6172 7429 0a20 2020 2020  pend(part).     
-00003380: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003390: 2020 2020 206d 6167 6963 5f70 6172 7473       magic_parts
-000033a0: 203d 2061 6c6c 5f70 6172 7473 5b69 3a5d   = all_parts[i:]
-000033b0: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
-000033c0: 616b 0a20 2020 2072 6574 7572 6e20 6465  ak.    return de
-000033d0: 6c69 6d69 7465 722e 6a6f 696e 286e 6f72  limiter.join(nor
-000033e0: 6d61 6c5f 7061 7274 7329 2c20 6465 6c69  mal_parts), deli
-000033f0: 6d69 7465 722e 6a6f 696e 286d 6167 6963  miter.join(magic
-00003400: 5f70 6172 7473 290a 0a0a 6465 6620 5f6c  _parts)...def _l
-00003410: 6973 745f 6f62 6a65 6374 735f 7265 6375  ist_objects_recu
-00003420: 7273 6976 6528 0a20 2020 2020 2020 2073  rsive(.        s
-00003430: 335f 636c 6965 6e74 2c20 6275 636b 6574  3_client, bucket
-00003440: 3a20 7374 722c 2070 7265 6669 783a 2073  : str, prefix: s
-00003450: 7472 2c20 6465 6c69 6d69 7465 723a 2073  tr, delimiter: s
-00003460: 7472 203d 2027 2729 3a0a 0a20 2020 2072  tr = ''):..    r
-00003470: 6573 7020 3d20 7333 5f63 6c69 656e 742e  esp = s3_client.
-00003480: 6c69 7374 5f6f 626a 6563 7473 5f76 3228  list_objects_v2(
-00003490: 0a20 2020 2020 2020 2042 7563 6b65 743d  .        Bucket=
-000034a0: 6275 636b 6574 2c20 5072 6566 6978 3d70  bucket, Prefix=p
-000034b0: 7265 6669 782c 2044 656c 696d 6974 6572  refix, Delimiter
-000034c0: 3d64 656c 696d 6974 6572 2c20 4d61 784b  =delimiter, MaxK
-000034d0: 6579 733d 6d61 785f 6b65 7973 290a 0a20  eys=max_keys).. 
-000034e0: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
-000034f0: 2020 2020 2020 2079 6965 6c64 2072 6573         yield res
-00003500: 700a 0a20 2020 2020 2020 2069 6620 6e6f  p..        if no
-00003510: 7420 7265 7370 5b27 4973 5472 756e 6361  t resp['IsTrunca
-00003520: 7465 6427 5d3a 0a20 2020 2020 2020 2020  ted']:.         
-00003530: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-00003540: 2020 7265 7370 203d 2073 335f 636c 6965    resp = s3_clie
-00003550: 6e74 2e6c 6973 745f 6f62 6a65 6374 735f  nt.list_objects_
-00003560: 7632 280a 2020 2020 2020 2020 2020 2020  v2(.            
-00003570: 4275 636b 6574 3d62 7563 6b65 742c 0a20  Bucket=bucket,. 
-00003580: 2020 2020 2020 2020 2020 2050 7265 6669             Prefi
-00003590: 783d 7072 6566 6978 2c0a 2020 2020 2020  x=prefix,.      
-000035a0: 2020 2020 2020 4465 6c69 6d69 7465 723d        Delimiter=
-000035b0: 6465 6c69 6d69 7465 722c 0a20 2020 2020  delimiter,.     
-000035c0: 2020 2020 2020 2043 6f6e 7469 6e75 6174         Continuat
-000035d0: 696f 6e54 6f6b 656e 3d72 6573 705b 274e  ionToken=resp['N
-000035e0: 6578 7443 6f6e 7469 6e75 6174 696f 6e54  extContinuationT
-000035f0: 6f6b 656e 275d 2c0a 2020 2020 2020 2020  oken'],.        
-00003600: 2020 2020 4d61 784b 6579 733d 6d61 785f      MaxKeys=max_
-00003610: 6b65 7973 290a 0a0a 6465 6620 5f6d 616b  keys)...def _mak
-00003620: 655f 7374 6174 2863 6f6e 7465 6e74 3a20  e_stat(content: 
-00003630: 4469 6374 5b73 7472 2c20 416e 795d 293a  Dict[str, Any]):
-00003640: 0a20 2020 2072 6574 7572 6e20 5374 6174  .    return Stat
-00003650: 5265 7375 6c74 280a 2020 2020 2020 2020  Result(.        
-00003660: 6973 6c6e 6b3d 636f 6e74 656e 742e 6765  islnk=content.ge
-00003670: 7428 2769 736c 6e6b 272c 2046 616c 7365  t('islnk', False
-00003680: 292c 0a20 2020 2020 2020 2073 697a 653d  ),.        size=
-00003690: 636f 6e74 656e 745b 2753 697a 6527 5d2c  content['Size'],
-000036a0: 0a20 2020 2020 2020 206d 7469 6d65 3d63  .        mtime=c
-000036b0: 6f6e 7465 6e74 5b27 4c61 7374 4d6f 6469  ontent['LastModi
-000036c0: 6669 6564 275d 2e74 696d 6573 7461 6d70  fied'].timestamp
-000036d0: 2829 2c0a 2020 2020 2020 2020 6578 7472  (),.        extr
-000036e0: 613d 636f 6e74 656e 742c 0a20 2020 2029  a=content,.    )
-000036f0: 0a0a 0a64 6566 205f 7333 5f67 6c6f 625f  ...def _s3_glob_
-00003700: 7374 6174 5f73 696e 676c 655f 7061 7468  stat_single_path
-00003710: 280a 2020 2020 2020 2020 7333 5f70 6174  (.        s3_pat
-00003720: 686e 616d 653a 2050 6174 684c 696b 652c  hname: PathLike,
-00003730: 0a20 2020 2020 2020 2072 6563 7572 7369  .        recursi
-00003740: 7665 3a20 626f 6f6c 203d 2054 7275 652c  ve: bool = True,
-00003750: 0a20 2020 2020 2020 206d 6973 7369 6e67  .        missing
-00003760: 5f6f 6b3a 2062 6f6f 6c20 3d20 5472 7565  _ok: bool = True
-00003770: 2c0a 2020 2020 2020 2020 666f 6c6c 6f77  ,.        follow
-00003780: 6c69 6e6b 733a 2062 6f6f 6c20 3d20 4661  links: bool = Fa
-00003790: 6c73 652c 0a20 2020 2020 2020 2070 726f  lse,.        pro
-000037a0: 6669 6c65 5f6e 616d 653a 204f 7074 696f  file_name: Optio
-000037b0: 6e61 6c5b 7374 725d 203d 204e 6f6e 6529  nal[str] = None)
-000037c0: 202d 3e20 4974 6572 6174 6f72 5b46 696c   -> Iterator[Fil
-000037d0: 6545 6e74 7279 5d3a 0a20 2020 2069 6620  eEntry]:.    if 
-000037e0: 6e6f 7420 7265 6375 7273 6976 653a 0a20  not recursive:. 
-000037f0: 2020 2020 2020 2023 2049 6620 6e6f 7420         # If not 
-00003800: 7265 6375 7273 6976 652c 2072 6570 6c61  recursive, repla
-00003810: 6365 202a 2a20 7769 7468 202a 0a20 2020  ce ** with *.   
-00003820: 2020 2020 2073 335f 7061 7468 6e61 6d65       s3_pathname
-00003830: 203d 2072 652e 7375 6228 7227 5c2a 7b32   = re.sub(r'\*{2
-00003840: 2c7d 272c 2027 2a27 2c20 7333 5f70 6174  ,}', '*', s3_pat
-00003850: 686e 616d 6529 0a20 2020 2074 6f70 5f64  hname).    top_d
-00003860: 6972 2c20 7769 6c64 6361 7264 5f70 6172  ir, wildcard_par
-00003870: 7420 3d20 5f73 335f 7370 6c69 745f 6d61  t = _s3_split_ma
-00003880: 6769 6328 7333 5f70 6174 686e 616d 6529  gic(s3_pathname)
-00003890: 0a20 2020 2073 6561 7263 685f 6469 7220  .    search_dir 
-000038a0: 3d20 7769 6c64 6361 7264 5f70 6172 742e  = wildcard_part.
-000038b0: 656e 6473 7769 7468 2827 2f27 290a 0a20  endswith('/').. 
-000038c0: 2020 2064 6566 2073 686f 756c 645f 7265     def should_re
-000038d0: 6375 7273 6976 6528 7769 6c64 6361 7264  cursive(wildcard
-000038e0: 5f70 6172 743a 2073 7472 2920 2d3e 2062  _part: str) -> b
-000038f0: 6f6f 6c3a 0a20 2020 2020 2020 2069 6620  ool:.        if 
-00003900: 272a 2a27 2069 6e20 7769 6c64 6361 7264  '**' in wildcard
-00003910: 5f70 6172 743a 0a20 2020 2020 2020 2020  _part:.         
-00003920: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00003930: 2020 2020 2020 2066 6f72 2065 7870 616e         for expan
-00003940: 6465 645f 7061 7468 2069 6e20 756e 676c  ded_path in ungl
-00003950: 6f62 6c69 7a65 2877 696c 6463 6172 645f  oblize(wildcard_
-00003960: 7061 7274 293a 0a20 2020 2020 2020 2020  part):.         
-00003970: 2020 2070 6172 7473 5f6c 656e 6774 6820     parts_length 
-00003980: 3d20 6c65 6e28 6578 7061 6e64 6564 5f70  = len(expanded_p
-00003990: 6174 682e 7370 6c69 7428 272f 2729 290a  ath.split('/')).
-000039a0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-000039b0: 6172 7473 5f6c 656e 6774 6820 2b20 7365  arts_length + se
-000039c0: 6172 6368 5f64 6972 203e 3d20 323a 0a20  arch_dir >= 2:. 
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000039e0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-000039f0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00003a00: 0a20 2020 2064 6566 2063 7265 6174 655f  .    def create_
-00003a10: 6765 6e65 7261 746f 7228 5f73 335f 7061  generator(_s3_pa
-00003a20: 7468 6e61 6d65 2920 2d3e 2049 7465 7261  thname) -> Itera
-00003a30: 746f 725b 4669 6c65 456e 7472 795d 3a0a  tor[FileEntry]:.
-00003a40: 2020 2020 2020 2020 6966 206e 6f74 2053          if not S
-00003a50: 3350 6174 6828 746f 705f 6469 7229 2e65  3Path(top_dir).e
-00003a60: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
-00003a70: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00003a80: 2020 2020 6966 206e 6f74 2068 6173 5f6d      if not has_m
-00003a90: 6167 6963 285f 7333 5f70 6174 686e 616d  agic(_s3_pathnam
-00003aa0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00003ab0: 5f73 335f 7061 7468 6e61 6d65 5f6f 626a  _s3_pathname_obj
-00003ac0: 203d 2053 3350 6174 6828 5f73 335f 7061   = S3Path(_s3_pa
-00003ad0: 7468 6e61 6d65 290a 2020 2020 2020 2020  thname).        
-00003ae0: 2020 2020 6966 205f 7333 5f70 6174 686e      if _s3_pathn
-00003af0: 616d 655f 6f62 6a2e 6973 5f66 696c 6528  ame_obj.is_file(
-00003b00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00003b10: 2020 2073 7461 7420 3d20 5333 5061 7468     stat = S3Path
-00003b20: 285f 7333 5f70 6174 686e 616d 6529 2e73  (_s3_pathname).s
-00003b30: 7461 7428 666f 6c6c 6f77 5f73 796d 6c69  tat(follow_symli
-00003b40: 6e6b 733d 666f 6c6c 6f77 6c69 6e6b 7329  nks=followlinks)
-00003b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b60: 2079 6965 6c64 2046 696c 6545 6e74 7279   yield FileEntry
-00003b70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00003b80: 2020 2020 2020 5f73 335f 7061 7468 6e61        _s3_pathna
-00003b90: 6d65 5f6f 626a 2e6e 616d 652c 205f 7333  me_obj.name, _s3
-00003ba0: 5f70 6174 686e 616d 655f 6f62 6a2e 7061  _pathname_obj.pa
-00003bb0: 7468 2c20 7374 6174 290a 2020 2020 2020  th, stat).      
-00003bc0: 2020 2020 2020 6966 205f 7333 5f70 6174        if _s3_pat
-00003bd0: 686e 616d 655f 6f62 6a2e 6973 5f64 6972  hname_obj.is_dir
-00003be0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00003bf0: 2020 2020 7969 656c 6420 4669 6c65 456e      yield FileEn
-00003c00: 7472 7928 0a20 2020 2020 2020 2020 2020  try(.           
-00003c10: 2020 2020 2020 2020 205f 7333 5f70 6174           _s3_pat
-00003c20: 686e 616d 655f 6f62 6a2e 6e61 6d65 2c20  hname_obj.name, 
-00003c30: 5f73 335f 7061 7468 6e61 6d65 5f6f 626a  _s3_pathname_obj
-00003c40: 2e70 6174 682c 0a20 2020 2020 2020 2020  .path,.         
-00003c50: 2020 2020 2020 2020 2020 2053 7461 7452             StatR
-00003c60: 6573 756c 7428 6973 6469 723d 5472 7565  esult(isdir=True
-00003c70: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-00003c80: 6574 7572 6e0a 0a20 2020 2020 2020 2064  eturn..        d
-00003c90: 656c 696d 6974 6572 203d 2027 270a 2020  elimiter = ''.  
-00003ca0: 2020 2020 2020 6966 206e 6f74 2073 686f        if not sho
-00003cb0: 756c 645f 7265 6375 7273 6976 6528 7769  uld_recursive(wi
-00003cc0: 6c64 6361 7264 5f70 6172 7429 3a0a 2020  ldcard_part):.  
-00003cd0: 2020 2020 2020 2020 2020 6465 6c69 6d69            delimi
-00003ce0: 7465 7220 3d20 272f 270a 0a20 2020 2020  ter = '/'..     
-00003cf0: 2020 2064 6972 6e61 6d65 7320 3d20 7365     dirnames = se
-00003d00: 7428 290a 2020 2020 2020 2020 7061 7474  t().        patt
-00003d10: 6572 6e20 3d20 7265 2e63 6f6d 7069 6c65  ern = re.compile
-00003d20: 2874 7261 6e73 6c61 7465 285f 7333 5f70  (translate(_s3_p
-00003d30: 6174 686e 616d 6529 290a 2020 2020 2020  athname)).      
-00003d40: 2020 6275 636b 6574 2c20 6b65 7920 3d20    bucket, key = 
-00003d50: 7061 7273 655f 7333 5f75 726c 2874 6f70  parse_s3_url(top
-00003d60: 5f64 6972 290a 2020 2020 2020 2020 7072  _dir).        pr
-00003d70: 6566 6978 203d 205f 6265 636f 6d65 5f70  efix = _become_p
-00003d80: 7265 6669 7828 6b65 7929 0a20 2020 2020  refix(key).     
-00003d90: 2020 2063 6c69 656e 7420 3d20 6765 745f     client = get_
-00003da0: 7333 5f63 6c69 656e 7428 7072 6f66 696c  s3_client(profil
-00003db0: 655f 6e61 6d65 3d70 726f 6669 6c65 5f6e  e_name=profile_n
-00003dc0: 616d 6529 0a20 2020 2020 2020 2077 6974  ame).        wit
-00003dd0: 6820 7261 6973 655f 7333 5f65 7272 6f72  h raise_s3_error
-00003de0: 285f 7333 5f70 6174 686e 616d 6529 3a0a  (_s3_pathname):.
-00003df0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00003e00: 7265 7370 2069 6e20 5f6c 6973 745f 6f62  resp in _list_ob
-00003e10: 6a65 6374 735f 7265 6375 7273 6976 6528  jects_recursive(
-00003e20: 636c 6965 6e74 2c20 6275 636b 6574 2c20  client, bucket, 
-00003e30: 7072 6566 6978 2c0a 2020 2020 2020 2020  prefix,.        
-00003e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e60: 2020 2020 2020 2020 6465 6c69 6d69 7465          delimite
-00003e70: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00003e80: 2020 2020 666f 7220 636f 6e74 656e 7420      for content 
-00003e90: 696e 2072 6573 702e 6765 7428 2743 6f6e  in resp.get('Con
-00003ea0: 7465 6e74 7327 2c20 5b5d 293a 0a20 2020  tents', []):.   
-00003eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ec0: 2070 6174 6820 3d20 7333 5f70 6174 685f   path = s3_path_
-00003ed0: 6a6f 696e 2827 7333 3a2f 2f27 2c20 6275  join('s3://', bu
-00003ee0: 636b 6574 2c20 636f 6e74 656e 745b 274b  cket, content['K
-00003ef0: 6579 275d 290a 2020 2020 2020 2020 2020  ey']).          
-00003f00: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00003f10: 2073 6561 7263 685f 6469 7220 616e 6420   search_dir and 
-00003f20: 7061 7474 6572 6e2e 6d61 7463 6828 7061  pattern.match(pa
-00003f30: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
-00003f40: 2020 2020 2020 2020 2020 2020 2079 6965               yie
-00003f50: 6c64 2046 696c 6545 6e74 7279 280a 2020  ld FileEntry(.  
+00000e10: 7429 3a0a 2020 2020 2020 2020 6966 2069  t):.        if i
+00000e20: 735f 7265 6164 6162 6c65 2872 6571 7565  s_readable(reque
+00000e30: 7374 5f64 6963 745b 2762 6f64 7927 5d29  st_dict['body'])
+00000e40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000e50: 7175 6573 745f 6469 6374 5b27 626f 6479  quest_dict['body
+00000e60: 275d 2e73 6565 6b28 3029 0a0a 2020 2020  '].seek(0)..    
+00000e70: 6465 6620 6265 666f 7265 5f63 616c 6c62  def before_callb
+00000e80: 6163 6b28 6f70 6572 6174 696f 6e5f 6d6f  ack(operation_mo
+00000e90: 6465 6c2c 2072 6571 7565 7374 5f64 6963  del, request_dic
+00000ea0: 742c 2072 6571 7565 7374 5f63 6f6e 7465  t, request_conte
+00000eb0: 7874 293a 0a20 2020 2020 2020 205f 6c6f  xt):.        _lo
+00000ec0: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+00000ed0: 2020 2020 2020 2020 2773 656e 6420 7333          'send s3
+00000ee0: 2072 6571 7565 7374 3a20 2572 2c20 7769   request: %r, wi
+00000ef0: 7468 2070 6172 616d 6574 6572 733a 2025  th parameters: %
+00000f00: 7327 2c20 6f70 6572 6174 696f 6e5f 6d6f  s', operation_mo
+00000f10: 6465 6c2e 6e61 6d65 2c0a 2020 2020 2020  del.name,.      
+00000f20: 2020 2020 2020 7265 7175 6573 745f 6469        request_di
+00000f30: 6374 290a 0a20 2020 2063 6c69 656e 742e  ct)..    client.
+00000f40: 5f6d 616b 655f 7265 7175 6573 7420 3d20  _make_request = 
+00000f50: 7061 7463 685f 6d65 7468 6f64 280a 2020  patch_method(.  
+00000f60: 2020 2020 2020 636c 6965 6e74 2e5f 6d61        client._ma
+00000f70: 6b65 5f72 6571 7565 7374 2c0a 2020 2020  ke_request,.    
+00000f80: 2020 2020 6d61 785f 7265 7472 6965 733d      max_retries=
+00000f90: 6d61 785f 7265 7472 6965 732c 0a20 2020  max_retries,.   
+00000fa0: 2020 2020 2073 686f 756c 645f 7265 7472       should_retr
+00000fb0: 793d 7333 5f73 686f 756c 645f 7265 7472  y=s3_should_retr
+00000fc0: 792c 0a20 2020 2020 2020 2061 6674 6572  y,.        after
+00000fd0: 5f63 616c 6c62 6163 6b3d 6166 7465 725f  _callback=after_
+00000fe0: 6361 6c6c 6261 636b 2c0a 2020 2020 2020  callback,.      
+00000ff0: 2020 6265 666f 7265 5f63 616c 6c62 6163    before_callbac
+00001000: 6b3d 6265 666f 7265 5f63 616c 6c62 6163  k=before_callbac
+00001010: 6b2c 0a20 2020 2020 2020 2072 6574 7279  k,.        retry
+00001020: 5f63 616c 6c62 6163 6b3d 7265 7472 795f  _callback=retry_
+00001030: 6361 6c6c 6261 636b 290a 2020 2020 7265  callback).    re
+00001040: 7475 726e 2063 6c69 656e 740a 0a0a 6465  turn client...de
+00001050: 6620 7061 7273 655f 7333 5f75 726c 2873  f parse_s3_url(s
+00001060: 335f 7572 6c3a 2050 6174 684c 696b 6529  3_url: PathLike)
+00001070: 202d 3e20 5475 706c 655b 7374 722c 2073   -> Tuple[str, s
+00001080: 7472 5d3a 0a20 2020 2073 335f 7572 6c20  tr]:.    s3_url 
+00001090: 3d20 6673 7061 7468 2873 335f 7572 6c29  = fspath(s3_url)
+000010a0: 0a20 2020 2069 6620 6e6f 7420 6973 5f73  .    if not is_s
+000010b0: 3328 7333 5f75 726c 293a 0a20 2020 2020  3(s3_url):.     
+000010c0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000010d0: 726f 7228 274e 6f74 2061 2073 3320 7572  ror('Not a s3 ur
+000010e0: 6c3a 2025 7227 2025 2073 335f 7572 6c29  l: %r' % s3_url)
+000010f0: 0a20 2020 2072 6967 6874 7061 7274 203d  .    rightpart =
+00001100: 2073 335f 7572 6c2e 7370 6c69 7428 273a   s3_url.split(':
+00001110: 2f2f 272c 206d 6178 7370 6c69 743d 3129  //', maxsplit=1)
+00001120: 5b31 5d0a 2020 2020 6275 636b 6574 6d61  [1].    bucketma
+00001130: 7463 6820 3d20 7265 2e6d 6174 6368 2827  tch = re.match('
+00001140: 282e 2a3f 292f 272c 2072 6967 6874 7061  (.*?)/', rightpa
+00001150: 7274 290a 2020 2020 6966 2062 7563 6b65  rt).    if bucke
+00001160: 746d 6174 6368 2069 7320 4e6f 6e65 3a0a  tmatch is None:.
+00001170: 2020 2020 2020 2020 6275 636b 6574 203d          bucket =
+00001180: 2072 6967 6874 7061 7274 0a20 2020 2020   rightpart.     
+00001190: 2020 2070 6174 6820 3d20 2727 0a20 2020     path = ''.   
+000011a0: 2065 6c73 653a 0a20 2020 2020 2020 2062   else:.        b
+000011b0: 7563 6b65 7420 3d20 6275 636b 6574 6d61  ucket = bucketma
+000011c0: 7463 682e 6772 6f75 7028 3129 0a20 2020  tch.group(1).   
+000011d0: 2020 2020 2070 6174 6820 3d20 7269 6768       path = righ
+000011e0: 7470 6172 745b 6c65 6e28 6275 636b 6574  tpart[len(bucket
+000011f0: 2920 2b20 313a 5d0a 2020 2020 7265 7475  ) + 1:].    retu
+00001200: 726e 2062 7563 6b65 742c 2070 6174 680a  rn bucket, path.
+00001210: 0a0a 6465 6620 6765 745f 7363 6f70 6564  ..def get_scoped
+00001220: 5f63 6f6e 6669 6728 7072 6f66 696c 655f  _config(profile_
+00001230: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
+00001240: 7472 5d20 3d20 4e6f 6e65 2920 2d3e 2044  tr] = None) -> D
+00001250: 6963 743a 0a20 2020 2072 6574 7572 6e20  ict:.    return 
+00001260: 6765 745f 7333 5f73 6573 7369 6f6e 280a  get_s3_session(.
+00001270: 2020 2020 2020 2020 7072 6f66 696c 655f          profile_
+00001280: 6e61 6d65 3d70 726f 6669 6c65 5f6e 616d  name=profile_nam
+00001290: 6529 2e5f 7365 7373 696f 6e2e 6765 745f  e)._session.get_
+000012a0: 7363 6f70 6564 5f63 6f6e 6669 6728 290a  scoped_config().
+000012b0: 0a0a 406c 7275 5f63 6163 6865 2829 0a64  ..@lru_cache().d
+000012c0: 6566 2077 6172 6e69 6e67 5f65 6e64 706f  ef warning_endpo
+000012d0: 696e 745f 7572 6c28 6b65 793a 2073 7472  int_url(key: str
+000012e0: 2c20 656e 6470 6f69 6e74 5f75 726c 3a20  , endpoint_url: 
+000012f0: 7374 7229 3a0a 2020 2020 5f6c 6f67 6765  str):.    _logge
+00001300: 722e 696e 666f 2822 7573 696e 6720 2573  r.info("using %s
+00001310: 3a20 2573 2220 2520 286b 6579 2c20 656e  : %s" % (key, en
+00001320: 6470 6f69 6e74 5f75 726c 2929 0a0a 0a64  dpoint_url))...d
+00001330: 6566 2067 6574 5f65 6e64 706f 696e 745f  ef get_endpoint_
+00001340: 7572 6c28 7072 6f66 696c 655f 6e61 6d65  url(profile_name
+00001350: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00001360: 3d20 4e6f 6e65 2920 2d3e 2073 7472 3a0a  = None) -> str:.
+00001370: 2020 2020 2727 2747 6574 2074 6865 2065      '''Get the e
+00001380: 6e64 706f 696e 7420 7572 6c20 6f66 2053  ndpoint url of S
+00001390: 330a 0a20 2020 203a 7265 7475 726e 733a  3..    :returns:
+000013a0: 2053 3320 656e 6470 6f69 6e74 2075 726c   S3 endpoint url
+000013b0: 0a20 2020 2027 2727 0a20 2020 2065 6e76  .    '''.    env
+000013c0: 6972 6f6e 5f6b 6579 203d 2066 277b 7072  iron_key = f'{pr
+000013d0: 6f66 696c 655f 6e61 6d65 7d5f 5f4f 5353  ofile_name}__OSS
+000013e0: 5f45 4e44 504f 494e 5427 2e75 7070 6572  _ENDPOINT'.upper
+000013f0: 280a 2020 2020 2920 6966 2070 726f 6669  (.    ) if profi
+00001400: 6c65 5f6e 616d 6520 656c 7365 2027 4f53  le_name else 'OS
+00001410: 535f 454e 4450 4f49 4e54 270a 2020 2020  S_ENDPOINT'.    
+00001420: 656e 7669 726f 6e5f 656e 6470 6f69 6e74  environ_endpoint
+00001430: 5f75 726c 203d 206f 732e 656e 7669 726f  _url = os.enviro
+00001440: 6e2e 6765 7428 656e 7669 726f 6e5f 6b65  n.get(environ_ke
+00001450: 7929 0a20 2020 2069 6620 656e 7669 726f  y).    if enviro
+00001460: 6e5f 656e 6470 6f69 6e74 5f75 726c 3a0a  n_endpoint_url:.
+00001470: 2020 2020 2020 2020 7761 726e 696e 675f          warning_
+00001480: 656e 6470 6f69 6e74 5f75 726c 2865 6e76  endpoint_url(env
+00001490: 6972 6f6e 5f6b 6579 2c20 656e 7669 726f  iron_key, enviro
+000014a0: 6e5f 656e 6470 6f69 6e74 5f75 726c 290a  n_endpoint_url).
+000014b0: 2020 2020 2020 2020 7265 7475 726e 2065          return e
+000014c0: 6e76 6972 6f6e 5f65 6e64 706f 696e 745f  nviron_endpoint_
+000014d0: 7572 6c0a 2020 2020 7472 793a 0a20 2020  url.    try:.   
+000014e0: 2020 2020 2063 6f6e 6669 675f 656e 6470       config_endp
+000014f0: 6f69 6e74 5f75 726c 203d 2067 6574 5f73  oint_url = get_s
+00001500: 636f 7065 645f 636f 6e66 6967 2870 726f  coped_config(pro
+00001510: 6669 6c65 5f6e 616d 653d 7072 6f66 696c  file_name=profil
+00001520: 655f 6e61 6d65 292e 6765 7428 0a20 2020  e_name).get(.   
+00001530: 2020 2020 2020 2020 2027 7333 272c 207b           's3', {
+00001540: 7d29 2e67 6574 2827 656e 6470 6f69 6e74  }).get('endpoint
+00001550: 5f75 726c 2729 0a20 2020 2020 2020 2069  _url').        i
+00001560: 6620 636f 6e66 6967 5f65 6e64 706f 696e  f config_endpoin
+00001570: 745f 7572 6c3a 0a20 2020 2020 2020 2020  t_url:.         
+00001580: 2020 2077 6172 6e69 6e67 5f65 6e64 706f     warning_endpo
+00001590: 696e 745f 7572 6c28 277e 2f2e 6177 732f  int_url('~/.aws/
+000015a0: 636f 6e66 6967 272c 2063 6f6e 6669 675f  config', config_
+000015b0: 656e 6470 6f69 6e74 5f75 726c 290a 2020  endpoint_url).  
+000015c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000015d0: 2063 6f6e 6669 675f 656e 6470 6f69 6e74   config_endpoint
+000015e0: 5f75 726c 0a20 2020 2065 7863 6570 7420  _url.    except 
+000015f0: 626f 746f 636f 7265 2e65 7863 6570 7469  botocore.excepti
+00001600: 6f6e 732e 5072 6f66 696c 654e 6f74 466f  ons.ProfileNotFo
+00001610: 756e 643a 2020 2320 7072 6167 6d61 3a20  und:  # pragma: 
+00001620: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
+00001630: 2070 6173 730a 2020 2020 7265 7475 726e   pass.    return
+00001640: 2065 6e64 706f 696e 745f 7572 6c0a 0a0a   endpoint_url...
+00001650: 6465 6620 6765 745f 7333 5f73 6573 7369  def get_s3_sessi
+00001660: 6f6e 2870 726f 6669 6c65 5f6e 616d 653d  on(profile_name=
+00001670: 4e6f 6e65 293a 0a20 2020 2027 2727 4765  None):.    '''Ge
+00001680: 7420 5333 2073 6573 7369 6f6e 0a0a 2020  t S3 session..  
+00001690: 2020 3a72 6574 7572 6e73 3a20 5333 2073    :returns: S3 s
+000016a0: 6573 7369 6f6e 0a20 2020 2027 2727 0a20  ession.    '''. 
+000016b0: 2020 2072 6574 7572 6e20 7468 7265 6164     return thread
+000016c0: 5f6c 6f63 616c 280a 2020 2020 2020 2020  _local(.        
+000016d0: 6627 7333 5f73 6573 7369 6f6e 3a7b 7072  f's3_session:{pr
+000016e0: 6f66 696c 655f 6e61 6d65 7d27 2c20 626f  ofile_name}', bo
+000016f0: 746f 332e 5365 7373 696f 6e2c 2070 726f  to3.Session, pro
+00001700: 6669 6c65 5f6e 616d 653d 7072 6f66 696c  file_name=profil
+00001710: 655f 6e61 6d65 290a 0a0a 6465 6620 6765  e_name)...def ge
+00001720: 745f 6163 6365 7373 5f74 6f6b 656e 2870  t_access_token(p
+00001730: 726f 6669 6c65 5f6e 616d 653d 4e6f 6e65  rofile_name=None
+00001740: 293a 0a20 2020 2061 6363 6573 735f 6b65  ):.    access_ke
+00001750: 795f 656e 765f 6e61 6d65 203d 2066 227b  y_env_name = f"{
+00001760: 7072 6f66 696c 655f 6e61 6d65 7d5f 5f41  profile_name}__A
+00001770: 5753 5f41 4343 4553 535f 4b45 595f 4944  WS_ACCESS_KEY_ID
+00001780: 222e 7570 7065 7228 0a20 2020 2029 2069  ".upper(.    ) i
+00001790: 6620 7072 6f66 696c 655f 6e61 6d65 2065  f profile_name e
+000017a0: 6c73 6520 2241 5753 5f41 4343 4553 535f  lse "AWS_ACCESS_
+000017b0: 4b45 595f 4944 220a 2020 2020 7365 6372  KEY_ID".    secr
+000017c0: 6574 5f6b 6579 5f65 6e76 5f6e 616d 6520  et_key_env_name 
+000017d0: 3d20 6622 7b70 726f 6669 6c65 5f6e 616d  = f"{profile_nam
+000017e0: 657d 5f5f 4157 535f 5345 4352 4554 5f41  e}__AWS_SECRET_A
+000017f0: 4343 4553 535f 4b45 5922 2e75 7070 6572  CCESS_KEY".upper
+00001800: 280a 2020 2020 2920 6966 2070 726f 6669  (.    ) if profi
+00001810: 6c65 5f6e 616d 6520 656c 7365 2022 4157  le_name else "AW
+00001820: 535f 5345 4352 4554 5f41 4343 4553 535f  S_SECRET_ACCESS_
+00001830: 4b45 5922 0a20 2020 2061 6363 6573 735f  KEY".    access_
+00001840: 6b65 7920 3d20 6f73 2e67 6574 656e 7628  key = os.getenv(
+00001850: 6163 6365 7373 5f6b 6579 5f65 6e76 5f6e  access_key_env_n
+00001860: 616d 6529 0a20 2020 2073 6563 7265 745f  ame).    secret_
+00001870: 6b65 7920 3d20 6f73 2e67 6574 656e 7628  key = os.getenv(
+00001880: 7365 6372 6574 5f6b 6579 5f65 6e76 5f6e  secret_key_env_n
+00001890: 616d 6529 0a20 2020 2069 6620 6163 6365  ame).    if acce
+000018a0: 7373 5f6b 6579 2061 6e64 2073 6563 7265  ss_key and secre
+000018b0: 745f 6b65 793a 0a20 2020 2020 2020 2072  t_key:.        r
+000018c0: 6574 7572 6e20 6163 6365 7373 5f6b 6579  eturn access_key
+000018d0: 2c20 7365 6372 6574 5f6b 6579 0a0a 2020  , secret_key..  
+000018e0: 2020 6372 6564 656e 7469 616c 7320 3d20    credentials = 
+000018f0: 6765 745f 7333 5f73 6573 7369 6f6e 2870  get_s3_session(p
+00001900: 726f 6669 6c65 5f6e 616d 653d 7072 6f66  rofile_name=prof
+00001910: 696c 655f 6e61 6d65 292e 6765 745f 6372  ile_name).get_cr
+00001920: 6564 656e 7469 616c 7328 290a 2020 2020  edentials().    
+00001930: 6966 2063 7265 6465 6e74 6961 6c73 3a0a  if credentials:.
+00001940: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
+00001950: 6363 6573 735f 6b65 793a 0a20 2020 2020  ccess_key:.     
+00001960: 2020 2020 2020 2061 6363 6573 735f 6b65         access_ke
+00001970: 7920 3d20 6372 6564 656e 7469 616c 732e  y = credentials.
+00001980: 6163 6365 7373 5f6b 6579 0a20 2020 2020  access_key.     
+00001990: 2020 2069 6620 6e6f 7420 7365 6372 6574     if not secret
+000019a0: 5f6b 6579 3a0a 2020 2020 2020 2020 2020  _key:.          
+000019b0: 2020 7365 6372 6574 5f6b 6579 203d 2063    secret_key = c
+000019c0: 7265 6465 6e74 6961 6c73 2e73 6563 7265  redentials.secre
+000019d0: 745f 6b65 790a 2020 2020 7265 7475 726e  t_key.    return
+000019e0: 2061 6363 6573 735f 6b65 792c 2073 6563   access_key, sec
+000019f0: 7265 745f 6b65 790a 0a0a 6465 6620 6765  ret_key...def ge
+00001a00: 745f 7333 5f63 6c69 656e 7428 0a20 2020  t_s3_client(.   
+00001a10: 2020 2020 2063 6f6e 6669 673a 204f 7074       config: Opt
+00001a20: 696f 6e61 6c5b 626f 746f 636f 7265 2e63  ional[botocore.c
+00001a30: 6f6e 6669 672e 436f 6e66 6967 5d20 3d20  onfig.Config] = 
+00001a40: 4e6f 6e65 2c0a 2020 2020 2020 2020 6361  None,.        ca
+00001a50: 6368 655f 6b65 793a 204f 7074 696f 6e61  che_key: Optiona
+00001a60: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00001a70: 2020 2020 2020 2070 726f 6669 6c65 5f6e         profile_n
+00001a80: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
+00001a90: 725d 203d 204e 6f6e 6529 3a0a 2020 2020  r] = None):.    
+00001aa0: 2727 2747 6574 2053 3320 636c 6965 6e74  '''Get S3 client
+00001ab0: 0a0a 2020 2020 3a72 6574 7572 6e73 3a20  ..    :returns: 
+00001ac0: 5333 2063 6c69 656e 740a 2020 2020 2727  S3 client.    ''
+00001ad0: 270a 2020 2020 6966 2063 6163 6865 5f6b  '.    if cache_k
+00001ae0: 6579 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ey is not None:.
+00001af0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00001b00: 6872 6561 645f 6c6f 6361 6c28 0a20 2020  hread_local(.   
+00001b10: 2020 2020 2020 2020 2063 6163 6865 5f6b           cache_k
+00001b20: 6579 2c20 6765 745f 7333 5f63 6c69 656e  ey, get_s3_clien
+00001b30: 742c 2063 6f6e 6669 673d 636f 6e66 6967  t, config=config
+00001b40: 2c20 7072 6f66 696c 655f 6e61 6d65 3d70  , profile_name=p
+00001b50: 726f 6669 6c65 5f6e 616d 6529 0a0a 2020  rofile_name)..  
+00001b60: 2020 6163 6365 7373 5f6b 6579 2c20 7365    access_key, se
+00001b70: 6372 6574 5f6b 6579 203d 2067 6574 5f61  cret_key = get_a
+00001b80: 6363 6573 735f 746f 6b65 6e28 7072 6f66  ccess_token(prof
+00001b90: 696c 655f 6e61 6d65 290a 2020 2020 636c  ile_name).    cl
+00001ba0: 6965 6e74 203d 2067 6574 5f73 335f 7365  ient = get_s3_se
+00001bb0: 7373 696f 6e28 292e 636c 6965 6e74 280a  ssion().client(.
+00001bc0: 2020 2020 2020 2020 2773 3327 2c0a 2020          's3',.  
+00001bd0: 2020 2020 2020 656e 6470 6f69 6e74 5f75        endpoint_u
+00001be0: 726c 3d67 6574 5f65 6e64 706f 696e 745f  rl=get_endpoint_
+00001bf0: 7572 6c28 7072 6f66 696c 655f 6e61 6d65  url(profile_name
+00001c00: 3d70 726f 6669 6c65 5f6e 616d 6529 2c0a  =profile_name),.
+00001c10: 2020 2020 2020 2020 636f 6e66 6967 3d63          config=c
+00001c20: 6f6e 6669 672c 0a20 2020 2020 2020 2061  onfig,.        a
+00001c30: 7773 5f61 6363 6573 735f 6b65 795f 6964  ws_access_key_id
+00001c40: 3d61 6363 6573 735f 6b65 792c 0a20 2020  =access_key,.   
+00001c50: 2020 2020 2061 7773 5f73 6563 7265 745f       aws_secret_
+00001c60: 6163 6365 7373 5f6b 6579 3d73 6563 7265  access_key=secre
+00001c70: 745f 6b65 792c 0a20 2020 2029 0a20 2020  t_key,.    ).   
+00001c80: 2063 6c69 656e 7420 3d20 5f70 6174 6368   client = _patch
+00001c90: 5f6d 616b 655f 7265 7175 6573 7428 636c  _make_request(cl
+00001ca0: 6965 6e74 290a 2020 2020 7265 7475 726e  ient).    return
+00001cb0: 2063 6c69 656e 740a 0a0a 6465 6620 7333   client...def s3
+00001cc0: 5f70 6174 685f 6a6f 696e 2870 6174 683a  _path_join(path:
+00001cd0: 2050 6174 684c 696b 652c 202a 6f74 6865   PathLike, *othe
+00001ce0: 725f 7061 7468 733a 2050 6174 684c 696b  r_paths: PathLik
+00001cf0: 6529 202d 3e20 7374 723a 0a20 2020 2027  e) -> str:.    '
+00001d00: 2727 0a20 2020 2043 6f6e 6361 7420 3220  ''.    Concat 2 
+00001d10: 6f72 206d 6f72 6520 7061 7468 2074 6f20  or more path to 
+00001d20: 6120 636f 6d70 6c65 7465 2070 6174 680a  a complete path.
+00001d30: 0a20 2020 203a 7061 7261 6d20 7061 7468  .    :param path
+00001d40: 3a20 4769 7665 6e20 7061 7468 0a20 2020  : Given path.   
+00001d50: 203a 7061 7261 6d20 6f74 6865 725f 7061   :param other_pa
+00001d60: 7468 733a 2050 6174 6873 2074 6f20 6265  ths: Paths to be
+00001d70: 2063 6f6e 6361 7465 6e61 7465 640a 2020   concatenated.  
+00001d80: 2020 3a72 6574 7572 6e73 3a20 436f 6e63    :returns: Conc
+00001d90: 6174 656e 6174 6564 2063 6f6d 706c 6574  atenated complet
+00001da0: 6520 7061 7468 0a0a 2020 2020 2e2e 206e  e path..    .. n
+00001db0: 6f74 6520 3a3a 0a0a 2020 2020 2020 2020  ote ::..        
+00001dc0: 5468 6520 6469 6666 6572 656e 6365 2062  The difference b
+00001dd0: 6574 7765 656e 2074 6869 7320 6675 6e63  etween this func
+00001de0: 7469 6f6e 2061 6e64 2060 606f 732e 7061  tion and ``os.pa
+00001df0: 7468 2e6a 6f69 6e60 6020 6973 2074 6861  th.join`` is tha
+00001e00: 7420 7468 6973 2066 756e 6374 696f 6e20  t this function 
+00001e10: 6967 6e6f 7265 7320 6c65 6674 2073 6964  ignores left sid
+00001e20: 6520 736c 6173 6820 2877 6869 6368 2069  e slash (which i
+00001e30: 6e64 6963 6174 6573 2061 6273 6f6c 7574  ndicates absolut
+00001e40: 6520 7061 7468 2920 696e 2060 606f 7468  e path) in ``oth
+00001e50: 6572 5f70 6174 6873 6060 2061 6e64 2077  er_paths`` and w
+00001e60: 696c 6c20 6469 7265 6374 6c79 2063 6f6e  ill directly con
+00001e70: 6361 742e 0a20 2020 2020 2020 2065 2e67  cat..        e.g
+00001e80: 2e20 6f73 2e70 6174 682e 6a6f 696e 2827  . os.path.join('
+00001e90: 2f70 6174 6827 2c20 2774 6f27 2c20 272f  /path', 'to', '/
+00001ea0: 6669 6c65 2729 203d 3e20 272f 6669 6c65  file') => '/file
+00001eb0: 272c 2062 7574 2073 335f 7061 7468 5f6a  ', but s3_path_j
+00001ec0: 6f69 6e28 272f 7061 7468 272c 2027 746f  oin('/path', 'to
+00001ed0: 272c 2027 2f66 696c 6527 2920 3d3e 2027  ', '/file') => '
+00001ee0: 2f70 6174 682f 746f 2f66 696c 6527 0a20  /path/to/file'. 
+00001ef0: 2020 2027 2727 0a20 2020 2072 6574 7572     '''.    retur
+00001f00: 6e20 7572 695f 6a6f 696e 2866 7370 6174  n uri_join(fspat
+00001f10: 6828 7061 7468 292c 202a 6d61 7028 6673  h(path), *map(fs
+00001f20: 7061 7468 2c20 6f74 6865 725f 7061 7468  path, other_path
+00001f30: 7329 290a 0a0a 6465 6620 5f6c 6973 745f  s))...def _list_
+00001f40: 616c 6c5f 6275 636b 6574 7328 7072 6f66  all_buckets(prof
+00001f50: 696c 655f 6e61 6d65 3a20 4f70 7469 6f6e  ile_name: Option
+00001f60: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2920  al[str] = None) 
+00001f70: 2d3e 204c 6973 745b 7374 725d 3a0a 2020  -> List[str]:.  
+00001f80: 2020 636c 6965 6e74 203d 2067 6574 5f73    client = get_s
+00001f90: 335f 636c 6965 6e74 2870 726f 6669 6c65  3_client(profile
+00001fa0: 5f6e 616d 653d 7072 6f66 696c 655f 6e61  _name=profile_na
+00001fb0: 6d65 290a 2020 2020 7265 7370 6f6e 7365  me).    response
+00001fc0: 203d 2063 6c69 656e 742e 6c69 7374 5f62   = client.list_b
+00001fd0: 7563 6b65 7473 2829 0a20 2020 2072 6574  uckets().    ret
+00001fe0: 7572 6e20 5b63 6f6e 7465 6e74 5b27 4e61  urn [content['Na
+00001ff0: 6d65 275d 2066 6f72 2063 6f6e 7465 6e74  me'] for content
+00002000: 2069 6e20 7265 7370 6f6e 7365 5b27 4275   in response['Bu
+00002010: 636b 6574 7327 5d5d 0a0a 0a64 6566 205f  ckets']]...def _
+00002020: 7061 7273 655f 7333 5f75 726c 5f69 676e  parse_s3_url_ign
+00002030: 6f72 655f 6272 6163 6528 7333 5f75 726c  ore_brace(s3_url
+00002040: 3a20 7374 7229 202d 3e20 5475 706c 655b  : str) -> Tuple[
+00002050: 7374 722c 2073 7472 5d3a 0a20 2020 2073  str, str]:.    s
+00002060: 335f 7572 6c20 3d20 6673 7061 7468 2873  3_url = fspath(s
+00002070: 335f 7572 6c29 0a20 2020 2073 335f 7363  3_url).    s3_sc
+00002080: 6865 6d65 2c20 7269 6768 7470 6172 7420  heme, rightpart 
+00002090: 3d20 7333 5f75 726c 5b3a 355d 2c20 7333  = s3_url[:5], s3
+000020a0: 5f75 726c 5b35 3a5d 0a20 2020 2069 6620  _url[5:].    if 
+000020b0: 7333 5f73 6368 656d 6520 213d 2027 7333  s3_scheme != 's3
+000020c0: 3a2f 2f27 3a0a 2020 2020 2020 2020 7261  ://':.        ra
+000020d0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+000020e0: 4e6f 7420 6120 7333 2075 726c 3a20 2572  Not a s3 url: %r
+000020f0: 2720 2520 7333 5f75 726c 290a 2020 2020  ' % s3_url).    
+00002100: 6c65 6674 5f62 7261 6365 203d 2046 616c  left_brace = Fal
+00002110: 7365 0a20 2020 2066 6f72 2063 7572 7265  se.    for curre
+00002120: 6e74 5f69 6e64 6578 2c20 6375 7272 656e  nt_index, curren
+00002130: 745f 6368 6172 6163 7465 7220 696e 2065  t_character in e
+00002140: 6e75 6d65 7261 7465 2872 6967 6874 7061  numerate(rightpa
+00002150: 7274 293a 0a20 2020 2020 2020 2069 6620  rt):.        if 
+00002160: 6375 7272 656e 745f 6368 6172 6163 7465  current_characte
+00002170: 7220 3d3d 2022 2f22 2061 6e64 206c 6566  r == "/" and lef
+00002180: 745f 6272 6163 6520 6973 2046 616c 7365  t_brace is False
+00002190: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000021a0: 7475 726e 2072 6967 6874 7061 7274 5b3a  turn rightpart[:
+000021b0: 6375 7272 656e 745f 696e 6465 785d 2c20  current_index], 
+000021c0: 7269 6768 7470 6172 745b 6375 7272 656e  rightpart[curren
+000021d0: 745f 696e 6465 7820 2b20 313a 5d0a 2020  t_index + 1:].  
+000021e0: 2020 2020 2020 656c 6966 2063 7572 7265        elif curre
+000021f0: 6e74 5f63 6861 7261 6374 6572 203d 3d20  nt_character == 
+00002200: 227b 223a 0a20 2020 2020 2020 2020 2020  "{":.           
+00002210: 206c 6566 745f 6272 6163 6520 3d20 5472   left_brace = Tr
+00002220: 7565 0a20 2020 2020 2020 2065 6c69 6620  ue.        elif 
+00002230: 6375 7272 656e 745f 6368 6172 6163 7465  current_characte
+00002240: 7220 3d3d 2022 7d22 3a0a 2020 2020 2020  r == "}":.      
+00002250: 2020 2020 2020 6c65 6674 5f62 7261 6365        left_brace
+00002260: 203d 2046 616c 7365 0a20 2020 2072 6574   = False.    ret
+00002270: 7572 6e20 7269 6768 7470 6172 742c 2022  urn rightpart, "
+00002280: 220a 0a0a 6465 6620 5f67 726f 7570 5f73  "...def _group_s
+00002290: 3370 6174 685f 6279 5f62 7563 6b65 7428  3path_by_bucket(
+000022a0: 0a20 2020 2020 2020 2073 335f 7061 7468  .        s3_path
+000022b0: 6e61 6d65 3a20 7374 722c 2070 726f 6669  name: str, profi
+000022c0: 6c65 5f6e 616d 653a 204f 7074 696f 6e61  le_name: Optiona
+000022d0: 6c5b 7374 725d 203d 204e 6f6e 6529 202d  l[str] = None) -
+000022e0: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
+000022f0: 2062 7563 6b65 742c 206b 6579 203d 205f   bucket, key = _
+00002300: 7061 7273 655f 7333 5f75 726c 5f69 676e  parse_s3_url_ign
+00002310: 6f72 655f 6272 6163 6528 7333 5f70 6174  ore_brace(s3_pat
+00002320: 686e 616d 6529 0a20 2020 2069 6620 6e6f  hname).    if no
+00002330: 7420 6275 636b 6574 3a0a 2020 2020 2020  t bucket:.      
+00002340: 2020 6966 206e 6f74 206b 6579 3a0a 2020    if not key:.  
+00002350: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00002360: 556e 7375 7070 6f72 7465 6445 7272 6f72  UnsupportedError
+00002370: 2827 476c 6f62 2077 686f 6c65 2073 3327  ('Glob whole s3'
+00002380: 2c20 7333 5f70 6174 686e 616d 6529 0a20  , s3_pathname). 
+00002390: 2020 2020 2020 2072 6169 7365 2053 3342         raise S3B
+000023a0: 7563 6b65 744e 6f74 466f 756e 6445 7272  ucketNotFoundErr
+000023b0: 6f72 2827 456d 7074 7920 6275 636b 6574  or('Empty bucket
+000023c0: 206e 616d 653a 2025 7227 2025 2073 335f   name: %r' % s3_
+000023d0: 7061 7468 6e61 6d65 290a 0a20 2020 2067  pathname)..    g
+000023e0: 726f 7570 6564 5f70 6174 6820 3d20 5b5d  rouped_path = []
+000023f0: 0a0a 2020 2020 6465 6620 6765 6e65 7261  ..    def genera
+00002400: 7465 5f73 335f 7061 7468 2862 7563 6b65  te_s3_path(bucke
+00002410: 743a 2073 7472 2c20 6b65 793a 2073 7472  t: str, key: str
+00002420: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00002430: 2020 6966 206b 6579 3a0a 2020 2020 2020    if key:.      
+00002440: 2020 2020 2020 7265 7475 726e 2022 7333        return "s3
+00002450: 3a2f 2f25 732f 2573 2220 2520 2862 7563  ://%s/%s" % (buc
+00002460: 6b65 742c 206b 6579 290a 2020 2020 2020  ket, key).      
+00002470: 2020 7265 7475 726e 2022 7333 3a2f 2f25    return "s3://%
+00002480: 7325 7322 2025 2028 6275 636b 6574 2c20  s%s" % (bucket, 
+00002490: 222f 2220 6966 2073 335f 7061 7468 6e61  "/" if s3_pathna
+000024a0: 6d65 2e65 6e64 7377 6974 6828 222f 2229  me.endswith("/")
+000024b0: 2065 6c73 6520 2222 290a 0a20 2020 2061   else "")..    a
+000024c0: 6c6c 5f62 7563 6b65 7420 3d20 6c72 755f  ll_bucket = lru_
+000024d0: 6361 6368 6528 6d61 7873 697a 653d 3129  cache(maxsize=1)
+000024e0: 285f 6c69 7374 5f61 6c6c 5f62 7563 6b65  (_list_all_bucke
+000024f0: 7473 290a 2020 2020 666f 7220 6275 636b  ts).    for buck
+00002500: 6574 6e61 6d65 2069 6e20 756e 676c 6f62  etname in unglob
+00002510: 6c69 7a65 2862 7563 6b65 7429 3a0a 2020  lize(bucket):.  
+00002520: 2020 2020 2020 6966 2068 6173 5f6d 6167        if has_mag
+00002530: 6963 2862 7563 6b65 746e 616d 6529 3a0a  ic(bucketname):.
+00002540: 2020 2020 2020 2020 2020 2020 7370 6c69              spli
+00002550: 745f 6275 636b 6574 6e61 6d65 203d 2062  t_bucketname = b
+00002560: 7563 6b65 746e 616d 652e 7370 6c69 7428  ucketname.split(
+00002570: 222f 222c 2031 290a 2020 2020 2020 2020  "/", 1).        
+00002580: 2020 2020 7061 7468 5f70 6172 7420 3d20      path_part = 
+00002590: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+000025a0: 2069 6620 6c65 6e28 7370 6c69 745f 6275   if len(split_bu
+000025b0: 636b 6574 6e61 6d65 2920 3d3d 2032 3a0a  cketname) == 2:.
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 6275 636b 6574 6e61 6d65 2c20 7061 7468  bucketname, path
+000025e0: 5f70 6172 7420 3d20 7370 6c69 745f 6275  _part = split_bu
+000025f0: 636b 6574 6e61 6d65 0a20 2020 2020 2020  cketname.       
+00002600: 2020 2020 2070 6174 7465 726e 203d 2072       pattern = r
+00002610: 652e 636f 6d70 696c 6528 7472 616e 736c  e.compile(transl
+00002620: 6174 6528 7265 2e73 7562 2872 275c 2a7b  ate(re.sub(r'\*{
+00002630: 322c 7d27 2c20 272a 272c 2062 7563 6b65  2,}', '*', bucke
+00002640: 746e 616d 6529 2929 0a0a 2020 2020 2020  tname)))..      
+00002650: 2020 2020 2020 666f 7220 6275 636b 6574        for bucket
+00002660: 2069 6e20 616c 6c5f 6275 636b 6574 2870   in all_bucket(p
+00002670: 726f 6669 6c65 5f6e 616d 6529 3a0a 2020  rofile_name):.  
+00002680: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002690: 2070 6174 7465 726e 2e66 756c 6c6d 6174   pattern.fullmat
+000026a0: 6368 2862 7563 6b65 7429 2069 7320 6e6f  ch(bucket) is no
+000026b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000026c0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+000026d0: 6174 685f 7061 7274 2069 7320 6e6f 7420  ath_part is not 
+000026e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000026f0: 2020 2020 2020 2020 2020 2020 2020 6275                bu
+00002700: 636b 6574 203d 2022 2573 2f25 7322 2025  cket = "%s/%s" %
+00002710: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00002720: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00002730: 7563 6b65 742c 2070 6174 685f 7061 7274  ucket, path_part
+00002740: 2920 2023 2070 7261 676d 613a 206e 6f20  )  # pragma: no 
+00002750: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+00002760: 2020 2020 2020 2020 2020 6772 6f75 7065            groupe
+00002770: 645f 7061 7468 2e61 7070 656e 6428 6765  d_path.append(ge
+00002780: 6e65 7261 7465 5f73 335f 7061 7468 2862  nerate_s3_path(b
+00002790: 7563 6b65 742c 206b 6579 2929 0a20 2020  ucket, key)).   
+000027a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000027b0: 2020 2020 2020 2067 726f 7570 6564 5f70         grouped_p
+000027c0: 6174 682e 6170 7065 6e64 2867 656e 6572  ath.append(gener
+000027d0: 6174 655f 7333 5f70 6174 6828 6275 636b  ate_s3_path(buck
+000027e0: 6574 6e61 6d65 2c20 6b65 7929 290a 0a20  etname, key)).. 
+000027f0: 2020 2072 6574 7572 6e20 6772 6f75 7065     return groupe
+00002800: 645f 7061 7468 0a0a 0a64 6566 205f 7333  d_path...def _s3
+00002810: 5f73 706c 6974 5f6d 6167 6963 5f69 676e  _split_magic_ign
+00002820: 6f72 655f 6272 6163 6528 7333 5f70 6174  ore_brace(s3_pat
+00002830: 686e 616d 653a 2073 7472 2920 2d3e 2054  hname: str) -> T
+00002840: 7570 6c65 5b73 7472 2c20 7374 725d 3a0a  uple[str, str]:.
+00002850: 2020 2020 6966 206e 6f74 2073 335f 7061      if not s3_pa
+00002860: 7468 6e61 6d65 3a0a 2020 2020 2020 2020  thname:.        
+00002870: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00002880: 2822 7333 5f70 6174 686e 616d 653a 2025  ("s3_pathname: %
+00002890: 7322 2c20 7333 5f70 6174 686e 616d 6529  s", s3_pathname)
+000028a0: 0a0a 2020 2020 6861 735f 7072 6f74 6f63  ..    has_protoc
+000028b0: 6f6c 203d 2046 616c 7365 0a20 2020 2069  ol = False.    i
+000028c0: 6620 7333 5f70 6174 686e 616d 652e 7374  f s3_pathname.st
+000028d0: 6172 7473 7769 7468 2822 7333 3a2f 2f22  artswith("s3://"
+000028e0: 293a 0a20 2020 2020 2020 2068 6173 5f70  ):.        has_p
+000028f0: 726f 746f 636f 6c20 3d20 5472 7565 0a20  rotocol = True. 
+00002900: 2020 2020 2020 2073 335f 7061 7468 6e61         s3_pathna
+00002910: 6d65 203d 2073 335f 7061 7468 6e61 6d65  me = s3_pathname
+00002920: 5b35 3a5d 0a0a 2020 2020 6861 735f 6465  [5:]..    has_de
+00002930: 6c69 6d69 7465 7220 3d20 4661 6c73 650a  limiter = False.
+00002940: 2020 2020 6966 2073 335f 7061 7468 6e61      if s3_pathna
+00002950: 6d65 2e65 6e64 7377 6974 6828 222f 2229  me.endswith("/")
+00002960: 3a0a 2020 2020 2020 2020 6861 735f 6465  :.        has_de
+00002970: 6c69 6d69 7465 7220 3d20 5472 7565 0a20  limiter = True. 
+00002980: 2020 2020 2020 2073 335f 7061 7468 6e61         s3_pathna
+00002990: 6d65 203d 2073 335f 7061 7468 6e61 6d65  me = s3_pathname
+000029a0: 5b3a 2d31 5d0a 0a20 2020 206e 6f72 6d61  [:-1]..    norma
+000029b0: 6c5f 7061 7274 7320 3d20 5b5d 0a20 2020  l_parts = [].   
+000029c0: 206d 6167 6963 5f70 6172 7473 203d 205b   magic_parts = [
+000029d0: 5d0a 2020 2020 6c65 6674 5f62 7261 6365  ].    left_brace
+000029e0: 203d 2046 616c 7365 0a20 2020 206c 6566   = False.    lef
+000029f0: 745f 696e 6465 7820 3d20 300a 2020 2020  t_index = 0.    
+00002a00: 666f 7220 6375 7272 656e 745f 696e 6465  for current_inde
+00002a10: 782c 2063 7572 7265 6e74 5f63 6861 7261  x, current_chara
+00002a20: 6374 6572 2069 6e20 656e 756d 6572 6174  cter in enumerat
+00002a30: 6528 7333 5f70 6174 686e 616d 6529 3a0a  e(s3_pathname):.
+00002a40: 2020 2020 2020 2020 6966 2063 7572 7265          if curre
+00002a50: 6e74 5f63 6861 7261 6374 6572 203d 3d20  nt_character == 
+00002a60: 222f 2220 616e 6420 6c65 6674 5f62 7261  "/" and left_bra
+00002a70: 6365 2069 7320 4661 6c73 653a 0a20 2020  ce is False:.   
+00002a80: 2020 2020 2020 2020 2069 6620 6861 735f           if has_
+00002a90: 6d61 6769 635f 6967 6e6f 7265 5f62 7261  magic_ignore_bra
+00002aa0: 6365 2873 335f 7061 7468 6e61 6d65 5b6c  ce(s3_pathname[l
+00002ab0: 6566 745f 696e 6465 783a 6375 7272 656e  eft_index:curren
+00002ac0: 745f 696e 6465 785d 293a 0a20 2020 2020  t_index]):.     
+00002ad0: 2020 2020 2020 2020 2020 206d 6167 6963             magic
+00002ae0: 5f70 6172 7473 2e61 7070 656e 6428 7333  _parts.append(s3
+00002af0: 5f70 6174 686e 616d 655b 6c65 6674 5f69  _pathname[left_i
+00002b00: 6e64 6578 3a63 7572 7265 6e74 5f69 6e64  ndex:current_ind
+00002b10: 6578 5d29 0a20 2020 2020 2020 2020 2020  ex]).           
+00002b20: 2020 2020 2069 6620 7333 5f70 6174 686e       if s3_pathn
+00002b30: 616d 655b 6375 7272 656e 745f 696e 6465  ame[current_inde
+00002b40: 7820 2b20 313a 5d3a 0a20 2020 2020 2020  x + 1:]:.       
+00002b50: 2020 2020 2020 2020 2020 2020 206d 6167               mag
+00002b60: 6963 5f70 6172 7473 2e61 7070 656e 6428  ic_parts.append(
+00002b70: 7333 5f70 6174 686e 616d 655b 6375 7272  s3_pathname[curr
+00002b80: 656e 745f 696e 6465 7820 2b20 313a 5d29  ent_index + 1:])
+00002b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ba0: 2020 2020 206c 6566 745f 696e 6465 7820       left_index 
+00002bb0: 3d20 6c65 6e28 7333 5f70 6174 686e 616d  = len(s3_pathnam
+00002bc0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00002bd0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00002be0: 2020 2020 206e 6f72 6d61 6c5f 7061 7274       normal_part
+00002bf0: 732e 6170 7065 6e64 2873 335f 7061 7468  s.append(s3_path
+00002c00: 6e61 6d65 5b6c 6566 745f 696e 6465 783a  name[left_index:
+00002c10: 6375 7272 656e 745f 696e 6465 785d 290a  current_index]).
+00002c20: 2020 2020 2020 2020 2020 2020 6c65 6674              left
+00002c30: 5f69 6e64 6578 203d 2063 7572 7265 6e74  _index = current
+00002c40: 5f69 6e64 6578 202b 2031 0a20 2020 2020  _index + 1.     
+00002c50: 2020 2065 6c69 6620 6375 7272 656e 745f     elif current_
+00002c60: 6368 6172 6163 7465 7220 3d3d 2022 7b22  character == "{"
+00002c70: 3a0a 2020 2020 2020 2020 2020 2020 6c65  :.            le
+00002c80: 6674 5f62 7261 6365 203d 2054 7275 650a  ft_brace = True.
+00002c90: 2020 2020 2020 2020 656c 6966 2063 7572          elif cur
+00002ca0: 7265 6e74 5f63 6861 7261 6374 6572 203d  rent_character =
+00002cb0: 3d20 227d 223a 0a20 2020 2020 2020 2020  = "}":.         
+00002cc0: 2020 206c 6566 745f 6272 6163 6520 3d20     left_brace = 
+00002cd0: 4661 6c73 650a 2020 2020 6966 2073 335f  False.    if s3_
+00002ce0: 7061 7468 6e61 6d65 5b6c 6566 745f 696e  pathname[left_in
+00002cf0: 6465 783a 5d3a 0a20 2020 2020 2020 2069  dex:]:.        i
+00002d00: 6620 6861 735f 6d61 6769 635f 6967 6e6f  f has_magic_igno
+00002d10: 7265 5f62 7261 6365 2873 335f 7061 7468  re_brace(s3_path
+00002d20: 6e61 6d65 5b6c 6566 745f 696e 6465 783a  name[left_index:
+00002d30: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00002d40: 6d61 6769 635f 7061 7274 732e 6170 7065  magic_parts.appe
+00002d50: 6e64 2873 335f 7061 7468 6e61 6d65 5b6c  nd(s3_pathname[l
+00002d60: 6566 745f 696e 6465 783a 5d29 0a20 2020  eft_index:]).   
+00002d70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00002d80: 2020 2020 2020 206e 6f72 6d61 6c5f 7061         normal_pa
+00002d90: 7274 732e 6170 7065 6e64 2873 335f 7061  rts.append(s3_pa
+00002da0: 7468 6e61 6d65 5b6c 6566 745f 696e 6465  thname[left_inde
+00002db0: 783a 5d29 0a0a 2020 2020 6966 2068 6173  x:])..    if has
+00002dc0: 5f70 726f 746f 636f 6c20 616e 6420 6e6f  _protocol and no
+00002dd0: 726d 616c 5f70 6172 7473 3a0a 2020 2020  rmal_parts:.    
+00002de0: 2020 2020 6e6f 726d 616c 5f70 6172 7473      normal_parts
+00002df0: 2e69 6e73 6572 7428 302c 2022 7333 3a2f  .insert(0, "s3:/
+00002e00: 2229 0a20 2020 2065 6c69 6620 6861 735f  ").    elif has_
+00002e10: 7072 6f74 6f63 6f6c 3a0a 2020 2020 2020  protocol:.      
+00002e20: 2020 6d61 6769 635f 7061 7274 732e 696e    magic_parts.in
+00002e30: 7365 7274 2830 2c20 2273 333a 2f22 290a  sert(0, "s3:/").
+00002e40: 0a20 2020 2069 6620 6861 735f 6465 6c69  .    if has_deli
+00002e50: 6d69 7465 7220 616e 6420 6d61 6769 635f  miter and magic_
+00002e60: 7061 7274 733a 0a20 2020 2020 2020 206d  parts:.        m
+00002e70: 6167 6963 5f70 6172 7473 2e61 7070 656e  agic_parts.appen
+00002e80: 6428 2222 290a 2020 2020 656c 6966 2068  d("").    elif h
+00002e90: 6173 5f64 656c 696d 6974 6572 3a0a 2020  as_delimiter:.  
+00002ea0: 2020 2020 2020 6e6f 726d 616c 5f70 6172        normal_par
+00002eb0: 7473 2e61 7070 656e 6428 2222 290a 0a20  ts.append("").. 
+00002ec0: 2020 2072 6574 7572 6e20 222f 222e 6a6f     return "/".jo
+00002ed0: 696e 286e 6f72 6d61 6c5f 7061 7274 7329  in(normal_parts)
+00002ee0: 2c20 222f 222e 6a6f 696e 286d 6167 6963  , "/".join(magic
+00002ef0: 5f70 6172 7473 290a 0a0a 6465 6620 5f67  _parts)...def _g
+00002f00: 726f 7570 5f73 3370 6174 685f 6279 5f70  roup_s3path_by_p
+00002f10: 7265 6669 7828 7333 5f70 6174 686e 616d  refix(s3_pathnam
+00002f20: 653a 2073 7472 2920 2d3e 204c 6973 745b  e: str) -> List[
+00002f30: 7374 725d 3a0a 0a20 2020 205f 2c20 6b65  str]:..    _, ke
+00002f40: 7920 3d20 7061 7273 655f 7333 5f75 726c  y = parse_s3_url
+00002f50: 2873 335f 7061 7468 6e61 6d65 290a 2020  (s3_pathname).  
+00002f60: 2020 6966 206e 6f74 206b 6579 3a0a 2020    if not key:.  
+00002f70: 2020 2020 2020 7265 7475 726e 2075 6e67        return ung
+00002f80: 6c6f 626c 697a 6528 7333 5f70 6174 686e  loblize(s3_pathn
+00002f90: 616d 6529 0a0a 2020 2020 746f 705f 6469  ame)..    top_di
+00002fa0: 722c 206d 6167 6963 5f70 6172 7420 3d20  r, magic_part = 
+00002fb0: 5f73 335f 7370 6c69 745f 6d61 6769 635f  _s3_split_magic_
+00002fc0: 6967 6e6f 7265 5f62 7261 6365 2873 335f  ignore_brace(s3_
+00002fd0: 7061 7468 6e61 6d65 290a 2020 2020 6966  pathname).    if
+00002fe0: 206e 6f74 2074 6f70 5f64 6972 3a0a 2020   not top_dir:.  
+00002ff0: 2020 2020 2020 7265 7475 726e 205b 6d61        return [ma
+00003000: 6769 635f 7061 7274 5d0a 2020 2020 6772  gic_part].    gr
+00003010: 6f75 7065 645f 7061 7468 203d 205b 5d0a  ouped_path = [].
+00003020: 2020 2020 666f 7220 7061 7468 6e61 6d65      for pathname
+00003030: 2069 6e20 756e 676c 6f62 6c69 7a65 2874   in ungloblize(t
+00003040: 6f70 5f64 6972 293a 0a20 2020 2020 2020  op_dir):.       
+00003050: 2069 6620 6d61 6769 635f 7061 7274 3a0a   if magic_part:.
+00003060: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00003070: 6e61 6d65 203d 2022 2f22 2e6a 6f69 6e28  name = "/".join(
+00003080: 5b70 6174 686e 616d 652c 206d 6167 6963  [pathname, magic
+00003090: 5f70 6172 745d 290a 2020 2020 2020 2020  _part]).        
+000030a0: 6772 6f75 7065 645f 7061 7468 2e61 7070  grouped_path.app
+000030b0: 656e 6428 7061 7468 6e61 6d65 290a 2020  end(pathname).  
+000030c0: 2020 7265 7475 726e 2067 726f 7570 6564    return grouped
+000030d0: 5f70 6174 680a 0a0a 6465 6620 5f62 6563  _path...def _bec
+000030e0: 6f6d 655f 7072 6566 6978 2870 7265 6669  ome_prefix(prefi
+000030f0: 783a 2073 7472 2920 2d3e 2073 7472 3a0a  x: str) -> str:.
+00003100: 2020 2020 6966 2070 7265 6669 7820 213d      if prefix !=
+00003110: 2027 2720 616e 6420 6e6f 7420 7072 6566   '' and not pref
+00003120: 6978 2e65 6e64 7377 6974 6828 272f 2729  ix.endswith('/')
+00003130: 3a0a 2020 2020 2020 2020 7072 6566 6978  :.        prefix
+00003140: 202b 3d20 272f 270a 2020 2020 7265 7475   += '/'.    retu
+00003150: 726e 2070 7265 6669 780a 0a0a 6465 6620  rn prefix...def 
+00003160: 5f73 335f 7370 6c69 745f 6d61 6769 6328  _s3_split_magic(
+00003170: 7333 5f70 6174 686e 616d 653a 2073 7472  s3_pathname: str
+00003180: 2920 2d3e 2054 7570 6c65 5b73 7472 2c20  ) -> Tuple[str, 
+00003190: 7374 725d 3a0a 2020 2020 6966 206e 6f74  str]:.    if not
+000031a0: 2068 6173 5f6d 6167 6963 2873 335f 7061   has_magic(s3_pa
+000031b0: 7468 6e61 6d65 293a 0a20 2020 2020 2020  thname):.       
+000031c0: 2072 6574 7572 6e20 7333 5f70 6174 686e   return s3_pathn
+000031d0: 616d 652c 2027 270a 2020 2020 6465 6c69  ame, ''.    deli
+000031e0: 6d69 7465 7220 3d20 272f 270a 2020 2020  miter = '/'.    
+000031f0: 6e6f 726d 616c 5f70 6172 7473 203d 205b  normal_parts = [
+00003200: 5d0a 2020 2020 6d61 6769 635f 7061 7274  ].    magic_part
+00003210: 7320 3d20 5b5d 0a20 2020 2061 6c6c 5f70  s = [].    all_p
+00003220: 6172 7473 203d 2073 335f 7061 7468 6e61  arts = s3_pathna
+00003230: 6d65 2e73 706c 6974 2864 656c 696d 6974  me.split(delimit
+00003240: 6572 290a 2020 2020 666f 7220 692c 2070  er).    for i, p
+00003250: 6172 7420 696e 2065 6e75 6d65 7261 7465  art in enumerate
+00003260: 2861 6c6c 5f70 6172 7473 293a 0a20 2020  (all_parts):.   
+00003270: 2020 2020 2069 6620 6e6f 7420 6861 735f       if not has_
+00003280: 6d61 6769 6328 7061 7274 293a 0a20 2020  magic(part):.   
+00003290: 2020 2020 2020 2020 206e 6f72 6d61 6c5f           normal_
+000032a0: 7061 7274 732e 6170 7065 6e64 2870 6172  parts.append(par
+000032b0: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
+000032c0: 0a20 2020 2020 2020 2020 2020 206d 6167  .            mag
+000032d0: 6963 5f70 6172 7473 203d 2061 6c6c 5f70  ic_parts = all_p
+000032e0: 6172 7473 5b69 3a5d 0a20 2020 2020 2020  arts[i:].       
+000032f0: 2020 2020 2062 7265 616b 0a20 2020 2072       break.    r
+00003300: 6574 7572 6e20 6465 6c69 6d69 7465 722e  eturn delimiter.
+00003310: 6a6f 696e 286e 6f72 6d61 6c5f 7061 7274  join(normal_part
+00003320: 7329 2c20 6465 6c69 6d69 7465 722e 6a6f  s), delimiter.jo
+00003330: 696e 286d 6167 6963 5f70 6172 7473 290a  in(magic_parts).
+00003340: 0a0a 6465 6620 5f6c 6973 745f 6f62 6a65  ..def _list_obje
+00003350: 6374 735f 7265 6375 7273 6976 6528 0a20  cts_recursive(. 
+00003360: 2020 2020 2020 2073 335f 636c 6965 6e74         s3_client
+00003370: 2c20 6275 636b 6574 3a20 7374 722c 2070  , bucket: str, p
+00003380: 7265 6669 783a 2073 7472 2c20 6465 6c69  refix: str, deli
+00003390: 6d69 7465 723a 2073 7472 203d 2027 2729  miter: str = '')
+000033a0: 3a0a 0a20 2020 2072 6573 7020 3d20 7333  :..    resp = s3
+000033b0: 5f63 6c69 656e 742e 6c69 7374 5f6f 626a  _client.list_obj
+000033c0: 6563 7473 5f76 3228 0a20 2020 2020 2020  ects_v2(.       
+000033d0: 2042 7563 6b65 743d 6275 636b 6574 2c20   Bucket=bucket, 
+000033e0: 5072 6566 6978 3d70 7265 6669 782c 2044  Prefix=prefix, D
+000033f0: 656c 696d 6974 6572 3d64 656c 696d 6974  elimiter=delimit
+00003400: 6572 2c20 4d61 784b 6579 733d 6d61 785f  er, MaxKeys=max_
+00003410: 6b65 7973 290a 0a20 2020 2077 6869 6c65  keys)..    while
+00003420: 2054 7275 653a 0a20 2020 2020 2020 2079   True:.        y
+00003430: 6965 6c64 2072 6573 700a 0a20 2020 2020  ield resp..     
+00003440: 2020 2069 6620 6e6f 7420 7265 7370 5b27     if not resp['
+00003450: 4973 5472 756e 6361 7465 6427 5d3a 0a20  IsTruncated']:. 
+00003460: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00003470: 0a0a 2020 2020 2020 2020 7265 7370 203d  ..        resp =
+00003480: 2073 335f 636c 6965 6e74 2e6c 6973 745f   s3_client.list_
+00003490: 6f62 6a65 6374 735f 7632 280a 2020 2020  objects_v2(.    
+000034a0: 2020 2020 2020 2020 4275 636b 6574 3d62          Bucket=b
+000034b0: 7563 6b65 742c 0a20 2020 2020 2020 2020  ucket,.         
+000034c0: 2020 2050 7265 6669 783d 7072 6566 6978     Prefix=prefix
+000034d0: 2c0a 2020 2020 2020 2020 2020 2020 4465  ,.            De
+000034e0: 6c69 6d69 7465 723d 6465 6c69 6d69 7465  limiter=delimite
+000034f0: 722c 0a20 2020 2020 2020 2020 2020 2043  r,.            C
+00003500: 6f6e 7469 6e75 6174 696f 6e54 6f6b 656e  ontinuationToken
+00003510: 3d72 6573 705b 274e 6578 7443 6f6e 7469  =resp['NextConti
+00003520: 6e75 6174 696f 6e54 6f6b 656e 275d 2c0a  nuationToken'],.
+00003530: 2020 2020 2020 2020 2020 2020 4d61 784b              MaxK
+00003540: 6579 733d 6d61 785f 6b65 7973 290a 0a0a  eys=max_keys)...
+00003550: 6465 6620 5f6d 616b 655f 7374 6174 2863  def _make_stat(c
+00003560: 6f6e 7465 6e74 3a20 4469 6374 5b73 7472  ontent: Dict[str
+00003570: 2c20 416e 795d 293a 0a20 2020 2072 6574  , Any]):.    ret
+00003580: 7572 6e20 5374 6174 5265 7375 6c74 280a  urn StatResult(.
+00003590: 2020 2020 2020 2020 6973 6c6e 6b3d 636f          islnk=co
+000035a0: 6e74 656e 742e 6765 7428 2769 736c 6e6b  ntent.get('islnk
+000035b0: 272c 2046 616c 7365 292c 0a20 2020 2020  ', False),.     
+000035c0: 2020 2073 697a 653d 636f 6e74 656e 745b     size=content[
+000035d0: 2753 697a 6527 5d2c 0a20 2020 2020 2020  'Size'],.       
+000035e0: 206d 7469 6d65 3d63 6f6e 7465 6e74 5b27   mtime=content['
+000035f0: 4c61 7374 4d6f 6469 6669 6564 275d 2e74  LastModified'].t
+00003600: 696d 6573 7461 6d70 2829 2c0a 2020 2020  imestamp(),.    
+00003610: 2020 2020 6578 7472 613d 636f 6e74 656e      extra=conten
+00003620: 742c 0a20 2020 2029 0a0a 0a64 6566 205f  t,.    )...def _
+00003630: 7333 5f67 6c6f 625f 7374 6174 5f73 696e  s3_glob_stat_sin
+00003640: 676c 655f 7061 7468 280a 2020 2020 2020  gle_path(.      
+00003650: 2020 7333 5f70 6174 686e 616d 653a 2050    s3_pathname: P
+00003660: 6174 684c 696b 652c 0a20 2020 2020 2020  athLike,.       
+00003670: 2072 6563 7572 7369 7665 3a20 626f 6f6c   recursive: bool
+00003680: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+00003690: 206d 6973 7369 6e67 5f6f 6b3a 2062 6f6f   missing_ok: boo
+000036a0: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+000036b0: 2020 666f 6c6c 6f77 6c69 6e6b 733a 2062    followlinks: b
+000036c0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+000036d0: 2020 2020 2070 726f 6669 6c65 5f6e 616d       profile_nam
+000036e0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+000036f0: 203d 204e 6f6e 6529 202d 3e20 4974 6572   = None) -> Iter
+00003700: 6174 6f72 5b46 696c 6545 6e74 7279 5d3a  ator[FileEntry]:
+00003710: 0a20 2020 2069 6620 6e6f 7420 7265 6375  .    if not recu
+00003720: 7273 6976 653a 0a20 2020 2020 2020 2023  rsive:.        #
+00003730: 2049 6620 6e6f 7420 7265 6375 7273 6976   If not recursiv
+00003740: 652c 2072 6570 6c61 6365 202a 2a20 7769  e, replace ** wi
+00003750: 7468 202a 0a20 2020 2020 2020 2073 335f  th *.        s3_
+00003760: 7061 7468 6e61 6d65 203d 2072 652e 7375  pathname = re.su
+00003770: 6228 7227 5c2a 7b32 2c7d 272c 2027 2a27  b(r'\*{2,}', '*'
+00003780: 2c20 7333 5f70 6174 686e 616d 6529 0a20  , s3_pathname). 
+00003790: 2020 2074 6f70 5f64 6972 2c20 7769 6c64     top_dir, wild
+000037a0: 6361 7264 5f70 6172 7420 3d20 5f73 335f  card_part = _s3_
+000037b0: 7370 6c69 745f 6d61 6769 6328 7333 5f70  split_magic(s3_p
+000037c0: 6174 686e 616d 6529 0a20 2020 2073 6561  athname).    sea
+000037d0: 7263 685f 6469 7220 3d20 7769 6c64 6361  rch_dir = wildca
+000037e0: 7264 5f70 6172 742e 656e 6473 7769 7468  rd_part.endswith
+000037f0: 2827 2f27 290a 0a20 2020 2064 6566 2073  ('/')..    def s
+00003800: 686f 756c 645f 7265 6375 7273 6976 6528  hould_recursive(
+00003810: 7769 6c64 6361 7264 5f70 6172 743a 2073  wildcard_part: s
+00003820: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
+00003830: 2020 2020 2069 6620 272a 2a27 2069 6e20       if '**' in 
+00003840: 7769 6c64 6361 7264 5f70 6172 743a 0a20  wildcard_part:. 
+00003850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00003860: 6e20 5472 7565 0a20 2020 2020 2020 2066  n True.        f
+00003870: 6f72 2065 7870 616e 6465 645f 7061 7468  or expanded_path
+00003880: 2069 6e20 756e 676c 6f62 6c69 7a65 2877   in ungloblize(w
+00003890: 696c 6463 6172 645f 7061 7274 293a 0a20  ildcard_part):. 
+000038a0: 2020 2020 2020 2020 2020 2070 6172 7473             parts
+000038b0: 5f6c 656e 6774 6820 3d20 6c65 6e28 6578  _length = len(ex
+000038c0: 7061 6e64 6564 5f70 6174 682e 7370 6c69  panded_path.spli
+000038d0: 7428 272f 2729 290a 2020 2020 2020 2020  t('/')).        
+000038e0: 2020 2020 6966 2070 6172 7473 5f6c 656e      if parts_len
+000038f0: 6774 6820 2b20 7365 6172 6368 5f64 6972  gth + search_dir
+00003900: 203e 3d20 323a 0a20 2020 2020 2020 2020   >= 2:.         
+00003910: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00003920: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00003930: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00003940: 2063 7265 6174 655f 6765 6e65 7261 746f   create_generato
+00003950: 7228 5f73 335f 7061 7468 6e61 6d65 2920  r(_s3_pathname) 
+00003960: 2d3e 2049 7465 7261 746f 725b 4669 6c65  -> Iterator[File
+00003970: 456e 7472 795d 3a0a 2020 2020 2020 2020  Entry]:.        
+00003980: 6966 206e 6f74 2053 3350 6174 6828 746f  if not S3Path(to
+00003990: 705f 6469 7229 2e65 7869 7374 7328 293a  p_dir).exists():
+000039a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000039b0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+000039c0: 6f74 2068 6173 5f6d 6167 6963 285f 7333  ot has_magic(_s3
+000039d0: 5f70 6174 686e 616d 6529 3a0a 2020 2020  _pathname):.    
+000039e0: 2020 2020 2020 2020 5f73 335f 7061 7468          _s3_path
+000039f0: 6e61 6d65 5f6f 626a 203d 2053 3350 6174  name_obj = S3Pat
+00003a00: 6828 5f73 335f 7061 7468 6e61 6d65 290a  h(_s3_pathname).
+00003a10: 2020 2020 2020 2020 2020 2020 6966 205f              if _
+00003a20: 7333 5f70 6174 686e 616d 655f 6f62 6a2e  s3_pathname_obj.
+00003a30: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
+00003a40: 2020 2020 2020 2020 2020 2073 7461 7420             stat 
+00003a50: 3d20 5333 5061 7468 285f 7333 5f70 6174  = S3Path(_s3_pat
+00003a60: 686e 616d 6529 2e73 7461 7428 666f 6c6c  hname).stat(foll
+00003a70: 6f77 5f73 796d 6c69 6e6b 733d 666f 6c6c  ow_symlinks=foll
+00003a80: 6f77 6c69 6e6b 7329 0a20 2020 2020 2020  owlinks).       
+00003a90: 2020 2020 2020 2020 2079 6965 6c64 2046           yield F
+00003aa0: 696c 6545 6e74 7279 280a 2020 2020 2020  ileEntry(.      
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
+00003ac0: 335f 7061 7468 6e61 6d65 5f6f 626a 2e6e  3_pathname_obj.n
+00003ad0: 616d 652c 205f 7333 5f70 6174 686e 616d  ame, _s3_pathnam
+00003ae0: 655f 6f62 6a2e 7061 7468 2c20 7374 6174  e_obj.path, stat
+00003af0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00003b00: 205f 7333 5f70 6174 686e 616d 655f 6f62   _s3_pathname_ob
+00003b10: 6a2e 6973 5f64 6972 2829 3a0a 2020 2020  j.is_dir():.    
+00003b20: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00003b30: 6420 4669 6c65 456e 7472 7928 0a20 2020  d FileEntry(.   
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b50: 205f 7333 5f70 6174 686e 616d 655f 6f62   _s3_pathname_ob
+00003b60: 6a2e 6e61 6d65 2c20 5f73 335f 7061 7468  j.name, _s3_path
+00003b70: 6e61 6d65 5f6f 626a 2e70 6174 682c 0a20  name_obj.path,. 
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 2020 2053 7461 7452 6573 756c 7428 6973     StatResult(is
+00003ba0: 6469 723d 5472 7565 2929 0a20 2020 2020  dir=True)).     
+00003bb0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+00003bc0: 2020 2020 2020 2064 656c 696d 6974 6572         delimiter
+00003bd0: 203d 2027 270a 2020 2020 2020 2020 6966   = ''.        if
+00003be0: 206e 6f74 2073 686f 756c 645f 7265 6375   not should_recu
+00003bf0: 7273 6976 6528 7769 6c64 6361 7264 5f70  rsive(wildcard_p
+00003c00: 6172 7429 3a0a 2020 2020 2020 2020 2020  art):.          
+00003c10: 2020 6465 6c69 6d69 7465 7220 3d20 272f    delimiter = '/
+00003c20: 270a 0a20 2020 2020 2020 2064 6972 6e61  '..        dirna
+00003c30: 6d65 7320 3d20 7365 7428 290a 2020 2020  mes = set().    
+00003c40: 2020 2020 7061 7474 6572 6e20 3d20 7265      pattern = re
+00003c50: 2e63 6f6d 7069 6c65 2874 7261 6e73 6c61  .compile(transla
+00003c60: 7465 285f 7333 5f70 6174 686e 616d 6529  te(_s3_pathname)
+00003c70: 290a 2020 2020 2020 2020 6275 636b 6574  ).        bucket
+00003c80: 2c20 6b65 7920 3d20 7061 7273 655f 7333  , key = parse_s3
+00003c90: 5f75 726c 2874 6f70 5f64 6972 290a 2020  _url(top_dir).  
+00003ca0: 2020 2020 2020 7072 6566 6978 203d 205f        prefix = _
+00003cb0: 6265 636f 6d65 5f70 7265 6669 7828 6b65  become_prefix(ke
+00003cc0: 7929 0a20 2020 2020 2020 2063 6c69 656e  y).        clien
+00003cd0: 7420 3d20 6765 745f 7333 5f63 6c69 656e  t = get_s3_clien
+00003ce0: 7428 7072 6f66 696c 655f 6e61 6d65 3d70  t(profile_name=p
+00003cf0: 726f 6669 6c65 5f6e 616d 6529 0a20 2020  rofile_name).   
+00003d00: 2020 2020 2077 6974 6820 7261 6973 655f       with raise_
+00003d10: 7333 5f65 7272 6f72 285f 7333 5f70 6174  s3_error(_s3_pat
+00003d20: 686e 616d 6529 3a0a 2020 2020 2020 2020  hname):.        
+00003d30: 2020 2020 666f 7220 7265 7370 2069 6e20      for resp in 
+00003d40: 5f6c 6973 745f 6f62 6a65 6374 735f 7265  _list_objects_re
+00003d50: 6375 7273 6976 6528 636c 6965 6e74 2c20  cursive(client, 
+00003d60: 6275 636b 6574 2c20 7072 6566 6978 2c0a  bucket, prefix,.
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003da0: 6465 6c69 6d69 7465 7229 3a0a 2020 2020  delimiter):.    
+00003db0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00003dc0: 636f 6e74 656e 7420 696e 2072 6573 702e  content in resp.
+00003dd0: 6765 7428 2743 6f6e 7465 6e74 7327 2c20  get('Contents', 
+00003de0: 5b5d 293a 0a20 2020 2020 2020 2020 2020  []):.           
+00003df0: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
+00003e00: 7333 5f70 6174 685f 6a6f 696e 2827 7333  s3_path_join('s3
+00003e10: 3a2f 2f27 2c20 6275 636b 6574 2c20 636f  ://', bucket, co
+00003e20: 6e74 656e 745b 274b 6579 275d 290a 2020  ntent['Key']).  
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e40: 2020 6966 206e 6f74 2073 6561 7263 685f    if not search_
+00003e50: 6469 7220 616e 6420 7061 7474 6572 6e2e  dir and pattern.
+00003e60: 6d61 7463 6828 7061 7468 293a 0a20 2020  match(path):.   
+00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e80: 2020 2020 2079 6965 6c64 2046 696c 6545       yield FileE
+00003e90: 6e74 7279 280a 2020 2020 2020 2020 2020  ntry(.          
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 5333 5061 7468 2870 6174 6829 2e6e    S3Path(path).n
+00003ec0: 616d 652c 2070 6174 682c 205f 6d61 6b65  ame, path, _make
+00003ed0: 5f73 7461 7428 636f 6e74 656e 7429 290a  _stat(content)).
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ef0: 2020 2020 6469 726e 616d 6520 3d20 6f73      dirname = os
+00003f00: 2e70 6174 682e 6469 726e 616d 6528 7061  .path.dirname(pa
+00003f10: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+00003f20: 2020 2020 2020 2020 7768 696c 6520 6469          while di
+00003f30: 726e 616d 6520 6e6f 7420 696e 2064 6972  rname not in dir
+00003f40: 6e61 6d65 7320 616e 6420 6469 726e 616d  names and dirnam
+00003f50: 6520 213d 2074 6f70 5f64 6972 3a0a 2020  e != top_dir:.  
 00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f70: 2020 2020 2020 2020 2020 5333 5061 7468            S3Path
-00003f80: 2870 6174 6829 2e6e 616d 652c 2070 6174  (path).name, pat
-00003f90: 682c 205f 6d61 6b65 5f73 7461 7428 636f  h, _make_stat(co
-00003fa0: 6e74 656e 7429 290a 2020 2020 2020 2020  ntent)).        
-00003fb0: 2020 2020 2020 2020 2020 2020 6469 726e              dirn
-00003fc0: 616d 6520 3d20 6f73 2e70 6174 682e 6469  ame = os.path.di
-00003fd0: 726e 616d 6528 7061 7468 290a 2020 2020  rname(path).    
-00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ff0: 7768 696c 6520 6469 726e 616d 6520 6e6f  while dirname no
-00004000: 7420 696e 2064 6972 6e61 6d65 7320 616e  t in dirnames an
-00004010: 6420 6469 726e 616d 6520 213d 2074 6f70  d dirname != top
-00004020: 5f64 6972 3a0a 2020 2020 2020 2020 2020  _dir:.          
-00004030: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00004040: 726e 616d 6573 2e61 6464 2864 6972 6e61  rnames.add(dirna
-00004050: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-00004060: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00004070: 203d 2064 6972 6e61 6d65 202b 2027 2f27   = dirname + '/'
-00004080: 2069 6620 7365 6172 6368 5f64 6972 2065   if search_dir e
-00004090: 6c73 6520 6469 726e 616d 650a 2020 2020  lse dirname.    
-000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040b0: 2020 2020 6966 2070 6174 7465 726e 2e6d      if pattern.m
-000040c0: 6174 6368 2870 6174 6829 3a0a 2020 2020  atch(path):.    
-000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040e0: 2020 2020 2020 2020 7969 656c 6420 4669          yield Fi
-000040f0: 6c65 456e 7472 7928 0a20 2020 2020 2020  leEntry(.       
-00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004110: 2020 2020 2020 2020 2053 3350 6174 6828           S3Path(
-00004120: 7061 7468 292e 6e61 6d65 2c20 7061 7468  path).name, path
-00004130: 2c20 5374 6174 5265 7375 6c74 2869 7364  , StatResult(isd
-00004140: 6972 3d54 7275 6529 290a 2020 2020 2020  ir=True)).      
-00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004160: 2020 6469 726e 616d 6520 3d20 6f73 2e70    dirname = os.p
-00004170: 6174 682e 6469 726e 616d 6528 6469 726e  ath.dirname(dirn
-00004180: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00004190: 2020 2020 2066 6f72 2063 6f6d 6d6f 6e5f       for common_
-000041a0: 7072 6566 6978 2069 6e20 7265 7370 2e67  prefix in resp.g
-000041b0: 6574 2827 436f 6d6d 6f6e 5072 6566 6978  et('CommonPrefix
-000041c0: 6573 272c 205b 5d29 3a0a 2020 2020 2020  es', []):.      
-000041d0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000041e0: 7468 203d 2073 335f 7061 7468 5f6a 6f69  th = s3_path_joi
-000041f0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00004200: 2020 2020 2020 2020 2020 2027 7333 3a2f             's3:/
-00004210: 2f27 2c20 6275 636b 6574 2c20 636f 6d6d  /', bucket, comm
-00004220: 6f6e 5f70 7265 6669 785b 2750 7265 6669  on_prefix['Prefi
-00004230: 7827 5d29 0a20 2020 2020 2020 2020 2020  x']).           
-00004240: 2020 2020 2020 2020 2064 6972 6e61 6d65           dirname
-00004250: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-00004260: 6d65 2870 6174 6829 0a20 2020 2020 2020  me(path).       
-00004270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004280: 6469 726e 616d 6520 6e6f 7420 696e 2064  dirname not in d
-00004290: 6972 6e61 6d65 7320 616e 6420 6469 726e  irnames and dirn
-000042a0: 616d 6520 213d 2074 6f70 5f64 6972 3a0a  ame != top_dir:.
-000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042c0: 2020 2020 2020 2020 6469 726e 616d 6573          dirnames
-000042d0: 2e61 6464 2864 6972 6e61 6d65 290a 2020  .add(dirname).  
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 2020 2020 7061 7468 203d 2064 6972        path = dir
-00004300: 6e61 6d65 202b 2027 2f27 2069 6620 7365  name + '/' if se
-00004310: 6172 6368 5f64 6972 2065 6c73 6520 6469  arch_dir else di
-00004320: 726e 616d 650a 2020 2020 2020 2020 2020  rname.          
-00004330: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004340: 2070 6174 7465 726e 2e6d 6174 6368 2870   pattern.match(p
-00004350: 6174 6829 3a0a 2020 2020 2020 2020 2020  ath):.          
+00003f70: 2020 2020 2020 6469 726e 616d 6573 2e61        dirnames.a
+00003f80: 6464 2864 6972 6e61 6d65 290a 2020 2020  dd(dirname).    
+00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fa0: 2020 2020 7061 7468 203d 2064 6972 6e61      path = dirna
+00003fb0: 6d65 202b 2027 2f27 2069 6620 7365 6172  me + '/' if sear
+00003fc0: 6368 5f64 6972 2065 6c73 6520 6469 726e  ch_dir else dirn
+00003fd0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00003fe0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00003ff0: 6174 7465 726e 2e6d 6174 6368 2870 6174  attern.match(pat
+00004000: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
+00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004020: 7969 656c 6420 4669 6c65 456e 7472 7928  yield FileEntry(
+00004030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004050: 2053 3350 6174 6828 7061 7468 292e 6e61   S3Path(path).na
+00004060: 6d65 2c20 7061 7468 2c20 5374 6174 5265  me, path, StatRe
+00004070: 7375 6c74 2869 7364 6972 3d54 7275 6529  sult(isdir=True)
+00004080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004090: 2020 2020 2020 2020 2020 6469 726e 616d            dirnam
+000040a0: 6520 3d20 6f73 2e70 6174 682e 6469 726e  e = os.path.dirn
+000040b0: 616d 6528 6469 726e 616d 6529 0a20 2020  ame(dirname).   
+000040c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000040d0: 2063 6f6d 6d6f 6e5f 7072 6566 6978 2069   common_prefix i
+000040e0: 6e20 7265 7370 2e67 6574 2827 436f 6d6d  n resp.get('Comm
+000040f0: 6f6e 5072 6566 6978 6573 272c 205b 5d29  onPrefixes', [])
+00004100: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004110: 2020 2020 2020 7061 7468 203d 2073 335f        path = s3_
+00004120: 7061 7468 5f6a 6f69 6e28 0a20 2020 2020  path_join(.     
+00004130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004140: 2020 2027 7333 3a2f 2f27 2c20 6275 636b     's3://', buck
+00004150: 6574 2c20 636f 6d6d 6f6e 5f70 7265 6669  et, common_prefi
+00004160: 785b 2750 7265 6669 7827 5d29 0a20 2020  x['Prefix']).   
+00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004180: 2064 6972 6e61 6d65 203d 206f 732e 7061   dirname = os.pa
+00004190: 7468 2e64 6972 6e61 6d65 2870 6174 6829  th.dirname(path)
+000041a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041b0: 2020 2020 2069 6620 6469 726e 616d 6520       if dirname 
+000041c0: 6e6f 7420 696e 2064 6972 6e61 6d65 7320  not in dirnames 
+000041d0: 616e 6420 6469 726e 616d 6520 213d 2074  and dirname != t
+000041e0: 6f70 5f64 6972 3a0a 2020 2020 2020 2020  op_dir:.        
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 6469 726e 616d 6573 2e61 6464 2864 6972  dirnames.add(dir
+00004210: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+00004220: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00004230: 7468 203d 2064 6972 6e61 6d65 202b 2027  th = dirname + '
+00004240: 2f27 2069 6620 7365 6172 6368 5f64 6972  /' if search_dir
+00004250: 2065 6c73 6520 6469 726e 616d 650a 2020   else dirname.  
+00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004270: 2020 2020 2020 6966 2070 6174 7465 726e        if pattern
+00004280: 2e6d 6174 6368 2870 6174 6829 3a0a 2020  .match(path):.  
+00004290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042a0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+000042b0: 4669 6c65 456e 7472 7928 0a20 2020 2020  FileEntry(.     
+000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042d0: 2020 2020 2020 2020 2020 2053 3350 6174             S3Pat
+000042e0: 6828 7061 7468 292e 6e61 6d65 2c20 7061  h(path).name, pa
+000042f0: 7468 2c20 5374 6174 5265 7375 6c74 2869  th, StatResult(i
+00004300: 7364 6972 3d54 7275 6529 290a 0a20 2020  sdir=True))..   
+00004310: 2072 6574 7572 6e20 6372 6561 7465 5f67   return create_g
+00004320: 656e 6572 6174 6f72 2873 335f 7061 7468  enerator(s3_path
+00004330: 6e61 6d65 290a 0a0a 6465 6620 5f73 335f  name)...def _s3_
+00004340: 7363 616e 5f70 6169 7273 2873 7263 5f75  scan_pairs(src_u
+00004350: 726c 3a20 5061 7468 4c69 6b65 2c0a 2020  rl: PathLike,.  
 00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 2020 7969 656c 6420 4669 6c65 456e 7472    yield FileEntr
-00004380: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
-00004390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043a0: 2020 2053 3350 6174 6828 7061 7468 292e     S3Path(path).
-000043b0: 6e61 6d65 2c20 7061 7468 2c20 5374 6174  name, path, Stat
-000043c0: 5265 7375 6c74 2869 7364 6972 3d54 7275  Result(isdir=Tru
-000043d0: 6529 290a 0a20 2020 2072 6574 7572 6e20  e))..    return 
-000043e0: 6372 6561 7465 5f67 656e 6572 6174 6f72  create_generator
-000043f0: 2873 335f 7061 7468 6e61 6d65 290a 0a0a  (s3_pathname)...
-00004400: 6465 6620 5f73 335f 7363 616e 5f70 6169  def _s3_scan_pai
-00004410: 7273 2873 7263 5f75 726c 3a20 5061 7468  rs(src_url: Path
-00004420: 4c69 6b65 2c0a 2020 2020 2020 2020 2020  Like,.          
-00004430: 2020 2020 2020 2020 2064 7374 5f75 726c           dst_url
-00004440: 3a20 5061 7468 4c69 6b65 2920 2d3e 2049  : PathLike) -> I
-00004450: 7465 7261 746f 725b 5475 706c 655b 5061  terator[Tuple[Pa
-00004460: 7468 4c69 6b65 2c20 5061 7468 4c69 6b65  thLike, PathLike
-00004470: 5d5d 3a0a 2020 2020 666f 7220 7372 635f  ]]:.    for src_
-00004480: 6669 6c65 5f70 6174 6820 696e 2053 3350  file_path in S3P
-00004490: 6174 6828 7372 635f 7572 6c29 2e73 6361  ath(src_url).sca
-000044a0: 6e28 293a 0a20 2020 2020 2020 2063 6f6e  n():.        con
-000044b0: 7465 6e74 5f70 6174 6820 3d20 7372 635f  tent_path = src_
-000044c0: 6669 6c65 5f70 6174 685b 6c65 6e28 7372  file_path[len(sr
-000044d0: 635f 7572 6c29 3a5d 0a20 2020 2020 2020  c_url):].       
-000044e0: 2069 6620 6c65 6e28 636f 6e74 656e 745f   if len(content_
-000044f0: 7061 7468 2920 3e20 303a 0a20 2020 2020  path) > 0:.     
-00004500: 2020 2020 2020 2064 7374 5f66 696c 655f         dst_file_
-00004510: 7061 7468 203d 2073 335f 7061 7468 5f6a  path = s3_path_j
-00004520: 6f69 6e28 6473 745f 7572 6c2c 2063 6f6e  oin(dst_url, con
-00004530: 7465 6e74 5f70 6174 6829 0a20 2020 2020  tent_path).     
-00004540: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00004550: 2020 2020 2064 7374 5f66 696c 655f 7061       dst_file_pa
-00004560: 7468 203d 2064 7374 5f75 726c 0a20 2020  th = dst_url.   
-00004570: 2020 2020 2079 6965 6c64 2073 7263 5f66       yield src_f
-00004580: 696c 655f 7061 7468 2c20 6473 745f 6669  ile_path, dst_fi
-00004590: 6c65 5f70 6174 680a 0a0a 6465 6620 6973  le_path...def is
-000045a0: 5f73 3328 7061 7468 3a20 5061 7468 4c69  _s3(path: PathLi
-000045b0: 6b65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ke) -> bool:.   
-000045c0: 2027 2727 0a20 2020 2031 2e20 4163 636f   '''.    1. Acco
-000045d0: 7264 696e 6720 746f 2060 6177 732d 636c  rding to `aws-cl
-000045e0: 6920 3c68 7474 7073 3a2f 2f64 6f63 732e  i <https://docs.
-000045f0: 6177 732e 616d 617a 6f6e 2e63 6f6d 2f63  aws.amazon.com/c
-00004600: 6c69 2f6c 6174 6573 742f 7265 6665 7265  li/latest/refere
-00004610: 6e63 652f 7333 2f69 6e64 6578 2e68 746d  nce/s3/index.htm
-00004620: 6c3e 605f 202c 2074 6573 7420 6966 2061  l>`_ , test if a
-00004630: 2070 6174 6820 6973 2073 3320 7061 7468   path is s3 path
-00004640: 2e0a 2020 2020 322e 206d 6567 6669 6c65  ..    2. megfile
-00004650: 2061 6c73 6f20 7375 7070 6f72 7420 7468   also support th
-00004660: 6520 7061 7468 206c 696b 6520 6073 335b  e path like `s3[
-00004670: 2b70 726f 6669 6c65 5f6e 616d 655d 3a2f  +profile_name]:/
-00004680: 2f62 7563 6b65 742f 6b65 7960 0a0a 2020  /bucket/key`..  
-00004690: 2020 3a70 6172 616d 2070 6174 683a 2050    :param path: P
-000046a0: 6174 6820 746f 2062 6520 7465 7374 6564  ath to be tested
-000046b0: 0a20 2020 203a 7265 7475 726e 733a 2054  .    :returns: T
-000046c0: 7275 6520 6966 2070 6174 6820 6973 2073  rue if path is s
-000046d0: 3320 7061 7468 2c20 656c 7365 2046 616c  3 path, else Fal
-000046e0: 7365 0a20 2020 2027 2727 0a20 2020 2070  se.    '''.    p
-000046f0: 6174 6820 3d20 6673 7061 7468 2870 6174  ath = fspath(pat
-00004700: 6829 0a20 2020 2069 6620 7265 2e6d 6174  h).    if re.mat
-00004710: 6368 2872 275e 7333 285c 2b5c 772b 293f  ch(r'^s3(\+\w+)?
-00004720: 3a5c 2f5c 2f27 2c20 7061 7468 293a 0a20  :\/\/', path):. 
-00004730: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00004740: 7565 0a20 2020 2072 6574 7572 6e20 4661  ue.    return Fa
-00004750: 6c73 650a 0a0a 6465 6620 5f73 335f 6269  lse...def _s3_bi
-00004760: 6e61 7279 5f6d 6f64 6528 7333 5f6f 7065  nary_mode(s3_ope
-00004770: 6e5f 6675 6e63 293a 0a0a 2020 2020 4077  n_func):..    @w
-00004780: 7261 7073 2873 335f 6f70 656e 5f66 756e  raps(s3_open_fun
-00004790: 6329 0a20 2020 2064 6566 2077 7261 7070  c).    def wrapp
-000047a0: 6572 2873 335f 7572 6c2c 206d 6f64 653a  er(s3_url, mode:
-000047b0: 2073 7472 203d 2027 7262 272c 202a 2a6b   str = 'rb', **k
-000047c0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-000047d0: 6275 636b 6574 2c20 6b65 7920 3d20 7061  bucket, key = pa
-000047e0: 7273 655f 7333 5f75 726c 2873 335f 7572  rse_s3_url(s3_ur
-000047f0: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
-00004800: 7420 6275 636b 6574 3a0a 2020 2020 2020  t bucket:.      
-00004810: 2020 2020 2020 7261 6973 6520 5333 4275        raise S3Bu
-00004820: 636b 6574 4e6f 7446 6f75 6e64 4572 726f  cketNotFoundErro
-00004830: 7228 2745 6d70 7479 2062 7563 6b65 7420  r('Empty bucket 
-00004840: 6e61 6d65 3a20 2572 2720 2520 7333 5f75  name: %r' % s3_u
-00004850: 726c 290a 0a20 2020 2020 2020 2069 6620  rl)..        if 
-00004860: 6e6f 7420 6b65 7920 6f72 206b 6579 2e65  not key or key.e
-00004870: 6e64 7377 6974 6828 272f 2729 3a0a 2020  ndswith('/'):.  
-00004880: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00004890: 5333 4973 4144 6972 6563 746f 7279 4572  S3IsADirectoryEr
-000048a0: 726f 7228 2749 7320 6120 6469 7265 6374  ror('Is a direct
-000048b0: 6f72 793a 2025 7227 2025 2073 335f 7572  ory: %r' % s3_ur
-000048c0: 6c29 0a0a 2020 2020 2020 2020 6966 2027  l)..        if '
-000048d0: 7827 2069 6e20 6d6f 6465 3a0a 2020 2020  x' in mode:.    
-000048e0: 2020 2020 2020 2020 6966 2053 3350 6174          if S3Pat
-000048f0: 6828 7333 5f75 726c 292e 6973 5f66 696c  h(s3_url).is_fil
-00004900: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
-00004910: 2020 2020 2072 6169 7365 2053 3346 696c       raise S3Fil
-00004920: 6545 7869 7374 7345 7272 6f72 2827 4669  eExistsError('Fi
-00004930: 6c65 2065 7869 7374 733a 2025 7227 2025  le exists: %r' %
-00004940: 2073 335f 7572 6c29 0a20 2020 2020 2020   s3_url).       
-00004950: 2020 2020 206d 6f64 6520 3d20 6d6f 6465       mode = mode
-00004960: 2e72 6570 6c61 6365 2827 7827 2c20 2777  .replace('x', 'w
-00004970: 2729 0a0a 2020 2020 2020 2020 6966 2027  ')..        if '
-00004980: 7727 2069 6e20 6d6f 6465 206f 7220 2761  w' in mode or 'a
-00004990: 2720 696e 206d 6f64 653a 0a20 2020 2020  ' in mode:.     
-000049a0: 2020 2020 2020 2069 6620 6e6f 7420 5333         if not S3
-000049b0: 5061 7468 2873 335f 7572 6c29 2e68 6173  Path(s3_url).has
-000049c0: 6275 636b 6574 2829 3a0a 2020 2020 2020  bucket():.      
-000049d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000049e0: 5333 4275 636b 6574 4e6f 7446 6f75 6e64  S3BucketNotFound
-000049f0: 4572 726f 7228 274e 6f20 7375 6368 2062  Error('No such b
-00004a00: 7563 6b65 743a 2025 7227 2025 2073 335f  ucket: %r' % s3_
-00004a10: 7572 6c29 0a0a 2020 2020 2020 2020 6669  url)..        fi
-00004a20: 6c65 6f62 6a20 3d20 7333 5f6f 7065 6e5f  leobj = s3_open_
-00004a30: 6675 6e63 2873 335f 7572 6c2c 2067 6574  func(s3_url, get
-00004a40: 5f62 696e 6172 795f 6d6f 6465 286d 6f64  _binary_mode(mod
-00004a50: 6529 2c20 2a2a 6b77 6172 6773 290a 2020  e), **kwargs).  
-00004a60: 2020 2020 2020 6966 2027 6227 206e 6f74        if 'b' not
-00004a70: 2069 6e20 6d6f 6465 3a0a 2020 2020 2020   in mode:.      
-00004a80: 2020 2020 2020 6669 6c65 6f62 6a20 3d20        fileobj = 
-00004a90: 696f 2e54 6578 7449 4f57 7261 7070 6572  io.TextIOWrapper
-00004aa0: 2866 696c 656f 626a 2920 2023 2070 7974  (fileobj)  # pyt
-00004ab0: 7970 653a 2064 6973 6162 6c65 3d77 726f  ype: disable=wro
-00004ac0: 6e67 2d61 7267 2d74 7970 6573 0a20 2020  ng-arg-types.   
-00004ad0: 2020 2020 2020 2020 2066 696c 656f 626a           fileobj
-00004ae0: 2e6d 6f64 6520 3d20 6d6f 6465 0a20 2020  .mode = mode.   
-00004af0: 2020 2020 2072 6574 7572 6e20 6669 6c65       return file
-00004b00: 6f62 6a0a 0a20 2020 2072 6574 7572 6e20  obj..    return 
-00004b10: 7772 6170 7065 720a 0a0a 405f 7333 5f62  wrapper...@_s3_b
-00004b20: 696e 6172 795f 6d6f 6465 0a64 6566 2073  inary_mode.def s
-00004b30: 335f 7072 6566 6574 6368 5f6f 7065 6e28  3_prefetch_open(
-00004b40: 0a20 2020 2020 2020 2073 335f 7572 6c3a  .        s3_url:
-00004b50: 2050 6174 684c 696b 652c 0a20 2020 2020   PathLike,.     
-00004b60: 2020 206d 6f64 653a 2073 7472 203d 2027     mode: str = '
-00004b70: 7262 272c 0a20 2020 2020 2020 2066 6f6c  rb',.        fol
-00004b80: 6c6f 776c 696e 6b73 3a20 626f 6f6c 203d  lowlinks: bool =
-00004b90: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00004ba0: 2a2c 0a20 2020 2020 2020 206d 6178 5f63  *,.        max_c
-00004bb0: 6f6e 6375 7272 656e 6379 3a20 4f70 7469  oncurrency: Opti
-00004bc0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00004bd0: 2c0a 2020 2020 2020 2020 6d61 785f 626c  ,.        max_bl
-00004be0: 6f63 6b5f 7369 7a65 3a20 696e 7420 3d20  ock_size: int = 
-00004bf0: 4445 4641 554c 545f 424c 4f43 4b5f 5349  DEFAULT_BLOCK_SI
-00004c00: 5a45 2920 2d3e 2053 3350 7265 6665 7463  ZE) -> S3Prefetc
-00004c10: 6852 6561 6465 723a 0a20 2020 2027 2727  hReader:.    '''
-00004c20: 4f70 656e 2061 2061 7379 6e63 6872 6f6e  Open a asynchron
-00004c30: 6f75 7320 7072 6566 6574 6368 2072 6561  ous prefetch rea
-00004c40: 6465 722c 2074 6f20 7375 7070 6f72 7420  der, to support 
-00004c50: 6661 7374 2073 6571 7565 6e74 6961 6c20  fast sequential 
-00004c60: 7265 6164 2061 6e64 2072 616e 646f 6d20  read and random 
-00004c70: 7265 6164 0a0a 2020 2020 2e2e 206e 6f74  read..    .. not
-00004c80: 6520 3a3a 0a0a 2020 2020 2020 2020 5573  e ::..        Us
-00004c90: 6572 2073 686f 756c 6420 6d61 6b65 2073  er should make s
-00004ca0: 7572 6520 7468 6174 2072 6561 6465 7220  ure that reader 
-00004cb0: 2f20 7772 6974 6572 2061 7265 2063 6c6f  / writer are clo
-00004cc0: 7365 6420 636f 7272 6563 746c 790a 0a20  sed correctly.. 
-00004cd0: 2020 2020 2020 2053 7570 706f 7274 7320         Supports 
-00004ce0: 636f 6e74 6578 7420 6d61 6e61 6765 720a  context manager.
-00004cf0: 0a20 2020 2020 2020 2053 6f6d 6520 7061  .        Some pa
-00004d00: 7261 6d65 7465 7220 7365 7474 696e 6720  rameter setting 
-00004d10: 6d61 7920 7065 7266 6f72 6d20 7765 6c6c  may perform well
-00004d20: 3a20 6d61 785f 636f 6e63 7572 7265 6e63  : max_concurrenc
-00004d30: 793d 3130 206f 7220 3230 2c20 6d61 785f  y=10 or 20, max_
-00004d40: 626c 6f63 6b5f 7369 7a65 3d38 206f 7220  block_size=8 or 
-00004d50: 3136 204d 422c 2064 6566 6175 6c74 2076  16 MB, default v
-00004d60: 616c 7565 204e 6f6e 6520 6d65 616e 7320  alue None means 
-00004d70: 7573 696e 6720 676c 6f62 616c 2074 6872  using global thr
-00004d80: 6561 6420 706f 6f6c 0a0a 2020 2020 3a70  ead pool..    :p
-00004d90: 6172 616d 206d 6178 5f63 6f6e 6375 7272  aram max_concurr
-00004da0: 656e 6379 3a20 4d61 7820 646f 776e 6c6f  ency: Max downlo
-00004db0: 6164 2074 6872 6561 6420 6e75 6d62 6572  ad thread number
-00004dc0: 2c20 4e6f 6e65 2062 7920 6465 6661 756c  , None by defaul
-00004dd0: 740a 2020 2020 3a70 6172 616d 206d 6178  t.    :param max
-00004de0: 5f62 6c6f 636b 5f73 697a 653a 204d 6178  _block_size: Max
-00004df0: 2064 6174 6120 7369 7a65 2064 6f77 6e6c   data size downl
-00004e00: 6f61 6465 6420 6279 2065 6163 6820 7468  oaded by each th
-00004e10: 7265 6164 2c20 696e 2062 7974 6573 2c20  read, in bytes, 
-00004e20: 384d 4220 6279 2064 6566 6175 6c74 0a20  8MB by default. 
-00004e30: 2020 203a 7265 7475 726e 733a 2041 6e20     :returns: An 
-00004e40: 6f70 656e 6564 2053 3350 7265 6665 7463  opened S3Prefetc
-00004e50: 6852 6561 6465 7220 6f62 6a65 6374 0a20  hReader object. 
-00004e60: 2020 203a 7261 6973 6573 3a20 5333 4669     :raises: S3Fi
-00004e70: 6c65 4e6f 7446 6f75 6e64 4572 726f 720a  leNotFoundError.
-00004e80: 2020 2020 2727 270a 2020 2020 6966 206d      '''.    if m
-00004e90: 6f64 6520 213d 2027 7262 273a 0a20 2020  ode != 'rb':.   
-00004ea0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00004eb0: 4572 726f 7228 2775 6e61 6363 6570 7461  Error('unaccepta
-00004ec0: 626c 6520 6d6f 6465 3a20 2572 2720 2520  ble mode: %r' % 
-00004ed0: 6d6f 6465 290a 2020 2020 7333 5f75 726c  mode).    s3_url
-00004ee0: 203d 2053 3350 6174 6828 7333 5f75 726c   = S3Path(s3_url
-00004ef0: 290a 2020 2020 6966 2066 6f6c 6c6f 776c  ).    if followl
-00004f00: 696e 6b73 3a0a 2020 2020 2020 2020 7472  inks:.        tr
-00004f10: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00004f20: 335f 7572 6c20 3d20 7333 5f75 726c 2e72  3_url = s3_url.r
-00004f30: 6561 646c 696e 6b28 290a 2020 2020 2020  eadlink().      
-00004f40: 2020 6578 6365 7074 2053 334e 6f74 414c    except S3NotAL
-00004f50: 696e 6b45 7272 6f72 3a0a 2020 2020 2020  inkError:.      
-00004f60: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00004f70: 6275 636b 6574 2c20 6b65 7920 3d20 7061  bucket, key = pa
-00004f80: 7273 655f 7333 5f75 726c 2873 335f 7572  rse_s3_url(s3_ur
-00004f90: 6c2e 7061 7468 5f77 6974 685f 7072 6f74  l.path_with_prot
-00004fa0: 6f63 6f6c 290a 2020 2020 636f 6e66 6967  ocol).    config
-00004fb0: 203d 2062 6f74 6f63 6f72 652e 636f 6e66   = botocore.conf
-00004fc0: 6967 2e43 6f6e 6669 6728 6d61 785f 706f  ig.Config(max_po
-00004fd0: 6f6c 5f63 6f6e 6e65 6374 696f 6e73 3d6d  ol_connections=m
-00004fe0: 6178 5f70 6f6f 6c5f 636f 6e6e 6563 7469  ax_pool_connecti
-00004ff0: 6f6e 7329 0a20 2020 2063 6c69 656e 7420  ons).    client 
-00005000: 3d20 6765 745f 7333 5f63 6c69 656e 7428  = get_s3_client(
-00005010: 0a20 2020 2020 2020 2063 6f6e 6669 673d  .        config=
-00005020: 636f 6e66 6967 2c0a 2020 2020 2020 2020  config,.        
-00005030: 6361 6368 655f 6b65 793d 2773 335f 6669  cache_key='s3_fi
-00005040: 6c65 6c69 6b65 5f63 6c69 656e 7427 2c0a  lelike_client',.
-00005050: 2020 2020 2020 2020 7072 6f66 696c 655f          profile_
-00005060: 6e61 6d65 3d73 335f 7572 6c2e 5f70 726f  name=s3_url._pro
-00005070: 6669 6c65 5f6e 616d 6529 0a20 2020 2072  file_name).    r
-00005080: 6574 7572 6e20 5333 5072 6566 6574 6368  eturn S3Prefetch
-00005090: 5265 6164 6572 280a 2020 2020 2020 2020  Reader(.        
-000050a0: 6275 636b 6574 2c0a 2020 2020 2020 2020  bucket,.        
-000050b0: 6b65 792c 0a20 2020 2020 2020 2073 335f  key,.        s3_
-000050c0: 636c 6965 6e74 3d63 6c69 656e 742c 0a20  client=client,. 
-000050d0: 2020 2020 2020 206d 6178 5f72 6574 7269         max_retri
-000050e0: 6573 3d6d 6178 5f72 6574 7269 6573 2c0a  es=max_retries,.
-000050f0: 2020 2020 2020 2020 6d61 785f 776f 726b          max_work
-00005100: 6572 733d 6d61 785f 636f 6e63 7572 7265  ers=max_concurre
-00005110: 6e63 792c 0a20 2020 2020 2020 2062 6c6f  ncy,.        blo
-00005120: 636b 5f73 697a 653d 6d61 785f 626c 6f63  ck_size=max_bloc
-00005130: 6b5f 7369 7a65 290a 0a0a 405f 7333 5f62  k_size)...@_s3_b
-00005140: 696e 6172 795f 6d6f 6465 0a64 6566 2073  inary_mode.def s
-00005150: 335f 7368 6172 655f 6361 6368 655f 6f70  3_share_cache_op
-00005160: 656e 280a 2020 2020 2020 2020 7333 5f75  en(.        s3_u
-00005170: 726c 3a20 5061 7468 4c69 6b65 2c0a 2020  rl: PathLike,.  
-00005180: 2020 2020 2020 6d6f 6465 3a20 7374 7220        mode: str 
-00005190: 3d20 2772 6227 2c0a 2020 2020 2020 2020  = 'rb',.        
-000051a0: 666f 6c6c 6f77 6c69 6e6b 733a 2062 6f6f  followlinks: boo
-000051b0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-000051c0: 2020 202a 2c0a 2020 2020 2020 2020 6361     *,.        ca
-000051d0: 6368 655f 6b65 793a 2073 7472 203d 2027  che_key: str = '
-000051e0: 6c72 7527 2c0a 2020 2020 2020 2020 6d61  lru',.        ma
-000051f0: 785f 636f 6e63 7572 7265 6e63 793a 204f  x_concurrency: O
-00005200: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00005210: 6f6e 652c 0a20 2020 2020 2020 206d 6178  one,.        max
-00005220: 5f62 6c6f 636b 5f73 697a 653a 2069 6e74  _block_size: int
-00005230: 203d 2044 4546 4155 4c54 5f42 4c4f 434b   = DEFAULT_BLOCK
-00005240: 5f53 495a 4529 202d 3e20 5333 5368 6172  _SIZE) -> S3Shar
-00005250: 6543 6163 6865 5265 6164 6572 3a0a 2020  eCacheReader:.  
-00005260: 2020 2727 274f 7065 6e20 6120 6173 796e    '''Open a asyn
-00005270: 6368 726f 6e6f 7573 2070 7265 6665 7463  chronous prefetc
-00005280: 6820 7265 6164 6572 2c20 746f 2073 7570  h reader, to sup
-00005290: 706f 7274 2066 6173 7420 7365 7175 656e  port fast sequen
-000052a0: 7469 616c 2072 6561 6420 616e 6420 7261  tial read and ra
-000052b0: 6e64 6f6d 2072 6561 640a 0a20 2020 202e  ndom read..    .
-000052c0: 2e20 6e6f 7465 203a 3a0a 0a20 2020 2020  . note ::..     
-000052d0: 2020 2055 7365 7220 7368 6f75 6c64 206d     User should m
-000052e0: 616b 6520 7375 7265 2074 6861 7420 7265  ake sure that re
-000052f0: 6164 6572 202f 2077 7269 7465 7220 6172  ader / writer ar
-00005300: 6520 636c 6f73 6564 2063 6f72 7265 6374  e closed correct
-00005310: 6c79 0a0a 2020 2020 2020 2020 5375 7070  ly..        Supp
-00005320: 6f72 7473 2063 6f6e 7465 7874 206d 616e  orts context man
-00005330: 6167 6572 0a0a 2020 2020 2020 2020 536f  ager..        So
-00005340: 6d65 2070 6172 616d 6574 6572 2073 6574  me parameter set
-00005350: 7469 6e67 206d 6179 2070 6572 666f 726d  ting may perform
-00005360: 2077 656c 6c3a 206d 6178 5f63 6f6e 6375   well: max_concu
-00005370: 7272 656e 6379 3d31 3020 6f72 2032 302c  rrency=10 or 20,
-00005380: 206d 6178 5f62 6c6f 636b 5f73 697a 653d   max_block_size=
-00005390: 3820 6f72 2031 3620 4d42 2c20 6465 6661  8 or 16 MB, defa
-000053a0: 756c 7420 7661 6c75 6520 4e6f 6e65 206d  ult value None m
-000053b0: 6561 6e73 2075 7369 6e67 2067 6c6f 6261  eans using globa
-000053c0: 6c20 7468 7265 6164 2070 6f6f 6c0a 0a20  l thread pool.. 
-000053d0: 2020 203a 7061 7261 6d20 6d61 785f 636f     :param max_co
-000053e0: 6e63 7572 7265 6e63 793a 204d 6178 2064  ncurrency: Max d
-000053f0: 6f77 6e6c 6f61 6420 7468 7265 6164 206e  ownload thread n
-00005400: 756d 6265 722c 204e 6f6e 6520 6279 2064  umber, None by d
-00005410: 6566 6175 6c74 0a20 2020 203a 7061 7261  efault.    :para
-00005420: 6d20 6d61 785f 626c 6f63 6b5f 7369 7a65  m max_block_size
-00005430: 3a20 4d61 7820 6461 7461 2073 697a 6520  : Max data size 
-00005440: 646f 776e 6c6f 6164 6564 2062 7920 6561  downloaded by ea
-00005450: 6368 2074 6872 6561 642c 2069 6e20 6279  ch thread, in by
-00005460: 7465 732c 2038 4d42 2062 7920 6465 6661  tes, 8MB by defa
-00005470: 756c 740a 2020 2020 3a72 6574 7572 6e73  ult.    :returns
-00005480: 3a20 416e 206f 7065 6e65 6420 5333 5368  : An opened S3Sh
-00005490: 6172 6543 6163 6865 5265 6164 6572 206f  areCacheReader o
-000054a0: 626a 6563 740a 2020 2020 3a72 6169 7365  bject.    :raise
-000054b0: 733a 2053 3346 696c 654e 6f74 466f 756e  s: S3FileNotFoun
-000054c0: 6445 7272 6f72 0a20 2020 2027 2727 0a20  dError.    '''. 
-000054d0: 2020 2069 6620 6d6f 6465 2021 3d20 2772     if mode != 'r
-000054e0: 6227 3a0a 2020 2020 2020 2020 7261 6973  b':.        rais
-000054f0: 6520 5661 6c75 6545 7272 6f72 2827 756e  e ValueError('un
-00005500: 6163 6365 7074 6162 6c65 206d 6f64 653a  acceptable mode:
-00005510: 2025 7227 2025 206d 6f64 6529 0a0a 2020   %r' % mode)..  
-00005520: 2020 7333 5f75 726c 203d 2053 3350 6174    s3_url = S3Pat
-00005530: 6828 7333 5f75 726c 290a 2020 2020 6966  h(s3_url).    if
-00005540: 2066 6f6c 6c6f 776c 696e 6b73 3a0a 2020   followlinks:.  
-00005550: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00005560: 2020 2020 2020 2073 335f 7572 6c20 3d20         s3_url = 
-00005570: 7333 5f75 726c 2e72 6561 646c 696e 6b28  s3_url.readlink(
-00005580: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00005590: 2053 334e 6f74 414c 696e 6b45 7272 6f72   S3NotALinkError
-000055a0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-000055b0: 7373 0a0a 2020 2020 6275 636b 6574 2c20  ss..    bucket, 
-000055c0: 6b65 7920 3d20 7061 7273 655f 7333 5f75  key = parse_s3_u
-000055d0: 726c 2873 335f 7572 6c2e 7061 7468 5f77  rl(s3_url.path_w
-000055e0: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
-000055f0: 2020 636f 6e66 6967 203d 2062 6f74 6f63    config = botoc
-00005600: 6f72 652e 636f 6e66 6967 2e43 6f6e 6669  ore.config.Confi
-00005610: 6728 6d61 785f 706f 6f6c 5f63 6f6e 6e65  g(max_pool_conne
-00005620: 6374 696f 6e73 3d6d 6178 5f70 6f6f 6c5f  ctions=max_pool_
-00005630: 636f 6e6e 6563 7469 6f6e 7329 0a20 2020  connections).   
-00005640: 2063 6c69 656e 7420 3d20 6765 745f 7333   client = get_s3
-00005650: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
-00005660: 2063 6f6e 6669 673d 636f 6e66 6967 2c0a   config=config,.
-00005670: 2020 2020 2020 2020 6361 6368 655f 6b65          cache_ke
-00005680: 793d 2773 335f 6669 6c65 6c69 6b65 5f63  y='s3_filelike_c
-00005690: 6c69 656e 7427 2c0a 2020 2020 2020 2020  lient',.        
-000056a0: 7072 6f66 696c 655f 6e61 6d65 3d73 335f  profile_name=s3_
-000056b0: 7572 6c2e 5f70 726f 6669 6c65 5f6e 616d  url._profile_nam
-000056c0: 6529 0a20 2020 2072 6574 7572 6e20 5333  e).    return S3
-000056d0: 5368 6172 6543 6163 6865 5265 6164 6572  ShareCacheReader
-000056e0: 280a 2020 2020 2020 2020 6275 636b 6574  (.        bucket
-000056f0: 2c0a 2020 2020 2020 2020 6b65 792c 0a20  ,.        key,. 
-00005700: 2020 2020 2020 2063 6163 6865 5f6b 6579         cache_key
-00005710: 3d63 6163 6865 5f6b 6579 2c0a 2020 2020  =cache_key,.    
-00005720: 2020 2020 7333 5f63 6c69 656e 743d 636c      s3_client=cl
-00005730: 6965 6e74 2c0a 2020 2020 2020 2020 6d61  ient,.        ma
-00005740: 785f 7265 7472 6965 733d 6d61 785f 7265  x_retries=max_re
-00005750: 7472 6965 732c 0a20 2020 2020 2020 206d  tries,.        m
-00005760: 6178 5f77 6f72 6b65 7273 3d6d 6178 5f63  ax_workers=max_c
-00005770: 6f6e 6375 7272 656e 6379 2c0a 2020 2020  oncurrency,.    
-00005780: 2020 2020 626c 6f63 6b5f 7369 7a65 3d6d      block_size=m
-00005790: 6178 5f62 6c6f 636b 5f73 697a 6529 0a0a  ax_block_size)..
-000057a0: 0a40 5f73 335f 6269 6e61 7279 5f6d 6f64  .@_s3_binary_mod
-000057b0: 650a 6465 6620 7333 5f70 6970 655f 6f70  e.def s3_pipe_op
-000057c0: 656e 280a 2020 2020 2020 2020 7333 5f75  en(.        s3_u
-000057d0: 726c 3a20 5061 7468 4c69 6b65 2c0a 2020  rl: PathLike,.  
-000057e0: 2020 2020 2020 6d6f 6465 3a20 7374 722c        mode: str,
-000057f0: 0a20 2020 2020 2020 2066 6f6c 6c6f 776c  .        followl
-00005800: 696e 6b73 3a20 626f 6f6c 203d 2046 616c  inks: bool = Fal
-00005810: 7365 2c0a 2020 2020 2020 2020 2a2c 0a20  se,.        *,. 
-00005820: 2020 2020 2020 206a 6f69 6e5f 7468 7265         join_thre
-00005830: 6164 3a20 626f 6f6c 203d 2054 7275 6529  ad: bool = True)
-00005840: 202d 3e20 5333 5069 7065 4861 6e64 6c65   -> S3PipeHandle
-00005850: 723a 0a20 2020 2027 2727 4f70 656e 2061  r:.    '''Open a
-00005860: 2061 7379 6e63 6872 6f6e 6f75 7320 7265   asynchronous re
-00005870: 6164 2d77 7269 7465 2072 6561 6465 7220  ad-write reader 
-00005880: 2f20 7772 6974 6572 2c20 746f 2073 7570  / writer, to sup
-00005890: 706f 7274 2066 6173 7420 7365 7175 656e  port fast sequen
-000058a0: 7469 616c 2072 6561 6420 2f20 7772 6974  tial read / writ
-000058b0: 650a 0a20 2020 202e 2e20 6e6f 7465 203a  e..    .. note :
-000058c0: 3a0a 0a20 2020 2020 2020 2055 7365 7220  :..        User 
-000058d0: 7368 6f75 6c64 206d 616b 6520 7375 7265  should make sure
-000058e0: 2074 6861 7420 7265 6164 6572 202f 2077   that reader / w
-000058f0: 7269 7465 7220 6172 6520 636c 6f73 6564  riter are closed
-00005900: 2063 6f72 7265 6374 6c79 0a0a 2020 2020   correctly..    
-00005910: 2020 2020 5375 7070 6f72 7473 2063 6f6e      Supports con
-00005920: 7465 7874 206d 616e 6167 6572 0a0a 2020  text manager..  
-00005930: 2020 2020 2020 5768 656e 206a 6f69 6e5f        When join_
-00005940: 7468 7265 6164 2069 7320 4661 6c73 652c  thread is False,
-00005950: 2077 6869 6c65 2074 6865 2066 696c 6520   while the file 
-00005960: 6861 6e64 6c65 2061 7265 2063 6c6f 7369  handle are closi
-00005970: 6e67 2c20 7468 6973 2066 756e 6374 696f  ng, this functio
-00005980: 6e20 7769 6c6c 206e 6f74 2077 6169 7420  n will not wait 
-00005990: 756e 7469 6c20 7468 6520 6173 796e 6368  until the asynch
-000059a0: 726f 6e6f 7573 2077 7269 7469 6e67 2066  ronous writing f
-000059b0: 696e 6973 6865 733b 0a20 2020 2020 2020  inishes;.       
-000059c0: 2046 616c 7365 2064 6f65 736e 2774 2061   False doesn't a
-000059d0: 6666 6563 7420 7265 6164 2d68 616e 646c  ffect read-handl
-000059e0: 652c 2062 7574 2074 6869 7320 6361 6e20  e, but this can 
-000059f0: 7370 6565 6420 7570 2077 7269 7465 2d68  speed up write-h
-00005a00: 616e 646c 6520 6265 6361 7573 6520 6669  andle because fi
-00005a10: 6c65 2077 696c 6c20 6265 2077 7269 7474  le will be writt
-00005a20: 656e 2061 7379 6e63 6872 6f6e 6f75 736c  en asynchronousl
-00005a30: 792e 0a20 2020 2020 2020 2042 7574 2061  y..        But a
-00005a40: 7379 6e63 6872 6f6e 6f75 7320 6265 6861  synchronous beha
-00005a50: 7669 6f75 7220 6361 6e20 6775 6172 616e  viour can guaran
-00005a60: 7465 6520 7468 6520 6669 6c65 2061 7265  tee the file are
-00005a70: 2073 7563 6365 7373 6675 6c6c 7920 7772   successfully wr
-00005a80: 6974 7465 6e2c 2061 6e64 2066 7265 7175  itten, and frequ
-00005a90: 656e 7420 6578 6563 7574 696f 6e20 6d61  ent execution ma
-00005aa0: 7920 6361 7573 6520 7468 7265 6164 2061  y cause thread a
-00005ab0: 6e64 2066 696c 6520 6861 6e64 6c65 2065  nd file handle e
-00005ac0: 7868 6175 7374 696f 6e0a 0a20 2020 203a  xhaustion..    :
-00005ad0: 7061 7261 6d20 6d6f 6465 3a20 4d6f 6465  param mode: Mode
-00005ae0: 2074 6f20 6f70 656e 2066 696c 652c 2065   to open file, e
-00005af0: 6974 6865 7220 2272 6222 206f 7220 2277  ither "rb" or "w
-00005b00: 6222 0a20 2020 203a 7061 7261 6d20 6a6f  b".    :param jo
-00005b10: 696e 5f74 6872 6561 643a 2049 6620 7761  in_thread: If wa
-00005b20: 6974 2061 6674 6572 2066 756e 6374 696f  it after functio
-00005b30: 6e20 6578 6563 7574 696f 6e20 756e 7469  n execution unti
-00005b40: 6c20 7333 2066 696e 6973 6865 7320 7772  l s3 finishes wr
-00005b50: 6974 696e 670a 2020 2020 3a72 6574 7572  iting.    :retur
-00005b60: 6e73 3a20 416e 206f 7065 6e65 6420 4275  ns: An opened Bu
-00005b70: 6666 6572 6564 5265 6164 6572 202f 2042  fferedReader / B
-00005b80: 7566 6665 7265 6457 7269 7465 7220 6f62  ufferedWriter ob
-00005b90: 6a65 6374 0a20 2020 2027 2727 0a20 2020  ject.    '''.   
-00005ba0: 2069 6620 6d6f 6465 206e 6f74 2069 6e20   if mode not in 
-00005bb0: 2827 7262 272c 2027 7762 2729 3a0a 2020  ('rb', 'wb'):.  
-00005bc0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00005bd0: 6545 7272 6f72 2827 756e 6163 6365 7074  eError('unaccept
-00005be0: 6162 6c65 206d 6f64 653a 2025 7227 2025  able mode: %r' %
-00005bf0: 206d 6f64 6529 0a0a 2020 2020 6966 206d   mode)..    if m
-00005c00: 6f64 655b 305d 203d 3d20 2772 2720 616e  ode[0] == 'r' an
-00005c10: 6420 6e6f 7420 5333 5061 7468 2873 335f  d not S3Path(s3_
-00005c20: 7572 6c29 2e69 735f 6669 6c65 2829 3a0a  url).is_file():.
-00005c30: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
-00005c40: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
-00005c50: 7228 274e 6f20 7375 6368 2066 696c 653a  r('No such file:
-00005c60: 2025 7227 2025 2073 335f 7572 6c29 0a0a   %r' % s3_url)..
-00005c70: 2020 2020 7333 5f75 726c 203d 2053 3350      s3_url = S3P
-00005c80: 6174 6828 7333 5f75 726c 290a 2020 2020  ath(s3_url).    
-00005c90: 6966 2066 6f6c 6c6f 776c 696e 6b73 3a0a  if followlinks:.
-00005ca0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00005cb0: 2020 2020 2020 2020 2073 335f 7572 6c20           s3_url 
-00005cc0: 3d20 7333 5f75 726c 2e72 6561 646c 696e  = s3_url.readlin
-00005cd0: 6b28 290a 2020 2020 2020 2020 6578 6365  k().        exce
-00005ce0: 7074 2053 334e 6f74 414c 696e 6b45 7272  pt S3NotALinkErr
-00005cf0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00005d00: 7061 7373 0a0a 2020 2020 6275 636b 6574  pass..    bucket
-00005d10: 2c20 6b65 7920 3d20 7061 7273 655f 7333  , key = parse_s3
-00005d20: 5f75 726c 2873 335f 7572 6c2e 7061 7468  _url(s3_url.path
-00005d30: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
-00005d40: 2020 2020 636f 6e66 6967 203d 2062 6f74      config = bot
-00005d50: 6f63 6f72 652e 636f 6e66 6967 2e43 6f6e  ocore.config.Con
-00005d60: 6669 6728 6d61 785f 706f 6f6c 5f63 6f6e  fig(max_pool_con
-00005d70: 6e65 6374 696f 6e73 3d6d 6178 5f70 6f6f  nections=max_poo
-00005d80: 6c5f 636f 6e6e 6563 7469 6f6e 7329 0a20  l_connections). 
-00005d90: 2020 2063 6c69 656e 7420 3d20 6765 745f     client = get_
-00005da0: 7333 5f63 6c69 656e 7428 0a20 2020 2020  s3_client(.     
-00005db0: 2020 2063 6f6e 6669 673d 636f 6e66 6967     config=config
-00005dc0: 2c0a 2020 2020 2020 2020 6361 6368 655f  ,.        cache_
-00005dd0: 6b65 793d 2773 335f 6669 6c65 6c69 6b65  key='s3_filelike
-00005de0: 5f63 6c69 656e 7427 2c0a 2020 2020 2020  _client',.      
-00005df0: 2020 7072 6f66 696c 655f 6e61 6d65 3d73    profile_name=s
-00005e00: 335f 7572 6c2e 5f70 726f 6669 6c65 5f6e  3_url._profile_n
-00005e10: 616d 6529 0a20 2020 2072 6574 7572 6e20  ame).    return 
-00005e20: 5333 5069 7065 4861 6e64 6c65 7228 0a20  S3PipeHandler(. 
-00005e30: 2020 2020 2020 2062 7563 6b65 742c 206b         bucket, k
-00005e40: 6579 2c20 6d6f 6465 2c20 7333 5f63 6c69  ey, mode, s3_cli
-00005e50: 656e 743d 636c 6965 6e74 2c20 6a6f 696e  ent=client, join
-00005e60: 5f74 6872 6561 643d 6a6f 696e 5f74 6872  _thread=join_thr
-00005e70: 6561 6429 0a0a 0a40 5f73 335f 6269 6e61  ead)...@_s3_bina
-00005e80: 7279 5f6d 6f64 650a 6465 6620 7333 5f63  ry_mode.def s3_c
-00005e90: 6163 6865 645f 6f70 656e 280a 2020 2020  ached_open(.    
-00005ea0: 2020 2020 7333 5f75 726c 3a20 5061 7468      s3_url: Path
-00005eb0: 4c69 6b65 2c0a 2020 2020 2020 2020 6d6f  Like,.        mo
-00005ec0: 6465 3a20 7374 722c 0a20 2020 2020 2020  de: str,.       
-00005ed0: 2066 6f6c 6c6f 776c 696e 6b73 3a20 626f   followlinks: bo
-00005ee0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00005ef0: 2020 2020 2a2c 0a20 2020 2020 2020 2063      *,.        c
-00005f00: 6163 6865 5f70 6174 683a 204f 7074 696f  ache_path: Optio
-00005f10: 6e61 6c5b 7374 725d 203d 204e 6f6e 6529  nal[str] = None)
-00005f20: 202d 3e20 5333 4361 6368 6564 4861 6e64   -> S3CachedHand
-00005f30: 6c65 723a 0a20 2020 2027 2727 4f70 656e  ler:.    '''Open
-00005f40: 2061 206c 6f63 616c 2d63 6163 6865 2066   a local-cache f
-00005f50: 696c 6520 7265 6164 6572 202f 2077 7269  ile reader / wri
-00005f60: 7465 722c 2066 6f72 2066 7265 7175 656e  ter, for frequen
-00005f70: 7420 7261 6e64 6f6d 2072 6561 6420 2f20  t random read / 
-00005f80: 7772 6974 650a 0a20 2020 202e 2e20 6e6f  write..    .. no
-00005f90: 7465 203a 3a0a 0a20 2020 2020 2020 2055  te ::..        U
-00005fa0: 7365 7220 7368 6f75 6c64 206d 616b 6520  ser should make 
-00005fb0: 7375 7265 2074 6861 7420 7265 6164 6572  sure that reader
-00005fc0: 202f 2077 7269 7465 7220 6172 6520 636c   / writer are cl
-00005fd0: 6f73 6564 2063 6f72 7265 6374 6c79 0a0a  osed correctly..
-00005fe0: 2020 2020 2020 2020 5375 7070 6f72 7473          Supports
-00005ff0: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
-00006000: 0a0a 2020 2020 2020 2020 6361 6368 655f  ..        cache_
-00006010: 7061 7468 2063 616e 2073 7065 6369 6679  path can specify
-00006020: 2074 6865 2070 6174 6820 6f66 2063 6163   the path of cac
-00006030: 6865 2066 696c 652e 2050 6572 666f 726d  he file. Perform
-00006040: 616e 6365 2063 6f75 6c64 2062 6520 6265  ance could be be
-00006050: 7474 6572 2069 6620 6361 6368 6520 6669  tter if cache fi
-00006060: 6c65 2070 6174 6820 6973 206f 6e20 7373  le path is on ss
-00006070: 6420 6f72 2074 6d70 6673 0a0a 2020 2020  d or tmpfs..    
-00006080: 3a70 6172 616d 206d 6f64 653a 204d 6f64  :param mode: Mod
-00006090: 6520 746f 206f 7065 6e20 6669 6c65 2c20  e to open file, 
-000060a0: 636f 756c 6420 6265 206f 6e65 206f 6620  could be one of 
-000060b0: 2272 6222 2c20 2277 6222 206f 7220 2261  "rb", "wb" or "a
-000060c0: 6222 0a20 2020 203a 7061 7261 6d20 6361  b".    :param ca
-000060d0: 6368 655f 7061 7468 3a20 6361 6368 6520  che_path: cache 
-000060e0: 6669 6c65 2070 6174 680a 2020 2020 3a72  file path.    :r
-000060f0: 6574 7572 6e73 3a20 416e 206f 7065 6e65  eturns: An opene
-00006100: 6420 4275 6666 6572 6564 5265 6164 6572  d BufferedReader
-00006110: 202f 2042 7566 6665 7265 6457 7269 7465   / BufferedWrite
-00006120: 7220 6f62 6a65 6374 0a20 2020 2027 2727  r object.    '''
-00006130: 0a20 2020 2069 6620 6d6f 6465 206e 6f74  .    if mode not
-00006140: 2069 6e20 2827 7262 272c 2027 7762 272c   in ('rb', 'wb',
-00006150: 2027 6162 272c 2027 7262 2b27 2c20 2777   'ab', 'rb+', 'w
-00006160: 622b 272c 2027 6162 2b27 293a 0a20 2020  b+', 'ab+'):.   
-00006170: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00006180: 4572 726f 7228 2775 6e61 6363 6570 7461  Error('unaccepta
-00006190: 626c 6520 6d6f 6465 3a20 2572 2720 2520  ble mode: %r' % 
-000061a0: 6d6f 6465 290a 2020 2020 7333 5f75 726c  mode).    s3_url
-000061b0: 203d 2053 3350 6174 6828 7333 5f75 726c   = S3Path(s3_url
-000061c0: 290a 2020 2020 6966 2066 6f6c 6c6f 776c  ).    if followl
-000061d0: 696e 6b73 3a0a 2020 2020 2020 2020 7472  inks:.        tr
-000061e0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-000061f0: 335f 7572 6c20 3d20 7333 5f75 726c 2e72  3_url = s3_url.r
-00006200: 6561 646c 696e 6b28 290a 2020 2020 2020  eadlink().      
-00006210: 2020 6578 6365 7074 2053 334e 6f74 414c    except S3NotAL
-00006220: 696e 6b45 7272 6f72 3a0a 2020 2020 2020  inkError:.      
-00006230: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00006240: 6275 636b 6574 2c20 6b65 7920 3d20 7061  bucket, key = pa
-00006250: 7273 655f 7333 5f75 726c 2873 335f 7572  rse_s3_url(s3_ur
-00006260: 6c2e 7061 7468 5f77 6974 685f 7072 6f74  l.path_with_prot
-00006270: 6f63 6f6c 290a 2020 2020 636f 6e66 6967  ocol).    config
-00006280: 203d 2062 6f74 6f63 6f72 652e 636f 6e66   = botocore.conf
-00006290: 6967 2e43 6f6e 6669 6728 6d61 785f 706f  ig.Config(max_po
-000062a0: 6f6c 5f63 6f6e 6e65 6374 696f 6e73 3d6d  ol_connections=m
-000062b0: 6178 5f70 6f6f 6c5f 636f 6e6e 6563 7469  ax_pool_connecti
-000062c0: 6f6e 7329 0a20 2020 2063 6c69 656e 7420  ons).    client 
-000062d0: 3d20 6765 745f 7333 5f63 6c69 656e 7428  = get_s3_client(
-000062e0: 0a20 2020 2020 2020 2063 6f6e 6669 673d  .        config=
-000062f0: 636f 6e66 6967 2c0a 2020 2020 2020 2020  config,.        
-00006300: 6361 6368 655f 6b65 793d 2773 335f 6669  cache_key='s3_fi
-00006310: 6c65 6c69 6b65 5f63 6c69 656e 7427 2c0a  lelike_client',.
-00006320: 2020 2020 2020 2020 7072 6f66 696c 655f          profile_
-00006330: 6e61 6d65 3d73 335f 7572 6c2e 5f70 726f  name=s3_url._pro
-00006340: 6669 6c65 5f6e 616d 6529 0a20 2020 2072  file_name).    r
-00006350: 6574 7572 6e20 5333 4361 6368 6564 4861  eturn S3CachedHa
-00006360: 6e64 6c65 7228 0a20 2020 2020 2020 2062  ndler(.        b
-00006370: 7563 6b65 742c 206b 6579 2c20 6d6f 6465  ucket, key, mode
-00006380: 2c20 7333 5f63 6c69 656e 743d 636c 6965  , s3_client=clie
-00006390: 6e74 2c20 6361 6368 655f 7061 7468 3d63  nt, cache_path=c
-000063a0: 6163 6865 5f70 6174 6829 0a0a 0a40 5f73  ache_path)...@_s
-000063b0: 335f 6269 6e61 7279 5f6d 6f64 650a 6465  3_binary_mode.de
-000063c0: 6620 7333 5f62 7566 6665 7265 645f 6f70  f s3_buffered_op
-000063d0: 656e 280a 2020 2020 2020 2020 7333 5f75  en(.        s3_u
-000063e0: 726c 3a20 5061 7468 4c69 6b65 2c0a 2020  rl: PathLike,.  
-000063f0: 2020 2020 2020 6d6f 6465 3a20 7374 722c        mode: str,
-00006400: 0a20 2020 2020 2020 2066 6f6c 6c6f 776c  .        followl
-00006410: 696e 6b73 3a20 626f 6f6c 203d 2046 616c  inks: bool = Fal
-00006420: 7365 2c0a 2020 2020 2020 2020 2a2c 0a20  se,.        *,. 
-00006430: 2020 2020 2020 206d 6178 5f63 6f6e 6375         max_concu
-00006440: 7272 656e 6379 3a20 4f70 7469 6f6e 616c  rrency: Optional
-00006450: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-00006460: 2020 2020 2020 6d61 785f 6275 6666 6572        max_buffer
-00006470: 5f73 697a 653a 2069 6e74 203d 2044 4546  _size: int = DEF
-00006480: 4155 4c54 5f4d 4158 5f42 5546 4645 525f  AULT_MAX_BUFFER_
-00006490: 5349 5a45 2c0a 2020 2020 2020 2020 666f  SIZE,.        fo
-000064a0: 7277 6172 645f 7261 7469 6f3a 204f 7074  rward_ratio: Opt
-000064b0: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
-000064c0: 6f6e 652c 0a20 2020 2020 2020 2062 6c6f  one,.        blo
-000064d0: 636b 5f73 697a 653a 2069 6e74 203d 2044  ck_size: int = D
-000064e0: 4546 4155 4c54 5f42 4c4f 434b 5f53 495a  EFAULT_BLOCK_SIZ
-000064f0: 452c 0a20 2020 2020 2020 206c 696d 6974  E,.        limit
-00006500: 6564 5f73 6565 6b61 626c 653a 2062 6f6f  ed_seekable: boo
-00006510: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-00006520: 2020 2062 7566 6665 7265 643a 2062 6f6f     buffered: boo
-00006530: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
-00006540: 2020 7368 6172 655f 6361 6368 655f 6b65    share_cache_ke
-00006550: 793a 204f 7074 696f 6e61 6c5b 7374 725d  y: Optional[str]
-00006560: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00006570: 2063 6163 6865 5f70 6174 683a 204f 7074   cache_path: Opt
-00006580: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00006590: 650a 2920 2d3e 2055 6e69 6f6e 5b53 3350  e.) -> Union[S3P
-000065a0: 7265 6665 7463 6852 6561 6465 722c 2053  refetchReader, S
-000065b0: 3342 7566 6665 7265 6457 7269 7465 722c  3BufferedWriter,
-000065c0: 2069 6f2e 4275 6666 6572 6564 5265 6164   io.BufferedRead
-000065d0: 6572 2c20 696f 2e0a 2020 2020 2020 2020  er, io..        
-000065e0: 2020 2042 7566 6665 7265 6457 7269 7465     BufferedWrite
-000065f0: 722c 2053 334d 656d 6f72 7948 616e 646c  r, S3MemoryHandl
-00006600: 6572 5d3a 0a20 2020 2027 2727 4f70 656e  er]:.    '''Open
-00006610: 2061 6e20 6173 796e 6368 726f 6e6f 7573   an asynchronous
-00006620: 2070 7265 6665 7463 6820 7265 6164 6572   prefetch reader
-00006630: 2c20 746f 2073 7570 706f 7274 2066 6173  , to support fas
-00006640: 7420 7365 7175 656e 7469 616c 2072 6561  t sequential rea
-00006650: 640a 0a20 2020 202e 2e20 6e6f 7465 203a  d..    .. note :
-00006660: 3a0a 0a20 2020 2020 2020 2055 7365 7220  :..        User 
-00006670: 7368 6f75 6c64 206d 616b 6520 7375 7265  should make sure
-00006680: 2074 6861 7420 7265 6164 6572 202f 2077   that reader / w
-00006690: 7269 7465 7220 6172 6520 636c 6f73 6564  riter are closed
-000066a0: 2063 6f72 7265 6374 6c79 0a0a 2020 2020   correctly..    
-000066b0: 2020 2020 5375 7070 6f72 7473 2063 6f6e      Supports con
-000066c0: 7465 7874 206d 616e 6167 6572 0a0a 2020  text manager..  
-000066d0: 2020 2020 2020 536f 6d65 2070 6172 616d        Some param
-000066e0: 6574 6572 2073 6574 7469 6e67 206d 6179  eter setting may
-000066f0: 2070 6572 666f 726d 2077 656c 6c3a 206d   perform well: m
-00006700: 6178 5f63 6f6e 6375 7272 656e 6379 3d31  ax_concurrency=1
-00006710: 3020 6f72 2032 302c 206d 6178 5f62 6c6f  0 or 20, max_blo
-00006720: 636b 5f73 697a 653d 3820 6f72 2031 3620  ck_size=8 or 16 
-00006730: 4d42 2c20 6465 6661 756c 7420 7661 6c75  MB, default valu
-00006740: 6520 4e6f 6e65 206d 6561 6e73 2075 7369  e None means usi
-00006750: 6e67 2067 6c6f 6261 6c20 7468 7265 6164  ng global thread
-00006760: 2070 6f6f 6c0a 0a20 2020 203a 7061 7261   pool..    :para
-00006770: 6d20 6d61 785f 636f 6e63 7572 7265 6e63  m max_concurrenc
-00006780: 793a 204d 6178 2064 6f77 6e6c 6f61 6420  y: Max download 
-00006790: 7468 7265 6164 206e 756d 6265 722c 204e  thread number, N
-000067a0: 6f6e 6520 6279 2064 6566 6175 6c74 0a20  one by default. 
-000067b0: 2020 203a 7061 7261 6d20 6d61 785f 6275     :param max_bu
-000067c0: 6666 6572 5f73 697a 653a 204d 6178 2063  ffer_size: Max c
-000067d0: 6163 6865 6420 6275 6666 6572 2073 697a  ached buffer siz
-000067e0: 6520 696e 206d 656d 6f72 792c 2031 3238  e in memory, 128
-000067f0: 4d42 2062 7920 6465 6661 756c 740a 2020  MB by default.  
-00006800: 2020 3a70 6172 616d 2062 6c6f 636b 5f73    :param block_s
-00006810: 697a 653a 2053 697a 6520 6f66 2073 696e  ize: Size of sin
-00006820: 676c 6520 626c 6f63 6b2c 2038 4d42 2062  gle block, 8MB b
-00006830: 7920 6465 6661 756c 742e 2045 6163 6820  y default. Each 
-00006840: 626c 6f63 6b20 7769 6c6c 2062 6520 7570  block will be up
-00006850: 6c6f 6164 6564 206f 7220 646f 776e 6c6f  loaded or downlo
-00006860: 6164 6564 2062 7920 7369 6e67 6c65 2074  aded by single t
-00006870: 6872 6561 642e 0a20 2020 203a 7061 7261  hread..    :para
-00006880: 6d20 6c69 6d69 7465 645f 7365 656b 6162  m limited_seekab
-00006890: 6c65 3a20 4966 2077 7269 7465 2d68 616e  le: If write-han
-000068a0: 646c 6520 7375 7070 6f72 7473 206c 696d  dle supports lim
-000068b0: 6974 6564 2073 6565 6b20 2862 6f74 6820  ited seek (both 
-000068c0: 6669 6c65 2068 6561 6420 7061 7274 2061  file head part a
-000068d0: 6e64 2074 6169 6c20 7061 7274 2063 616e  nd tail part can
-000068e0: 2073 6565 6b20 626c 6f63 6b5f 7369 7a65   seek block_size
-000068f0: 292e 204e 6f74 6573 3a20 5468 6973 2070  ). Notes: This p
-00006900: 6172 616d 6574 6572 2061 7265 2076 616c  arameter are val
-00006910: 6964 206f 6e6c 7920 666f 7220 7772 6974  id only for writ
-00006920: 652d 6861 6e64 6c65 2e20 5265 6164 2d68  e-handle. Read-h
-00006930: 616e 646c 6520 7375 7070 6f72 7420 6172  andle support ar
-00006940: 6269 7472 6172 7920 7365 656b 0a20 2020  bitrary seek.   
-00006950: 203a 7265 7475 726e 733a 2041 6e20 6f70   :returns: An op
-00006960: 656e 6564 2053 3350 7265 6665 7463 6852  ened S3PrefetchR
-00006970: 6561 6465 7220 6f62 6a65 6374 0a20 2020  eader object.   
-00006980: 203a 7261 6973 6573 3a20 5333 4669 6c65   :raises: S3File
-00006990: 4e6f 7446 6f75 6e64 4572 726f 720a 2020  NotFoundError.  
-000069a0: 2020 2727 270a 2020 2020 6966 206d 6f64    '''.    if mod
-000069b0: 6520 6e6f 7420 696e 2028 2772 6227 2c20  e not in ('rb', 
-000069c0: 2777 6227 2c20 2761 6227 2c20 2772 622b  'wb', 'ab', 'rb+
-000069d0: 272c 2027 7762 2b27 2c20 2761 622b 2729  ', 'wb+', 'ab+')
-000069e0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-000069f0: 5661 6c75 6545 7272 6f72 2827 756e 6163  ValueError('unac
-00006a00: 6365 7074 6162 6c65 206d 6f64 653a 2025  ceptable mode: %
-00006a10: 7227 2025 206d 6f64 6529 0a20 2020 2073  r' % mode).    s
-00006a20: 335f 7572 6c20 3d20 5333 5061 7468 2873  3_url = S3Path(s
-00006a30: 335f 7572 6c29 0a20 2020 2069 6620 666f  3_url).    if fo
-00006a40: 6c6c 6f77 6c69 6e6b 733a 0a20 2020 2020  llowlinks:.     
-00006a50: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00006a60: 2020 2020 7333 5f75 726c 203d 2073 335f      s3_url = s3_
-00006a70: 7572 6c2e 7265 6164 6c69 6e6b 2829 0a20  url.readlink(). 
-00006a80: 2020 2020 2020 2065 7863 6570 7420 5333         except S3
-00006a90: 4e6f 7441 4c69 6e6b 4572 726f 723a 0a20  NotALinkError:. 
-00006aa0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00006ab0: 0a20 2020 2062 7563 6b65 742c 206b 6579  .    bucket, key
-00006ac0: 203d 2070 6172 7365 5f73 335f 7572 6c28   = parse_s3_url(
-00006ad0: 7333 5f75 726c 2e70 6174 685f 7769 7468  s3_url.path_with
-00006ae0: 5f70 726f 746f 636f 6c29 0a20 2020 2063  _protocol).    c
-00006af0: 6f6e 6669 6720 3d20 626f 746f 636f 7265  onfig = botocore
-00006b00: 2e63 6f6e 6669 672e 436f 6e66 6967 286d  .config.Config(m
-00006b10: 6178 5f70 6f6f 6c5f 636f 6e6e 6563 7469  ax_pool_connecti
-00006b20: 6f6e 733d 6d61 785f 706f 6f6c 5f63 6f6e  ons=max_pool_con
-00006b30: 6e65 6374 696f 6e73 290a 2020 2020 636c  nections).    cl
-00006b40: 6965 6e74 203d 2067 6574 5f73 335f 636c  ient = get_s3_cl
-00006b50: 6965 6e74 280a 2020 2020 2020 2020 636f  ient(.        co
-00006b60: 6e66 6967 3d63 6f6e 6669 672c 0a20 2020  nfig=config,.   
-00006b70: 2020 2020 2063 6163 6865 5f6b 6579 3d27       cache_key='
-00006b80: 7333 5f66 696c 656c 696b 655f 636c 6965  s3_filelike_clie
-00006b90: 6e74 272c 0a20 2020 2020 2020 2070 726f  nt',.        pro
-00006ba0: 6669 6c65 5f6e 616d 653d 7333 5f75 726c  file_name=s3_url
-00006bb0: 2e5f 7072 6f66 696c 655f 6e61 6d65 290a  ._profile_name).
-00006bc0: 0a20 2020 2069 6620 2761 2720 696e 206d  .    if 'a' in m
-00006bd0: 6f64 6520 6f72 2027 2b27 2069 6e20 6d6f  ode or '+' in mo
-00006be0: 6465 3a0a 2020 2020 2020 2020 6966 2063  de:.        if c
-00006bf0: 6163 6865 5f70 6174 6820 6973 204e 6f6e  ache_path is Non
-00006c00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00006c10: 6574 7572 6e20 5333 4d65 6d6f 7279 4861  eturn S3MemoryHa
-00006c20: 6e64 6c65 7228 6275 636b 6574 2c20 6b65  ndler(bucket, ke
-00006c30: 792c 206d 6f64 652c 2073 335f 636c 6965  y, mode, s3_clie
-00006c40: 6e74 3d63 6c69 656e 7429 0a20 2020 2020  nt=client).     
-00006c50: 2020 2072 6574 7572 6e20 5333 4361 6368     return S3Cach
-00006c60: 6564 4861 6e64 6c65 7228 0a20 2020 2020  edHandler(.     
-00006c70: 2020 2020 2020 2062 7563 6b65 742c 206b         bucket, k
-00006c80: 6579 2c20 6d6f 6465 2c20 7333 5f63 6c69  ey, mode, s3_cli
-00006c90: 656e 743d 636c 6965 6e74 2c20 6361 6368  ent=client, cach
-00006ca0: 655f 7061 7468 3d63 6163 6865 5f70 6174  e_path=cache_pat
-00006cb0: 6829 0a0a 2020 2020 6966 206d 6f64 6520  h)..    if mode 
-00006cc0: 3d3d 2027 7262 273a 0a20 2020 2020 2020  == 'rb':.       
-00006cd0: 2023 2041 2072 6f75 6768 2063 6f6e 7665   # A rough conve
-00006ce0: 7273 696f 6e20 616c 676f 7269 7468 6d20  rsion algorithm 
-00006cf0: 746f 2061 6c69 676e 2032 2074 7970 6573  to align 2 types
-00006d00: 206f 6620 5265 6164 6572 202f 2057 7269   of Reader / Wri
-00006d10: 7465 7220 7061 7261 6d65 7465 7273 0a20  ter parameters. 
-00006d20: 2020 2020 2020 2023 2054 4f44 4f3a 204f         # TODO: O
-00006d30: 7074 696d 697a 6520 7468 6520 636f 6e76  ptimize the conv
-00006d40: 6572 7369 6f6e 2061 6c67 6f72 6974 686d  ersion algorithm
-00006d50: 0a20 2020 2020 2020 2062 6c6f 636b 5f63  .        block_c
-00006d60: 6170 6163 6974 7920 3d20 6d61 785f 6275  apacity = max_bu
-00006d70: 6666 6572 5f73 697a 6520 2f2f 2062 6c6f  ffer_size // blo
-00006d80: 636b 5f73 697a 650a 2020 2020 2020 2020  ck_size.        
-00006d90: 6966 2066 6f72 7761 7264 5f72 6174 696f  if forward_ratio
-00006da0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00006db0: 2020 2020 2020 626c 6f63 6b5f 666f 7277        block_forw
-00006dc0: 6172 6420 3d20 4e6f 6e65 0a20 2020 2020  ard = None.     
-00006dd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00006de0: 2020 2020 2062 6c6f 636b 5f66 6f72 7761       block_forwa
-00006df0: 7264 203d 206d 6178 2869 6e74 2862 6c6f  rd = max(int(blo
-00006e00: 636b 5f63 6170 6163 6974 7920 2a20 666f  ck_capacity * fo
-00006e10: 7277 6172 645f 7261 7469 6f29 2c20 3129  rward_ratio), 1)
-00006e20: 0a20 2020 2020 2020 2069 6620 7368 6172  .        if shar
-00006e30: 655f 6361 6368 655f 6b65 7920 6973 206e  e_cache_key is n
-00006e40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00006e50: 2020 2020 2072 6561 6465 7220 3d20 5333       reader = S3
-00006e60: 5368 6172 6543 6163 6865 5265 6164 6572  ShareCacheReader
-00006e70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00006e80: 2020 6275 636b 6574 2c0a 2020 2020 2020    bucket,.      
-00006e90: 2020 2020 2020 2020 2020 6b65 792c 0a20            key,. 
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006eb0: 6163 6865 5f6b 6579 3d73 6861 7265 5f63  ache_key=share_c
-00006ec0: 6163 6865 5f6b 6579 2c0a 2020 2020 2020  ache_key,.      
-00006ed0: 2020 2020 2020 2020 2020 7333 5f63 6c69            s3_cli
-00006ee0: 656e 743d 636c 6965 6e74 2c0a 2020 2020  ent=client,.    
-00006ef0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-00006f00: 7265 7472 6965 733d 6d61 785f 7265 7472  retries=max_retr
-00006f10: 6965 732c 0a20 2020 2020 2020 2020 2020  ies,.           
-00006f20: 2020 2020 206d 6178 5f77 6f72 6b65 7273       max_workers
-00006f30: 3d6d 6178 5f63 6f6e 6375 7272 656e 6379  =max_concurrency
-00006f40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006f50: 2020 626c 6f63 6b5f 7369 7a65 3d62 6c6f    block_size=blo
-00006f60: 636b 5f73 697a 652c 0a20 2020 2020 2020  ck_size,.       
-00006f70: 2020 2020 2020 2020 2062 6c6f 636b 5f66           block_f
-00006f80: 6f72 7761 7264 3d62 6c6f 636b 5f66 6f72  orward=block_for
-00006f90: 7761 7264 290a 2020 2020 2020 2020 656c  ward).        el
-00006fa0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00006fb0: 7265 6164 6572 203d 2053 3350 7265 6665  reader = S3Prefe
-00006fc0: 7463 6852 6561 6465 7228 0a20 2020 2020  tchReader(.     
-00006fd0: 2020 2020 2020 2020 2020 2062 7563 6b65             bucke
-00006fe0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00006ff0: 2020 206b 6579 2c0a 2020 2020 2020 2020     key,.        
-00007000: 2020 2020 2020 2020 7333 5f63 6c69 656e          s3_clien
-00007010: 743d 636c 6965 6e74 2c0a 2020 2020 2020  t=client,.      
-00007020: 2020 2020 2020 2020 2020 6d61 785f 7265            max_re
-00007030: 7472 6965 733d 6d61 785f 7265 7472 6965  tries=max_retrie
-00007040: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00007050: 2020 206d 6178 5f77 6f72 6b65 7273 3d6d     max_workers=m
-00007060: 6178 5f63 6f6e 6375 7272 656e 6379 2c0a  ax_concurrency,.
-00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 626c 6f63 6b5f 6361 7061 6369 7479 3d62  block_capacity=b
-00007090: 6c6f 636b 5f63 6170 6163 6974 792c 0a20  lock_capacity,. 
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000070b0: 6c6f 636b 5f66 6f72 7761 7264 3d62 6c6f  lock_forward=blo
-000070c0: 636b 5f66 6f72 7761 7264 2c0a 2020 2020  ck_forward,.    
-000070d0: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
-000070e0: 6b5f 7369 7a65 3d62 6c6f 636b 5f73 697a  k_size=block_siz
-000070f0: 6529 0a20 2020 2020 2020 2069 6620 6275  e).        if bu
-00007100: 6666 6572 6564 3a0a 2020 2020 2020 2020  ffered:.        
-00007110: 2020 2020 7265 6164 6572 203d 2069 6f2e      reader = io.
-00007120: 4275 6666 6572 6564 5265 6164 6572 2872  BufferedReader(r
-00007130: 6561 6465 7229 2020 2320 7079 7479 7065  eader)  # pytype
-00007140: 3a20 6469 7361 626c 653d 7772 6f6e 672d  : disable=wrong-
-00007150: 6172 672d 7479 7065 730a 2020 2020 2020  arg-types.      
-00007160: 2020 7265 7475 726e 2072 6561 6465 720a    return reader.
-00007170: 0a20 2020 2069 6620 6c69 6d69 7465 645f  .    if limited_
-00007180: 7365 656b 6162 6c65 3a0a 2020 2020 2020  seekable:.      
-00007190: 2020 7772 6974 6572 203d 2053 334c 696d    writer = S3Lim
-000071a0: 6974 6564 5365 656b 6162 6c65 5772 6974  itedSeekableWrit
-000071b0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-000071c0: 6275 636b 6574 2c0a 2020 2020 2020 2020  bucket,.        
-000071d0: 2020 2020 6b65 792c 0a20 2020 2020 2020      key,.       
-000071e0: 2020 2020 2073 335f 636c 6965 6e74 3d63       s3_client=c
-000071f0: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
-00007200: 2020 206d 6178 5f77 6f72 6b65 7273 3d6d     max_workers=m
-00007210: 6178 5f63 6f6e 6375 7272 656e 6379 2c0a  ax_concurrency,.
-00007220: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-00007230: 6275 6666 6572 5f73 697a 653d 6d61 785f  buffer_size=max_
-00007240: 6275 6666 6572 5f73 697a 652c 0a20 2020  buffer_size,.   
-00007250: 2020 2020 2020 2020 2062 6c6f 636b 5f73           block_s
-00007260: 697a 653d 626c 6f63 6b5f 7369 7a65 290a  ize=block_size).
-00007270: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00007280: 2020 7772 6974 6572 203d 2053 3342 7566    writer = S3Buf
-00007290: 6665 7265 6457 7269 7465 7228 0a20 2020  feredWriter(.   
-000072a0: 2020 2020 2020 2020 2062 7563 6b65 742c           bucket,
-000072b0: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
-000072c0: 2c0a 2020 2020 2020 2020 2020 2020 7333  ,.            s3
-000072d0: 5f63 6c69 656e 743d 636c 6965 6e74 2c0a  _client=client,.
-000072e0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-000072f0: 776f 726b 6572 733d 6d61 785f 636f 6e63  workers=max_conc
-00007300: 7572 7265 6e63 792c 0a20 2020 2020 2020  urrency,.       
-00007310: 2020 2020 206d 6178 5f62 7566 6665 725f       max_buffer_
-00007320: 7369 7a65 3d6d 6178 5f62 7566 6665 725f  size=max_buffer_
-00007330: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
-00007340: 2020 626c 6f63 6b5f 7369 7a65 3d62 6c6f    block_size=blo
-00007350: 636b 5f73 697a 6529 0a20 2020 2069 6620  ck_size).    if 
-00007360: 6275 6666 6572 6564 3a0a 2020 2020 2020  buffered:.      
-00007370: 2020 7772 6974 6572 203d 2069 6f2e 4275    writer = io.Bu
-00007380: 6666 6572 6564 5772 6974 6572 2877 7269  fferedWriter(wri
-00007390: 7465 7229 2020 2320 7079 7479 7065 3a20  ter)  # pytype: 
-000073a0: 6469 7361 626c 653d 7772 6f6e 672d 6172  disable=wrong-ar
-000073b0: 672d 7479 7065 730a 2020 2020 7265 7475  g-types.    retu
-000073c0: 726e 2077 7269 7465 720a 0a0a 405f 7333  rn writer...@_s3
-000073d0: 5f62 696e 6172 795f 6d6f 6465 0a64 6566  _binary_mode.def
-000073e0: 2073 335f 6d65 6d6f 7279 5f6f 7065 6e28   s3_memory_open(
-000073f0: 0a20 2020 2020 2020 2073 335f 7572 6c3a  .        s3_url:
-00007400: 2050 6174 684c 696b 652c 206d 6f64 653a   PathLike, mode:
-00007410: 2073 7472 2c0a 2020 2020 2020 2020 666f   str,.        fo
-00007420: 6c6c 6f77 6c69 6e6b 733a 2062 6f6f 6c20  llowlinks: bool 
-00007430: 3d20 4661 6c73 6529 202d 3e20 5333 4d65  = False) -> S3Me
-00007440: 6d6f 7279 4861 6e64 6c65 723a 0a20 2020  moryHandler:.   
-00007450: 2027 2727 4f70 656e 2061 206d 656d 6f72   '''Open a memor
-00007460: 792d 6361 6368 6520 6669 6c65 2072 6561  y-cache file rea
-00007470: 6465 7220 2f20 7772 6974 6572 2c20 666f  der / writer, fo
-00007480: 7220 6672 6571 7565 6e74 2072 616e 646f  r frequent rando
-00007490: 6d20 7265 6164 202f 2077 7269 7465 0a0a  m read / write..
-000074a0: 2020 2020 2e2e 206e 6f74 6520 3a3a 0a0a      .. note ::..
-000074b0: 2020 2020 2020 2020 5573 6572 2073 686f          User sho
-000074c0: 756c 6420 6d61 6b65 2073 7572 6520 7468  uld make sure th
-000074d0: 6174 2072 6561 6465 7220 2f20 7772 6974  at reader / writ
-000074e0: 6572 2061 7265 2063 6c6f 7365 6420 636f  er are closed co
-000074f0: 7272 6563 746c 790a 0a20 2020 2020 2020  rrectly..       
-00007500: 2053 7570 706f 7274 7320 636f 6e74 6578   Supports contex
-00007510: 7420 6d61 6e61 6765 720a 0a20 2020 203a  t manager..    :
-00007520: 7061 7261 6d20 6d6f 6465 3a20 4d6f 6465  param mode: Mode
-00007530: 2074 6f20 6f70 656e 2066 696c 652c 2063   to open file, c
-00007540: 6f75 6c64 2062 6520 6f6e 6520 6f66 2022  ould be one of "
-00007550: 7262 222c 2022 7762 222c 2022 6162 222c  rb", "wb", "ab",
-00007560: 2022 7262 2b22 2c20 2277 622b 2220 6f72   "rb+", "wb+" or
-00007570: 2022 6162 2b22 0a20 2020 203a 7265 7475   "ab+".    :retu
-00007580: 726e 733a 2041 6e20 6f70 656e 6564 2042  rns: An opened B
-00007590: 7566 6665 7265 6452 6561 6465 7220 2f20  ufferedReader / 
-000075a0: 4275 6666 6572 6564 5772 6974 6572 206f  BufferedWriter o
-000075b0: 626a 6563 740a 2020 2020 2727 270a 2020  bject.    '''.  
-000075c0: 2020 6966 206d 6f64 6520 6e6f 7420 696e    if mode not in
-000075d0: 2028 2772 6227 2c20 2777 6227 2c20 2761   ('rb', 'wb', 'a
-000075e0: 6227 2c20 2772 622b 272c 2027 7762 2b27  b', 'rb+', 'wb+'
-000075f0: 2c20 2761 622b 2729 3a0a 2020 2020 2020  , 'ab+'):.      
-00007600: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00007610: 6f72 2827 756e 6163 6365 7074 6162 6c65  or('unacceptable
-00007620: 206d 6f64 653a 2025 7227 2025 206d 6f64   mode: %r' % mod
-00007630: 6529 0a20 2020 2073 335f 7572 6c20 3d20  e).    s3_url = 
-00007640: 5333 5061 7468 2873 335f 7572 6c29 0a20  S3Path(s3_url). 
-00007650: 2020 2069 6620 666f 6c6c 6f77 6c69 6e6b     if followlink
-00007660: 733a 0a20 2020 2020 2020 2074 7279 3a0a  s:.        try:.
-00007670: 2020 2020 2020 2020 2020 2020 7333 5f75              s3_u
-00007680: 726c 203d 2073 335f 7572 6c2e 7265 6164  rl = s3_url.read
-00007690: 6c69 6e6b 2829 0a20 2020 2020 2020 2065  link().        e
-000076a0: 7863 6570 7420 5333 4e6f 7441 4c69 6e6b  xcept S3NotALink
-000076b0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-000076c0: 2020 2070 6173 730a 0a20 2020 2062 7563     pass..    buc
-000076d0: 6b65 742c 206b 6579 203d 2070 6172 7365  ket, key = parse
-000076e0: 5f73 335f 7572 6c28 7333 5f75 726c 2e70  _s3_url(s3_url.p
-000076f0: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
-00007700: 6c29 0a20 2020 2063 6f6e 6669 6720 3d20  l).    config = 
-00007710: 626f 746f 636f 7265 2e63 6f6e 6669 672e  botocore.config.
-00007720: 436f 6e66 6967 286d 6178 5f70 6f6f 6c5f  Config(max_pool_
-00007730: 636f 6e6e 6563 7469 6f6e 733d 6d61 785f  connections=max_
-00007740: 706f 6f6c 5f63 6f6e 6e65 6374 696f 6e73  pool_connections
-00007750: 290a 2020 2020 636c 6965 6e74 203d 2067  ).    client = g
-00007760: 6574 5f73 335f 636c 6965 6e74 280a 2020  et_s3_client(.  
-00007770: 2020 2020 2020 636f 6e66 6967 3d63 6f6e        config=con
-00007780: 6669 672c 0a20 2020 2020 2020 2063 6163  fig,.        cac
-00007790: 6865 5f6b 6579 3d27 7333 5f66 696c 656c  he_key='s3_filel
-000077a0: 696b 655f 636c 6965 6e74 272c 0a20 2020  ike_client',.   
-000077b0: 2020 2020 2070 726f 6669 6c65 5f6e 616d       profile_nam
-000077c0: 653d 7333 5f75 726c 2e5f 7072 6f66 696c  e=s3_url._profil
-000077d0: 655f 6e61 6d65 290a 2020 2020 7265 7475  e_name).    retu
-000077e0: 726e 2053 334d 656d 6f72 7948 616e 646c  rn S3MemoryHandl
-000077f0: 6572 2862 7563 6b65 742c 206b 6579 2c20  er(bucket, key, 
-00007800: 6d6f 6465 2c20 7333 5f63 6c69 656e 743d  mode, s3_client=
-00007810: 636c 6965 6e74 290a 0a0a 7333 5f6f 7065  client)...s3_ope
-00007820: 6e20 3d20 7333 5f62 7566 6665 7265 645f  n = s3_buffered_
-00007830: 6f70 656e 0a0a 0a64 6566 2073 335f 646f  open...def s3_do
-00007840: 776e 6c6f 6164 280a 2020 2020 2020 2020  wnload(.        
-00007850: 7372 635f 7572 6c3a 2050 6174 684c 696b  src_url: PathLik
-00007860: 652c 0a20 2020 2020 2020 2064 7374 5f75  e,.        dst_u
-00007870: 726c 3a20 5061 7468 4c69 6b65 2c0a 2020  rl: PathLike,.  
-00007880: 2020 2020 2020 666f 6c6c 6f77 6c69 6e6b        followlink
-00007890: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-000078a0: 0a20 2020 2020 2020 2063 616c 6c62 6163  .        callbac
-000078b0: 6b3a 204f 7074 696f 6e61 6c5b 4361 6c6c  k: Optional[Call
-000078c0: 6162 6c65 5b5b 696e 745d 2c20 4e6f 6e65  able[[int], None
-000078d0: 5d5d 203d 204e 6f6e 6529 202d 3e20 4e6f  ]] = None) -> No
-000078e0: 6e65 3a0a 2020 2020 2727 270a 2020 2020  ne:.    '''.    
-000078f0: 446f 776e 6c6f 6164 7320 6120 6669 6c65  Downloads a file
-00007900: 2066 726f 6d20 7333 2074 6f20 6c6f 6361   from s3 to loca
-00007910: 6c20 6669 6c65 7379 7374 656d 2e0a 2020  l filesystem..  
-00007920: 2020 3a70 6172 616d 2073 7263 5f75 726c    :param src_url
-00007930: 3a20 736f 7572 6365 2073 3320 7061 7468  : source s3 path
-00007940: 0a20 2020 203a 7061 7261 6d20 6473 745f  .    :param dst_
-00007950: 7572 6c3a 2074 6172 6765 7420 6673 2070  url: target fs p
-00007960: 6174 680a 2020 2020 3a70 6172 616d 2063  ath.    :param c
-00007970: 616c 6c62 6163 6b3a 2043 616c 6c65 6420  allback: Called 
-00007980: 7065 7269 6f64 6963 616c 6c79 2064 7572  periodically dur
-00007990: 696e 6720 636f 7079 2c20 616e 6420 7468  ing copy, and th
-000079a0: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
-000079b0: 7220 6973 2074 6865 2064 6174 6120 7369  r is the data si
-000079c0: 7a65 2028 696e 2062 7974 6573 2920 6f66  ze (in bytes) of
-000079d0: 2063 6f70 7920 7369 6e63 6520 7468 6520   copy since the 
-000079e0: 6c61 7374 2063 616c 6c0a 2020 2020 2727  last call.    ''
-000079f0: 270a 2020 2020 7372 635f 7572 6c20 3d20  '.    src_url = 
-00007a00: 5333 5061 7468 2873 7263 5f75 726c 290a  S3Path(src_url).
-00007a10: 2020 2020 6966 2066 6f6c 6c6f 776c 696e      if followlin
-00007a20: 6b73 3a0a 2020 2020 2020 2020 7472 793a  ks:.        try:
-00007a30: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-00007a40: 5f75 726c 203d 2073 7263 5f75 726c 2e72  _url = src_url.r
-00007a50: 6561 646c 696e 6b28 290a 2020 2020 2020  eadlink().      
-00007a60: 2020 6578 6365 7074 2053 334e 6f74 414c    except S3NotAL
-00007a70: 696e 6b45 7272 6f72 3a0a 2020 2020 2020  inkError:.      
-00007a80: 2020 2020 2020 7061 7373 0a20 2020 2073        pass.    s
-00007a90: 7263 5f62 7563 6b65 742c 2073 7263 5f6b  rc_bucket, src_k
-00007aa0: 6579 203d 2070 6172 7365 5f73 335f 7572  ey = parse_s3_ur
-00007ab0: 6c28 7372 635f 7572 6c2e 7061 7468 5f77  l(src_url.path_w
-00007ac0: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
-00007ad0: 2020 6966 206e 6f74 2073 7263 5f62 7563    if not src_buc
-00007ae0: 6b65 743a 0a20 2020 2020 2020 2072 6169  ket:.        rai
-00007af0: 7365 2053 3342 7563 6b65 744e 6f74 466f  se S3BucketNotFo
-00007b00: 756e 6445 7272 6f72 280a 2020 2020 2020  undError(.      
-00007b10: 2020 2020 2020 2745 6d70 7479 2062 7563        'Empty buc
-00007b20: 6b65 7420 6e61 6d65 3a20 2572 2720 2520  ket name: %r' % 
-00007b30: 7372 635f 7572 6c2e 7061 7468 5f77 6974  src_url.path_wit
-00007b40: 685f 7072 6f74 6f63 6f6c 290a 0a20 2020  h_protocol)..   
-00007b50: 2069 6620 6e6f 7420 7372 635f 7572 6c2e   if not src_url.
-00007b60: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-00007b70: 2020 7261 6973 6520 5333 4669 6c65 4e6f    raise S3FileNo
-00007b80: 7446 6f75 6e64 4572 726f 7228 0a20 2020  tFoundError(.   
-00007b90: 2020 2020 2020 2020 2027 4669 6c65 206e           'File n
-00007ba0: 6f74 2066 6f75 6e64 3a20 2572 2720 2520  ot found: %r' % 
-00007bb0: 7372 635f 7572 6c2e 7061 7468 5f77 6974  src_url.path_wit
-00007bc0: 685f 7072 6f74 6f63 6f6c 290a 0a20 2020  h_protocol)..   
-00007bd0: 2069 6620 6e6f 7420 7372 635f 7572 6c2e   if not src_url.
-00007be0: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
-00007bf0: 2020 2072 6169 7365 2053 3349 7341 4469     raise S3IsADi
-00007c00: 7265 6374 6f72 7945 7272 6f72 280a 2020  rectoryError(.  
-00007c10: 2020 2020 2020 2020 2020 2749 7320 6120            'Is a 
-00007c20: 6469 7265 6374 6f72 793a 2025 7227 2025  directory: %r' %
-00007c30: 2073 7263 5f75 726c 2e70 6174 685f 7769   src_url.path_wi
-00007c40: 7468 5f70 726f 746f 636f 6c29 0a0a 2020  th_protocol)..  
-00007c50: 2020 6473 745f 7572 6c20 3d20 6673 7061    dst_url = fspa
-00007c60: 7468 2864 7374 5f75 726c 290a 2020 2020  th(dst_url).    
-00007c70: 6966 206e 6f74 2064 7374 5f75 726c 206f  if not dst_url o
-00007c80: 7220 6473 745f 7572 6c2e 656e 6473 7769  r dst_url.endswi
-00007c90: 7468 2827 2f27 293a 0a20 2020 2020 2020  th('/'):.       
-00007ca0: 2072 6169 7365 2053 3349 7341 4469 7265   raise S3IsADire
-00007cb0: 6374 6f72 7945 7272 6f72 2827 4973 2061  ctoryError('Is a
-00007cc0: 2064 6972 6563 746f 7279 3a20 2572 2720   directory: %r' 
-00007cd0: 2520 6473 745f 7572 6c29 0a0a 2020 2020  % dst_url)..    
-00007ce0: 6473 745f 6469 7265 6374 6f72 7920 3d20  dst_directory = 
-00007cf0: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-00007d00: 6473 745f 7572 6c29 0a20 2020 2069 6620  dst_url).    if 
-00007d10: 6473 745f 6469 7265 6374 6f72 7920 213d  dst_directory !=
-00007d20: 2027 273a 0a20 2020 2020 2020 206f 732e   '':.        os.
-00007d30: 6d61 6b65 6469 7273 2864 7374 5f64 6972  makedirs(dst_dir
-00007d40: 6563 746f 7279 2c20 6578 6973 745f 6f6b  ectory, exist_ok
-00007d50: 3d54 7275 6529 0a0a 2020 2020 636c 6965  =True)..    clie
-00007d60: 6e74 203d 2067 6574 5f73 335f 636c 6965  nt = get_s3_clie
-00007d70: 6e74 2870 726f 6669 6c65 5f6e 616d 653d  nt(profile_name=
-00007d80: 7372 635f 7572 6c2e 5f70 726f 6669 6c65  src_url._profile
-00007d90: 5f6e 616d 6529 0a20 2020 2074 7279 3a0a  _name).    try:.
-00007da0: 2020 2020 2020 2020 636c 6965 6e74 2e64          client.d
-00007db0: 6f77 6e6c 6f61 645f 6669 6c65 2873 7263  ownload_file(src
-00007dc0: 5f62 7563 6b65 742c 2073 7263 5f6b 6579  _bucket, src_key
-00007dd0: 2c20 6473 745f 7572 6c2c 2043 616c 6c62  , dst_url, Callb
-00007de0: 6163 6b3d 6361 6c6c 6261 636b 290a 2020  ack=callback).  
-00007df0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00007e00: 6f6e 2061 7320 6572 726f 723a 2020 2320  on as error:  # 
-00007e10: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-00007e20: 0a20 2020 2020 2020 2065 7272 6f72 203d  .        error =
-00007e30: 2074 7261 6e73 6c61 7465 5f66 735f 6572   translate_fs_er
-00007e40: 726f 7228 6572 726f 722c 2064 7374 5f75  ror(error, dst_u
-00007e50: 726c 290a 2020 2020 2020 2020 6572 726f  rl).        erro
-00007e60: 7220 3d20 7472 616e 736c 6174 655f 7333  r = translate_s3
-00007e70: 5f65 7272 6f72 2865 7272 6f72 2c20 7372  _error(error, sr
-00007e80: 635f 7572 6c2e 7061 7468 5f77 6974 685f  c_url.path_with_
-00007e90: 7072 6f74 6f63 6f6c 290a 2020 2020 2020  protocol).      
-00007ea0: 2020 7261 6973 6520 6572 726f 720a 0a20    raise error.. 
-00007eb0: 2020 2073 7263 5f73 7461 7420 3d20 7372     src_stat = sr
-00007ec0: 635f 7572 6c2e 7374 6174 2829 0a20 2020  c_url.stat().   
-00007ed0: 206f 732e 7574 696d 6528 6473 745f 7572   os.utime(dst_ur
-00007ee0: 6c2c 2028 7372 635f 7374 6174 2e73 745f  l, (src_stat.st_
-00007ef0: 6d74 696d 652c 2073 7263 5f73 7461 742e  mtime, src_stat.
-00007f00: 7374 5f6d 7469 6d65 2929 0a0a 0a64 6566  st_mtime))...def
-00007f10: 2073 335f 7570 6c6f 6164 280a 2020 2020   s3_upload(.    
-00007f20: 2020 2020 7372 635f 7572 6c3a 2050 6174      src_url: Pat
-00007f30: 684c 696b 652c 0a20 2020 2020 2020 2064  hLike,.        d
-00007f40: 7374 5f75 726c 3a20 5061 7468 4c69 6b65  st_url: PathLike
-00007f50: 2c0a 2020 2020 2020 2020 6361 6c6c 6261  ,.        callba
-00007f60: 636b 3a20 4f70 7469 6f6e 616c 5b43 616c  ck: Optional[Cal
-00007f70: 6c61 626c 655b 5b69 6e74 5d2c 204e 6f6e  lable[[int], Non
-00007f80: 655d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  e]] = None,.    
-00007f90: 2020 2020 2a2a 6b77 6172 6773 2920 2d3e      **kwargs) ->
-00007fa0: 204e 6f6e 653a 0a20 2020 2027 2727 0a20   None:.    '''. 
-00007fb0: 2020 2055 706c 6f61 6473 2061 2066 696c     Uploads a fil
-00007fc0: 6520 6672 6f6d 206c 6f63 616c 2066 696c  e from local fil
-00007fd0: 6573 7973 7465 6d20 746f 2073 332e 0a20  esystem to s3.. 
-00007fe0: 2020 203a 7061 7261 6d20 7372 635f 7572     :param src_ur
-00007ff0: 6c3a 2073 6f75 7263 6520 6673 2070 6174  l: source fs pat
-00008000: 680a 2020 2020 3a70 6172 616d 2064 7374  h.    :param dst
-00008010: 5f75 726c 3a20 7461 7267 6574 2073 3320  _url: target s3 
-00008020: 7061 7468 0a20 2020 203a 7061 7261 6d20  path.    :param 
-00008030: 6361 6c6c 6261 636b 3a20 4361 6c6c 6564  callback: Called
-00008040: 2070 6572 696f 6469 6361 6c6c 7920 6475   periodically du
-00008050: 7269 6e67 2063 6f70 792c 2061 6e64 2074  ring copy, and t
-00008060: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
-00008070: 6572 2069 7320 7468 6520 6461 7461 2073  er is the data s
-00008080: 697a 6520 2869 6e20 6279 7465 7329 206f  ize (in bytes) o
-00008090: 6620 636f 7079 2073 696e 6365 2074 6865  f copy since the
-000080a0: 206c 6173 7420 6361 6c6c 0a20 2020 2027   last call.    '
-000080b0: 2727 0a20 2020 2064 7374 5f62 7563 6b65  ''.    dst_bucke
-000080c0: 742c 2064 7374 5f6b 6579 203d 2070 6172  t, dst_key = par
-000080d0: 7365 5f73 335f 7572 6c28 6473 745f 7572  se_s3_url(dst_ur
-000080e0: 6c29 0a20 2020 2069 6620 6e6f 7420 6473  l).    if not ds
-000080f0: 745f 6275 636b 6574 3a0a 2020 2020 2020  t_bucket:.      
-00008100: 2020 7261 6973 6520 5333 4275 636b 6574    raise S3Bucket
-00008110: 4e6f 7446 6f75 6e64 4572 726f 7228 2745  NotFoundError('E
-00008120: 6d70 7479 2062 7563 6b65 7420 6e61 6d65  mpty bucket name
-00008130: 3a20 2572 2720 2520 6473 745f 7572 6c29  : %r' % dst_url)
-00008140: 0a20 2020 2069 6620 6e6f 7420 6473 745f  .    if not dst_
-00008150: 6b65 7920 6f72 2064 7374 5f6b 6579 2e65  key or dst_key.e
-00008160: 6e64 7377 6974 6828 272f 2729 3a0a 2020  ndswith('/'):.  
-00008170: 2020 2020 2020 7261 6973 6520 5333 4973        raise S3Is
-00008180: 4144 6972 6563 746f 7279 4572 726f 7228  ADirectoryError(
-00008190: 2749 7320 6120 6469 7265 6374 6f72 793a  'Is a directory:
-000081a0: 2025 7227 2025 2064 7374 5f75 726c 290a   %r' % dst_url).
-000081b0: 0a20 2020 2063 6c69 656e 7420 3d20 6765  .    client = ge
-000081c0: 745f 7333 5f63 6c69 656e 7428 7072 6f66  t_s3_client(prof
-000081d0: 696c 655f 6e61 6d65 3d53 3350 6174 6828  ile_name=S3Path(
-000081e0: 6473 745f 7572 6c29 2e5f 7072 6f66 696c  dst_url)._profil
-000081f0: 655f 6e61 6d65 290a 2020 2020 7769 7468  e_name).    with
-00008200: 206f 7065 6e28 7372 635f 7572 6c2c 2027   open(src_url, '
-00008210: 7262 2729 2061 7320 7372 633a 0a20 2020  rb') as src:.   
-00008220: 2020 2020 2077 6974 6820 7261 6973 655f       with raise_
-00008230: 7333 5f65 7272 6f72 2864 7374 5f75 726c  s3_error(dst_url
-00008240: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00008250: 6c69 656e 742e 7570 6c6f 6164 5f66 696c  lient.upload_fil
-00008260: 656f 626a 280a 2020 2020 2020 2020 2020  eobj(.          
-00008270: 2020 2020 2020 7372 632c 2042 7563 6b65        src, Bucke
-00008280: 743d 6473 745f 6275 636b 6574 2c20 4b65  t=dst_bucket, Ke
-00008290: 793d 6473 745f 6b65 792c 2043 616c 6c62  y=dst_key, Callb
-000082a0: 6163 6b3d 6361 6c6c 6261 636b 290a 0a0a  ack=callback)...
-000082b0: 6465 6620 7333 5f6c 6f61 645f 636f 6e74  def s3_load_cont
-000082c0: 656e 7428 0a20 2020 2020 2020 2073 335f  ent(.        s3_
-000082d0: 7572 6c2c 0a20 2020 2020 2020 2073 7461  url,.        sta
-000082e0: 7274 3a20 4f70 7469 6f6e 616c 5b69 6e74  rt: Optional[int
-000082f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00008300: 2020 7374 6f70 3a20 4f70 7469 6f6e 616c    stop: Optional
-00008310: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-00008320: 2020 2020 2020 666f 6c6c 6f77 6c69 6e6b        followlink
-00008330: 733a 2062 6f6f 6c20 3d20 4661 6c73 6529  s: bool = False)
-00008340: 202d 3e20 6279 7465 733a 0a20 2020 2027   -> bytes:.    '
-00008350: 2727 0a20 2020 2047 6574 2073 7065 6369  ''.    Get speci
-00008360: 6669 6564 2066 696c 6520 6672 6f6d 205b  fied file from [
-00008370: 7374 6172 742c 2073 746f 7029 2069 6e20  start, stop) in 
-00008380: 6279 7465 730a 0a20 2020 203a 7061 7261  bytes..    :para
-00008390: 6d20 7333 5f75 726c 3a20 5370 6563 6966  m s3_url: Specif
-000083a0: 6965 6420 7061 7468 0a20 2020 203a 7061  ied path.    :pa
-000083b0: 7261 6d20 7374 6172 743a 2073 7461 7274  ram start: start
-000083c0: 2069 6e64 6578 0a20 2020 203a 7061 7261   index.    :para
-000083d0: 6d20 7374 6f70 3a20 7374 6f70 2069 6e64  m stop: stop ind
-000083e0: 6578 0a20 2020 203a 7265 7475 726e 733a  ex.    :returns:
-000083f0: 2062 7974 6573 2063 6f6e 7465 6e74 2069   bytes content i
-00008400: 6e20 7261 6e67 6520 5b73 7461 7274 2c20  n range [start, 
-00008410: 7374 6f70 290a 2020 2020 2727 270a 0a20  stop).    '''.. 
-00008420: 2020 2064 6566 205f 6765 745f 6f62 6a65     def _get_obje
-00008430: 6374 2863 6c69 656e 742c 2062 7563 6b65  ct(client, bucke
-00008440: 742c 206b 6579 2c20 7261 6e67 655f 7374  t, key, range_st
-00008450: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
-00008460: 726e 2063 6c69 656e 742e 6765 745f 6f62  rn client.get_ob
-00008470: 6a65 6374 280a 2020 2020 2020 2020 2020  ject(.          
-00008480: 2020 4275 636b 6574 3d62 7563 6b65 742c    Bucket=bucket,
-00008490: 204b 6579 3d6b 6579 2c20 5261 6e67 653d   Key=key, Range=
-000084a0: 7261 6e67 655f 7374 7229 5b27 426f 6479  range_str)['Body
-000084b0: 275d 2e72 6561 6428 290a 0a20 2020 2073  '].read()..    s
-000084c0: 335f 7572 6c20 3d20 5333 5061 7468 2873  3_url = S3Path(s
-000084d0: 335f 7572 6c29 0a20 2020 2069 6620 666f  3_url).    if fo
-000084e0: 6c6c 6f77 6c69 6e6b 733a 0a20 2020 2020  llowlinks:.     
-000084f0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00008500: 2020 2020 7333 5f75 726c 203d 2073 335f      s3_url = s3_
-00008510: 7572 6c2e 7265 6164 6c69 6e6b 2829 0a20  url.readlink(). 
-00008520: 2020 2020 2020 2065 7863 6570 7420 5333         except S3
-00008530: 4e6f 7441 4c69 6e6b 4572 726f 723a 0a20  NotALinkError:. 
-00008540: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00008550: 0a20 2020 2062 7563 6b65 742c 206b 6579  .    bucket, key
-00008560: 203d 2070 6172 7365 5f73 335f 7572 6c28   = parse_s3_url(
-00008570: 7333 5f75 726c 2e70 6174 685f 7769 7468  s3_url.path_with
-00008580: 5f70 726f 746f 636f 6c29 0a20 2020 2069  _protocol).    i
-00008590: 6620 6e6f 7420 6275 636b 6574 3a0a 2020  f not bucket:.  
-000085a0: 2020 2020 2020 7261 6973 6520 5333 4275        raise S3Bu
-000085b0: 636b 6574 4e6f 7446 6f75 6e64 4572 726f  cketNotFoundErro
-000085c0: 7228 2745 6d70 7479 2062 7563 6b65 7420  r('Empty bucket 
-000085d0: 6e61 6d65 3a20 2572 2720 2520 7333 5f75  name: %r' % s3_u
-000085e0: 726c 290a 2020 2020 6966 206e 6f74 206b  rl).    if not k
-000085f0: 6579 206f 7220 6b65 792e 656e 6473 7769  ey or key.endswi
-00008600: 7468 2827 2f27 293a 0a20 2020 2020 2020  th('/'):.       
-00008610: 2072 6169 7365 2053 3349 7341 4469 7265   raise S3IsADire
-00008620: 6374 6f72 7945 7272 6f72 2827 4973 2061  ctoryError('Is a
-00008630: 2064 6972 6563 746f 7279 3a20 2572 2720   directory: %r' 
-00008640: 2520 7333 5f75 726c 290a 0a20 2020 2073  % s3_url)..    s
-00008650: 7461 7274 2c20 7374 6f70 203d 2067 6574  tart, stop = get
-00008660: 5f63 6f6e 7465 6e74 5f6f 6666 7365 7428  _content_offset(
-00008670: 0a20 2020 2020 2020 2073 7461 7274 2c20  .        start, 
-00008680: 7374 6f70 2c20 7333 5f75 726c 2e67 6574  stop, s3_url.get
-00008690: 7369 7a65 2866 6f6c 6c6f 775f 7379 6d6c  size(follow_syml
-000086a0: 696e 6b73 3d46 616c 7365 2929 0a20 2020  inks=False)).   
-000086b0: 2069 6620 7374 6172 7420 3d3d 2030 2061   if start == 0 a
-000086c0: 6e64 2073 746f 7020 3d3d 2030 3a0a 2020  nd stop == 0:.  
-000086d0: 2020 2020 2020 7265 7475 726e 2062 2727        return b''
-000086e0: 0a20 2020 2072 616e 6765 5f73 7472 203d  .    range_str =
-000086f0: 2027 6279 7465 733d 2564 2d25 6427 2025   'bytes=%d-%d' %
-00008700: 2028 7374 6172 742c 2073 746f 7020 2d20   (start, stop - 
-00008710: 3129 0a0a 2020 2020 636c 6965 6e74 203d  1)..    client =
-00008720: 2067 6574 5f73 335f 636c 6965 6e74 2870   get_s3_client(p
-00008730: 726f 6669 6c65 5f6e 616d 653d 7333 5f75  rofile_name=s3_u
-00008740: 726c 2e5f 7072 6f66 696c 655f 6e61 6d65  rl._profile_name
-00008750: 290a 2020 2020 7769 7468 2072 6169 7365  ).    with raise
-00008760: 5f73 335f 6572 726f 7228 7333 5f75 726c  _s3_error(s3_url
-00008770: 2e70 6174 6829 3a0a 2020 2020 2020 2020  .path):.        
-00008780: 7265 7475 726e 2070 6174 6368 5f6d 6574  return patch_met
-00008790: 686f 6428 0a20 2020 2020 2020 2020 2020  hod(.           
-000087a0: 205f 6765 745f 6f62 6a65 6374 2c0a 2020   _get_object,.  
-000087b0: 2020 2020 2020 2020 2020 6d61 785f 7265            max_re
-000087c0: 7472 6965 733d 6d61 785f 7265 7472 6965  tries=max_retrie
-000087d0: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
-000087e0: 686f 756c 645f 7265 7472 793d 7333 5f73  hould_retry=s3_s
-000087f0: 686f 756c 645f 7265 7472 792c 0a20 2020  hould_retry,.   
-00008800: 2020 2020 2029 2863 6c69 656e 742c 2062       )(client, b
-00008810: 7563 6b65 742c 206b 6579 2c20 7261 6e67  ucket, key, rang
-00008820: 655f 7374 7229 0a0a 0a64 6566 2073 335f  e_str)...def s3_
-00008830: 7265 6164 6c69 6e6b 2870 6174 6829 202d  readlink(path) -
-00008840: 3e20 7374 723a 0a20 2020 2027 2727 0a20  > str:.    '''. 
-00008850: 2020 2052 6574 7572 6e20 6120 7374 7269     Return a stri
-00008860: 6e67 2072 6570 7265 7365 6e74 696e 6720  ng representing 
-00008870: 7468 6520 7061 7468 2074 6f20 7768 6963  the path to whic
-00008880: 6820 7468 6520 7379 6d62 6f6c 6963 206c  h the symbolic l
-00008890: 696e 6b20 706f 696e 7473 2e0a 0a20 2020  ink points...   
-000088a0: 203a 7265 7475 726e 733a 2052 6574 7572   :returns: Retur
-000088b0: 6e20 6120 7374 7269 6e67 2072 6570 7265  n a string repre
-000088c0: 7365 6e74 696e 6720 7468 6520 7061 7468  senting the path
-000088d0: 2074 6f20 7768 6963 6820 7468 6520 7379   to which the sy
-000088e0: 6d62 6f6c 6963 206c 696e 6b20 706f 696e  mbolic link poin
-000088f0: 7473 2e0a 2020 2020 3a72 6169 7365 733a  ts..    :raises:
-00008900: 2053 334e 616d 6554 6f6f 4c6f 6e67 4572   S3NameTooLongEr
-00008910: 726f 722c 2053 3342 7563 6b65 744e 6f74  ror, S3BucketNot
-00008920: 466f 756e 6445 7272 6f72 2c20 5333 4973  FoundError, S3Is
-00008930: 4144 6972 6563 746f 7279 4572 726f 722c  ADirectoryError,
-00008940: 2053 334e 6f74 414c 696e 6b45 7272 6f72   S3NotALinkError
-00008950: 0a20 2020 2027 2727 0a20 2020 2072 6574  .    '''.    ret
-00008960: 7572 6e20 5333 5061 7468 2870 6174 6829  urn S3Path(path)
-00008970: 2e72 6561 646c 696e 6b28 292e 7061 7468  .readlink().path
-00008980: 5f77 6974 685f 7072 6f74 6f63 6f6c 0a0a  _with_protocol..
-00008990: 0a64 6566 2073 335f 7265 6e61 6d65 2873  .def s3_rename(s
-000089a0: 7263 5f75 726c 3a20 5061 7468 4c69 6b65  rc_url: PathLike
-000089b0: 2c20 6473 745f 7572 6c3a 2050 6174 684c  , dst_url: PathL
-000089c0: 696b 6529 3a0a 2020 2020 2727 270a 2020  ike):.    '''.  
-000089d0: 2020 4d6f 7665 2073 3320 6669 6c65 2070    Move s3 file p
-000089e0: 6174 6820 6672 6f6d 2073 7263 5f75 726c  ath from src_url
-000089f0: 2074 6f20 6473 745f 7572 6c0a 0a20 2020   to dst_url..   
-00008a00: 203a 7061 7261 6d20 6473 745f 7572 6c3a   :param dst_url:
-00008a10: 2047 6976 656e 2064 6573 7469 6e61 7469   Given destinati
-00008a20: 6f6e 2070 6174 680a 2020 2020 2727 270a  on path.    '''.
-00008a30: 2020 2020 7372 635f 7061 7468 5f69 6e73      src_path_ins
-00008a40: 203d 2053 3350 6174 6828 7372 635f 7572   = S3Path(src_ur
-00008a50: 6c29 0a20 2020 2069 6620 7372 635f 7061  l).    if src_pa
-00008a60: 7468 5f69 6e73 2e69 735f 6669 6c65 2829  th_ins.is_file()
-00008a70: 3a0a 2020 2020 2020 2020 7372 635f 7061  :.        src_pa
-00008a80: 7468 5f69 6e73 2e63 6f70 7928 6473 745f  th_ins.copy(dst_
-00008a90: 7572 6c29 0a20 2020 2065 6c73 653a 0a20  url).    else:. 
-00008aa0: 2020 2020 2020 2073 7263 5f70 6174 685f         src_path_
-00008ab0: 696e 732e 7379 6e63 2864 7374 5f75 726c  ins.sync(dst_url
-00008ac0: 290a 2020 2020 7372 635f 7061 7468 5f69  ).    src_path_i
-00008ad0: 6e73 2e72 656d 6f76 6528 290a 0a0a 636c  ns.remove()...cl
-00008ae0: 6173 7320 5333 4361 6368 6572 2846 696c  ass S3Cacher(Fil
-00008af0: 6543 6163 6865 7229 3a0a 2020 2020 6361  eCacher):.    ca
-00008b00: 6368 655f 7061 7468 203d 204e 6f6e 650a  che_path = None.
-00008b10: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00008b20: 5f28 0a20 2020 2020 2020 2020 2020 2073  _(.            s
-00008b30: 656c 662c 2070 6174 683a 2073 7472 2c20  elf, path: str, 
-00008b40: 6361 6368 655f 7061 7468 3a20 4f70 7469  cache_path: Opti
-00008b50: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00008b60: 2c20 6d6f 6465 3a20 7374 7220 3d20 2772  , mode: str = 'r
-00008b70: 2729 3a0a 2020 2020 2020 2020 6966 206d  '):.        if m
-00008b80: 6f64 6520 6e6f 7420 696e 2028 2772 272c  ode not in ('r',
-00008b90: 2027 7727 2c20 2761 2729 3a0a 2020 2020   'w', 'a'):.    
-00008ba0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00008bb0: 6c75 6545 7272 6f72 2827 756e 6163 6365  lueError('unacce
-00008bc0: 7074 6162 6c65 206d 6f64 653a 2025 7227  ptable mode: %r'
-00008bd0: 2025 206d 6f64 6529 0a20 2020 2020 2020   % mode).       
-00008be0: 2069 6620 6d6f 6465 2069 6e20 2827 7227   if mode in ('r'
-00008bf0: 2c20 2761 2729 3a0a 2020 2020 2020 2020  , 'a'):.        
-00008c00: 2020 2020 6966 2063 6163 6865 5f70 6174      if cache_pat
-00008c10: 6820 6973 204e 6f6e 653a 0a20 2020 2020  h is None:.     
-00008c20: 2020 2020 2020 2020 2020 2063 6163 6865             cache
-00008c30: 5f70 6174 6820 3d20 6765 6e65 7261 7465  _path = generate
-00008c40: 5f63 6163 6865 5f70 6174 6828 7061 7468  _cache_path(path
-00008c50: 290a 2020 2020 2020 2020 2020 2020 7333  ).            s3
-00008c60: 5f64 6f77 6e6c 6f61 6428 7061 7468 2c20  _download(path, 
-00008c70: 6361 6368 655f 7061 7468 290a 2020 2020  cache_path).    
-00008c80: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
-00008c90: 7061 7468 0a20 2020 2020 2020 2073 656c  path.        sel
-00008ca0: 662e 6d6f 6465 203d 206d 6f64 650a 2020  f.mode = mode.  
-00008cb0: 2020 2020 2020 7365 6c66 2e63 6163 6865        self.cache
-00008cc0: 5f70 6174 6820 3d20 6361 6368 655f 7061  _path = cache_pa
-00008cd0: 7468 0a0a 2020 2020 6465 6620 5f63 6c6f  th..    def _clo
-00008ce0: 7365 2873 656c 6629 3a0a 2020 2020 2020  se(self):.      
-00008cf0: 2020 6966 2073 656c 662e 6361 6368 655f    if self.cache_
-00008d00: 7061 7468 2069 7320 6e6f 7420 4e6f 6e65  path is not None
-00008d10: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
-00008d20: 2020 206f 732e 7061 7468 2e65 7869 7374     os.path.exist
-00008d30: 7328 7365 6c66 2e63 6163 6865 5f70 6174  s(self.cache_pat
-00008d40: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
-00008d50: 6966 2073 656c 662e 6d6f 6465 2069 6e20  if self.mode in 
-00008d60: 2827 7727 2c20 2761 2729 3a0a 2020 2020  ('w', 'a'):.    
-00008d70: 2020 2020 2020 2020 2020 2020 7333 5f75              s3_u
-00008d80: 706c 6f61 6428 7365 6c66 2e63 6163 6865  pload(self.cache
-00008d90: 5f70 6174 682c 2073 656c 662e 6e61 6d65  _path, self.name
-00008da0: 290a 2020 2020 2020 2020 2020 2020 6f73  ).            os
-00008db0: 2e75 6e6c 696e 6b28 7365 6c66 2e63 6163  .unlink(self.cac
-00008dc0: 6865 5f70 6174 6829 0a0a 0a64 6566 2073  he_path)...def s
-00008dd0: 335f 676c 6f62 280a 2020 2020 2020 2020  3_glob(.        
-00008de0: 7061 7468 3a20 5061 7468 4c69 6b65 2c0a  path: PathLike,.
-00008df0: 2020 2020 2020 2020 7265 6375 7273 6976          recursiv
-00008e00: 653a 2062 6f6f 6c20 3d20 5472 7565 2c0a  e: bool = True,.
-00008e10: 2020 2020 2020 2020 6d69 7373 696e 675f          missing_
-00008e20: 6f6b 3a20 626f 6f6c 203d 2054 7275 652c  ok: bool = True,
-00008e30: 0a20 2020 2020 2020 2066 6f6c 6c6f 776c  .        followl
-00008e40: 696e 6b73 3a20 626f 6f6c 203d 2046 616c  inks: bool = Fal
-00008e50: 7365 2c0a 2920 2d3e 204c 6973 745b 7374  se,.) -> List[st
-00008e60: 725d 3a0a 2020 2020 2727 2752 6574 7572  r]:.    '''Retur
-00008e70: 6e20 7333 2070 6174 6820 6c69 7374 2069  n s3 path list i
-00008e80: 6e20 6173 6365 6e64 696e 6720 616c 7068  n ascending alph
-00008e90: 6162 6574 6963 616c 206f 7264 6572 2c20  abetical order, 
-00008ea0: 696e 2077 6869 6368 2070 6174 6820 6d61  in which path ma
-00008eb0: 7463 6865 7320 676c 6f62 2070 6174 7465  tches glob patte
-00008ec0: 726e 0a20 2020 204e 6f74 6573 3a20 4f6e  rn.    Notes: On
-00008ed0: 6c79 2067 6c6f 6220 696e 2062 7563 6b65  ly glob in bucke
-00008ee0: 742e 2049 6620 7472 7969 6e67 2074 6f20  t. If trying to 
-00008ef0: 6d61 7463 6820 6275 636b 6574 2077 6974  match bucket wit
-00008f00: 6820 7769 6c64 6361 7264 2063 6861 7261  h wildcard chara
-00008f10: 6374 6572 732c 2072 6169 7365 2055 6e73  cters, raise Uns
-00008f20: 7570 706f 7274 6564 4572 726f 720a 0a20  upportedError.. 
-00008f30: 2020 203a 7061 7261 6d20 7265 6375 7273     :param recurs
-00008f40: 6976 653a 2049 6620 4661 6c73 652c 2060  ive: If False, `
-00008f50: 2a2a 6020 7769 6c6c 206e 6f74 2073 6561  **` will not sea
-00008f60: 7263 6820 6469 7265 6374 6f72 7920 7265  rch directory re
-00008f70: 6375 7273 6976 656c 790a 2020 2020 3a70  cursively.    :p
-00008f80: 6172 616d 206d 6973 7369 6e67 5f6f 6b3a  aram missing_ok:
-00008f90: 2049 6620 4661 6c73 6520 616e 6420 7461   If False and ta
-00008fa0: 7267 6574 2070 6174 6820 646f 6573 6e27  rget path doesn'
-00008fb0: 7420 6d61 7463 6820 616e 7920 6669 6c65  t match any file
-00008fc0: 2c20 7261 6973 6520 4669 6c65 4e6f 7446  , raise FileNotF
-00008fd0: 6f75 6e64 4572 726f 720a 2020 2020 3a72  oundError.    :r
-00008fe0: 6169 7365 733a 2055 6e73 7570 706f 7274  aises: Unsupport
-00008ff0: 6564 4572 726f 722c 2077 6865 6e20 6275  edError, when bu
-00009000: 636b 6574 2070 6172 7420 636f 6e74 6169  cket part contai
-00009010: 6e73 2077 696c 6463 6172 6420 6368 6172  ns wildcard char
-00009020: 6163 7465 7273 0a20 2020 203a 7265 7475  acters.    :retu
-00009030: 726e 733a 2041 206c 6973 7420 636f 6e74  rns: A list cont
-00009040: 6169 6e73 2070 6174 6873 206d 6174 6368  ains paths match
-00009050: 2060 7333 5f70 6174 686e 616d 6560 0a20   `s3_pathname`. 
-00009060: 2020 2027 2727 0a20 2020 2072 6574 7572     '''.    retur
-00009070: 6e20 6c69 7374 280a 2020 2020 2020 2020  n list(.        
-00009080: 7333 5f69 676c 6f62 280a 2020 2020 2020  s3_iglob(.      
-00009090: 2020 2020 2020 7061 7468 3d70 6174 682c        path=path,
-000090a0: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
-000090b0: 7572 7369 7665 3d72 6563 7572 7369 7665  ursive=recursive
-000090c0: 2c0a 2020 2020 2020 2020 2020 2020 6d69  ,.            mi
-000090d0: 7373 696e 675f 6f6b 3d6d 6973 7369 6e67  ssing_ok=missing
-000090e0: 5f6f 6b2c 0a20 2020 2020 2020 2020 2020  _ok,.           
-000090f0: 2066 6f6c 6c6f 776c 696e 6b73 3d66 6f6c   followlinks=fol
-00009100: 6c6f 776c 696e 6b73 2929 0a0a 0a64 6566  lowlinks))...def
-00009110: 2073 335f 676c 6f62 5f73 7461 7428 0a20   s3_glob_stat(. 
-00009120: 2020 2020 2020 2070 6174 683a 2050 6174         path: Pat
-00009130: 684c 696b 652c 0a20 2020 2020 2020 2072  hLike,.        r
-00009140: 6563 7572 7369 7665 3a20 626f 6f6c 203d  ecursive: bool =
-00009150: 2054 7275 652c 0a20 2020 2020 2020 206d   True,.        m
-00009160: 6973 7369 6e67 5f6f 6b3a 2062 6f6f 6c20  issing_ok: bool 
-00009170: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
-00009180: 666f 6c6c 6f77 6c69 6e6b 733a 2062 6f6f  followlinks: boo
-00009190: 6c20 3d20 4661 6c73 6529 202d 3e20 4974  l = False) -> It
-000091a0: 6572 6174 6f72 5b46 696c 6545 6e74 7279  erator[FileEntry
-000091b0: 5d3a 0a20 2020 2027 2727 5265 7475 726e  ]:.    '''Return
-000091c0: 2061 2067 656e 6572 6174 6f72 2063 6f6e   a generator con
-000091d0: 7461 696e 7320 7475 706c 6573 206f 6620  tains tuples of 
-000091e0: 7061 7468 2061 6e64 2066 696c 6520 7374  path and file st
-000091f0: 6174 2c20 696e 2061 7363 656e 6469 6e67  at, in ascending
-00009200: 2061 6c70 6861 6265 7469 6361 6c20 6f72   alphabetical or
-00009210: 6465 722c 2069 6e20 7768 6963 6820 7061  der, in which pa
-00009220: 7468 206d 6174 6368 6573 2067 6c6f 6220  th matches glob 
-00009230: 7061 7474 6572 6e0a 2020 2020 4e6f 7465  pattern.    Note
-00009240: 733a 204f 6e6c 7920 676c 6f62 2069 6e20  s: Only glob in 
-00009250: 6275 636b 6574 2e20 4966 2074 7279 696e  bucket. If tryin
-00009260: 6720 746f 206d 6174 6368 2062 7563 6b65  g to match bucke
-00009270: 7420 7769 7468 2077 696c 6463 6172 6420  t with wildcard 
-00009280: 6368 6172 6163 7465 7273 2c20 7261 6973  characters, rais
-00009290: 6520 556e 7375 7070 6f72 7465 6445 7272  e UnsupportedErr
-000092a0: 6f72 0a0a 2020 2020 3a70 6172 616d 2072  or..    :param r
-000092b0: 6563 7572 7369 7665 3a20 4966 2046 616c  ecursive: If Fal
-000092c0: 7365 2c20 602a 2a60 2077 696c 6c20 6e6f  se, `**` will no
-000092d0: 7420 7365 6172 6368 2064 6972 6563 746f  t search directo
-000092e0: 7279 2072 6563 7572 7369 7665 6c79 0a20  ry recursively. 
-000092f0: 2020 203a 7061 7261 6d20 6d69 7373 696e     :param missin
-00009300: 675f 6f6b 3a20 4966 2046 616c 7365 2061  g_ok: If False a
-00009310: 6e64 2074 6172 6765 7420 7061 7468 2064  nd target path d
-00009320: 6f65 736e 2774 206d 6174 6368 2061 6e79  oesn't match any
-00009330: 2066 696c 652c 2072 6169 7365 2046 696c   file, raise Fil
-00009340: 654e 6f74 466f 756e 6445 7272 6f72 0a20  eNotFoundError. 
-00009350: 2020 203a 7261 6973 6573 3a20 556e 7375     :raises: Unsu
-00009360: 7070 6f72 7465 6445 7272 6f72 2c20 7768  pportedError, wh
-00009370: 656e 2062 7563 6b65 7420 7061 7274 2063  en bucket part c
-00009380: 6f6e 7461 696e 7320 7769 6c64 6361 7264  ontains wildcard
-00009390: 2063 6861 7261 6374 6572 730a 2020 2020   characters.    
-000093a0: 3a72 6574 7572 6e73 3a20 4120 6765 6e65  :returns: A gene
-000093b0: 7261 746f 7220 636f 6e74 6169 6e73 2074  rator contains t
-000093c0: 7570 6c65 7320 6f66 2070 6174 6820 616e  uples of path an
-000093d0: 6420 6669 6c65 2073 7461 742c 2069 6e20  d file stat, in 
-000093e0: 7768 6963 6820 7061 7468 7320 6d61 7463  which paths matc
-000093f0: 6820 6073 335f 7061 7468 6e61 6d65 600a  h `s3_pathname`.
-00009400: 2020 2020 2727 270a 2020 2020 7265 7475      '''.    retu
-00009410: 726e 2053 3350 6174 6828 7061 7468 292e  rn S3Path(path).
-00009420: 676c 6f62 5f73 7461 7428 0a20 2020 2020  glob_stat(.     
-00009430: 2020 2070 6174 7465 726e 3d22 222c 0a20     pattern="",. 
-00009440: 2020 2020 2020 2072 6563 7572 7369 7665         recursive
-00009450: 3d72 6563 7572 7369 7665 2c0a 2020 2020  =recursive,.    
-00009460: 2020 2020 6d69 7373 696e 675f 6f6b 3d6d      missing_ok=m
-00009470: 6973 7369 6e67 5f6f 6b2c 0a20 2020 2020  issing_ok,.     
-00009480: 2020 2066 6f6c 6c6f 776c 696e 6b73 3d66     followlinks=f
-00009490: 6f6c 6c6f 776c 696e 6b73 290a 0a0a 6465  ollowlinks)...de
-000094a0: 6620 7333 5f69 676c 6f62 280a 2020 2020  f s3_iglob(.    
-000094b0: 2020 2020 7061 7468 3a20 5061 7468 4c69      path: PathLi
-000094c0: 6b65 2c0a 2020 2020 2020 2020 7265 6375  ke,.        recu
-000094d0: 7273 6976 653a 2062 6f6f 6c20 3d20 5472  rsive: bool = Tr
-000094e0: 7565 2c0a 2020 2020 2020 2020 6d69 7373  ue,.        miss
-000094f0: 696e 675f 6f6b 3a20 626f 6f6c 203d 2054  ing_ok: bool = T
-00009500: 7275 652c 0a20 2020 2020 2020 2066 6f6c  rue,.        fol
-00009510: 6c6f 776c 696e 6b73 3a20 626f 6f6c 203d  lowlinks: bool =
-00009520: 2046 616c 7365 2c0a 2920 2d3e 2049 7465   False,.) -> Ite
-00009530: 7261 746f 725b 7374 725d 3a0a 2020 2020  rator[str]:.    
-00009540: 2727 2752 6574 7572 6e20 7333 2070 6174  '''Return s3 pat
-00009550: 6820 6974 6572 6174 6f72 2069 6e20 6173  h iterator in as
-00009560: 6365 6e64 696e 6720 616c 7068 6162 6574  cending alphabet
-00009570: 6963 616c 206f 7264 6572 2c20 696e 2077  ical order, in w
-00009580: 6869 6368 2070 6174 6820 6d61 7463 6865  hich path matche
-00009590: 7320 676c 6f62 2070 6174 7465 726e 0a20  s glob pattern. 
-000095a0: 2020 204e 6f74 6573 3a20 4f6e 6c79 2067     Notes: Only g
-000095b0: 6c6f 6220 696e 2062 7563 6b65 742e 2049  lob in bucket. I
-000095c0: 6620 7472 7969 6e67 2074 6f20 6d61 7463  f trying to matc
-000095d0: 6820 6275 636b 6574 2077 6974 6820 7769  h bucket with wi
-000095e0: 6c64 6361 7264 2063 6861 7261 6374 6572  ldcard character
-000095f0: 732c 2072 6169 7365 2055 6e73 7570 706f  s, raise Unsuppo
-00009600: 7274 6564 4572 726f 720a 0a20 2020 203a  rtedError..    :
-00009610: 7061 7261 6d20 7265 6375 7273 6976 653a  param recursive:
-00009620: 2049 6620 4661 6c73 652c 2060 2a2a 6020   If False, `**` 
-00009630: 7769 6c6c 206e 6f74 2073 6561 7263 6820  will not search 
-00009640: 6469 7265 6374 6f72 7920 7265 6375 7273  directory recurs
-00009650: 6976 656c 790a 2020 2020 3a70 6172 616d  ively.    :param
-00009660: 206d 6973 7369 6e67 5f6f 6b3a 2049 6620   missing_ok: If 
-00009670: 4661 6c73 6520 616e 6420 7461 7267 6574  False and target
-00009680: 2070 6174 6820 646f 6573 6e27 7420 6d61   path doesn't ma
-00009690: 7463 6820 616e 7920 6669 6c65 2c20 7261  tch any file, ra
-000096a0: 6973 6520 4669 6c65 4e6f 7446 6f75 6e64  ise FileNotFound
-000096b0: 4572 726f 720a 2020 2020 3a72 6169 7365  Error.    :raise
-000096c0: 733a 2055 6e73 7570 706f 7274 6564 4572  s: UnsupportedEr
-000096d0: 726f 722c 2077 6865 6e20 6275 636b 6574  ror, when bucket
-000096e0: 2070 6172 7420 636f 6e74 6169 6e73 2077   part contains w
-000096f0: 696c 6463 6172 6420 6368 6172 6163 7465  ildcard characte
-00009700: 7273 0a20 2020 203a 7265 7475 726e 733a  rs.    :returns:
-00009710: 2041 6e20 6974 6572 6174 6f72 2063 6f6e   An iterator con
-00009720: 7461 696e 7320 7061 7468 7320 6d61 7463  tains paths matc
-00009730: 6820 6073 335f 7061 7468 6e61 6d65 600a  h `s3_pathname`.
-00009740: 2020 2020 2727 270a 2020 2020 666f 7220      '''.    for 
-00009750: 7061 7468 5f6f 626a 2069 6e20 5333 5061  path_obj in S3Pa
-00009760: 7468 2870 6174 6829 2e69 676c 6f62 2870  th(path).iglob(p
-00009770: 6174 7465 726e 3d22 222c 2072 6563 7572  attern="", recur
-00009780: 7369 7665 3d72 6563 7572 7369 7665 2c0a  sive=recursive,.
-00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097b0: 2020 2020 2020 206d 6973 7369 6e67 5f6f         missing_o
-000097c0: 6b3d 6d69 7373 696e 675f 6f6b 2c0a 2020  k=missing_ok,.  
-000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097f0: 2020 2020 2066 6f6c 6c6f 776c 696e 6b73       followlinks
-00009800: 3d66 6f6c 6c6f 776c 696e 6b73 293a 0a20  =followlinks):. 
-00009810: 2020 2020 2020 2079 6965 6c64 2070 6174         yield pat
-00009820: 685f 6f62 6a2e 7061 7468 5f77 6974 685f  h_obj.path_with_
-00009830: 7072 6f74 6f63 6f6c 0a0a 0a64 6566 2073  protocol...def s
-00009840: 335f 6d61 6b65 6469 7273 2870 6174 683a  3_makedirs(path:
-00009850: 2050 6174 684c 696b 652c 2065 7869 7374   PathLike, exist
-00009860: 5f6f 6b3a 2062 6f6f 6c20 3d20 4661 6c73  _ok: bool = Fals
-00009870: 6529 3a0a 2020 2020 2727 270a 2020 2020  e):.    '''.    
-00009880: 4372 6561 7465 2061 6e20 7333 2064 6972  Create an s3 dir
-00009890: 6563 746f 7279 2e0a 2020 2020 5075 7265  ectory..    Pure
-000098a0: 6c79 2063 7265 6174 696e 6720 6469 7265  ly creating dire
-000098b0: 6374 6f72 7920 6973 2069 6e76 616c 6964  ctory is invalid
-000098c0: 2062 6563 6175 7365 2069 7427 7320 756e   because it's un
-000098d0: 6176 6169 6c61 626c 6520 6f6e 204f 5353  available on OSS
-000098e0: 2e0a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
-000098f0: 696f 6e20 6973 2074 6f20 7465 7374 2074  ion is to test t
-00009900: 6865 2074 6172 6765 7420 6275 636b 6574  he target bucket
-00009910: 2068 6176 6520 5752 4954 4520 6163 6365   have WRITE acce
-00009920: 7373 2e0a 0a20 2020 203a 7061 7261 6d20  ss...    :param 
-00009930: 7061 7468 3a20 4769 7665 6e20 7061 7468  path: Given path
-00009940: 0a20 2020 203a 7061 7261 6d20 6578 6973  .    :param exis
-00009950: 745f 6f6b 3a20 4966 2046 616c 7365 2061  t_ok: If False a
-00009960: 6e64 2074 6172 6765 7420 6469 7265 6374  nd target direct
-00009970: 6f72 7920 6578 6973 7473 2c20 7261 6973  ory exists, rais
-00009980: 6520 5333 4669 6c65 4578 6973 7473 4572  e S3FileExistsEr
-00009990: 726f 720a 2020 2020 3a72 6169 7365 733a  ror.    :raises:
-000099a0: 2053 3342 7563 6b65 744e 6f74 466f 756e   S3BucketNotFoun
-000099b0: 6445 7272 6f72 2c20 5333 4669 6c65 4578  dError, S3FileEx
-000099c0: 6973 7473 4572 726f 720a 2020 2020 2727  istsError.    ''
-000099d0: 270a 2020 2020 7265 7475 726e 2053 3350  '.    return S3P
-000099e0: 6174 6828 7061 7468 292e 6d6b 6469 7228  ath(path).mkdir(
-000099f0: 7061 7265 6e74 733d 5472 7565 2c20 6578  parents=True, ex
-00009a00: 6973 745f 6f6b 3d65 7869 7374 5f6f 6b29  ist_ok=exist_ok)
-00009a10: 0a0a 0a64 6566 205f 6772 6f75 705f 7372  ...def _group_sr
-00009a20: 635f 7061 7468 735f 6279 5f62 6c6f 636b  c_paths_by_block
-00009a30: 280a 2020 2020 2020 2020 7372 635f 7061  (.        src_pa
-00009a40: 7468 733a 204c 6973 745b 5061 7468 4c69  ths: List[PathLi
-00009a50: 6b65 5d2c 2062 6c6f 636b 5f73 697a 653a  ke], block_size:
-00009a60: 2069 6e74 203d 2044 4546 4155 4c54 5f42   int = DEFAULT_B
-00009a70: 4c4f 434b 5f53 495a 450a 2920 2d3e 204c  LOCK_SIZE.) -> L
-00009a80: 6973 745b 4c69 7374 5b54 7570 6c65 5b50  ist[List[Tuple[P
-00009a90: 6174 684c 696b 652c 204f 7074 696f 6e61  athLike, Optiona
-00009aa0: 6c5b 7374 725d 5d5d 5d3a 0a20 2020 2067  l[str]]]]:.    g
-00009ab0: 726f 7570 7320 3d20 5b5d 0a20 2020 2063  roups = [].    c
-00009ac0: 7572 7265 6e74 5f67 726f 7570 2c20 6375  urrent_group, cu
-00009ad0: 7272 656e 745f 6772 6f75 705f 7369 7a65  rrent_group_size
-00009ae0: 203d 205b 5d2c 2030 0a20 2020 2066 6f72   = [], 0.    for
-00009af0: 2073 7263 5f70 6174 6820 696e 2073 7263   src_path in src
-00009b00: 5f70 6174 6873 3a0a 2020 2020 2020 2020  _paths:.        
-00009b10: 6375 7272 656e 745f 6669 6c65 5f73 697a  current_file_siz
-00009b20: 6520 3d20 5333 5061 7468 2873 7263 5f70  e = S3Path(src_p
-00009b30: 6174 6829 2e73 7461 7428 292e 7369 7a65  ath).stat().size
-00009b40: 0a20 2020 2020 2020 2069 6620 6375 7272  .        if curr
-00009b50: 656e 745f 6669 6c65 5f73 697a 6520 3d3d  ent_file_size ==
-00009b60: 2030 3a20 2023 2070 7261 676d 613a 206e   0:  # pragma: n
-00009b70: 6f20 636f 7665 720a 2020 2020 2020 2020  o cover.        
-00009b80: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
-00009b90: 2020 2020 2020 6966 2063 7572 7265 6e74        if current
-00009ba0: 5f66 696c 655f 7369 7a65 203e 3d20 626c  _file_size >= bl
-00009bb0: 6f63 6b5f 7369 7a65 3a0a 2020 2020 2020  ock_size:.      
-00009bc0: 2020 2020 2020 6966 206c 656e 2867 726f        if len(gro
-00009bd0: 7570 7329 203d 3d20 303a 0a20 2020 2020  ups) == 0:.     
-00009be0: 2020 2020 2020 2020 2020 2069 6620 6375             if cu
-00009bf0: 7272 656e 745f 6772 6f75 705f 7369 7a65  rrent_group_size
-00009c00: 202b 2063 7572 7265 6e74 5f66 696c 655f   + current_file_
-00009c10: 7369 7a65 203e 2032 202a 2062 6c6f 636b  size > 2 * block
-00009c20: 5f73 697a 653a 0a20 2020 2020 2020 2020  _size:.         
-00009c30: 2020 2020 2020 2020 2020 2067 726f 7570             group
-00009c40: 5f6c 6163 6b5f 7369 7a65 203d 2062 6c6f  _lack_size = blo
-00009c50: 636b 5f73 697a 6520 2d20 6375 7272 656e  ck_size - curren
-00009c60: 745f 6772 6f75 705f 7369 7a65 0a20 2020  t_group_size.   
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2063 7572 7265 6e74 5f67 726f 7570 2e61   current_group.a
-00009c90: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-00009ca0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00009cb0: 7372 635f 7061 7468 2c20 6627 6279 7465  src_path, f'byte
-00009cc0: 733d 302d 7b67 726f 7570 5f6c 6163 6b5f  s=0-{group_lack_
-00009cd0: 7369 7a65 2d31 7d27 2929 0a20 2020 2020  size-1}')).     
-00009ce0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00009cf0: 726f 7570 732e 6578 7465 6e64 280a 2020  roups.extend(.  
-00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d10: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d30: 2020 2020 6375 7272 656e 745f 6772 6f75      current_grou
-00009d40: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
-00009d50: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00009d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009da0: 2020 2020 2020 2073 7263 5f70 6174 682c         src_path,
-00009db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2020 2020 2066 2762 7974 6573 3d7b 6772       f'bytes={gr
-00009de0: 6f75 705f 6c61 636b 5f73 697a 657d 2d7b  oup_lack_size}-{
-00009df0: 6375 7272 656e 745f 6669 6c65 5f73 697a  current_file_siz
-00009e00: 652d 317d 270a 2020 2020 2020 2020 2020  e-1}'.          
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e40: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00009e50: 2020 2020 2020 2020 2020 2020 2020 5d29                ])
-00009e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009e80: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00009e90: 6e74 5f67 726f 7570 2e61 7070 656e 6428  nt_group.append(
-00009ea0: 2873 7263 5f70 6174 682c 204e 6f6e 6529  (src_path, None)
-00009eb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009ec0: 2020 2020 2020 6772 6f75 7073 2e61 7070        groups.app
-00009ed0: 656e 6428 6375 7272 656e 745f 6772 6f75  end(current_grou
-00009ee0: 7029 0a20 2020 2020 2020 2020 2020 2065  p).            e
-00009ef0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009f00: 2020 2020 2067 726f 7570 735b 2d31 5d2e       groups[-1].
-00009f10: 6578 7465 6e64 2863 7572 7265 6e74 5f67  extend(current_g
-00009f20: 726f 7570 290a 2020 2020 2020 2020 2020  roup).          
-00009f30: 2020 2020 2020 6772 6f75 7073 2e61 7070        groups.app
-00009f40: 656e 6428 5b28 7372 635f 7061 7468 2c20  end([(src_path, 
-00009f50: 4e6f 6e65 295d 290a 2020 2020 2020 2020  None)]).        
-00009f60: 2020 2020 6375 7272 656e 745f 6772 6f75      current_grou
-00009f70: 702c 2063 7572 7265 6e74 5f67 726f 7570  p, current_group
-00009f80: 5f73 697a 6520 3d20 5b5d 2c20 300a 2020  _size = [], 0.  
-00009f90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009fa0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00009fb0: 6772 6f75 702e 6170 7065 6e64 2828 7372  group.append((sr
-00009fc0: 635f 7061 7468 2c20 4e6f 6e65 2929 0a20  c_path, None)). 
-00009fd0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00009fe0: 6e74 5f67 726f 7570 5f73 697a 6520 2b3d  nt_group_size +=
-00009ff0: 2063 7572 7265 6e74 5f66 696c 655f 7369   current_file_si
-0000a000: 7a65 0a20 2020 2020 2020 2020 2020 2069  ze.            i
-0000a010: 6620 6375 7272 656e 745f 6772 6f75 705f  f current_group_
-0000a020: 7369 7a65 203e 3d20 626c 6f63 6b5f 7369  size >= block_si
-0000a030: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
-0000a040: 2020 2020 6772 6f75 7073 2e61 7070 656e      groups.appen
-0000a050: 6428 6375 7272 656e 745f 6772 6f75 7029  d(current_group)
-0000a060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a070: 2063 7572 7265 6e74 5f67 726f 7570 2c20   current_group, 
-0000a080: 6375 7272 656e 745f 6772 6f75 705f 7369  current_group_si
-0000a090: 7a65 203d 205b 5d2c 2030 0a20 2020 2069  ze = [], 0.    i
-0000a0a0: 6620 6375 7272 656e 745f 6772 6f75 703a  f current_group:
-0000a0b0: 0a20 2020 2020 2020 2067 726f 7570 732e  .        groups.
-0000a0c0: 6170 7065 6e64 2863 7572 7265 6e74 5f67  append(current_g
-0000a0d0: 726f 7570 290a 2020 2020 7265 7475 726e  roup).    return
-0000a0e0: 2067 726f 7570 730a 0a0a 6465 6620 7333   groups...def s3
-0000a0f0: 5f63 6f6e 6361 7428 0a20 2020 2020 2020  _concat(.       
-0000a100: 2073 7263 5f70 6174 6873 3a20 4c69 7374   src_paths: List
-0000a110: 5b50 6174 684c 696b 655d 2c0a 2020 2020  [PathLike],.    
-0000a120: 2020 2020 6473 745f 7061 7468 3a20 5061      dst_path: Pa
-0000a130: 7468 4c69 6b65 2c0a 2020 2020 2020 2020  thLike,.        
-0000a140: 626c 6f63 6b5f 7369 7a65 3a20 696e 7420  block_size: int 
-0000a150: 3d20 4445 4641 554c 545f 424c 4f43 4b5f  = DEFAULT_BLOCK_
-0000a160: 5349 5a45 2c0a 2020 2020 2020 2020 6d61  SIZE,.        ma
-0000a170: 785f 776f 726b 6572 733a 2069 6e74 203d  x_workers: int =
-0000a180: 2047 4c4f 4241 4c5f 4d41 585f 574f 524b   GLOBAL_MAX_WORK
-0000a190: 4552 5329 202d 3e20 4e6f 6e65 3a0a 2020  ERS) -> None:.  
-0000a1a0: 2020 2727 2743 6f6e 6361 7465 6e61 7465    '''Concatenate
-0000a1b0: 2073 3320 6669 6c65 7320 746f 206f 6e65   s3 files to one
-0000a1c0: 2066 696c 652e 0a0a 2020 2020 3a70 6172   file...    :par
-0000a1d0: 616d 2073 7263 5f70 6174 6873 3a20 4769  am src_paths: Gi
-0000a1e0: 7665 6e20 736f 7572 6365 2070 6174 6873  ven source paths
-0000a1f0: 0a20 2020 203a 7061 7261 6d20 6473 745f  .    :param dst_
-0000a200: 7061 7468 3a20 4769 7665 6e20 6465 7374  path: Given dest
-0000a210: 696e 6174 696f 6e20 7061 7468 0a20 2020  ination path.   
-0000a220: 2027 2727 0a20 2020 2063 6c69 656e 7420   '''.    client 
-0000a230: 3d20 5333 5061 7468 2864 7374 5f70 6174  = S3Path(dst_pat
-0000a240: 6829 2e5f 636c 6965 6e74 0a20 2020 2077  h)._client.    w
-0000a250: 6974 6820 7261 6973 655f 7333 5f65 7272  ith raise_s3_err
-0000a260: 6f72 2864 7374 5f70 6174 6829 3a0a 2020  or(dst_path):.  
-0000a270: 2020 2020 2020 6966 2062 6c6f 636b 5f73        if block_s
-0000a280: 697a 6520 3d3d 2030 3a20 2023 2070 7261  ize == 0:  # pra
-0000a290: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-0000a2a0: 2020 2020 2020 2020 2020 6772 6f75 7073            groups
-0000a2b0: 203d 205b 5b28 7372 635f 7061 7468 2c20   = [[(src_path, 
-0000a2c0: 4e6f 6e65 295d 2066 6f72 2073 7263 5f70  None)] for src_p
-0000a2d0: 6174 6820 696e 2073 7263 5f70 6174 6873  ath in src_paths
-0000a2e0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-0000a2f0: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-0000a300: 7073 203d 205f 6772 6f75 705f 7372 635f  ps = _group_src_
-0000a310: 7061 7468 735f 6279 5f62 6c6f 636b 2873  paths_by_block(s
-0000a320: 7263 5f70 6174 6873 2c20 626c 6f63 6b5f  rc_paths, block_
-0000a330: 7369 7a65 3d62 6c6f 636b 5f73 697a 6529  size=block_size)
-0000a340: 0a0a 2020 2020 2020 2020 7769 7468 204d  ..        with M
-0000a350: 756c 7469 5061 7274 5772 6974 6572 2863  ultiPartWriter(c
-0000a360: 6c69 656e 742c 2064 7374 5f70 6174 6829  lient, dst_path)
-0000a370: 2061 7320 7772 6974 6572 2c20 5468 7265   as writer, Thre
-0000a380: 6164 506f 6f6c 4578 6563 7574 6f72 280a  adPoolExecutor(.
-0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3a0: 6d61 785f 776f 726b 6572 733d 6d61 785f  max_workers=max_
-0000a3b0: 776f 726b 6572 7329 2061 7320 6578 6563  workers) as exec
-0000a3c0: 7574 6f72 3a0a 2020 2020 2020 2020 2020  utor:.          
-0000a3d0: 2020 666f 7220 696e 6465 782c 2067 726f    for index, gro
-0000a3e0: 7570 2069 6e20 656e 756d 6572 6174 6528  up in enumerate(
-0000a3f0: 6772 6f75 7073 2c20 7374 6172 743d 3129  groups, start=1)
-0000a400: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a410: 2020 6966 206c 656e 2867 726f 7570 2920    if len(group) 
-0000a420: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-0000a430: 2020 2020 2020 2020 2020 6578 6563 7574            execut
-0000a440: 6f72 2e73 7562 6d69 7428 0a20 2020 2020  or.submit(.     
-0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a460: 2020 2077 7269 7465 722e 7570 6c6f 6164     writer.upload
-0000a470: 5f70 6172 745f 636f 7079 2c20 696e 6465  _part_copy, inde
-0000a480: 782c 2067 726f 7570 5b30 5d5b 305d 2c0a  x, group[0][0],.
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 2020 2020 6772 6f75 705b 305d          group[0]
-0000a4b0: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
-0000a4c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a4e0: 7865 6375 746f 722e 7375 626d 6974 2877  xecutor.submit(w
-0000a4f0: 7269 7465 722e 7570 6c6f 6164 5f70 6172  riter.upload_par
-0000a500: 745f 6279 5f70 6174 6873 2c20 696e 6465  t_by_paths, inde
-0000a510: 782c 2067 726f 7570 290a 0a0a 4053 6d61  x, group)...@Sma
-0000a520: 7274 5061 7468 2e72 6567 6973 7465 720a  rtPath.register.
-0000a530: 636c 6173 7320 5333 5061 7468 2855 5249  class S3Path(URI
-0000a540: 5061 7468 293a 0a0a 2020 2020 7072 6f74  Path):..    prot
-0000a550: 6f63 6f6c 203d 2022 7333 220a 0a20 2020  ocol = "s3"..   
-0000a560: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0000a570: 6c66 2c20 7061 7468 3a20 2250 6174 684c  lf, path: "PathL
-0000a580: 696b 6522 2c20 2a6f 7468 6572 5f70 6174  ike", *other_pat
-0000a590: 6873 3a20 2250 6174 684c 696b 6522 293a  hs: "PathLike"):
-0000a5a0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-0000a5b0: 2e5f 5f69 6e69 745f 5f28 7061 7468 2c20  .__init__(path, 
-0000a5c0: 2a6f 7468 6572 5f70 6174 6873 290a 2020  *other_paths).  
-0000a5d0: 2020 2020 2020 7072 6f74 6f63 6f6c 203d        protocol =
-0000a5e0: 2067 6574 5f75 726c 5f73 6368 656d 6528   get_url_scheme(
-0000a5f0: 7365 6c66 2e70 6174 6829 0a20 2020 2020  self.path).     
-0000a600: 2020 2073 656c 662e 5f70 726f 746f 636f     self._protoco
-0000a610: 6c5f 7769 7468 5f70 726f 6669 6c65 203d  l_with_profile =
-0000a620: 2073 656c 662e 7072 6f74 6f63 6f6c 0a20   self.protocol. 
-0000a630: 2020 2020 2020 2073 656c 662e 5f70 726f         self._pro
-0000a640: 6669 6c65 5f6e 616d 6520 3d20 4e6f 6e65  file_name = None
-0000a650: 0a20 2020 2020 2020 2069 6620 7072 6f74  .        if prot
-0000a660: 6f63 6f6c 2e73 7461 7274 7377 6974 6828  ocol.startswith(
-0000a670: 2773 332b 2729 3a0a 2020 2020 2020 2020  's3+'):.        
-0000a680: 2020 2020 7365 6c66 2e5f 7072 6f74 6f63      self._protoc
-0000a690: 6f6c 5f77 6974 685f 7072 6f66 696c 6520  ol_with_profile 
-0000a6a0: 3d20 7072 6f74 6f63 6f6c 0a20 2020 2020  = protocol.     
-0000a6b0: 2020 2020 2020 2073 656c 662e 5f70 726f         self._pro
-0000a6c0: 6669 6c65 5f6e 616d 6520 3d20 7072 6f74  file_name = prot
-0000a6d0: 6f63 6f6c 5b33 3a5d 0a20 2020 2020 2020  ocol[3:].       
-0000a6e0: 2020 2020 2073 656c 662e 5f73 335f 7061       self._s3_pa
-0000a6f0: 7468 203d 2066 2273 333a 2f2f 7b73 656c  th = f"s3://{sel
-0000a700: 662e 7061 7468 5b6c 656e 2870 726f 746f  f.path[len(proto
-0000a710: 636f 6c29 2b33 3a5d 7d22 0a20 2020 2020  col)+3:]}".     
-0000a720: 2020 2065 6c69 6620 6e6f 7420 7072 6f74     elif not prot
-0000a730: 6f63 6f6c 3a0a 2020 2020 2020 2020 2020  ocol:.          
-0000a740: 2020 7365 6c66 2e5f 7333 5f70 6174 6820    self._s3_path 
-0000a750: 3d20 6622 7333 3a2f 2f7b 7365 6c66 2e70  = f"s3://{self.p
-0000a760: 6174 682e 6c73 7472 6970 2827 2f27 297d  ath.lstrip('/')}
-0000a770: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
-0000a780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a790: 2e5f 7333 5f70 6174 6820 3d20 7365 6c66  ._s3_path = self
-0000a7a0: 2e70 6174 680a 0a20 2020 2040 6361 6368  .path..    @cach
-0000a7b0: 6564 7072 6f70 6572 7479 0a20 2020 2064  edproperty.    d
-0000a7c0: 6566 2070 6174 685f 7769 7468 5f70 726f  ef path_with_pro
-0000a7d0: 746f 636f 6c28 7365 6c66 2920 2d3e 2073  tocol(self) -> s
-0000a7e0: 7472 3a0a 2020 2020 2020 2020 2727 2752  tr:.        '''R
-0000a7f0: 6574 7572 6e20 7061 7468 2077 6974 6820  eturn path with 
-0000a800: 7072 6f74 6f63 6f6c 2c20 6c69 6b65 2066  protocol, like f
-0000a810: 696c 653a 2f2f 2f72 6f6f 742c 2073 333a  ile:///root, s3:
-0000a820: 2f2f 6275 636b 6574 2f6b 6579 2727 270a  //bucket/key'''.
-0000a830: 2020 2020 2020 2020 7061 7468 203d 2073          path = s
-0000a840: 656c 662e 7061 7468 0a20 2020 2020 2020  elf.path.       
-0000a850: 2070 726f 746f 636f 6c5f 7072 6566 6978   protocol_prefix
-0000a860: 203d 2073 656c 662e 5f70 726f 746f 636f   = self._protoco
-0000a870: 6c5f 7769 7468 5f70 726f 6669 6c65 202b  l_with_profile +
-0000a880: 2022 3a2f 2f22 0a20 2020 2020 2020 2069   "://".        i
-0000a890: 6620 7061 7468 2e73 7461 7274 7377 6974  f path.startswit
-0000a8a0: 6828 7072 6f74 6f63 6f6c 5f70 7265 6669  h(protocol_prefi
-0000a8b0: 7829 3a0a 2020 2020 2020 2020 2020 2020  x):.            
-0000a8c0: 7265 7475 726e 2070 6174 680a 2020 2020  return path.    
-0000a8d0: 2020 2020 7265 7475 726e 2070 726f 746f      return proto
-0000a8e0: 636f 6c5f 7072 6566 6978 202b 2070 6174  col_prefix + pat
-0000a8f0: 682e 6c73 7472 6970 2827 2f27 290a 0a20  h.lstrip('/').. 
-0000a900: 2020 2040 6361 6368 6564 7072 6f70 6572     @cachedproper
-0000a910: 7479 0a20 2020 2064 6566 2070 6174 685f  ty.    def path_
-0000a920: 7769 7468 6f75 745f 7072 6f74 6f63 6f6c  without_protocol
-0000a930: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-0000a940: 2020 2020 2020 2027 2727 5265 7475 726e         '''Return
-0000a950: 2070 6174 6820 7769 7468 6f75 7420 7072   path without pr
-0000a960: 6f74 6f63 6f6c 2c20 6578 616d 706c 653a  otocol, example:
-0000a970: 2069 6620 7061 7468 2069 7320 7333 3a2f   if path is s3:/
-0000a980: 2f62 7563 6b65 742f 6b65 792c 2072 6574  /bucket/key, ret
-0000a990: 7572 6e20 6275 636b 6574 2f6b 6579 2727  urn bucket/key''
-0000a9a0: 270a 2020 2020 2020 2020 7061 7468 203d  '.        path =
-0000a9b0: 2073 656c 662e 7061 7468 0a20 2020 2020   self.path.     
-0000a9c0: 2020 2070 726f 746f 636f 6c5f 7072 6566     protocol_pref
-0000a9d0: 6978 203d 2073 656c 662e 5f70 726f 746f  ix = self._proto
-0000a9e0: 636f 6c5f 7769 7468 5f70 726f 6669 6c65  col_with_profile
-0000a9f0: 202b 2022 3a2f 2f22 0a20 2020 2020 2020   + "://".       
-0000aa00: 2069 6620 7061 7468 2e73 7461 7274 7377   if path.startsw
-0000aa10: 6974 6828 7072 6f74 6f63 6f6c 5f70 7265  ith(protocol_pre
-0000aa20: 6669 7829 3a0a 2020 2020 2020 2020 2020  fix):.          
-0000aa30: 2020 7061 7468 203d 2070 6174 685b 6c65    path = path[le
-0000aa40: 6e28 7072 6f74 6f63 6f6c 5f70 7265 6669  n(protocol_prefi
-0000aa50: 7829 3a5d 0a20 2020 2020 2020 2072 6574  x):].        ret
-0000aa60: 7572 6e20 7061 7468 0a0a 2020 2020 4063  urn path..    @c
-0000aa70: 6163 6865 6470 726f 7065 7274 790a 2020  achedproperty.  
-0000aa80: 2020 6465 6620 5f63 6c69 656e 7428 7365    def _client(se
-0000aa90: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-0000aaa0: 7572 6e20 6765 745f 7333 5f63 6c69 656e  urn get_s3_clien
-0000aab0: 7428 7072 6f66 696c 655f 6e61 6d65 3d73  t(profile_name=s
-0000aac0: 656c 662e 5f70 726f 6669 6c65 5f6e 616d  elf._profile_nam
-0000aad0: 6529 0a0a 2020 2020 6465 6620 5f73 335f  e)..    def _s3_
-0000aae0: 6765 745f 6d65 7461 6461 7461 2873 656c  get_metadata(sel
-0000aaf0: 6629 202d 3e20 6469 6374 3a0a 2020 2020  f) -> dict:.    
-0000ab00: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0000ab10: 4765 7420 6f62 6a65 6374 206d 6574 6164  Get object metad
-0000ab20: 6174 610a 0a20 2020 2020 2020 203a 7061  ata..        :pa
-0000ab30: 7261 6d20 7061 7468 3a20 4f62 6a65 6374  ram path: Object
-0000ab40: 2070 6174 680a 2020 2020 2020 2020 3a72   path.        :r
-0000ab50: 6574 7572 6e73 3a20 4f62 6a65 6374 206d  eturns: Object m
-0000ab60: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
-0000ab70: 2727 270a 2020 2020 2020 2020 6275 636b  '''.        buck
-0000ab80: 6574 2c20 6b65 7920 3d20 7061 7273 655f  et, key = parse_
-0000ab90: 7333 5f75 726c 2873 656c 662e 7061 7468  s3_url(self.path
-0000aba0: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
-0000abb0: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
-0000abc0: 7563 6b65 743a 0a20 2020 2020 2020 2020  ucket:.         
-0000abd0: 2020 2072 6574 7572 6e20 7b7d 0a20 2020     return {}.   
-0000abe0: 2020 2020 2069 6620 6e6f 7420 6b65 7920       if not key 
-0000abf0: 6f72 206b 6579 2e65 6e64 7377 6974 6828  or key.endswith(
-0000ac00: 272f 2729 3a0a 2020 2020 2020 2020 2020  '/'):.          
-0000ac10: 2020 7265 7475 726e 207b 7d0a 2020 2020    return {}.    
-0000ac20: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000ac30: 2020 2020 2077 6974 6820 7261 6973 655f       with raise_
-0000ac40: 7333 5f65 7272 6f72 2873 656c 662e 7061  s3_error(self.pa
-0000ac50: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
-0000ac60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ac70: 2020 2072 6573 7020 3d20 7365 6c66 2e5f     resp = self._
-0000ac80: 636c 6965 6e74 2e68 6561 645f 6f62 6a65  client.head_obje
-0000ac90: 6374 2842 7563 6b65 743d 6275 636b 6574  ct(Bucket=bucket
-0000aca0: 2c20 4b65 793d 6b65 7929 0a20 2020 2020  , Key=key).     
-0000acb0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-0000acc0: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-0000acd0: 2020 2020 286b 6579 2e6c 6f77 6572 2829      (key.lower()
-0000ace0: 2c20 7661 6c75 6529 2066 6f72 206b 6579  , value) for key
-0000acf0: 2c20 7661 6c75 6520 696e 2072 6573 705b  , value in resp[
-0000ad00: 274d 6574 6164 6174 6127 5d2e 6974 656d  'Metadata'].item
-0000ad10: 7328 2929 0a20 2020 2020 2020 2065 7863  s()).        exc
-0000ad20: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-0000ad30: 2065 7272 6f72 3a0a 2020 2020 2020 2020   error:.        
-0000ad40: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0000ad50: 6528 6572 726f 722c 0a20 2020 2020 2020  e(error,.       
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2020 2028 5333 556e 6b6e 6f77 6e45 7272     (S3UnknownErr
-0000ad80: 6f72 2c20 5333 436f 6e66 6967 4572 726f  or, S3ConfigErro
-0000ad90: 722c 2053 3350 6572 6d69 7373 696f 6e45  r, S3PermissionE
-0000ada0: 7272 6f72 2929 3a0a 2020 2020 2020 2020  rror)):.        
-0000adb0: 2020 2020 2020 2020 7261 6973 6520 6572          raise er
-0000adc0: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
-0000add0: 7265 7475 726e 207b 7d0a 0a20 2020 2064  return {}..    d
-0000ade0: 6566 2061 6363 6573 7328 0a20 2020 2020  ef access(.     
-0000adf0: 2020 2020 2020 2073 656c 662c 206d 6f64         self, mod
-0000ae00: 653a 2041 6363 6573 7320 3d20 4163 6365  e: Access = Acce
-0000ae10: 7373 2e52 4541 442c 0a20 2020 2020 2020  ss.READ,.       
-0000ae20: 2020 2020 2066 6f6c 6c6f 776c 696e 6b73       followlinks
-0000ae30: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-0000ae40: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-0000ae50: 2027 2727 0a20 2020 2020 2020 2054 6573   '''.        Tes
-0000ae60: 7420 6966 2070 6174 6820 6861 7320 6163  t if path has ac
-0000ae70: 6365 7373 2070 6572 6d69 7373 696f 6e20  cess permission 
-0000ae80: 6465 7363 7269 6265 6420 6279 206d 6f64  described by mod
-0000ae90: 650a 2020 2020 2020 2020 5573 696e 6720  e.        Using 
-0000aea0: 6865 6164 5f62 7563 6b65 7428 292c 206e  head_bucket(), n
-0000aeb0: 6f77 2052 4541 442f 5752 4954 4520 6172  ow READ/WRITE ar
-0000aec0: 6520 7361 6d65 2e0a 0a20 2020 2020 2020  e same...       
-0000aed0: 203a 7061 7261 6d20 6d6f 6465 3a20 6163   :param mode: ac
-0000aee0: 6365 7373 206d 6f64 650a 2020 2020 2020  cess mode.      
-0000aef0: 2020 3a72 6574 7572 6e73 3a20 626f 6f6c    :returns: bool
-0000af00: 2c20 6966 2074 6865 2062 7563 6b65 7420  , if the bucket 
-0000af10: 6f66 2073 335f 7572 6c20 6861 7320 7265  of s3_url has re
-0000af20: 6164 2f77 7269 7465 2061 6363 6573 732e  ad/write access.
-0000af30: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0000af40: 2020 2020 2073 335f 7572 6c20 3d20 7365       s3_url = se
-0000af50: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
-0000af60: 746f 636f 6c0a 2020 2020 2020 2020 6966  tocol.        if
-0000af70: 2066 6f6c 6c6f 776c 696e 6b73 3a0a 2020   followlinks:.  
-0000af80: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000af90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000afa0: 335f 7572 6c20 3d20 7365 6c66 2e72 6561  3_url = self.rea
-0000afb0: 646c 696e 6b28 292e 7061 7468 5f77 6974  dlink().path_wit
-0000afc0: 685f 7072 6f74 6f63 6f6c 0a20 2020 2020  h_protocol.     
-0000afd0: 2020 2020 2020 2065 7863 6570 7420 5333         except S3
-0000afe0: 4e6f 7441 4c69 6e6b 4572 726f 723a 0a20  NotALinkError:. 
-0000aff0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000b000: 6173 730a 2020 2020 2020 2020 6275 636b  ass.        buck
-0000b010: 6574 2c20 5f20 3d20 7061 7273 655f 7333  et, _ = parse_s3
-0000b020: 5f75 726c 2873 335f 7572 6c29 2020 2320  _url(s3_url)  # 
-0000b030: 6f6e 6c79 2063 6865 636b 2062 7563 6b65  only check bucke
-0000b040: 7420 6163 6365 7373 6962 696c 6974 790a  t accessibility.
-0000b050: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
-0000b060: 7563 6b65 743a 0a20 2020 2020 2020 2020  ucket:.         
-0000b070: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
-0000b080: 6f6e 2822 4e6f 2061 7661 696c 6162 6c65  on("No available
-0000b090: 2062 7563 6b65 7422 290a 2020 2020 2020   bucket").      
-0000b0a0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-0000b0b0: 6e63 6528 6d6f 6465 2c20 4163 6365 7373  nce(mode, Access
-0000b0c0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000b0d0: 6169 7365 2054 7970 6545 7272 6f72 280a  aise TypeError(.
-0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0f0: 2755 6e73 7570 706f 7274 6564 206d 6f64  'Unsupported mod
-0000b100: 653a 207b 7d20 2d2d 204d 6f64 6520 7368  e: {} -- Mode sh
-0000b110: 6f75 6c64 2075 7365 206f 6e65 206f 6620  ould use one of 
-0000b120: 7468 6520 656e 756d 7320 6265 6c6f 6e67  the enums belong
-0000b130: 696e 6720 746f 3a20 207b 7d27 0a20 2020  ing to:  {}'.   
-0000b140: 2020 2020 2020 2020 2020 2020 202e 666f               .fo
-0000b150: 726d 6174 286d 6f64 652c 2027 2c20 272e  rmat(mode, ', '.
-0000b160: 6a6f 696e 285b 7374 7228 6129 2066 6f72  join([str(a) for
-0000b170: 2061 2069 6e20 4163 6365 7373 5d29 2929   a in Access])))
-0000b180: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
-0000b190: 206e 6f74 2069 6e20 2841 6363 6573 732e   not in (Access.
-0000b1a0: 5245 4144 2c20 4163 6365 7373 2e57 5249  READ, Access.WRI
-0000b1b0: 5445 293a 0a20 2020 2020 2020 2020 2020  TE):.           
-0000b1c0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-0000b1d0: 2827 556e 7375 7070 6f72 7465 6420 6d6f  ('Unsupported mo
-0000b1e0: 6465 3a20 7b7d 272e 666f 726d 6174 286d  de: {}'.format(m
-0000b1f0: 6f64 6529 290a 2020 2020 2020 2020 7472  ode)).        tr
-0000b200: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0000b210: 656c 662e 5f63 6c69 656e 742e 6865 6164  elf._client.head
-0000b220: 5f62 7563 6b65 7428 4275 636b 6574 3d62  _bucket(Bucket=b
-0000b230: 7563 6b65 7429 0a20 2020 2020 2020 2065  ucket).        e
-0000b240: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000b250: 6173 2065 7272 6f72 3a0a 2020 2020 2020  as error:.      
-0000b260: 2020 2020 2020 6572 726f 7220 3d20 7472        error = tr
-0000b270: 616e 736c 6174 655f 7333 5f65 7272 6f72  anslate_s3_error
-0000b280: 2865 7272 6f72 2c20 7333 5f75 726c 290a  (error, s3_url).
-0000b290: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000b2a0: 7369 6e73 7461 6e63 6528 6572 726f 722c  sinstance(error,
-0000b2b0: 2028 5333 5065 726d 6973 7369 6f6e 4572   (S3PermissionEr
-0000b2c0: 726f 722c 2053 3346 696c 654e 6f74 466f  ror, S3FileNotFo
-0000b2d0: 756e 6445 7272 6f72 2c0a 2020 2020 2020  undError,.      
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2f0: 2020 2020 2020 2020 2020 2020 5333 4275              S3Bu
-0000b300: 636b 6574 4e6f 7446 6f75 6e64 4572 726f  cketNotFoundErro
-0000b310: 7229 293a 0a20 2020 2020 2020 2020 2020  r)):.           
-0000b320: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0000b330: 650a 2020 2020 2020 2020 2020 2020 7261  e.            ra
-0000b340: 6973 6520 6572 726f 720a 2020 2020 2020  ise error.      
-0000b350: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-0000b360: 2020 2064 6566 2065 7869 7374 7328 7365     def exists(se
-0000b370: 6c66 2c20 666f 6c6c 6f77 6c69 6e6b 733a  lf, followlinks:
-0000b380: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
-0000b390: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0000b3a0: 2727 270a 2020 2020 2020 2020 5465 7374  '''.        Test
-0000b3b0: 2069 6620 7333 5f75 726c 2065 7869 7374   if s3_url exist
-0000b3c0: 730a 0a20 2020 2020 2020 2049 6620 7468  s..        If th
-0000b3d0: 6520 6275 636b 6574 206f 6620 7333 5f75  e bucket of s3_u
-0000b3e0: 726c 2061 7265 206e 6f74 2070 6572 6d69  rl are not permi
-0000b3f0: 7474 6564 2074 6f20 7265 6164 2c20 7265  tted to read, re
-0000b400: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-0000b410: 2020 2020 3a72 6574 7572 6e73 3a20 5472      :returns: Tr
-0000b420: 7565 2069 6620 7333 5f75 726c 2065 6978  ue if s3_url eix
-0000b430: 7374 732c 2065 6c73 6520 4661 6c73 650a  sts, else False.
-0000b440: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000b450: 2020 2020 6275 636b 6574 2c20 6b65 7920      bucket, key 
-0000b460: 3d20 7061 7273 655f 7333 5f75 726c 2873  = parse_s3_url(s
-0000b470: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
-0000b480: 6f74 6f63 6f6c 290a 2020 2020 2020 2020  otocol).        
-0000b490: 6966 206e 6f74 2062 7563 6b65 743a 2020  if not bucket:  
-0000b4a0: 2320 7333 3a2f 2f20 3d3e 2054 7275 652c  # s3:// => True,
-0000b4b0: 2073 333a 2f2f 2f6b 6579 203d 3e20 4661   s3:///key => Fa
-0000b4c0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-0000b4d0: 7265 7475 726e 206e 6f74 206b 6579 0a0a  return not key..
-0000b4e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000b4f0: 656c 662e 6973 5f64 6972 2829 206f 7220  elf.is_dir() or 
-0000b500: 7365 6c66 2e69 735f 6669 6c65 2866 6f6c  self.is_file(fol
-0000b510: 6c6f 776c 696e 6b73 290a 0a20 2020 2064  lowlinks)..    d
-0000b520: 6566 2067 6574 6d74 696d 6528 7365 6c66  ef getmtime(self
-0000b530: 2c20 666f 6c6c 6f77 5f73 796d 6c69 6e6b  , follow_symlink
-0000b540: 733a 2062 6f6f 6c20 3d20 4661 6c73 6529  s: bool = False)
-0000b550: 202d 3e20 666c 6f61 743a 0a20 2020 2020   -> float:.     
-0000b560: 2020 2027 2727 0a20 2020 2020 2020 2047     '''.        G
-0000b570: 6574 206c 6173 742d 6d6f 6469 6669 6564  et last-modified
-0000b580: 2074 696d 6520 6f66 2074 6865 2066 696c   time of the fil
-0000b590: 6520 6f6e 2074 6865 2067 6976 656e 2073  e on the given s
-0000b5a0: 335f 7572 6c20 7061 7468 2028 696e 2055  3_url path (in U
-0000b5b0: 6e69 7820 7469 6d65 7374 616d 7020 666f  nix timestamp fo
-0000b5c0: 726d 6174 292e 0a20 2020 2020 2020 2049  rmat)..        I
-0000b5d0: 6620 7468 6520 7061 7468 2069 7320 616e  f the path is an
-0000b5e0: 2065 7869 7374 656e 7420 6469 7265 6374   existent direct
-0000b5f0: 6f72 792c 2072 6574 7572 6e20 7468 6520  ory, return the 
-0000b600: 6c61 7465 7374 206d 6f64 6966 6965 6420  latest modified 
-0000b610: 7469 6d65 206f 6620 616c 6c20 6669 6c65  time of all file
-0000b620: 2069 6e20 6974 2e20 5468 6520 6d74 696d   in it. The mtim
-0000b630: 6520 6f66 2065 6d70 7479 2064 6972 6563  e of empty direc
-0000b640: 746f 7279 2069 7320 3139 3730 2d30 312d  tory is 1970-01-
-0000b650: 3031 2030 303a 3030 3a30 300a 0a20 2020  01 00:00:00..   
-0000b660: 2020 2020 2049 6620 7333 5f75 726c 2069       If s3_url i
-0000b670: 7320 6e6f 7420 616e 2065 7869 7374 656e  s not an existen
-0000b680: 7420 7061 7468 2c20 7768 6963 6820 6d65  t path, which me
-0000b690: 616e 7320 7333 5f65 7869 7374 2873 335f  ans s3_exist(s3_
-0000b6a0: 7572 6c29 2072 6574 7572 6e73 2046 616c  url) returns Fal
-0000b6b0: 7365 2c20 7468 656e 2072 6169 7365 2053  se, then raise S
-0000b6c0: 3346 696c 654e 6f74 466f 756e 6445 7272  3FileNotFoundErr
-0000b6d0: 6f72 0a0a 2020 2020 2020 2020 3a72 6574  or..        :ret
-0000b6e0: 7572 6e73 3a20 4c61 7374 2d6d 6f64 6966  urns: Last-modif
-0000b6f0: 6965 6420 7469 6d65 0a20 2020 2020 2020  ied time.       
-0000b700: 203a 7261 6973 6573 3a20 5333 4669 6c65   :raises: S3File
-0000b710: 4e6f 7446 6f75 6e64 4572 726f 722c 2055  NotFoundError, U
-0000b720: 6e73 7570 706f 7274 6564 4572 726f 720a  nsupportedError.
-0000b730: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000b740: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000b750: 7374 6174 2866 6f6c 6c6f 775f 7379 6d6c  stat(follow_syml
-0000b760: 696e 6b73 3d66 6f6c 6c6f 775f 7379 6d6c  inks=follow_syml
-0000b770: 696e 6b73 292e 6d74 696d 650a 0a20 2020  inks).mtime..   
-0000b780: 2064 6566 2067 6574 7369 7a65 2873 656c   def getsize(sel
-0000b790: 662c 2066 6f6c 6c6f 775f 7379 6d6c 696e  f, follow_symlin
-0000b7a0: 6b73 3a20 626f 6f6c 203d 2046 616c 7365  ks: bool = False
-0000b7b0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-0000b7c0: 2020 2727 270a 2020 2020 2020 2020 4765    '''.        Ge
-0000b7d0: 7420 6669 6c65 2073 697a 6520 6f6e 2074  t file size on t
-0000b7e0: 6865 2067 6976 656e 2073 335f 7572 6c20  he given s3_url 
-0000b7f0: 7061 7468 2028 696e 2062 7974 6573 292e  path (in bytes).
-0000b800: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
-0000b810: 7061 7468 2069 6e20 6120 6469 7265 6374  path in a direct
-0000b820: 6f72 792c 2072 6574 7572 6e20 7468 6520  ory, return the 
-0000b830: 7375 6d20 6f66 2061 6c6c 2066 696c 6520  sum of all file 
-0000b840: 7369 7a65 2069 6e20 6974 2c20 696e 636c  size in it, incl
-0000b850: 7564 696e 6720 6669 6c65 2069 6e20 7375  uding file in su
-0000b860: 6264 6972 6563 746f 7269 6573 2028 6966  bdirectories (if
-0000b870: 2065 7869 7374 292e 0a20 2020 2020 2020   exist)..       
-0000b880: 2054 6865 2072 6573 756c 7420 6578 636c   The result excl
-0000b890: 7564 6573 2074 6865 2073 697a 6520 6f66  udes the size of
-0000b8a0: 2064 6972 6563 746f 7279 2069 7473 656c   directory itsel
-0000b8b0: 662e 2049 6e20 6f74 6865 7220 776f 7264  f. In other word
-0000b8c0: 732c 2072 6574 7572 6e20 3020 4279 7465  s, return 0 Byte
-0000b8d0: 206f 6e20 616e 2065 6d70 7479 2064 6972   on an empty dir
-0000b8e0: 6563 746f 7279 2070 6174 682e 0a0a 2020  ectory path...  
-0000b8f0: 2020 2020 2020 4966 2073 335f 7572 6c20        If s3_url 
-0000b900: 6973 206e 6f74 2061 6e20 6578 6973 7465  is not an existe
-0000b910: 6e74 2070 6174 682c 2077 6869 6368 206d  nt path, which m
-0000b920: 6561 6e73 2073 335f 6578 6973 7428 7333  eans s3_exist(s3
-0000b930: 5f75 726c 2920 7265 7475 726e 7320 4661  _url) returns Fa
-0000b940: 6c73 652c 2074 6865 6e20 7261 6973 6520  lse, then raise 
-0000b950: 5333 4669 6c65 4e6f 7446 6f75 6e64 4572  S3FileNotFoundEr
-0000b960: 726f 720a 0a20 2020 2020 2020 203a 7265  ror..        :re
-0000b970: 7475 726e 733a 2046 696c 6520 7369 7a65  turns: File size
-0000b980: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
-0000b990: 3a20 5333 4669 6c65 4e6f 7446 6f75 6e64  : S3FileNotFound
-0000b9a0: 4572 726f 722c 2055 6e73 7570 706f 7274  Error, Unsupport
-0000b9b0: 6564 4572 726f 720a 2020 2020 2020 2020  edError.        
-0000b9c0: 2727 270a 2020 2020 2020 2020 7265 7475  '''.        retu
-0000b9d0: 726e 2073 656c 662e 7374 6174 2866 6f6c  rn self.stat(fol
-0000b9e0: 6c6f 775f 7379 6d6c 696e 6b73 3d66 6f6c  low_symlinks=fol
-0000b9f0: 6c6f 775f 7379 6d6c 696e 6b73 292e 7369  low_symlinks).si
-0000ba00: 7a65 0a0a 2020 2020 6465 6620 676c 6f62  ze..    def glob
-0000ba10: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0000ba20: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0000ba30: 7061 7474 6572 6e2c 0a20 2020 2020 2020  pattern,.       
-0000ba40: 2020 2020 2072 6563 7572 7369 7665 3a20       recursive: 
-0000ba50: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-0000ba60: 2020 2020 2020 2020 206d 6973 7369 6e67           missing
-0000ba70: 5f6f 6b3a 2062 6f6f 6c20 3d20 5472 7565  _ok: bool = True
-0000ba80: 2c0a 2020 2020 2020 2020 2020 2020 666f  ,.            fo
-0000ba90: 6c6c 6f77 6c69 6e6b 733a 2062 6f6f 6c20  llowlinks: bool 
-0000baa0: 3d20 4661 6c73 652c 0a20 2020 2029 202d  = False,.    ) -
-0000bab0: 3e20 4c69 7374 5b27 5333 5061 7468 275d  > List['S3Path']
-0000bac0: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
-0000bad0: 7572 6e20 7333 2070 6174 6820 6c69 7374  urn s3 path list
-0000bae0: 2069 6e20 6173 6365 6e64 696e 6720 616c   in ascending al
-0000baf0: 7068 6162 6574 6963 616c 206f 7264 6572  phabetical order
-0000bb00: 2c20 696e 2077 6869 6368 2070 6174 6820  , in which path 
-0000bb10: 6d61 7463 6865 7320 676c 6f62 2070 6174  matches glob pat
-0000bb20: 7465 726e 0a20 2020 2020 2020 204e 6f74  tern.        Not
-0000bb30: 6573 3a20 4f6e 6c79 2067 6c6f 6220 696e  es: Only glob in
-0000bb40: 2062 7563 6b65 742e 2049 6620 7472 7969   bucket. If tryi
-0000bb50: 6e67 2074 6f20 6d61 7463 6820 6275 636b  ng to match buck
-0000bb60: 6574 2077 6974 6820 7769 6c64 6361 7264  et with wildcard
-0000bb70: 2063 6861 7261 6374 6572 732c 2072 6169   characters, rai
-0000bb80: 7365 2055 6e73 7570 706f 7274 6564 4572  se UnsupportedEr
-0000bb90: 726f 720a 0a20 2020 2020 2020 203a 7061  ror..        :pa
-0000bba0: 7261 6d20 7061 7474 6572 6e3a 2047 6c6f  ram pattern: Glo
-0000bbb0: 6220 7468 6520 6769 7665 6e20 7265 6c61  b the given rela
-0000bbc0: 7469 7665 2070 6174 7465 726e 2069 6e20  tive pattern in 
-0000bbd0: 7468 6520 6469 7265 6374 6f72 7920 7265  the directory re
-0000bbe0: 7072 6573 656e 7465 6420 6279 2074 6869  presented by thi
-0000bbf0: 7320 7061 7468 0a20 2020 2020 2020 203a  s path.        :
-0000bc00: 7061 7261 6d20 7265 6375 7273 6976 653a  param recursive:
-0000bc10: 2049 6620 4661 6c73 652c 2060 2a2a 6020   If False, `**` 
-0000bc20: 7769 6c6c 206e 6f74 2073 6561 7263 6820  will not search 
-0000bc30: 6469 7265 6374 6f72 7920 7265 6375 7273  directory recurs
-0000bc40: 6976 656c 790a 2020 2020 2020 2020 3a70  ively.        :p
-0000bc50: 6172 616d 206d 6973 7369 6e67 5f6f 6b3a  aram missing_ok:
-0000bc60: 2049 6620 4661 6c73 6520 616e 6420 7461   If False and ta
-0000bc70: 7267 6574 2070 6174 6820 646f 6573 6e27  rget path doesn'
-0000bc80: 7420 6d61 7463 6820 616e 7920 6669 6c65  t match any file
-0000bc90: 2c20 7261 6973 6520 4669 6c65 4e6f 7446  , raise FileNotF
-0000bca0: 6f75 6e64 4572 726f 720a 2020 2020 2020  oundError.      
-0000bcb0: 2020 3a72 6169 7365 733a 2055 6e73 7570    :raises: Unsup
-0000bcc0: 706f 7274 6564 4572 726f 722c 2077 6865  portedError, whe
-0000bcd0: 6e20 6275 636b 6574 2070 6172 7420 636f  n bucket part co
-0000bce0: 6e74 6169 6e73 2077 696c 6463 6172 6420  ntains wildcard 
-0000bcf0: 6368 6172 6163 7465 7273 0a20 2020 2020  characters.     
-0000bd00: 2020 203a 7265 7475 726e 733a 2041 206c     :returns: A l
-0000bd10: 6973 7420 636f 6e74 6169 6e73 2070 6174  ist contains pat
-0000bd20: 6873 206d 6174 6368 2060 7333 5f70 6174  hs match `s3_pat
-0000bd30: 686e 616d 6560 0a20 2020 2020 2020 2027  hname`.        '
-0000bd40: 2727 0a20 2020 2020 2020 2072 6574 7572  ''.        retur
-0000bd50: 6e20 6c69 7374 280a 2020 2020 2020 2020  n list(.        
-0000bd60: 2020 2020 7365 6c66 2e69 676c 6f62 280a      self.iglob(.
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd80: 7061 7474 6572 6e3d 7061 7474 6572 6e2c  pattern=pattern,
-0000bd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bda0: 2072 6563 7572 7369 7665 3d72 6563 7572   recursive=recur
-0000bdb0: 7369 7665 2c0a 2020 2020 2020 2020 2020  sive,.          
-0000bdc0: 2020 2020 2020 6d69 7373 696e 675f 6f6b        missing_ok
-0000bdd0: 3d6d 6973 7369 6e67 5f6f 6b2c 0a20 2020  =missing_ok,.   
-0000bde0: 2020 2020 2020 2020 2020 2020 2066 6f6c               fol
-0000bdf0: 6c6f 776c 696e 6b73 3d66 6f6c 6c6f 776c  lowlinks=followl
-0000be00: 696e 6b73 2929 0a0a 2020 2020 6465 6620  inks))..    def 
-0000be10: 676c 6f62 5f73 7461 7428 0a20 2020 2020  glob_stat(.     
-0000be20: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000be30: 2020 2020 2020 2020 2070 6174 7465 726e           pattern
-0000be40: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-0000be50: 6375 7273 6976 653a 2062 6f6f 6c20 3d20  cursive: bool = 
-0000be60: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000be70: 2020 6d69 7373 696e 675f 6f6b 3a20 626f    missing_ok: bo
-0000be80: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-0000be90: 2020 2020 2020 2066 6f6c 6c6f 776c 696e         followlin
-0000bea0: 6b73 3a20 626f 6f6c 203d 2046 616c 7365  ks: bool = False
-0000beb0: 2920 2d3e 2049 7465 7261 746f 725b 4669  ) -> Iterator[Fi
-0000bec0: 6c65 456e 7472 795d 3a0a 2020 2020 2020  leEntry]:.      
-0000bed0: 2020 2727 2752 6574 7572 6e20 6120 6765    '''Return a ge
-0000bee0: 6e65 7261 746f 7220 636f 6e74 6169 6e73  nerator contains
-0000bef0: 2074 7570 6c65 7320 6f66 2070 6174 6820   tuples of path 
-0000bf00: 616e 6420 6669 6c65 2073 7461 742c 2069  and file stat, i
-0000bf10: 6e20 6173 6365 6e64 696e 6720 616c 7068  n ascending alph
-0000bf20: 6162 6574 6963 616c 206f 7264 6572 2c20  abetical order, 
-0000bf30: 696e 2077 6869 6368 2070 6174 6820 6d61  in which path ma
-0000bf40: 7463 6865 7320 676c 6f62 2070 6174 7465  tches glob patte
-0000bf50: 726e 0a20 2020 2020 2020 204e 6f74 6573  rn.        Notes
-0000bf60: 3a20 4f6e 6c79 2067 6c6f 6220 696e 2062  : Only glob in b
-0000bf70: 7563 6b65 742e 2049 6620 7472 7969 6e67  ucket. If trying
-0000bf80: 2074 6f20 6d61 7463 6820 6275 636b 6574   to match bucket
-0000bf90: 2077 6974 6820 7769 6c64 6361 7264 2063   with wildcard c
-0000bfa0: 6861 7261 6374 6572 732c 2072 6169 7365  haracters, raise
-0000bfb0: 2055 6e73 7570 706f 7274 6564 4572 726f   UnsupportedErro
-0000bfc0: 720a 0a20 2020 2020 2020 203a 7061 7261  r..        :para
-0000bfd0: 6d20 7061 7474 6572 6e3a 2047 6c6f 6220  m pattern: Glob 
-0000bfe0: 7468 6520 6769 7665 6e20 7265 6c61 7469  the given relati
-0000bff0: 7665 2070 6174 7465 726e 2069 6e20 7468  ve pattern in th
-0000c000: 6520 6469 7265 6374 6f72 7920 7265 7072  e directory repr
-0000c010: 6573 656e 7465 6420 6279 2074 6869 7320  esented by this 
-0000c020: 7061 7468 0a20 2020 2020 2020 203a 7061  path.        :pa
-0000c030: 7261 6d20 7265 6375 7273 6976 653a 2049  ram recursive: I
-0000c040: 6620 4661 6c73 652c 2060 2a2a 6020 7769  f False, `**` wi
-0000c050: 6c6c 206e 6f74 2073 6561 7263 6820 6469  ll not search di
-0000c060: 7265 6374 6f72 7920 7265 6375 7273 6976  rectory recursiv
-0000c070: 656c 790a 2020 2020 2020 2020 3a70 6172  ely.        :par
-0000c080: 616d 206d 6973 7369 6e67 5f6f 6b3a 2049  am missing_ok: I
-0000c090: 6620 4661 6c73 6520 616e 6420 7461 7267  f False and targ
-0000c0a0: 6574 2070 6174 6820 646f 6573 6e27 7420  et path doesn't 
-0000c0b0: 6d61 7463 6820 616e 7920 6669 6c65 2c20  match any file, 
-0000c0c0: 7261 6973 6520 4669 6c65 4e6f 7446 6f75  raise FileNotFou
-0000c0d0: 6e64 4572 726f 720a 2020 2020 2020 2020  ndError.        
-0000c0e0: 3a72 6169 7365 733a 2055 6e73 7570 706f  :raises: Unsuppo
-0000c0f0: 7274 6564 4572 726f 722c 2077 6865 6e20  rtedError, when 
-0000c100: 6275 636b 6574 2070 6172 7420 636f 6e74  bucket part cont
-0000c110: 6169 6e73 2077 696c 6463 6172 6420 6368  ains wildcard ch
-0000c120: 6172 6163 7465 7273 0a20 2020 2020 2020  aracters.       
-0000c130: 203a 7265 7475 726e 733a 2041 2067 656e   :returns: A gen
-0000c140: 6572 6174 6f72 2063 6f6e 7461 696e 7320  erator contains 
-0000c150: 7475 706c 6573 206f 6620 7061 7468 2061  tuples of path a
-0000c160: 6e64 2066 696c 6520 7374 6174 2c20 696e  nd file stat, in
-0000c170: 2077 6869 6368 2070 6174 6873 206d 6174   which paths mat
-0000c180: 6368 2060 7333 5f70 6174 686e 616d 6560  ch `s3_pathname`
-0000c190: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0000c1a0: 2020 2020 2067 6c6f 625f 7061 7468 203d       glob_path =
-0000c1b0: 2073 656c 662e 5f73 335f 7061 7468 0a20   self._s3_path. 
-0000c1c0: 2020 2020 2020 2069 6620 7061 7474 6572         if patter
-0000c1d0: 6e3a 0a20 2020 2020 2020 2020 2020 2067  n:.            g
-0000c1e0: 6c6f 625f 7061 7468 203d 2073 656c 662e  lob_path = self.
-0000c1f0: 6a6f 696e 7061 7468 2870 6174 7465 726e  joinpath(pattern
-0000c200: 292e 5f73 335f 7061 7468 2020 2320 7079  )._s3_path  # py
-0000c210: 7479 7065 3a20 6469 7361 626c 653d 6174  type: disable=at
-0000c220: 7472 6962 7574 652d 6572 726f 720a 2020  tribute-error.  
-0000c230: 2020 2020 2020 7333 5f70 6174 686e 616d        s3_pathnam
-0000c240: 6520 3d20 6673 7061 7468 2867 6c6f 625f  e = fspath(glob_
-0000c250: 7061 7468 290a 0a20 2020 2020 2020 2064  path)..        d
-0000c260: 6566 2063 7265 6174 655f 6765 6e65 7261  ef create_genera
-0000c270: 746f 7228 293a 0a20 2020 2020 2020 2020  tor():.         
-0000c280: 2020 2066 6f72 2067 726f 7570 5f73 335f     for group_s3_
-0000c290: 7061 7468 6e61 6d65 5f31 2069 6e20 5f67  pathname_1 in _g
-0000c2a0: 726f 7570 5f73 3370 6174 685f 6279 5f62  roup_s3path_by_b
-0000c2b0: 7563 6b65 7428 0a20 2020 2020 2020 2020  ucket(.         
-0000c2c0: 2020 2020 2020 2020 2020 2073 335f 7061             s3_pa
-0000c2d0: 7468 6e61 6d65 2c20 7365 6c66 2e5f 7072  thname, self._pr
-0000c2e0: 6f66 696c 655f 6e61 6d65 293a 0a20 2020  ofile_name):.   
-0000c2f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000c300: 2067 726f 7570 5f73 335f 7061 7468 6e61   group_s3_pathna
-0000c310: 6d65 5f32 2069 6e20 5f67 726f 7570 5f73  me_2 in _group_s
-0000c320: 3370 6174 685f 6279 5f70 7265 6669 7828  3path_by_prefix(
-0000c330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c340: 2020 2020 2020 2020 2067 726f 7570 5f73           group_s
-0000c350: 335f 7061 7468 6e61 6d65 5f31 293a 0a20  3_pathname_1):. 
+00004370: 2064 7374 5f75 726c 3a20 5061 7468 4c69   dst_url: PathLi
+00004380: 6b65 2920 2d3e 2049 7465 7261 746f 725b  ke) -> Iterator[
+00004390: 5475 706c 655b 5061 7468 4c69 6b65 2c20  Tuple[PathLike, 
+000043a0: 5061 7468 4c69 6b65 5d5d 3a0a 2020 2020  PathLike]]:.    
+000043b0: 666f 7220 7372 635f 6669 6c65 5f70 6174  for src_file_pat
+000043c0: 6820 696e 2053 3350 6174 6828 7372 635f  h in S3Path(src_
+000043d0: 7572 6c29 2e73 6361 6e28 293a 0a20 2020  url).scan():.   
+000043e0: 2020 2020 2063 6f6e 7465 6e74 5f70 6174       content_pat
+000043f0: 6820 3d20 7372 635f 6669 6c65 5f70 6174  h = src_file_pat
+00004400: 685b 6c65 6e28 7372 635f 7572 6c29 3a5d  h[len(src_url):]
+00004410: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00004420: 636f 6e74 656e 745f 7061 7468 2920 3e20  content_path) > 
+00004430: 303a 0a20 2020 2020 2020 2020 2020 2064  0:.            d
+00004440: 7374 5f66 696c 655f 7061 7468 203d 2073  st_file_path = s
+00004450: 335f 7061 7468 5f6a 6f69 6e28 6473 745f  3_path_join(dst_
+00004460: 7572 6c2c 2063 6f6e 7465 6e74 5f70 6174  url, content_pat
+00004470: 6829 0a20 2020 2020 2020 2065 6c73 653a  h).        else:
+00004480: 0a20 2020 2020 2020 2020 2020 2064 7374  .            dst
+00004490: 5f66 696c 655f 7061 7468 203d 2064 7374  _file_path = dst
+000044a0: 5f75 726c 0a20 2020 2020 2020 2079 6965  _url.        yie
+000044b0: 6c64 2073 7263 5f66 696c 655f 7061 7468  ld src_file_path
+000044c0: 2c20 6473 745f 6669 6c65 5f70 6174 680a  , dst_file_path.
+000044d0: 0a0a 6465 6620 6973 5f73 3328 7061 7468  ..def is_s3(path
+000044e0: 3a20 5061 7468 4c69 6b65 2920 2d3e 2062  : PathLike) -> b
+000044f0: 6f6f 6c3a 0a20 2020 2027 2727 0a20 2020  ool:.    '''.   
+00004500: 2031 2e20 4163 636f 7264 696e 6720 746f   1. According to
+00004510: 2060 6177 732d 636c 6920 3c68 7474 7073   `aws-cli <https
+00004520: 3a2f 2f64 6f63 732e 6177 732e 616d 617a  ://docs.aws.amaz
+00004530: 6f6e 2e63 6f6d 2f63 6c69 2f6c 6174 6573  on.com/cli/lates
+00004540: 742f 7265 6665 7265 6e63 652f 7333 2f69  t/reference/s3/i
+00004550: 6e64 6578 2e68 746d 6c3e 605f 202c 2074  ndex.html>`_ , t
+00004560: 6573 7420 6966 2061 2070 6174 6820 6973  est if a path is
+00004570: 2073 3320 7061 7468 2e0a 2020 2020 322e   s3 path..    2.
+00004580: 206d 6567 6669 6c65 2061 6c73 6f20 7375   megfile also su
+00004590: 7070 6f72 7420 7468 6520 7061 7468 206c  pport the path l
+000045a0: 696b 6520 6073 335b 2b70 726f 6669 6c65  ike `s3[+profile
+000045b0: 5f6e 616d 655d 3a2f 2f62 7563 6b65 742f  _name]://bucket/
+000045c0: 6b65 7960 0a0a 2020 2020 3a70 6172 616d  key`..    :param
+000045d0: 2070 6174 683a 2050 6174 6820 746f 2062   path: Path to b
+000045e0: 6520 7465 7374 6564 0a20 2020 203a 7265  e tested.    :re
+000045f0: 7475 726e 733a 2054 7275 6520 6966 2070  turns: True if p
+00004600: 6174 6820 6973 2073 3320 7061 7468 2c20  ath is s3 path, 
+00004610: 656c 7365 2046 616c 7365 0a20 2020 2027  else False.    '
+00004620: 2727 0a20 2020 2070 6174 6820 3d20 6673  ''.    path = fs
+00004630: 7061 7468 2870 6174 6829 0a20 2020 2069  path(path).    i
+00004640: 6620 7265 2e6d 6174 6368 2872 275e 7333  f re.match(r'^s3
+00004650: 285c 2b5c 772b 293f 3a5c 2f5c 2f27 2c20  (\+\w+)?:\/\/', 
+00004660: 7061 7468 293a 0a20 2020 2020 2020 2072  path):.        r
+00004670: 6574 7572 6e20 5472 7565 0a20 2020 2072  eturn True.    r
+00004680: 6574 7572 6e20 4661 6c73 650a 0a0a 6465  eturn False...de
+00004690: 6620 5f73 335f 6269 6e61 7279 5f6d 6f64  f _s3_binary_mod
+000046a0: 6528 7333 5f6f 7065 6e5f 6675 6e63 293a  e(s3_open_func):
+000046b0: 0a0a 2020 2020 4077 7261 7073 2873 335f  ..    @wraps(s3_
+000046c0: 6f70 656e 5f66 756e 6329 0a20 2020 2064  open_func).    d
+000046d0: 6566 2077 7261 7070 6572 2873 335f 7572  ef wrapper(s3_ur
+000046e0: 6c2c 206d 6f64 653a 2073 7472 203d 2027  l, mode: str = '
+000046f0: 7262 272c 202a 2a6b 7761 7267 7329 3a0a  rb', **kwargs):.
+00004700: 2020 2020 2020 2020 6275 636b 6574 2c20          bucket, 
+00004710: 6b65 7920 3d20 7061 7273 655f 7333 5f75  key = parse_s3_u
+00004720: 726c 2873 335f 7572 6c29 0a20 2020 2020  rl(s3_url).     
+00004730: 2020 2069 6620 6e6f 7420 6275 636b 6574     if not bucket
+00004740: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00004750: 6973 6520 5333 4275 636b 6574 4e6f 7446  ise S3BucketNotF
+00004760: 6f75 6e64 4572 726f 7228 2745 6d70 7479  oundError('Empty
+00004770: 2062 7563 6b65 7420 6e61 6d65 3a20 2572   bucket name: %r
+00004780: 2720 2520 7333 5f75 726c 290a 0a20 2020  ' % s3_url)..   
+00004790: 2020 2020 2069 6620 6e6f 7420 6b65 7920       if not key 
+000047a0: 6f72 206b 6579 2e65 6e64 7377 6974 6828  or key.endswith(
+000047b0: 272f 2729 3a0a 2020 2020 2020 2020 2020  '/'):.          
+000047c0: 2020 7261 6973 6520 5333 4973 4144 6972    raise S3IsADir
+000047d0: 6563 746f 7279 4572 726f 7228 2749 7320  ectoryError('Is 
+000047e0: 6120 6469 7265 6374 6f72 793a 2025 7227  a directory: %r'
+000047f0: 2025 2073 335f 7572 6c29 0a0a 2020 2020   % s3_url)..    
+00004800: 2020 2020 6966 2027 7827 2069 6e20 6d6f      if 'x' in mo
+00004810: 6465 3a0a 2020 2020 2020 2020 2020 2020  de:.            
+00004820: 6966 2053 3350 6174 6828 7333 5f75 726c  if S3Path(s3_url
+00004830: 292e 6973 5f66 696c 6528 293a 0a20 2020  ).is_file():.   
+00004840: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00004850: 7365 2053 3346 696c 6545 7869 7374 7345  se S3FileExistsE
+00004860: 7272 6f72 2827 4669 6c65 2065 7869 7374  rror('File exist
+00004870: 733a 2025 7227 2025 2073 335f 7572 6c29  s: %r' % s3_url)
+00004880: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+00004890: 6520 3d20 6d6f 6465 2e72 6570 6c61 6365  e = mode.replace
+000048a0: 2827 7827 2c20 2777 2729 0a0a 2020 2020  ('x', 'w')..    
+000048b0: 2020 2020 6966 2027 7727 2069 6e20 6d6f      if 'w' in mo
+000048c0: 6465 206f 7220 2761 2720 696e 206d 6f64  de or 'a' in mod
+000048d0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+000048e0: 6620 6e6f 7420 5333 5061 7468 2873 335f  f not S3Path(s3_
+000048f0: 7572 6c29 2e68 6173 6275 636b 6574 2829  url).hasbucket()
+00004900: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004910: 2020 7261 6973 6520 5333 4275 636b 6574    raise S3Bucket
+00004920: 4e6f 7446 6f75 6e64 4572 726f 7228 274e  NotFoundError('N
+00004930: 6f20 7375 6368 2062 7563 6b65 743a 2025  o such bucket: %
+00004940: 7227 2025 2073 335f 7572 6c29 0a0a 2020  r' % s3_url)..  
+00004950: 2020 2020 2020 6669 6c65 6f62 6a20 3d20        fileobj = 
+00004960: 7333 5f6f 7065 6e5f 6675 6e63 2873 335f  s3_open_func(s3_
+00004970: 7572 6c2c 2067 6574 5f62 696e 6172 795f  url, get_binary_
+00004980: 6d6f 6465 286d 6f64 6529 2c20 2a2a 6b77  mode(mode), **kw
+00004990: 6172 6773 290a 2020 2020 2020 2020 6966  args).        if
+000049a0: 2027 6227 206e 6f74 2069 6e20 6d6f 6465   'b' not in mode
+000049b0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+000049c0: 6c65 6f62 6a20 3d20 696f 2e54 6578 7449  leobj = io.TextI
+000049d0: 4f57 7261 7070 6572 2866 696c 656f 626a  OWrapper(fileobj
+000049e0: 2920 2023 2070 7974 7970 653a 2064 6973  )  # pytype: dis
+000049f0: 6162 6c65 3d77 726f 6e67 2d61 7267 2d74  able=wrong-arg-t
+00004a00: 7970 6573 0a20 2020 2020 2020 2020 2020  ypes.           
+00004a10: 2066 696c 656f 626a 2e6d 6f64 6520 3d20   fileobj.mode = 
+00004a20: 6d6f 6465 0a20 2020 2020 2020 2072 6574  mode.        ret
+00004a30: 7572 6e20 6669 6c65 6f62 6a0a 0a20 2020  urn fileobj..   
+00004a40: 2072 6574 7572 6e20 7772 6170 7065 720a   return wrapper.
+00004a50: 0a0a 405f 7333 5f62 696e 6172 795f 6d6f  ..@_s3_binary_mo
+00004a60: 6465 0a64 6566 2073 335f 7072 6566 6574  de.def s3_prefet
+00004a70: 6368 5f6f 7065 6e28 0a20 2020 2020 2020  ch_open(.       
+00004a80: 2073 335f 7572 6c3a 2050 6174 684c 696b   s3_url: PathLik
+00004a90: 652c 0a20 2020 2020 2020 206d 6f64 653a  e,.        mode:
+00004aa0: 2073 7472 203d 2027 7262 272c 0a20 2020   str = 'rb',.   
+00004ab0: 2020 2020 2066 6f6c 6c6f 776c 696e 6b73       followlinks
+00004ac0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00004ad0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+00004ae0: 2020 206d 6178 5f63 6f6e 6375 7272 656e     max_concurren
+00004af0: 6379 3a20 4f70 7469 6f6e 616c 5b69 6e74  cy: Optional[int
+00004b00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00004b10: 2020 6d61 785f 626c 6f63 6b5f 7369 7a65    max_block_size
+00004b20: 3a20 696e 7420 3d20 4445 4641 554c 545f  : int = DEFAULT_
+00004b30: 424c 4f43 4b5f 5349 5a45 2920 2d3e 2053  BLOCK_SIZE) -> S
+00004b40: 3350 7265 6665 7463 6852 6561 6465 723a  3PrefetchReader:
+00004b50: 0a20 2020 2027 2727 4f70 656e 2061 2061  .    '''Open a a
+00004b60: 7379 6e63 6872 6f6e 6f75 7320 7072 6566  synchronous pref
+00004b70: 6574 6368 2072 6561 6465 722c 2074 6f20  etch reader, to 
+00004b80: 7375 7070 6f72 7420 6661 7374 2073 6571  support fast seq
+00004b90: 7565 6e74 6961 6c20 7265 6164 2061 6e64  uential read and
+00004ba0: 2072 616e 646f 6d20 7265 6164 0a0a 2020   random read..  
+00004bb0: 2020 2e2e 206e 6f74 6520 3a3a 0a0a 2020    .. note ::..  
+00004bc0: 2020 2020 2020 5573 6572 2073 686f 756c        User shoul
+00004bd0: 6420 6d61 6b65 2073 7572 6520 7468 6174  d make sure that
+00004be0: 2072 6561 6465 7220 2f20 7772 6974 6572   reader / writer
+00004bf0: 2061 7265 2063 6c6f 7365 6420 636f 7272   are closed corr
+00004c00: 6563 746c 790a 0a20 2020 2020 2020 2053  ectly..        S
+00004c10: 7570 706f 7274 7320 636f 6e74 6578 7420  upports context 
+00004c20: 6d61 6e61 6765 720a 0a20 2020 2020 2020  manager..       
+00004c30: 2053 6f6d 6520 7061 7261 6d65 7465 7220   Some parameter 
+00004c40: 7365 7474 696e 6720 6d61 7920 7065 7266  setting may perf
+00004c50: 6f72 6d20 7765 6c6c 3a20 6d61 785f 636f  orm well: max_co
+00004c60: 6e63 7572 7265 6e63 793d 3130 206f 7220  ncurrency=10 or 
+00004c70: 3230 2c20 6d61 785f 626c 6f63 6b5f 7369  20, max_block_si
+00004c80: 7a65 3d38 206f 7220 3136 204d 422c 2064  ze=8 or 16 MB, d
+00004c90: 6566 6175 6c74 2076 616c 7565 204e 6f6e  efault value Non
+00004ca0: 6520 6d65 616e 7320 7573 696e 6720 676c  e means using gl
+00004cb0: 6f62 616c 2074 6872 6561 6420 706f 6f6c  obal thread pool
+00004cc0: 0a0a 2020 2020 3a70 6172 616d 206d 6178  ..    :param max
+00004cd0: 5f63 6f6e 6375 7272 656e 6379 3a20 4d61  _concurrency: Ma
+00004ce0: 7820 646f 776e 6c6f 6164 2074 6872 6561  x download threa
+00004cf0: 6420 6e75 6d62 6572 2c20 4e6f 6e65 2062  d number, None b
+00004d00: 7920 6465 6661 756c 740a 2020 2020 3a70  y default.    :p
+00004d10: 6172 616d 206d 6178 5f62 6c6f 636b 5f73  aram max_block_s
+00004d20: 697a 653a 204d 6178 2064 6174 6120 7369  ize: Max data si
+00004d30: 7a65 2064 6f77 6e6c 6f61 6465 6420 6279  ze downloaded by
+00004d40: 2065 6163 6820 7468 7265 6164 2c20 696e   each thread, in
+00004d50: 2062 7974 6573 2c20 384d 4220 6279 2064   bytes, 8MB by d
+00004d60: 6566 6175 6c74 0a20 2020 203a 7265 7475  efault.    :retu
+00004d70: 726e 733a 2041 6e20 6f70 656e 6564 2053  rns: An opened S
+00004d80: 3350 7265 6665 7463 6852 6561 6465 7220  3PrefetchReader 
+00004d90: 6f62 6a65 6374 0a20 2020 203a 7261 6973  object.    :rais
+00004da0: 6573 3a20 5333 4669 6c65 4e6f 7446 6f75  es: S3FileNotFou
+00004db0: 6e64 4572 726f 720a 2020 2020 2727 270a  ndError.    '''.
+00004dc0: 2020 2020 6966 206d 6f64 6520 213d 2027      if mode != '
+00004dd0: 7262 273a 0a20 2020 2020 2020 2072 6169  rb':.        rai
+00004de0: 7365 2056 616c 7565 4572 726f 7228 2775  se ValueError('u
+00004df0: 6e61 6363 6570 7461 626c 6520 6d6f 6465  nacceptable mode
+00004e00: 3a20 2572 2720 2520 6d6f 6465 290a 2020  : %r' % mode).  
+00004e10: 2020 7333 5f75 726c 203d 2053 3350 6174    s3_url = S3Pat
+00004e20: 6828 7333 5f75 726c 290a 2020 2020 6966  h(s3_url).    if
+00004e30: 2066 6f6c 6c6f 776c 696e 6b73 3a0a 2020   followlinks:.  
+00004e40: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00004e50: 2020 2020 2020 2073 335f 7572 6c20 3d20         s3_url = 
+00004e60: 7333 5f75 726c 2e72 6561 646c 696e 6b28  s3_url.readlink(
+00004e70: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00004e80: 2053 334e 6f74 414c 696e 6b45 7272 6f72   S3NotALinkError
+00004e90: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00004ea0: 7373 0a0a 2020 2020 6275 636b 6574 2c20  ss..    bucket, 
+00004eb0: 6b65 7920 3d20 7061 7273 655f 7333 5f75  key = parse_s3_u
+00004ec0: 726c 2873 335f 7572 6c2e 7061 7468 5f77  rl(s3_url.path_w
+00004ed0: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
+00004ee0: 2020 636f 6e66 6967 203d 2062 6f74 6f63    config = botoc
+00004ef0: 6f72 652e 636f 6e66 6967 2e43 6f6e 6669  ore.config.Confi
+00004f00: 6728 6d61 785f 706f 6f6c 5f63 6f6e 6e65  g(max_pool_conne
+00004f10: 6374 696f 6e73 3d6d 6178 5f70 6f6f 6c5f  ctions=max_pool_
+00004f20: 636f 6e6e 6563 7469 6f6e 7329 0a20 2020  connections).   
+00004f30: 2063 6c69 656e 7420 3d20 6765 745f 7333   client = get_s3
+00004f40: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
+00004f50: 2063 6f6e 6669 673d 636f 6e66 6967 2c0a   config=config,.
+00004f60: 2020 2020 2020 2020 6361 6368 655f 6b65          cache_ke
+00004f70: 793d 2773 335f 6669 6c65 6c69 6b65 5f63  y='s3_filelike_c
+00004f80: 6c69 656e 7427 2c0a 2020 2020 2020 2020  lient',.        
+00004f90: 7072 6f66 696c 655f 6e61 6d65 3d73 335f  profile_name=s3_
+00004fa0: 7572 6c2e 5f70 726f 6669 6c65 5f6e 616d  url._profile_nam
+00004fb0: 6529 0a20 2020 2072 6574 7572 6e20 5333  e).    return S3
+00004fc0: 5072 6566 6574 6368 5265 6164 6572 280a  PrefetchReader(.
+00004fd0: 2020 2020 2020 2020 6275 636b 6574 2c0a          bucket,.
+00004fe0: 2020 2020 2020 2020 6b65 792c 0a20 2020          key,.   
+00004ff0: 2020 2020 2073 335f 636c 6965 6e74 3d63       s3_client=c
+00005000: 6c69 656e 742c 0a20 2020 2020 2020 206d  lient,.        m
+00005010: 6178 5f72 6574 7269 6573 3d6d 6178 5f72  ax_retries=max_r
+00005020: 6574 7269 6573 2c0a 2020 2020 2020 2020  etries,.        
+00005030: 6d61 785f 776f 726b 6572 733d 6d61 785f  max_workers=max_
+00005040: 636f 6e63 7572 7265 6e63 792c 0a20 2020  concurrency,.   
+00005050: 2020 2020 2062 6c6f 636b 5f73 697a 653d       block_size=
+00005060: 6d61 785f 626c 6f63 6b5f 7369 7a65 290a  max_block_size).
+00005070: 0a0a 405f 7333 5f62 696e 6172 795f 6d6f  ..@_s3_binary_mo
+00005080: 6465 0a64 6566 2073 335f 7368 6172 655f  de.def s3_share_
+00005090: 6361 6368 655f 6f70 656e 280a 2020 2020  cache_open(.    
+000050a0: 2020 2020 7333 5f75 726c 3a20 5061 7468      s3_url: Path
+000050b0: 4c69 6b65 2c0a 2020 2020 2020 2020 6d6f  Like,.        mo
+000050c0: 6465 3a20 7374 7220 3d20 2772 6227 2c0a  de: str = 'rb',.
+000050d0: 2020 2020 2020 2020 666f 6c6c 6f77 6c69          followli
+000050e0: 6e6b 733a 2062 6f6f 6c20 3d20 4661 6c73  nks: bool = Fals
+000050f0: 652c 0a20 2020 2020 2020 202a 2c0a 2020  e,.        *,.  
+00005100: 2020 2020 2020 6361 6368 655f 6b65 793a        cache_key:
+00005110: 2073 7472 203d 2027 6c72 7527 2c0a 2020   str = 'lru',.  
+00005120: 2020 2020 2020 6d61 785f 636f 6e63 7572        max_concur
+00005130: 7265 6e63 793a 204f 7074 696f 6e61 6c5b  rency: Optional[
+00005140: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+00005150: 2020 2020 206d 6178 5f62 6c6f 636b 5f73       max_block_s
+00005160: 697a 653a 2069 6e74 203d 2044 4546 4155  ize: int = DEFAU
+00005170: 4c54 5f42 4c4f 434b 5f53 495a 4529 202d  LT_BLOCK_SIZE) -
+00005180: 3e20 5333 5368 6172 6543 6163 6865 5265  > S3ShareCacheRe
+00005190: 6164 6572 3a0a 2020 2020 2727 274f 7065  ader:.    '''Ope
+000051a0: 6e20 6120 6173 796e 6368 726f 6e6f 7573  n a asynchronous
+000051b0: 2070 7265 6665 7463 6820 7265 6164 6572   prefetch reader
+000051c0: 2c20 746f 2073 7570 706f 7274 2066 6173  , to support fas
+000051d0: 7420 7365 7175 656e 7469 616c 2072 6561  t sequential rea
+000051e0: 6420 616e 6420 7261 6e64 6f6d 2072 6561  d and random rea
+000051f0: 640a 0a20 2020 202e 2e20 6e6f 7465 203a  d..    .. note :
+00005200: 3a0a 0a20 2020 2020 2020 2055 7365 7220  :..        User 
+00005210: 7368 6f75 6c64 206d 616b 6520 7375 7265  should make sure
+00005220: 2074 6861 7420 7265 6164 6572 202f 2077   that reader / w
+00005230: 7269 7465 7220 6172 6520 636c 6f73 6564  riter are closed
+00005240: 2063 6f72 7265 6374 6c79 0a0a 2020 2020   correctly..    
+00005250: 2020 2020 5375 7070 6f72 7473 2063 6f6e      Supports con
+00005260: 7465 7874 206d 616e 6167 6572 0a0a 2020  text manager..  
+00005270: 2020 2020 2020 536f 6d65 2070 6172 616d        Some param
+00005280: 6574 6572 2073 6574 7469 6e67 206d 6179  eter setting may
+00005290: 2070 6572 666f 726d 2077 656c 6c3a 206d   perform well: m
+000052a0: 6178 5f63 6f6e 6375 7272 656e 6379 3d31  ax_concurrency=1
+000052b0: 3020 6f72 2032 302c 206d 6178 5f62 6c6f  0 or 20, max_blo
+000052c0: 636b 5f73 697a 653d 3820 6f72 2031 3620  ck_size=8 or 16 
+000052d0: 4d42 2c20 6465 6661 756c 7420 7661 6c75  MB, default valu
+000052e0: 6520 4e6f 6e65 206d 6561 6e73 2075 7369  e None means usi
+000052f0: 6e67 2067 6c6f 6261 6c20 7468 7265 6164  ng global thread
+00005300: 2070 6f6f 6c0a 0a20 2020 203a 7061 7261   pool..    :para
+00005310: 6d20 6d61 785f 636f 6e63 7572 7265 6e63  m max_concurrenc
+00005320: 793a 204d 6178 2064 6f77 6e6c 6f61 6420  y: Max download 
+00005330: 7468 7265 6164 206e 756d 6265 722c 204e  thread number, N
+00005340: 6f6e 6520 6279 2064 6566 6175 6c74 0a20  one by default. 
+00005350: 2020 203a 7061 7261 6d20 6d61 785f 626c     :param max_bl
+00005360: 6f63 6b5f 7369 7a65 3a20 4d61 7820 6461  ock_size: Max da
+00005370: 7461 2073 697a 6520 646f 776e 6c6f 6164  ta size download
+00005380: 6564 2062 7920 6561 6368 2074 6872 6561  ed by each threa
+00005390: 642c 2069 6e20 6279 7465 732c 2038 4d42  d, in bytes, 8MB
+000053a0: 2062 7920 6465 6661 756c 740a 2020 2020   by default.    
+000053b0: 3a72 6574 7572 6e73 3a20 416e 206f 7065  :returns: An ope
+000053c0: 6e65 6420 5333 5368 6172 6543 6163 6865  ned S3ShareCache
+000053d0: 5265 6164 6572 206f 626a 6563 740a 2020  Reader object.  
+000053e0: 2020 3a72 6169 7365 733a 2053 3346 696c    :raises: S3Fil
+000053f0: 654e 6f74 466f 756e 6445 7272 6f72 0a20  eNotFoundError. 
+00005400: 2020 2027 2727 0a20 2020 2069 6620 6d6f     '''.    if mo
+00005410: 6465 2021 3d20 2772 6227 3a0a 2020 2020  de != 'rb':.    
+00005420: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00005430: 7272 6f72 2827 756e 6163 6365 7074 6162  rror('unacceptab
+00005440: 6c65 206d 6f64 653a 2025 7227 2025 206d  le mode: %r' % m
+00005450: 6f64 6529 0a0a 2020 2020 7333 5f75 726c  ode)..    s3_url
+00005460: 203d 2053 3350 6174 6828 7333 5f75 726c   = S3Path(s3_url
+00005470: 290a 2020 2020 6966 2066 6f6c 6c6f 776c  ).    if followl
+00005480: 696e 6b73 3a0a 2020 2020 2020 2020 7472  inks:.        tr
+00005490: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+000054a0: 335f 7572 6c20 3d20 7333 5f75 726c 2e72  3_url = s3_url.r
+000054b0: 6561 646c 696e 6b28 290a 2020 2020 2020  eadlink().      
+000054c0: 2020 6578 6365 7074 2053 334e 6f74 414c    except S3NotAL
+000054d0: 696e 6b45 7272 6f72 3a0a 2020 2020 2020  inkError:.      
+000054e0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000054f0: 6275 636b 6574 2c20 6b65 7920 3d20 7061  bucket, key = pa
+00005500: 7273 655f 7333 5f75 726c 2873 335f 7572  rse_s3_url(s3_ur
+00005510: 6c2e 7061 7468 5f77 6974 685f 7072 6f74  l.path_with_prot
+00005520: 6f63 6f6c 290a 2020 2020 636f 6e66 6967  ocol).    config
+00005530: 203d 2062 6f74 6f63 6f72 652e 636f 6e66   = botocore.conf
+00005540: 6967 2e43 6f6e 6669 6728 6d61 785f 706f  ig.Config(max_po
+00005550: 6f6c 5f63 6f6e 6e65 6374 696f 6e73 3d6d  ol_connections=m
+00005560: 6178 5f70 6f6f 6c5f 636f 6e6e 6563 7469  ax_pool_connecti
+00005570: 6f6e 7329 0a20 2020 2063 6c69 656e 7420  ons).    client 
+00005580: 3d20 6765 745f 7333 5f63 6c69 656e 7428  = get_s3_client(
+00005590: 0a20 2020 2020 2020 2063 6f6e 6669 673d  .        config=
+000055a0: 636f 6e66 6967 2c0a 2020 2020 2020 2020  config,.        
+000055b0: 6361 6368 655f 6b65 793d 2773 335f 6669  cache_key='s3_fi
+000055c0: 6c65 6c69 6b65 5f63 6c69 656e 7427 2c0a  lelike_client',.
+000055d0: 2020 2020 2020 2020 7072 6f66 696c 655f          profile_
+000055e0: 6e61 6d65 3d73 335f 7572 6c2e 5f70 726f  name=s3_url._pro
+000055f0: 6669 6c65 5f6e 616d 6529 0a20 2020 2072  file_name).    r
+00005600: 6574 7572 6e20 5333 5368 6172 6543 6163  eturn S3ShareCac
+00005610: 6865 5265 6164 6572 280a 2020 2020 2020  heReader(.      
+00005620: 2020 6275 636b 6574 2c0a 2020 2020 2020    bucket,.      
+00005630: 2020 6b65 792c 0a20 2020 2020 2020 2063    key,.        c
+00005640: 6163 6865 5f6b 6579 3d63 6163 6865 5f6b  ache_key=cache_k
+00005650: 6579 2c0a 2020 2020 2020 2020 7333 5f63  ey,.        s3_c
+00005660: 6c69 656e 743d 636c 6965 6e74 2c0a 2020  lient=client,.  
+00005670: 2020 2020 2020 6d61 785f 7265 7472 6965        max_retrie
+00005680: 733d 6d61 785f 7265 7472 6965 732c 0a20  s=max_retries,. 
+00005690: 2020 2020 2020 206d 6178 5f77 6f72 6b65         max_worke
+000056a0: 7273 3d6d 6178 5f63 6f6e 6375 7272 656e  rs=max_concurren
+000056b0: 6379 2c0a 2020 2020 2020 2020 626c 6f63  cy,.        bloc
+000056c0: 6b5f 7369 7a65 3d6d 6178 5f62 6c6f 636b  k_size=max_block
+000056d0: 5f73 697a 6529 0a0a 0a40 5f73 335f 6269  _size)...@_s3_bi
+000056e0: 6e61 7279 5f6d 6f64 650a 6465 6620 7333  nary_mode.def s3
+000056f0: 5f70 6970 655f 6f70 656e 280a 2020 2020  _pipe_open(.    
+00005700: 2020 2020 7333 5f75 726c 3a20 5061 7468      s3_url: Path
+00005710: 4c69 6b65 2c0a 2020 2020 2020 2020 6d6f  Like,.        mo
+00005720: 6465 3a20 7374 722c 0a20 2020 2020 2020  de: str,.       
+00005730: 2066 6f6c 6c6f 776c 696e 6b73 3a20 626f   followlinks: bo
+00005740: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00005750: 2020 2020 2a2c 0a20 2020 2020 2020 206a      *,.        j
+00005760: 6f69 6e5f 7468 7265 6164 3a20 626f 6f6c  oin_thread: bool
+00005770: 203d 2054 7275 6529 202d 3e20 5333 5069   = True) -> S3Pi
+00005780: 7065 4861 6e64 6c65 723a 0a20 2020 2027  peHandler:.    '
+00005790: 2727 4f70 656e 2061 2061 7379 6e63 6872  ''Open a asynchr
+000057a0: 6f6e 6f75 7320 7265 6164 2d77 7269 7465  onous read-write
+000057b0: 2072 6561 6465 7220 2f20 7772 6974 6572   reader / writer
+000057c0: 2c20 746f 2073 7570 706f 7274 2066 6173  , to support fas
+000057d0: 7420 7365 7175 656e 7469 616c 2072 6561  t sequential rea
+000057e0: 6420 2f20 7772 6974 650a 0a20 2020 202e  d / write..    .
+000057f0: 2e20 6e6f 7465 203a 3a0a 0a20 2020 2020  . note ::..     
+00005800: 2020 2055 7365 7220 7368 6f75 6c64 206d     User should m
+00005810: 616b 6520 7375 7265 2074 6861 7420 7265  ake sure that re
+00005820: 6164 6572 202f 2077 7269 7465 7220 6172  ader / writer ar
+00005830: 6520 636c 6f73 6564 2063 6f72 7265 6374  e closed correct
+00005840: 6c79 0a0a 2020 2020 2020 2020 5375 7070  ly..        Supp
+00005850: 6f72 7473 2063 6f6e 7465 7874 206d 616e  orts context man
+00005860: 6167 6572 0a0a 2020 2020 2020 2020 5768  ager..        Wh
+00005870: 656e 206a 6f69 6e5f 7468 7265 6164 2069  en join_thread i
+00005880: 7320 4661 6c73 652c 2077 6869 6c65 2074  s False, while t
+00005890: 6865 2066 696c 6520 6861 6e64 6c65 2061  he file handle a
+000058a0: 7265 2063 6c6f 7369 6e67 2c20 7468 6973  re closing, this
+000058b0: 2066 756e 6374 696f 6e20 7769 6c6c 206e   function will n
+000058c0: 6f74 2077 6169 7420 756e 7469 6c20 7468  ot wait until th
+000058d0: 6520 6173 796e 6368 726f 6e6f 7573 2077  e asynchronous w
+000058e0: 7269 7469 6e67 2066 696e 6973 6865 733b  riting finishes;
+000058f0: 0a20 2020 2020 2020 2046 616c 7365 2064  .        False d
+00005900: 6f65 736e 2774 2061 6666 6563 7420 7265  oesn't affect re
+00005910: 6164 2d68 616e 646c 652c 2062 7574 2074  ad-handle, but t
+00005920: 6869 7320 6361 6e20 7370 6565 6420 7570  his can speed up
+00005930: 2077 7269 7465 2d68 616e 646c 6520 6265   write-handle be
+00005940: 6361 7573 6520 6669 6c65 2077 696c 6c20  cause file will 
+00005950: 6265 2077 7269 7474 656e 2061 7379 6e63  be written async
+00005960: 6872 6f6e 6f75 736c 792e 0a20 2020 2020  hronously..     
+00005970: 2020 2042 7574 2061 7379 6e63 6872 6f6e     But asynchron
+00005980: 6f75 7320 6265 6861 7669 6f75 7220 6361  ous behaviour ca
+00005990: 6e20 6775 6172 616e 7465 6520 7468 6520  n guarantee the 
+000059a0: 6669 6c65 2061 7265 2073 7563 6365 7373  file are success
+000059b0: 6675 6c6c 7920 7772 6974 7465 6e2c 2061  fully written, a
+000059c0: 6e64 2066 7265 7175 656e 7420 6578 6563  nd frequent exec
+000059d0: 7574 696f 6e20 6d61 7920 6361 7573 6520  ution may cause 
+000059e0: 7468 7265 6164 2061 6e64 2066 696c 6520  thread and file 
+000059f0: 6861 6e64 6c65 2065 7868 6175 7374 696f  handle exhaustio
+00005a00: 6e0a 0a20 2020 203a 7061 7261 6d20 6d6f  n..    :param mo
+00005a10: 6465 3a20 4d6f 6465 2074 6f20 6f70 656e  de: Mode to open
+00005a20: 2066 696c 652c 2065 6974 6865 7220 2272   file, either "r
+00005a30: 6222 206f 7220 2277 6222 0a20 2020 203a  b" or "wb".    :
+00005a40: 7061 7261 6d20 6a6f 696e 5f74 6872 6561  param join_threa
+00005a50: 643a 2049 6620 7761 6974 2061 6674 6572  d: If wait after
+00005a60: 2066 756e 6374 696f 6e20 6578 6563 7574   function execut
+00005a70: 696f 6e20 756e 7469 6c20 7333 2066 696e  ion until s3 fin
+00005a80: 6973 6865 7320 7772 6974 696e 670a 2020  ishes writing.  
+00005a90: 2020 3a72 6574 7572 6e73 3a20 416e 206f    :returns: An o
+00005aa0: 7065 6e65 6420 4275 6666 6572 6564 5265  pened BufferedRe
+00005ab0: 6164 6572 202f 2042 7566 6665 7265 6457  ader / BufferedW
+00005ac0: 7269 7465 7220 6f62 6a65 6374 0a20 2020  riter object.   
+00005ad0: 2027 2727 0a20 2020 2069 6620 6d6f 6465   '''.    if mode
+00005ae0: 206e 6f74 2069 6e20 2827 7262 272c 2027   not in ('rb', '
+00005af0: 7762 2729 3a0a 2020 2020 2020 2020 7261  wb'):.        ra
+00005b00: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00005b10: 756e 6163 6365 7074 6162 6c65 206d 6f64  unacceptable mod
+00005b20: 653a 2025 7227 2025 206d 6f64 6529 0a0a  e: %r' % mode)..
+00005b30: 2020 2020 6966 206d 6f64 655b 305d 203d      if mode[0] =
+00005b40: 3d20 2772 2720 616e 6420 6e6f 7420 5333  = 'r' and not S3
+00005b50: 5061 7468 2873 335f 7572 6c29 2e69 735f  Path(s3_url).is_
+00005b60: 6669 6c65 2829 3a0a 2020 2020 2020 2020  file():.        
+00005b70: 7261 6973 6520 5333 4669 6c65 4e6f 7446  raise S3FileNotF
+00005b80: 6f75 6e64 4572 726f 7228 274e 6f20 7375  oundError('No su
+00005b90: 6368 2066 696c 653a 2025 7227 2025 2073  ch file: %r' % s
+00005ba0: 335f 7572 6c29 0a0a 2020 2020 7333 5f75  3_url)..    s3_u
+00005bb0: 726c 203d 2053 3350 6174 6828 7333 5f75  rl = S3Path(s3_u
+00005bc0: 726c 290a 2020 2020 6966 2066 6f6c 6c6f  rl).    if follo
+00005bd0: 776c 696e 6b73 3a0a 2020 2020 2020 2020  wlinks:.        
+00005be0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00005bf0: 2073 335f 7572 6c20 3d20 7333 5f75 726c   s3_url = s3_url
+00005c00: 2e72 6561 646c 696e 6b28 290a 2020 2020  .readlink().    
+00005c10: 2020 2020 6578 6365 7074 2053 334e 6f74      except S3Not
+00005c20: 414c 696e 6b45 7272 6f72 3a0a 2020 2020  ALinkError:.    
+00005c30: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00005c40: 2020 6275 636b 6574 2c20 6b65 7920 3d20    bucket, key = 
+00005c50: 7061 7273 655f 7333 5f75 726c 2873 335f  parse_s3_url(s3_
+00005c60: 7572 6c2e 7061 7468 5f77 6974 685f 7072  url.path_with_pr
+00005c70: 6f74 6f63 6f6c 290a 2020 2020 636f 6e66  otocol).    conf
+00005c80: 6967 203d 2062 6f74 6f63 6f72 652e 636f  ig = botocore.co
+00005c90: 6e66 6967 2e43 6f6e 6669 6728 6d61 785f  nfig.Config(max_
+00005ca0: 706f 6f6c 5f63 6f6e 6e65 6374 696f 6e73  pool_connections
+00005cb0: 3d6d 6178 5f70 6f6f 6c5f 636f 6e6e 6563  =max_pool_connec
+00005cc0: 7469 6f6e 7329 0a20 2020 2063 6c69 656e  tions).    clien
+00005cd0: 7420 3d20 6765 745f 7333 5f63 6c69 656e  t = get_s3_clien
+00005ce0: 7428 0a20 2020 2020 2020 2063 6f6e 6669  t(.        confi
+00005cf0: 673d 636f 6e66 6967 2c0a 2020 2020 2020  g=config,.      
+00005d00: 2020 6361 6368 655f 6b65 793d 2773 335f    cache_key='s3_
+00005d10: 6669 6c65 6c69 6b65 5f63 6c69 656e 7427  filelike_client'
+00005d20: 2c0a 2020 2020 2020 2020 7072 6f66 696c  ,.        profil
+00005d30: 655f 6e61 6d65 3d73 335f 7572 6c2e 5f70  e_name=s3_url._p
+00005d40: 726f 6669 6c65 5f6e 616d 6529 0a20 2020  rofile_name).   
+00005d50: 2072 6574 7572 6e20 5333 5069 7065 4861   return S3PipeHa
+00005d60: 6e64 6c65 7228 0a20 2020 2020 2020 2062  ndler(.        b
+00005d70: 7563 6b65 742c 206b 6579 2c20 6d6f 6465  ucket, key, mode
+00005d80: 2c20 7333 5f63 6c69 656e 743d 636c 6965  , s3_client=clie
+00005d90: 6e74 2c20 6a6f 696e 5f74 6872 6561 643d  nt, join_thread=
+00005da0: 6a6f 696e 5f74 6872 6561 6429 0a0a 0a40  join_thread)...@
+00005db0: 5f73 335f 6269 6e61 7279 5f6d 6f64 650a  _s3_binary_mode.
+00005dc0: 6465 6620 7333 5f63 6163 6865 645f 6f70  def s3_cached_op
+00005dd0: 656e 280a 2020 2020 2020 2020 7333 5f75  en(.        s3_u
+00005de0: 726c 3a20 5061 7468 4c69 6b65 2c0a 2020  rl: PathLike,.  
+00005df0: 2020 2020 2020 6d6f 6465 3a20 7374 722c        mode: str,
+00005e00: 0a20 2020 2020 2020 2066 6f6c 6c6f 776c  .        followl
+00005e10: 696e 6b73 3a20 626f 6f6c 203d 2046 616c  inks: bool = Fal
+00005e20: 7365 2c0a 2020 2020 2020 2020 2a2c 0a20  se,.        *,. 
+00005e30: 2020 2020 2020 2063 6163 6865 5f70 6174         cache_pat
+00005e40: 683a 204f 7074 696f 6e61 6c5b 7374 725d  h: Optional[str]
+00005e50: 203d 204e 6f6e 6529 202d 3e20 5333 4361   = None) -> S3Ca
+00005e60: 6368 6564 4861 6e64 6c65 723a 0a20 2020  chedHandler:.   
+00005e70: 2027 2727 4f70 656e 2061 206c 6f63 616c   '''Open a local
+00005e80: 2d63 6163 6865 2066 696c 6520 7265 6164  -cache file read
+00005e90: 6572 202f 2077 7269 7465 722c 2066 6f72  er / writer, for
+00005ea0: 2066 7265 7175 656e 7420 7261 6e64 6f6d   frequent random
+00005eb0: 2072 6561 6420 2f20 7772 6974 650a 0a20   read / write.. 
+00005ec0: 2020 202e 2e20 6e6f 7465 203a 3a0a 0a20     .. note ::.. 
+00005ed0: 2020 2020 2020 2055 7365 7220 7368 6f75         User shou
+00005ee0: 6c64 206d 616b 6520 7375 7265 2074 6861  ld make sure tha
+00005ef0: 7420 7265 6164 6572 202f 2077 7269 7465  t reader / write
+00005f00: 7220 6172 6520 636c 6f73 6564 2063 6f72  r are closed cor
+00005f10: 7265 6374 6c79 0a0a 2020 2020 2020 2020  rectly..        
+00005f20: 5375 7070 6f72 7473 2063 6f6e 7465 7874  Supports context
+00005f30: 206d 616e 6167 6572 0a0a 2020 2020 2020   manager..      
+00005f40: 2020 6361 6368 655f 7061 7468 2063 616e    cache_path can
+00005f50: 2073 7065 6369 6679 2074 6865 2070 6174   specify the pat
+00005f60: 6820 6f66 2063 6163 6865 2066 696c 652e  h of cache file.
+00005f70: 2050 6572 666f 726d 616e 6365 2063 6f75   Performance cou
+00005f80: 6c64 2062 6520 6265 7474 6572 2069 6620  ld be better if 
+00005f90: 6361 6368 6520 6669 6c65 2070 6174 6820  cache file path 
+00005fa0: 6973 206f 6e20 7373 6420 6f72 2074 6d70  is on ssd or tmp
+00005fb0: 6673 0a0a 2020 2020 3a70 6172 616d 206d  fs..    :param m
+00005fc0: 6f64 653a 204d 6f64 6520 746f 206f 7065  ode: Mode to ope
+00005fd0: 6e20 6669 6c65 2c20 636f 756c 6420 6265  n file, could be
+00005fe0: 206f 6e65 206f 6620 2272 6222 2c20 2277   one of "rb", "w
+00005ff0: 6222 206f 7220 2261 6222 0a20 2020 203a  b" or "ab".    :
+00006000: 7061 7261 6d20 6361 6368 655f 7061 7468  param cache_path
+00006010: 3a20 6361 6368 6520 6669 6c65 2070 6174  : cache file pat
+00006020: 680a 2020 2020 3a72 6574 7572 6e73 3a20  h.    :returns: 
+00006030: 416e 206f 7065 6e65 6420 4275 6666 6572  An opened Buffer
+00006040: 6564 5265 6164 6572 202f 2042 7566 6665  edReader / Buffe
+00006050: 7265 6457 7269 7465 7220 6f62 6a65 6374  redWriter object
+00006060: 0a20 2020 2027 2727 0a20 2020 2069 6620  .    '''.    if 
+00006070: 6d6f 6465 206e 6f74 2069 6e20 2827 7262  mode not in ('rb
+00006080: 272c 2027 7762 272c 2027 6162 272c 2027  ', 'wb', 'ab', '
+00006090: 7262 2b27 2c20 2777 622b 272c 2027 6162  rb+', 'wb+', 'ab
+000060a0: 2b27 293a 0a20 2020 2020 2020 2072 6169  +'):.        rai
+000060b0: 7365 2056 616c 7565 4572 726f 7228 2775  se ValueError('u
+000060c0: 6e61 6363 6570 7461 626c 6520 6d6f 6465  nacceptable mode
+000060d0: 3a20 2572 2720 2520 6d6f 6465 290a 2020  : %r' % mode).  
+000060e0: 2020 7333 5f75 726c 203d 2053 3350 6174    s3_url = S3Pat
+000060f0: 6828 7333 5f75 726c 290a 2020 2020 6966  h(s3_url).    if
+00006100: 2066 6f6c 6c6f 776c 696e 6b73 3a0a 2020   followlinks:.  
+00006110: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00006120: 2020 2020 2020 2073 335f 7572 6c20 3d20         s3_url = 
+00006130: 7333 5f75 726c 2e72 6561 646c 696e 6b28  s3_url.readlink(
+00006140: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00006150: 2053 334e 6f74 414c 696e 6b45 7272 6f72   S3NotALinkError
+00006160: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00006170: 7373 0a0a 2020 2020 6275 636b 6574 2c20  ss..    bucket, 
+00006180: 6b65 7920 3d20 7061 7273 655f 7333 5f75  key = parse_s3_u
+00006190: 726c 2873 335f 7572 6c2e 7061 7468 5f77  rl(s3_url.path_w
+000061a0: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
+000061b0: 2020 636f 6e66 6967 203d 2062 6f74 6f63    config = botoc
+000061c0: 6f72 652e 636f 6e66 6967 2e43 6f6e 6669  ore.config.Confi
+000061d0: 6728 6d61 785f 706f 6f6c 5f63 6f6e 6e65  g(max_pool_conne
+000061e0: 6374 696f 6e73 3d6d 6178 5f70 6f6f 6c5f  ctions=max_pool_
+000061f0: 636f 6e6e 6563 7469 6f6e 7329 0a20 2020  connections).   
+00006200: 2063 6c69 656e 7420 3d20 6765 745f 7333   client = get_s3
+00006210: 5f63 6c69 656e 7428 0a20 2020 2020 2020  _client(.       
+00006220: 2063 6f6e 6669 673d 636f 6e66 6967 2c0a   config=config,.
+00006230: 2020 2020 2020 2020 6361 6368 655f 6b65          cache_ke
+00006240: 793d 2773 335f 6669 6c65 6c69 6b65 5f63  y='s3_filelike_c
+00006250: 6c69 656e 7427 2c0a 2020 2020 2020 2020  lient',.        
+00006260: 7072 6f66 696c 655f 6e61 6d65 3d73 335f  profile_name=s3_
+00006270: 7572 6c2e 5f70 726f 6669 6c65 5f6e 616d  url._profile_nam
+00006280: 6529 0a20 2020 2072 6574 7572 6e20 5333  e).    return S3
+00006290: 4361 6368 6564 4861 6e64 6c65 7228 0a20  CachedHandler(. 
+000062a0: 2020 2020 2020 2062 7563 6b65 742c 206b         bucket, k
+000062b0: 6579 2c20 6d6f 6465 2c20 7333 5f63 6c69  ey, mode, s3_cli
+000062c0: 656e 743d 636c 6965 6e74 2c20 6361 6368  ent=client, cach
+000062d0: 655f 7061 7468 3d63 6163 6865 5f70 6174  e_path=cache_pat
+000062e0: 6829 0a0a 0a40 5f73 335f 6269 6e61 7279  h)...@_s3_binary
+000062f0: 5f6d 6f64 650a 6465 6620 7333 5f62 7566  _mode.def s3_buf
+00006300: 6665 7265 645f 6f70 656e 280a 2020 2020  fered_open(.    
+00006310: 2020 2020 7333 5f75 726c 3a20 5061 7468      s3_url: Path
+00006320: 4c69 6b65 2c0a 2020 2020 2020 2020 6d6f  Like,.        mo
+00006330: 6465 3a20 7374 722c 0a20 2020 2020 2020  de: str,.       
+00006340: 2066 6f6c 6c6f 776c 696e 6b73 3a20 626f   followlinks: bo
+00006350: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00006360: 2020 2020 2a2c 0a20 2020 2020 2020 206d      *,.        m
+00006370: 6178 5f63 6f6e 6375 7272 656e 6379 3a20  ax_concurrency: 
+00006380: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00006390: 4e6f 6e65 2c0a 2020 2020 2020 2020 6d61  None,.        ma
+000063a0: 785f 6275 6666 6572 5f73 697a 653a 2069  x_buffer_size: i
+000063b0: 6e74 203d 2044 4546 4155 4c54 5f4d 4158  nt = DEFAULT_MAX
+000063c0: 5f42 5546 4645 525f 5349 5a45 2c0a 2020  _BUFFER_SIZE,.  
+000063d0: 2020 2020 2020 666f 7277 6172 645f 7261        forward_ra
+000063e0: 7469 6f3a 204f 7074 696f 6e61 6c5b 666c  tio: Optional[fl
+000063f0: 6f61 745d 203d 204e 6f6e 652c 0a20 2020  oat] = None,.   
+00006400: 2020 2020 2062 6c6f 636b 5f73 697a 653a       block_size:
+00006410: 2069 6e74 203d 2044 4546 4155 4c54 5f42   int = DEFAULT_B
+00006420: 4c4f 434b 5f53 495a 452c 0a20 2020 2020  LOCK_SIZE,.     
+00006430: 2020 206c 696d 6974 6564 5f73 6565 6b61     limited_seeka
+00006440: 626c 653a 2062 6f6f 6c20 3d20 4661 6c73  ble: bool = Fals
+00006450: 652c 0a20 2020 2020 2020 2062 7566 6665  e,.        buffe
+00006460: 7265 643a 2062 6f6f 6c20 3d20 5472 7565  red: bool = True
+00006470: 2c0a 2020 2020 2020 2020 7368 6172 655f  ,.        share_
+00006480: 6361 6368 655f 6b65 793a 204f 7074 696f  cache_key: Optio
+00006490: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+000064a0: 0a20 2020 2020 2020 2063 6163 6865 5f70  .        cache_p
+000064b0: 6174 683a 204f 7074 696f 6e61 6c5b 7374  ath: Optional[st
+000064c0: 725d 203d 204e 6f6e 650a 2920 2d3e 2055  r] = None.) -> U
+000064d0: 6e69 6f6e 5b53 3350 7265 6665 7463 6852  nion[S3PrefetchR
+000064e0: 6561 6465 722c 2053 3342 7566 6665 7265  eader, S3Buffere
+000064f0: 6457 7269 7465 722c 2069 6f2e 4275 6666  dWriter, io.Buff
+00006500: 6572 6564 5265 6164 6572 2c20 696f 2e0a  eredReader, io..
+00006510: 2020 2020 2020 2020 2020 2042 7566 6665             Buffe
+00006520: 7265 6457 7269 7465 722c 2053 334d 656d  redWriter, S3Mem
+00006530: 6f72 7948 616e 646c 6572 5d3a 0a20 2020  oryHandler]:.   
+00006540: 2027 2727 4f70 656e 2061 6e20 6173 796e   '''Open an asyn
+00006550: 6368 726f 6e6f 7573 2070 7265 6665 7463  chronous prefetc
+00006560: 6820 7265 6164 6572 2c20 746f 2073 7570  h reader, to sup
+00006570: 706f 7274 2066 6173 7420 7365 7175 656e  port fast sequen
+00006580: 7469 616c 2072 6561 640a 0a20 2020 202e  tial read..    .
+00006590: 2e20 6e6f 7465 203a 3a0a 0a20 2020 2020  . note ::..     
+000065a0: 2020 2055 7365 7220 7368 6f75 6c64 206d     User should m
+000065b0: 616b 6520 7375 7265 2074 6861 7420 7265  ake sure that re
+000065c0: 6164 6572 202f 2077 7269 7465 7220 6172  ader / writer ar
+000065d0: 6520 636c 6f73 6564 2063 6f72 7265 6374  e closed correct
+000065e0: 6c79 0a0a 2020 2020 2020 2020 5375 7070  ly..        Supp
+000065f0: 6f72 7473 2063 6f6e 7465 7874 206d 616e  orts context man
+00006600: 6167 6572 0a0a 2020 2020 2020 2020 536f  ager..        So
+00006610: 6d65 2070 6172 616d 6574 6572 2073 6574  me parameter set
+00006620: 7469 6e67 206d 6179 2070 6572 666f 726d  ting may perform
+00006630: 2077 656c 6c3a 206d 6178 5f63 6f6e 6375   well: max_concu
+00006640: 7272 656e 6379 3d31 3020 6f72 2032 302c  rrency=10 or 20,
+00006650: 206d 6178 5f62 6c6f 636b 5f73 697a 653d   max_block_size=
+00006660: 3820 6f72 2031 3620 4d42 2c20 6465 6661  8 or 16 MB, defa
+00006670: 756c 7420 7661 6c75 6520 4e6f 6e65 206d  ult value None m
+00006680: 6561 6e73 2075 7369 6e67 2067 6c6f 6261  eans using globa
+00006690: 6c20 7468 7265 6164 2070 6f6f 6c0a 0a20  l thread pool.. 
+000066a0: 2020 203a 7061 7261 6d20 6d61 785f 636f     :param max_co
+000066b0: 6e63 7572 7265 6e63 793a 204d 6178 2064  ncurrency: Max d
+000066c0: 6f77 6e6c 6f61 6420 7468 7265 6164 206e  ownload thread n
+000066d0: 756d 6265 722c 204e 6f6e 6520 6279 2064  umber, None by d
+000066e0: 6566 6175 6c74 0a20 2020 203a 7061 7261  efault.    :para
+000066f0: 6d20 6d61 785f 6275 6666 6572 5f73 697a  m max_buffer_siz
+00006700: 653a 204d 6178 2063 6163 6865 6420 6275  e: Max cached bu
+00006710: 6666 6572 2073 697a 6520 696e 206d 656d  ffer size in mem
+00006720: 6f72 792c 2031 3238 4d42 2062 7920 6465  ory, 128MB by de
+00006730: 6661 756c 740a 2020 2020 3a70 6172 616d  fault.    :param
+00006740: 2062 6c6f 636b 5f73 697a 653a 2053 697a   block_size: Siz
+00006750: 6520 6f66 2073 696e 676c 6520 626c 6f63  e of single bloc
+00006760: 6b2c 2038 4d42 2062 7920 6465 6661 756c  k, 8MB by defaul
+00006770: 742e 2045 6163 6820 626c 6f63 6b20 7769  t. Each block wi
+00006780: 6c6c 2062 6520 7570 6c6f 6164 6564 206f  ll be uploaded o
+00006790: 7220 646f 776e 6c6f 6164 6564 2062 7920  r downloaded by 
+000067a0: 7369 6e67 6c65 2074 6872 6561 642e 0a20  single thread.. 
+000067b0: 2020 203a 7061 7261 6d20 6c69 6d69 7465     :param limite
+000067c0: 645f 7365 656b 6162 6c65 3a20 4966 2077  d_seekable: If w
+000067d0: 7269 7465 2d68 616e 646c 6520 7375 7070  rite-handle supp
+000067e0: 6f72 7473 206c 696d 6974 6564 2073 6565  orts limited see
+000067f0: 6b20 2862 6f74 6820 6669 6c65 2068 6561  k (both file hea
+00006800: 6420 7061 7274 2061 6e64 2074 6169 6c20  d part and tail 
+00006810: 7061 7274 2063 616e 2073 6565 6b20 626c  part can seek bl
+00006820: 6f63 6b5f 7369 7a65 292e 204e 6f74 6573  ock_size). Notes
+00006830: 3a20 5468 6973 2070 6172 616d 6574 6572  : This parameter
+00006840: 2061 7265 2076 616c 6964 206f 6e6c 7920   are valid only 
+00006850: 666f 7220 7772 6974 652d 6861 6e64 6c65  for write-handle
+00006860: 2e20 5265 6164 2d68 616e 646c 6520 7375  . Read-handle su
+00006870: 7070 6f72 7420 6172 6269 7472 6172 7920  pport arbitrary 
+00006880: 7365 656b 0a20 2020 203a 7265 7475 726e  seek.    :return
+00006890: 733a 2041 6e20 6f70 656e 6564 2053 3350  s: An opened S3P
+000068a0: 7265 6665 7463 6852 6561 6465 7220 6f62  refetchReader ob
+000068b0: 6a65 6374 0a20 2020 203a 7261 6973 6573  ject.    :raises
+000068c0: 3a20 5333 4669 6c65 4e6f 7446 6f75 6e64  : S3FileNotFound
+000068d0: 4572 726f 720a 2020 2020 2727 270a 2020  Error.    '''.  
+000068e0: 2020 6966 206d 6f64 6520 6e6f 7420 696e    if mode not in
+000068f0: 2028 2772 6227 2c20 2777 6227 2c20 2761   ('rb', 'wb', 'a
+00006900: 6227 2c20 2772 622b 272c 2027 7762 2b27  b', 'rb+', 'wb+'
+00006910: 2c20 2761 622b 2729 3a0a 2020 2020 2020  , 'ab+'):.      
+00006920: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00006930: 6f72 2827 756e 6163 6365 7074 6162 6c65  or('unacceptable
+00006940: 206d 6f64 653a 2025 7227 2025 206d 6f64   mode: %r' % mod
+00006950: 6529 0a20 2020 2073 335f 7572 6c20 3d20  e).    s3_url = 
+00006960: 5333 5061 7468 2873 335f 7572 6c29 0a20  S3Path(s3_url). 
+00006970: 2020 2069 6620 666f 6c6c 6f77 6c69 6e6b     if followlink
+00006980: 733a 0a20 2020 2020 2020 2074 7279 3a0a  s:.        try:.
+00006990: 2020 2020 2020 2020 2020 2020 7333 5f75              s3_u
+000069a0: 726c 203d 2073 335f 7572 6c2e 7265 6164  rl = s3_url.read
+000069b0: 6c69 6e6b 2829 0a20 2020 2020 2020 2065  link().        e
+000069c0: 7863 6570 7420 5333 4e6f 7441 4c69 6e6b  xcept S3NotALink
+000069d0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+000069e0: 2020 2070 6173 730a 0a20 2020 2062 7563     pass..    buc
+000069f0: 6b65 742c 206b 6579 203d 2070 6172 7365  ket, key = parse
+00006a00: 5f73 335f 7572 6c28 7333 5f75 726c 2e70  _s3_url(s3_url.p
+00006a10: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
+00006a20: 6c29 0a20 2020 2063 6f6e 6669 6720 3d20  l).    config = 
+00006a30: 626f 746f 636f 7265 2e63 6f6e 6669 672e  botocore.config.
+00006a40: 436f 6e66 6967 286d 6178 5f70 6f6f 6c5f  Config(max_pool_
+00006a50: 636f 6e6e 6563 7469 6f6e 733d 6d61 785f  connections=max_
+00006a60: 706f 6f6c 5f63 6f6e 6e65 6374 696f 6e73  pool_connections
+00006a70: 290a 2020 2020 636c 6965 6e74 203d 2067  ).    client = g
+00006a80: 6574 5f73 335f 636c 6965 6e74 280a 2020  et_s3_client(.  
+00006a90: 2020 2020 2020 636f 6e66 6967 3d63 6f6e        config=con
+00006aa0: 6669 672c 0a20 2020 2020 2020 2063 6163  fig,.        cac
+00006ab0: 6865 5f6b 6579 3d27 7333 5f66 696c 656c  he_key='s3_filel
+00006ac0: 696b 655f 636c 6965 6e74 272c 0a20 2020  ike_client',.   
+00006ad0: 2020 2020 2070 726f 6669 6c65 5f6e 616d       profile_nam
+00006ae0: 653d 7333 5f75 726c 2e5f 7072 6f66 696c  e=s3_url._profil
+00006af0: 655f 6e61 6d65 290a 0a20 2020 2069 6620  e_name)..    if 
+00006b00: 2761 2720 696e 206d 6f64 6520 6f72 2027  'a' in mode or '
+00006b10: 2b27 2069 6e20 6d6f 6465 3a0a 2020 2020  +' in mode:.    
+00006b20: 2020 2020 6966 2063 6163 6865 5f70 6174      if cache_pat
+00006b30: 6820 6973 204e 6f6e 653a 0a20 2020 2020  h is None:.     
+00006b40: 2020 2020 2020 2072 6574 7572 6e20 5333         return S3
+00006b50: 4d65 6d6f 7279 4861 6e64 6c65 7228 6275  MemoryHandler(bu
+00006b60: 636b 6574 2c20 6b65 792c 206d 6f64 652c  cket, key, mode,
+00006b70: 2073 335f 636c 6965 6e74 3d63 6c69 656e   s3_client=clien
+00006b80: 7429 0a20 2020 2020 2020 2072 6574 7572  t).        retur
+00006b90: 6e20 5333 4361 6368 6564 4861 6e64 6c65  n S3CachedHandle
+00006ba0: 7228 0a20 2020 2020 2020 2020 2020 2062  r(.            b
+00006bb0: 7563 6b65 742c 206b 6579 2c20 6d6f 6465  ucket, key, mode
+00006bc0: 2c20 7333 5f63 6c69 656e 743d 636c 6965  , s3_client=clie
+00006bd0: 6e74 2c20 6361 6368 655f 7061 7468 3d63  nt, cache_path=c
+00006be0: 6163 6865 5f70 6174 6829 0a0a 2020 2020  ache_path)..    
+00006bf0: 6966 206d 6f64 6520 3d3d 2027 7262 273a  if mode == 'rb':
+00006c00: 0a20 2020 2020 2020 2023 2041 2072 6f75  .        # A rou
+00006c10: 6768 2063 6f6e 7665 7273 696f 6e20 616c  gh conversion al
+00006c20: 676f 7269 7468 6d20 746f 2061 6c69 676e  gorithm to align
+00006c30: 2032 2074 7970 6573 206f 6620 5265 6164   2 types of Read
+00006c40: 6572 202f 2057 7269 7465 7220 7061 7261  er / Writer para
+00006c50: 6d65 7465 7273 0a20 2020 2020 2020 2023  meters.        #
+00006c60: 2054 4f44 4f3a 204f 7074 696d 697a 6520   TODO: Optimize 
+00006c70: 7468 6520 636f 6e76 6572 7369 6f6e 2061  the conversion a
+00006c80: 6c67 6f72 6974 686d 0a20 2020 2020 2020  lgorithm.       
+00006c90: 2062 6c6f 636b 5f63 6170 6163 6974 7920   block_capacity 
+00006ca0: 3d20 6d61 785f 6275 6666 6572 5f73 697a  = max_buffer_siz
+00006cb0: 6520 2f2f 2062 6c6f 636b 5f73 697a 650a  e // block_size.
+00006cc0: 2020 2020 2020 2020 6966 2066 6f72 7761          if forwa
+00006cd0: 7264 5f72 6174 696f 2069 7320 4e6f 6e65  rd_ratio is None
+00006ce0: 3a0a 2020 2020 2020 2020 2020 2020 626c  :.            bl
+00006cf0: 6f63 6b5f 666f 7277 6172 6420 3d20 4e6f  ock_forward = No
+00006d00: 6e65 0a20 2020 2020 2020 2065 6c73 653a  ne.        else:
+00006d10: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
+00006d20: 636b 5f66 6f72 7761 7264 203d 206d 6178  ck_forward = max
+00006d30: 2869 6e74 2862 6c6f 636b 5f63 6170 6163  (int(block_capac
+00006d40: 6974 7920 2a20 666f 7277 6172 645f 7261  ity * forward_ra
+00006d50: 7469 6f29 2c20 3129 0a20 2020 2020 2020  tio), 1).       
+00006d60: 2069 6620 7368 6172 655f 6361 6368 655f   if share_cache_
+00006d70: 6b65 7920 6973 206e 6f74 204e 6f6e 653a  key is not None:
+00006d80: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+00006d90: 6465 7220 3d20 5333 5368 6172 6543 6163  der = S3ShareCac
+00006da0: 6865 5265 6164 6572 280a 2020 2020 2020  heReader(.      
+00006db0: 2020 2020 2020 2020 2020 6275 636b 6574            bucket
+00006dc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006dd0: 2020 6b65 792c 0a20 2020 2020 2020 2020    key,.         
+00006de0: 2020 2020 2020 2063 6163 6865 5f6b 6579         cache_key
+00006df0: 3d73 6861 7265 5f63 6163 6865 5f6b 6579  =share_cache_key
+00006e00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006e10: 2020 7333 5f63 6c69 656e 743d 636c 6965    s3_client=clie
+00006e20: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00006e30: 2020 2020 6d61 785f 7265 7472 6965 733d      max_retries=
+00006e40: 6d61 785f 7265 7472 6965 732c 0a20 2020  max_retries,.   
+00006e50: 2020 2020 2020 2020 2020 2020 206d 6178               max
+00006e60: 5f77 6f72 6b65 7273 3d6d 6178 5f63 6f6e  _workers=max_con
+00006e70: 6375 7272 656e 6379 2c0a 2020 2020 2020  currency,.      
+00006e80: 2020 2020 2020 2020 2020 626c 6f63 6b5f            block_
+00006e90: 7369 7a65 3d62 6c6f 636b 5f73 697a 652c  size=block_size,
+00006ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006eb0: 2062 6c6f 636b 5f66 6f72 7761 7264 3d62   block_forward=b
+00006ec0: 6c6f 636b 5f66 6f72 7761 7264 290a 2020  lock_forward).  
+00006ed0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00006ee0: 2020 2020 2020 2020 7265 6164 6572 203d          reader =
+00006ef0: 2053 3350 7265 6665 7463 6852 6561 6465   S3PrefetchReade
+00006f00: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00006f10: 2020 2062 7563 6b65 742c 0a20 2020 2020     bucket,.     
+00006f20: 2020 2020 2020 2020 2020 206b 6579 2c0a             key,.
+00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f40: 7333 5f63 6c69 656e 743d 636c 6965 6e74  s3_client=client
+00006f50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006f60: 2020 6d61 785f 7265 7472 6965 733d 6d61    max_retries=ma
+00006f70: 785f 7265 7472 6965 732c 0a20 2020 2020  x_retries,.     
+00006f80: 2020 2020 2020 2020 2020 206d 6178 5f77             max_w
+00006f90: 6f72 6b65 7273 3d6d 6178 5f63 6f6e 6375  orkers=max_concu
+00006fa0: 7272 656e 6379 2c0a 2020 2020 2020 2020  rrency,.        
+00006fb0: 2020 2020 2020 2020 626c 6f63 6b5f 6361          block_ca
+00006fc0: 7061 6369 7479 3d62 6c6f 636b 5f63 6170  pacity=block_cap
+00006fd0: 6163 6974 792c 0a20 2020 2020 2020 2020  acity,.         
+00006fe0: 2020 2020 2020 2062 6c6f 636b 5f66 6f72         block_for
+00006ff0: 7761 7264 3d62 6c6f 636b 5f66 6f72 7761  ward=block_forwa
+00007000: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
+00007010: 2020 2020 626c 6f63 6b5f 7369 7a65 3d62      block_size=b
+00007020: 6c6f 636b 5f73 697a 6529 0a20 2020 2020  lock_size).     
+00007030: 2020 2069 6620 6275 6666 6572 6564 3a0a     if buffered:.
+00007040: 2020 2020 2020 2020 2020 2020 7265 6164              read
+00007050: 6572 203d 2069 6f2e 4275 6666 6572 6564  er = io.Buffered
+00007060: 5265 6164 6572 2872 6561 6465 7229 2020  Reader(reader)  
+00007070: 2320 7079 7479 7065 3a20 6469 7361 626c  # pytype: disabl
+00007080: 653d 7772 6f6e 672d 6172 672d 7479 7065  e=wrong-arg-type
+00007090: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+000070a0: 2072 6561 6465 720a 0a20 2020 2069 6620   reader..    if 
+000070b0: 6c69 6d69 7465 645f 7365 656b 6162 6c65  limited_seekable
+000070c0: 3a0a 2020 2020 2020 2020 7772 6974 6572  :.        writer
+000070d0: 203d 2053 334c 696d 6974 6564 5365 656b   = S3LimitedSeek
+000070e0: 6162 6c65 5772 6974 6572 280a 2020 2020  ableWriter(.    
+000070f0: 2020 2020 2020 2020 6275 636b 6574 2c0a          bucket,.
+00007100: 2020 2020 2020 2020 2020 2020 6b65 792c              key,
+00007110: 0a20 2020 2020 2020 2020 2020 2073 335f  .            s3_
+00007120: 636c 6965 6e74 3d63 6c69 656e 742c 0a20  client=client,. 
+00007130: 2020 2020 2020 2020 2020 206d 6178 5f77             max_w
+00007140: 6f72 6b65 7273 3d6d 6178 5f63 6f6e 6375  orkers=max_concu
+00007150: 7272 656e 6379 2c0a 2020 2020 2020 2020  rrency,.        
+00007160: 2020 2020 6d61 785f 6275 6666 6572 5f73      max_buffer_s
+00007170: 697a 653d 6d61 785f 6275 6666 6572 5f73  ize=max_buffer_s
+00007180: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
+00007190: 2062 6c6f 636b 5f73 697a 653d 626c 6f63   block_size=bloc
+000071a0: 6b5f 7369 7a65 290a 2020 2020 656c 7365  k_size).    else
+000071b0: 3a0a 2020 2020 2020 2020 7772 6974 6572  :.        writer
+000071c0: 203d 2053 3342 7566 6665 7265 6457 7269   = S3BufferedWri
+000071d0: 7465 7228 0a20 2020 2020 2020 2020 2020  ter(.           
+000071e0: 2062 7563 6b65 742c 0a20 2020 2020 2020   bucket,.       
+000071f0: 2020 2020 206b 6579 2c0a 2020 2020 2020       key,.      
+00007200: 2020 2020 2020 7333 5f63 6c69 656e 743d        s3_client=
+00007210: 636c 6965 6e74 2c0a 2020 2020 2020 2020  client,.        
+00007220: 2020 2020 6d61 785f 776f 726b 6572 733d      max_workers=
+00007230: 6d61 785f 636f 6e63 7572 7265 6e63 792c  max_concurrency,
+00007240: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00007250: 5f62 7566 6665 725f 7369 7a65 3d6d 6178  _buffer_size=max
+00007260: 5f62 7566 6665 725f 7369 7a65 2c0a 2020  _buffer_size,.  
+00007270: 2020 2020 2020 2020 2020 626c 6f63 6b5f            block_
+00007280: 7369 7a65 3d62 6c6f 636b 5f73 697a 6529  size=block_size)
+00007290: 0a20 2020 2069 6620 6275 6666 6572 6564  .    if buffered
+000072a0: 3a0a 2020 2020 2020 2020 7772 6974 6572  :.        writer
+000072b0: 203d 2069 6f2e 4275 6666 6572 6564 5772   = io.BufferedWr
+000072c0: 6974 6572 2877 7269 7465 7229 2020 2320  iter(writer)  # 
+000072d0: 7079 7479 7065 3a20 6469 7361 626c 653d  pytype: disable=
+000072e0: 7772 6f6e 672d 6172 672d 7479 7065 730a  wrong-arg-types.
+000072f0: 2020 2020 7265 7475 726e 2077 7269 7465      return write
+00007300: 720a 0a0a 405f 7333 5f62 696e 6172 795f  r...@_s3_binary_
+00007310: 6d6f 6465 0a64 6566 2073 335f 6d65 6d6f  mode.def s3_memo
+00007320: 7279 5f6f 7065 6e28 0a20 2020 2020 2020  ry_open(.       
+00007330: 2073 335f 7572 6c3a 2050 6174 684c 696b   s3_url: PathLik
+00007340: 652c 206d 6f64 653a 2073 7472 2c0a 2020  e, mode: str,.  
+00007350: 2020 2020 2020 666f 6c6c 6f77 6c69 6e6b        followlink
+00007360: 733a 2062 6f6f 6c20 3d20 4661 6c73 6529  s: bool = False)
+00007370: 202d 3e20 5333 4d65 6d6f 7279 4861 6e64   -> S3MemoryHand
+00007380: 6c65 723a 0a20 2020 2027 2727 4f70 656e  ler:.    '''Open
+00007390: 2061 206d 656d 6f72 792d 6361 6368 6520   a memory-cache 
+000073a0: 6669 6c65 2072 6561 6465 7220 2f20 7772  file reader / wr
+000073b0: 6974 6572 2c20 666f 7220 6672 6571 7565  iter, for freque
+000073c0: 6e74 2072 616e 646f 6d20 7265 6164 202f  nt random read /
+000073d0: 2077 7269 7465 0a0a 2020 2020 2e2e 206e   write..    .. n
+000073e0: 6f74 6520 3a3a 0a0a 2020 2020 2020 2020  ote ::..        
+000073f0: 5573 6572 2073 686f 756c 6420 6d61 6b65  User should make
+00007400: 2073 7572 6520 7468 6174 2072 6561 6465   sure that reade
+00007410: 7220 2f20 7772 6974 6572 2061 7265 2063  r / writer are c
+00007420: 6c6f 7365 6420 636f 7272 6563 746c 790a  losed correctly.
+00007430: 0a20 2020 2020 2020 2053 7570 706f 7274  .        Support
+00007440: 7320 636f 6e74 6578 7420 6d61 6e61 6765  s context manage
+00007450: 720a 0a20 2020 203a 7061 7261 6d20 6d6f  r..    :param mo
+00007460: 6465 3a20 4d6f 6465 2074 6f20 6f70 656e  de: Mode to open
+00007470: 2066 696c 652c 2063 6f75 6c64 2062 6520   file, could be 
+00007480: 6f6e 6520 6f66 2022 7262 222c 2022 7762  one of "rb", "wb
+00007490: 222c 2022 6162 222c 2022 7262 2b22 2c20  ", "ab", "rb+", 
+000074a0: 2277 622b 2220 6f72 2022 6162 2b22 0a20  "wb+" or "ab+". 
+000074b0: 2020 203a 7265 7475 726e 733a 2041 6e20     :returns: An 
+000074c0: 6f70 656e 6564 2042 7566 6665 7265 6452  opened BufferedR
+000074d0: 6561 6465 7220 2f20 4275 6666 6572 6564  eader / Buffered
+000074e0: 5772 6974 6572 206f 626a 6563 740a 2020  Writer object.  
+000074f0: 2020 2727 270a 2020 2020 6966 206d 6f64    '''.    if mod
+00007500: 6520 6e6f 7420 696e 2028 2772 6227 2c20  e not in ('rb', 
+00007510: 2777 6227 2c20 2761 6227 2c20 2772 622b  'wb', 'ab', 'rb+
+00007520: 272c 2027 7762 2b27 2c20 2761 622b 2729  ', 'wb+', 'ab+')
+00007530: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00007540: 5661 6c75 6545 7272 6f72 2827 756e 6163  ValueError('unac
+00007550: 6365 7074 6162 6c65 206d 6f64 653a 2025  ceptable mode: %
+00007560: 7227 2025 206d 6f64 6529 0a20 2020 2073  r' % mode).    s
+00007570: 335f 7572 6c20 3d20 5333 5061 7468 2873  3_url = S3Path(s
+00007580: 335f 7572 6c29 0a20 2020 2069 6620 666f  3_url).    if fo
+00007590: 6c6c 6f77 6c69 6e6b 733a 0a20 2020 2020  llowlinks:.     
+000075a0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000075b0: 2020 2020 7333 5f75 726c 203d 2073 335f      s3_url = s3_
+000075c0: 7572 6c2e 7265 6164 6c69 6e6b 2829 0a20  url.readlink(). 
+000075d0: 2020 2020 2020 2065 7863 6570 7420 5333         except S3
+000075e0: 4e6f 7441 4c69 6e6b 4572 726f 723a 0a20  NotALinkError:. 
+000075f0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00007600: 0a20 2020 2062 7563 6b65 742c 206b 6579  .    bucket, key
+00007610: 203d 2070 6172 7365 5f73 335f 7572 6c28   = parse_s3_url(
+00007620: 7333 5f75 726c 2e70 6174 685f 7769 7468  s3_url.path_with
+00007630: 5f70 726f 746f 636f 6c29 0a20 2020 2063  _protocol).    c
+00007640: 6f6e 6669 6720 3d20 626f 746f 636f 7265  onfig = botocore
+00007650: 2e63 6f6e 6669 672e 436f 6e66 6967 286d  .config.Config(m
+00007660: 6178 5f70 6f6f 6c5f 636f 6e6e 6563 7469  ax_pool_connecti
+00007670: 6f6e 733d 6d61 785f 706f 6f6c 5f63 6f6e  ons=max_pool_con
+00007680: 6e65 6374 696f 6e73 290a 2020 2020 636c  nections).    cl
+00007690: 6965 6e74 203d 2067 6574 5f73 335f 636c  ient = get_s3_cl
+000076a0: 6965 6e74 280a 2020 2020 2020 2020 636f  ient(.        co
+000076b0: 6e66 6967 3d63 6f6e 6669 672c 0a20 2020  nfig=config,.   
+000076c0: 2020 2020 2063 6163 6865 5f6b 6579 3d27       cache_key='
+000076d0: 7333 5f66 696c 656c 696b 655f 636c 6965  s3_filelike_clie
+000076e0: 6e74 272c 0a20 2020 2020 2020 2070 726f  nt',.        pro
+000076f0: 6669 6c65 5f6e 616d 653d 7333 5f75 726c  file_name=s3_url
+00007700: 2e5f 7072 6f66 696c 655f 6e61 6d65 290a  ._profile_name).
+00007710: 2020 2020 7265 7475 726e 2053 334d 656d      return S3Mem
+00007720: 6f72 7948 616e 646c 6572 2862 7563 6b65  oryHandler(bucke
+00007730: 742c 206b 6579 2c20 6d6f 6465 2c20 7333  t, key, mode, s3
+00007740: 5f63 6c69 656e 743d 636c 6965 6e74 290a  _client=client).
+00007750: 0a0a 7333 5f6f 7065 6e20 3d20 7333 5f62  ..s3_open = s3_b
+00007760: 7566 6665 7265 645f 6f70 656e 0a0a 0a64  uffered_open...d
+00007770: 6566 2073 335f 646f 776e 6c6f 6164 280a  ef s3_download(.
+00007780: 2020 2020 2020 2020 7372 635f 7572 6c3a          src_url:
+00007790: 2050 6174 684c 696b 652c 0a20 2020 2020   PathLike,.     
+000077a0: 2020 2064 7374 5f75 726c 3a20 5061 7468     dst_url: Path
+000077b0: 4c69 6b65 2c0a 2020 2020 2020 2020 666f  Like,.        fo
+000077c0: 6c6c 6f77 6c69 6e6b 733a 2062 6f6f 6c20  llowlinks: bool 
+000077d0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+000077e0: 2063 616c 6c62 6163 6b3a 204f 7074 696f   callback: Optio
+000077f0: 6e61 6c5b 4361 6c6c 6162 6c65 5b5b 696e  nal[Callable[[in
+00007800: 745d 2c20 4e6f 6e65 5d5d 203d 204e 6f6e  t], None]] = Non
+00007810: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
+00007820: 2727 270a 2020 2020 446f 776e 6c6f 6164  '''.    Download
+00007830: 7320 6120 6669 6c65 2066 726f 6d20 7333  s a file from s3
+00007840: 2074 6f20 6c6f 6361 6c20 6669 6c65 7379   to local filesy
+00007850: 7374 656d 2e0a 2020 2020 3a70 6172 616d  stem..    :param
+00007860: 2073 7263 5f75 726c 3a20 736f 7572 6365   src_url: source
+00007870: 2073 3320 7061 7468 0a20 2020 203a 7061   s3 path.    :pa
+00007880: 7261 6d20 6473 745f 7572 6c3a 2074 6172  ram dst_url: tar
+00007890: 6765 7420 6673 2070 6174 680a 2020 2020  get fs path.    
+000078a0: 3a70 6172 616d 2063 616c 6c62 6163 6b3a  :param callback:
+000078b0: 2043 616c 6c65 6420 7065 7269 6f64 6963   Called periodic
+000078c0: 616c 6c79 2064 7572 696e 6720 636f 7079  ally during copy
+000078d0: 2c20 616e 6420 7468 6520 696e 7075 7420  , and the input 
+000078e0: 7061 7261 6d65 7465 7220 6973 2074 6865  parameter is the
+000078f0: 2064 6174 6120 7369 7a65 2028 696e 2062   data size (in b
+00007900: 7974 6573 2920 6f66 2063 6f70 7920 7369  ytes) of copy si
+00007910: 6e63 6520 7468 6520 6c61 7374 2063 616c  nce the last cal
+00007920: 6c0a 2020 2020 2727 270a 2020 2020 7372  l.    '''.    sr
+00007930: 635f 7572 6c20 3d20 5333 5061 7468 2873  c_url = S3Path(s
+00007940: 7263 5f75 726c 290a 2020 2020 6966 2066  rc_url).    if f
+00007950: 6f6c 6c6f 776c 696e 6b73 3a0a 2020 2020  ollowlinks:.    
+00007960: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00007970: 2020 2020 2073 7263 5f75 726c 203d 2073       src_url = s
+00007980: 7263 5f75 726c 2e72 6561 646c 696e 6b28  rc_url.readlink(
+00007990: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+000079a0: 2053 334e 6f74 414c 696e 6b45 7272 6f72   S3NotALinkError
+000079b0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+000079c0: 7373 0a20 2020 2073 7263 5f62 7563 6b65  ss.    src_bucke
+000079d0: 742c 2073 7263 5f6b 6579 203d 2070 6172  t, src_key = par
+000079e0: 7365 5f73 335f 7572 6c28 7372 635f 7572  se_s3_url(src_ur
+000079f0: 6c2e 7061 7468 5f77 6974 685f 7072 6f74  l.path_with_prot
+00007a00: 6f63 6f6c 290a 2020 2020 6966 206e 6f74  ocol).    if not
+00007a10: 2073 7263 5f62 7563 6b65 743a 0a20 2020   src_bucket:.   
+00007a20: 2020 2020 2072 6169 7365 2053 3342 7563       raise S3Buc
+00007a30: 6b65 744e 6f74 466f 756e 6445 7272 6f72  ketNotFoundError
+00007a40: 280a 2020 2020 2020 2020 2020 2020 2745  (.            'E
+00007a50: 6d70 7479 2062 7563 6b65 7420 6e61 6d65  mpty bucket name
+00007a60: 3a20 2572 2720 2520 7372 635f 7572 6c2e  : %r' % src_url.
+00007a70: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
+00007a80: 6f6c 290a 0a20 2020 2069 6620 6e6f 7420  ol)..    if not 
+00007a90: 7372 635f 7572 6c2e 6578 6973 7473 2829  src_url.exists()
+00007aa0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00007ab0: 5333 4669 6c65 4e6f 7446 6f75 6e64 4572  S3FileNotFoundEr
+00007ac0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00007ad0: 2027 4669 6c65 206e 6f74 2066 6f75 6e64   'File not found
+00007ae0: 3a20 2572 2720 2520 7372 635f 7572 6c2e  : %r' % src_url.
+00007af0: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
+00007b00: 6f6c 290a 0a20 2020 2069 6620 6e6f 7420  ol)..    if not 
+00007b10: 7372 635f 7572 6c2e 6973 5f66 696c 6528  src_url.is_file(
+00007b20: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+00007b30: 2053 3349 7341 4469 7265 6374 6f72 7945   S3IsADirectoryE
+00007b40: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00007b50: 2020 2749 7320 6120 6469 7265 6374 6f72    'Is a director
+00007b60: 793a 2025 7227 2025 2073 7263 5f75 726c  y: %r' % src_url
+00007b70: 2e70 6174 685f 7769 7468 5f70 726f 746f  .path_with_proto
+00007b80: 636f 6c29 0a0a 2020 2020 6473 745f 7572  col)..    dst_ur
+00007b90: 6c20 3d20 6673 7061 7468 2864 7374 5f75  l = fspath(dst_u
+00007ba0: 726c 290a 2020 2020 6966 206e 6f74 2064  rl).    if not d
+00007bb0: 7374 5f75 726c 206f 7220 6473 745f 7572  st_url or dst_ur
+00007bc0: 6c2e 656e 6473 7769 7468 2827 2f27 293a  l.endswith('/'):
+00007bd0: 0a20 2020 2020 2020 2072 6169 7365 2053  .        raise S
+00007be0: 3349 7341 4469 7265 6374 6f72 7945 7272  3IsADirectoryErr
+00007bf0: 6f72 2827 4973 2061 2064 6972 6563 746f  or('Is a directo
+00007c00: 7279 3a20 2572 2720 2520 6473 745f 7572  ry: %r' % dst_ur
+00007c10: 6c29 0a0a 2020 2020 6473 745f 6469 7265  l)..    dst_dire
+00007c20: 6374 6f72 7920 3d20 6f73 2e70 6174 682e  ctory = os.path.
+00007c30: 6469 726e 616d 6528 6473 745f 7572 6c29  dirname(dst_url)
+00007c40: 0a20 2020 2069 6620 6473 745f 6469 7265  .    if dst_dire
+00007c50: 6374 6f72 7920 213d 2027 273a 0a20 2020  ctory != '':.   
+00007c60: 2020 2020 206f 732e 6d61 6b65 6469 7273       os.makedirs
+00007c70: 2864 7374 5f64 6972 6563 746f 7279 2c20  (dst_directory, 
+00007c80: 6578 6973 745f 6f6b 3d54 7275 6529 0a0a  exist_ok=True)..
+00007c90: 2020 2020 636c 6965 6e74 203d 2067 6574      client = get
+00007ca0: 5f73 335f 636c 6965 6e74 2870 726f 6669  _s3_client(profi
+00007cb0: 6c65 5f6e 616d 653d 7372 635f 7572 6c2e  le_name=src_url.
+00007cc0: 5f70 726f 6669 6c65 5f6e 616d 6529 0a20  _profile_name). 
+00007cd0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00007ce0: 636c 6965 6e74 2e64 6f77 6e6c 6f61 645f  client.download_
+00007cf0: 6669 6c65 2873 7263 5f62 7563 6b65 742c  file(src_bucket,
+00007d00: 2073 7263 5f6b 6579 2c20 6473 745f 7572   src_key, dst_ur
+00007d10: 6c2c 2043 616c 6c62 6163 6b3d 6361 6c6c  l, Callback=call
+00007d20: 6261 636b 290a 2020 2020 6578 6365 7074  back).    except
+00007d30: 2045 7863 6570 7469 6f6e 2061 7320 6572   Exception as er
+00007d40: 726f 723a 2020 2320 7072 6167 6d61 3a20  ror:  # pragma: 
+00007d50: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
+00007d60: 2065 7272 6f72 203d 2074 7261 6e73 6c61   error = transla
+00007d70: 7465 5f66 735f 6572 726f 7228 6572 726f  te_fs_error(erro
+00007d80: 722c 2064 7374 5f75 726c 290a 2020 2020  r, dst_url).    
+00007d90: 2020 2020 6572 726f 7220 3d20 7472 616e      error = tran
+00007da0: 736c 6174 655f 7333 5f65 7272 6f72 2865  slate_s3_error(e
+00007db0: 7272 6f72 2c20 7372 635f 7572 6c2e 7061  rror, src_url.pa
+00007dc0: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
+00007dd0: 290a 2020 2020 2020 2020 7261 6973 6520  ).        raise 
+00007de0: 6572 726f 720a 0a20 2020 2073 7263 5f73  error..    src_s
+00007df0: 7461 7420 3d20 7372 635f 7572 6c2e 7374  tat = src_url.st
+00007e00: 6174 2829 0a20 2020 206f 732e 7574 696d  at().    os.utim
+00007e10: 6528 6473 745f 7572 6c2c 2028 7372 635f  e(dst_url, (src_
+00007e20: 7374 6174 2e73 745f 6d74 696d 652c 2073  stat.st_mtime, s
+00007e30: 7263 5f73 7461 742e 7374 5f6d 7469 6d65  rc_stat.st_mtime
+00007e40: 2929 0a0a 0a64 6566 2073 335f 7570 6c6f  ))...def s3_uplo
+00007e50: 6164 280a 2020 2020 2020 2020 7372 635f  ad(.        src_
+00007e60: 7572 6c3a 2050 6174 684c 696b 652c 0a20  url: PathLike,. 
+00007e70: 2020 2020 2020 2064 7374 5f75 726c 3a20         dst_url: 
+00007e80: 5061 7468 4c69 6b65 2c0a 2020 2020 2020  PathLike,.      
+00007e90: 2020 6361 6c6c 6261 636b 3a20 4f70 7469    callback: Opti
+00007ea0: 6f6e 616c 5b43 616c 6c61 626c 655b 5b69  onal[Callable[[i
+00007eb0: 6e74 5d2c 204e 6f6e 655d 5d20 3d20 4e6f  nt], None]] = No
+00007ec0: 6e65 2c0a 2020 2020 2020 2020 2a2a 6b77  ne,.        **kw
+00007ed0: 6172 6773 2920 2d3e 204e 6f6e 653a 0a20  args) -> None:. 
+00007ee0: 2020 2027 2727 0a20 2020 2055 706c 6f61     '''.    Uploa
+00007ef0: 6473 2061 2066 696c 6520 6672 6f6d 206c  ds a file from l
+00007f00: 6f63 616c 2066 696c 6573 7973 7465 6d20  ocal filesystem 
+00007f10: 746f 2073 332e 0a20 2020 203a 7061 7261  to s3..    :para
+00007f20: 6d20 7372 635f 7572 6c3a 2073 6f75 7263  m src_url: sourc
+00007f30: 6520 6673 2070 6174 680a 2020 2020 3a70  e fs path.    :p
+00007f40: 6172 616d 2064 7374 5f75 726c 3a20 7461  aram dst_url: ta
+00007f50: 7267 6574 2073 3320 7061 7468 0a20 2020  rget s3 path.   
+00007f60: 203a 7061 7261 6d20 6361 6c6c 6261 636b   :param callback
+00007f70: 3a20 4361 6c6c 6564 2070 6572 696f 6469  : Called periodi
+00007f80: 6361 6c6c 7920 6475 7269 6e67 2063 6f70  cally during cop
+00007f90: 792c 2061 6e64 2074 6865 2069 6e70 7574  y, and the input
+00007fa0: 2070 6172 616d 6574 6572 2069 7320 7468   parameter is th
+00007fb0: 6520 6461 7461 2073 697a 6520 2869 6e20  e data size (in 
+00007fc0: 6279 7465 7329 206f 6620 636f 7079 2073  bytes) of copy s
+00007fd0: 696e 6365 2074 6865 206c 6173 7420 6361  ince the last ca
+00007fe0: 6c6c 0a20 2020 2027 2727 0a20 2020 2064  ll.    '''.    d
+00007ff0: 7374 5f62 7563 6b65 742c 2064 7374 5f6b  st_bucket, dst_k
+00008000: 6579 203d 2070 6172 7365 5f73 335f 7572  ey = parse_s3_ur
+00008010: 6c28 6473 745f 7572 6c29 0a20 2020 2069  l(dst_url).    i
+00008020: 6620 6e6f 7420 6473 745f 6275 636b 6574  f not dst_bucket
+00008030: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00008040: 5333 4275 636b 6574 4e6f 7446 6f75 6e64  S3BucketNotFound
+00008050: 4572 726f 7228 2745 6d70 7479 2062 7563  Error('Empty buc
+00008060: 6b65 7420 6e61 6d65 3a20 2572 2720 2520  ket name: %r' % 
+00008070: 6473 745f 7572 6c29 0a20 2020 2069 6620  dst_url).    if 
+00008080: 6e6f 7420 6473 745f 6b65 7920 6f72 2064  not dst_key or d
+00008090: 7374 5f6b 6579 2e65 6e64 7377 6974 6828  st_key.endswith(
+000080a0: 272f 2729 3a0a 2020 2020 2020 2020 7261  '/'):.        ra
+000080b0: 6973 6520 5333 4973 4144 6972 6563 746f  ise S3IsADirecto
+000080c0: 7279 4572 726f 7228 2749 7320 6120 6469  ryError('Is a di
+000080d0: 7265 6374 6f72 793a 2025 7227 2025 2064  rectory: %r' % d
+000080e0: 7374 5f75 726c 290a 0a20 2020 2063 6c69  st_url)..    cli
+000080f0: 656e 7420 3d20 6765 745f 7333 5f63 6c69  ent = get_s3_cli
+00008100: 656e 7428 7072 6f66 696c 655f 6e61 6d65  ent(profile_name
+00008110: 3d53 3350 6174 6828 6473 745f 7572 6c29  =S3Path(dst_url)
+00008120: 2e5f 7072 6f66 696c 655f 6e61 6d65 290a  ._profile_name).
+00008130: 2020 2020 7769 7468 206f 7065 6e28 7372      with open(sr
+00008140: 635f 7572 6c2c 2027 7262 2729 2061 7320  c_url, 'rb') as 
+00008150: 7372 633a 0a20 2020 2020 2020 2077 6974  src:.        wit
+00008160: 6820 7261 6973 655f 7333 5f65 7272 6f72  h raise_s3_error
+00008170: 2864 7374 5f75 726c 293a 0a20 2020 2020  (dst_url):.     
+00008180: 2020 2020 2020 2063 6c69 656e 742e 7570         client.up
+00008190: 6c6f 6164 5f66 696c 656f 626a 280a 2020  load_fileobj(.  
+000081a0: 2020 2020 2020 2020 2020 2020 2020 7372                sr
+000081b0: 632c 2042 7563 6b65 743d 6473 745f 6275  c, Bucket=dst_bu
+000081c0: 636b 6574 2c20 4b65 793d 6473 745f 6b65  cket, Key=dst_ke
+000081d0: 792c 2043 616c 6c62 6163 6b3d 6361 6c6c  y, Callback=call
+000081e0: 6261 636b 290a 0a0a 6465 6620 7333 5f6c  back)...def s3_l
+000081f0: 6f61 645f 636f 6e74 656e 7428 0a20 2020  oad_content(.   
+00008200: 2020 2020 2073 335f 7572 6c2c 0a20 2020       s3_url,.   
+00008210: 2020 2020 2073 7461 7274 3a20 4f70 7469       start: Opti
+00008220: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00008230: 2c0a 2020 2020 2020 2020 7374 6f70 3a20  ,.        stop: 
+00008240: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00008250: 4e6f 6e65 2c0a 2020 2020 2020 2020 666f  None,.        fo
+00008260: 6c6c 6f77 6c69 6e6b 733a 2062 6f6f 6c20  llowlinks: bool 
+00008270: 3d20 4661 6c73 6529 202d 3e20 6279 7465  = False) -> byte
+00008280: 733a 0a20 2020 2027 2727 0a20 2020 2047  s:.    '''.    G
+00008290: 6574 2073 7065 6369 6669 6564 2066 696c  et specified fil
+000082a0: 6520 6672 6f6d 205b 7374 6172 742c 2073  e from [start, s
+000082b0: 746f 7029 2069 6e20 6279 7465 730a 0a20  top) in bytes.. 
+000082c0: 2020 203a 7061 7261 6d20 7333 5f75 726c     :param s3_url
+000082d0: 3a20 5370 6563 6966 6965 6420 7061 7468  : Specified path
+000082e0: 0a20 2020 203a 7061 7261 6d20 7374 6172  .    :param star
+000082f0: 743a 2073 7461 7274 2069 6e64 6578 0a20  t: start index. 
+00008300: 2020 203a 7061 7261 6d20 7374 6f70 3a20     :param stop: 
+00008310: 7374 6f70 2069 6e64 6578 0a20 2020 203a  stop index.    :
+00008320: 7265 7475 726e 733a 2062 7974 6573 2063  returns: bytes c
+00008330: 6f6e 7465 6e74 2069 6e20 7261 6e67 6520  ontent in range 
+00008340: 5b73 7461 7274 2c20 7374 6f70 290a 2020  [start, stop).  
+00008350: 2020 2727 270a 0a20 2020 2064 6566 205f    '''..    def _
+00008360: 6765 745f 6f62 6a65 6374 2863 6c69 656e  get_object(clien
+00008370: 742c 2062 7563 6b65 742c 206b 6579 2c20  t, bucket, key, 
+00008380: 7261 6e67 655f 7374 7229 3a0a 2020 2020  range_str):.    
+00008390: 2020 2020 7265 7475 726e 2063 6c69 656e      return clien
+000083a0: 742e 6765 745f 6f62 6a65 6374 280a 2020  t.get_object(.  
+000083b0: 2020 2020 2020 2020 2020 4275 636b 6574            Bucket
+000083c0: 3d62 7563 6b65 742c 204b 6579 3d6b 6579  =bucket, Key=key
+000083d0: 2c20 5261 6e67 653d 7261 6e67 655f 7374  , Range=range_st
+000083e0: 7229 5b27 426f 6479 275d 2e72 6561 6428  r)['Body'].read(
+000083f0: 290a 0a20 2020 2073 335f 7572 6c20 3d20  )..    s3_url = 
+00008400: 5333 5061 7468 2873 335f 7572 6c29 0a20  S3Path(s3_url). 
+00008410: 2020 2069 6620 666f 6c6c 6f77 6c69 6e6b     if followlink
+00008420: 733a 0a20 2020 2020 2020 2074 7279 3a0a  s:.        try:.
+00008430: 2020 2020 2020 2020 2020 2020 7333 5f75              s3_u
+00008440: 726c 203d 2073 335f 7572 6c2e 7265 6164  rl = s3_url.read
+00008450: 6c69 6e6b 2829 0a20 2020 2020 2020 2065  link().        e
+00008460: 7863 6570 7420 5333 4e6f 7441 4c69 6e6b  xcept S3NotALink
+00008470: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+00008480: 2020 2070 6173 730a 0a20 2020 2062 7563     pass..    buc
+00008490: 6b65 742c 206b 6579 203d 2070 6172 7365  ket, key = parse
+000084a0: 5f73 335f 7572 6c28 7333 5f75 726c 2e70  _s3_url(s3_url.p
+000084b0: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
+000084c0: 6c29 0a20 2020 2069 6620 6e6f 7420 6275  l).    if not bu
+000084d0: 636b 6574 3a0a 2020 2020 2020 2020 7261  cket:.        ra
+000084e0: 6973 6520 5333 4275 636b 6574 4e6f 7446  ise S3BucketNotF
+000084f0: 6f75 6e64 4572 726f 7228 2745 6d70 7479  oundError('Empty
+00008500: 2062 7563 6b65 7420 6e61 6d65 3a20 2572   bucket name: %r
+00008510: 2720 2520 7333 5f75 726c 290a 2020 2020  ' % s3_url).    
+00008520: 6966 206e 6f74 206b 6579 206f 7220 6b65  if not key or ke
+00008530: 792e 656e 6473 7769 7468 2827 2f27 293a  y.endswith('/'):
+00008540: 0a20 2020 2020 2020 2072 6169 7365 2053  .        raise S
+00008550: 3349 7341 4469 7265 6374 6f72 7945 7272  3IsADirectoryErr
+00008560: 6f72 2827 4973 2061 2064 6972 6563 746f  or('Is a directo
+00008570: 7279 3a20 2572 2720 2520 7333 5f75 726c  ry: %r' % s3_url
+00008580: 290a 0a20 2020 2073 7461 7274 2c20 7374  )..    start, st
+00008590: 6f70 203d 2067 6574 5f63 6f6e 7465 6e74  op = get_content
+000085a0: 5f6f 6666 7365 7428 0a20 2020 2020 2020  _offset(.       
+000085b0: 2073 7461 7274 2c20 7374 6f70 2c20 7333   start, stop, s3
+000085c0: 5f75 726c 2e67 6574 7369 7a65 2866 6f6c  _url.getsize(fol
+000085d0: 6c6f 775f 7379 6d6c 696e 6b73 3d46 616c  low_symlinks=Fal
+000085e0: 7365 2929 0a20 2020 2069 6620 7374 6172  se)).    if star
+000085f0: 7420 3d3d 2030 2061 6e64 2073 746f 7020  t == 0 and stop 
+00008600: 3d3d 2030 3a0a 2020 2020 2020 2020 7265  == 0:.        re
+00008610: 7475 726e 2062 2727 0a20 2020 2072 616e  turn b''.    ran
+00008620: 6765 5f73 7472 203d 2027 6279 7465 733d  ge_str = 'bytes=
+00008630: 2564 2d25 6427 2025 2028 7374 6172 742c  %d-%d' % (start,
+00008640: 2073 746f 7020 2d20 3129 0a0a 2020 2020   stop - 1)..    
+00008650: 636c 6965 6e74 203d 2067 6574 5f73 335f  client = get_s3_
+00008660: 636c 6965 6e74 2870 726f 6669 6c65 5f6e  client(profile_n
+00008670: 616d 653d 7333 5f75 726c 2e5f 7072 6f66  ame=s3_url._prof
+00008680: 696c 655f 6e61 6d65 290a 2020 2020 7769  ile_name).    wi
+00008690: 7468 2072 6169 7365 5f73 335f 6572 726f  th raise_s3_erro
+000086a0: 7228 7333 5f75 726c 2e70 6174 6829 3a0a  r(s3_url.path):.
+000086b0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+000086c0: 6174 6368 5f6d 6574 686f 6428 0a20 2020  atch_method(.   
+000086d0: 2020 2020 2020 2020 205f 6765 745f 6f62           _get_ob
+000086e0: 6a65 6374 2c0a 2020 2020 2020 2020 2020  ject,.          
+000086f0: 2020 6d61 785f 7265 7472 6965 733d 6d61    max_retries=ma
+00008700: 785f 7265 7472 6965 732c 0a20 2020 2020  x_retries,.     
+00008710: 2020 2020 2020 2073 686f 756c 645f 7265         should_re
+00008720: 7472 793d 7333 5f73 686f 756c 645f 7265  try=s3_should_re
+00008730: 7472 792c 0a20 2020 2020 2020 2029 2863  try,.        )(c
+00008740: 6c69 656e 742c 2062 7563 6b65 742c 206b  lient, bucket, k
+00008750: 6579 2c20 7261 6e67 655f 7374 7229 0a0a  ey, range_str)..
+00008760: 0a64 6566 2073 335f 7265 6164 6c69 6e6b  .def s3_readlink
+00008770: 2870 6174 6829 202d 3e20 7374 723a 0a20  (path) -> str:. 
+00008780: 2020 2027 2727 0a20 2020 2052 6574 7572     '''.    Retur
+00008790: 6e20 6120 7374 7269 6e67 2072 6570 7265  n a string repre
+000087a0: 7365 6e74 696e 6720 7468 6520 7061 7468  senting the path
+000087b0: 2074 6f20 7768 6963 6820 7468 6520 7379   to which the sy
+000087c0: 6d62 6f6c 6963 206c 696e 6b20 706f 696e  mbolic link poin
+000087d0: 7473 2e0a 0a20 2020 203a 7265 7475 726e  ts...    :return
+000087e0: 733a 2052 6574 7572 6e20 6120 7374 7269  s: Return a stri
+000087f0: 6e67 2072 6570 7265 7365 6e74 696e 6720  ng representing 
+00008800: 7468 6520 7061 7468 2074 6f20 7768 6963  the path to whic
+00008810: 6820 7468 6520 7379 6d62 6f6c 6963 206c  h the symbolic l
+00008820: 696e 6b20 706f 696e 7473 2e0a 2020 2020  ink points..    
+00008830: 3a72 6169 7365 733a 2053 334e 616d 6554  :raises: S3NameT
+00008840: 6f6f 4c6f 6e67 4572 726f 722c 2053 3342  ooLongError, S3B
+00008850: 7563 6b65 744e 6f74 466f 756e 6445 7272  ucketNotFoundErr
+00008860: 6f72 2c20 5333 4973 4144 6972 6563 746f  or, S3IsADirecto
+00008870: 7279 4572 726f 722c 2053 334e 6f74 414c  ryError, S3NotAL
+00008880: 696e 6b45 7272 6f72 0a20 2020 2027 2727  inkError.    '''
+00008890: 0a20 2020 2072 6574 7572 6e20 5333 5061  .    return S3Pa
+000088a0: 7468 2870 6174 6829 2e72 6561 646c 696e  th(path).readlin
+000088b0: 6b28 292e 7061 7468 5f77 6974 685f 7072  k().path_with_pr
+000088c0: 6f74 6f63 6f6c 0a0a 0a64 6566 2073 335f  otocol...def s3_
+000088d0: 7265 6e61 6d65 2873 7263 5f75 726c 3a20  rename(src_url: 
+000088e0: 5061 7468 4c69 6b65 2c20 6473 745f 7572  PathLike, dst_ur
+000088f0: 6c3a 2050 6174 684c 696b 6529 3a0a 2020  l: PathLike):.  
+00008900: 2020 2727 270a 2020 2020 4d6f 7665 2073    '''.    Move s
+00008910: 3320 6669 6c65 2070 6174 6820 6672 6f6d  3 file path from
+00008920: 2073 7263 5f75 726c 2074 6f20 6473 745f   src_url to dst_
+00008930: 7572 6c0a 0a20 2020 203a 7061 7261 6d20  url..    :param 
+00008940: 6473 745f 7572 6c3a 2047 6976 656e 2064  dst_url: Given d
+00008950: 6573 7469 6e61 7469 6f6e 2070 6174 680a  estination path.
+00008960: 2020 2020 2727 270a 2020 2020 7372 635f      '''.    src_
+00008970: 7061 7468 5f69 6e73 203d 2053 3350 6174  path_ins = S3Pat
+00008980: 6828 7372 635f 7572 6c29 0a20 2020 2069  h(src_url).    i
+00008990: 6620 7372 635f 7061 7468 5f69 6e73 2e69  f src_path_ins.i
+000089a0: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
+000089b0: 2020 7372 635f 7061 7468 5f69 6e73 2e63    src_path_ins.c
+000089c0: 6f70 7928 6473 745f 7572 6c29 0a20 2020  opy(dst_url).   
+000089d0: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
+000089e0: 7263 5f70 6174 685f 696e 732e 7379 6e63  rc_path_ins.sync
+000089f0: 2864 7374 5f75 726c 290a 2020 2020 7372  (dst_url).    sr
+00008a00: 635f 7061 7468 5f69 6e73 2e72 656d 6f76  c_path_ins.remov
+00008a10: 6528 290a 0a0a 636c 6173 7320 5333 4361  e()...class S3Ca
+00008a20: 6368 6572 2846 696c 6543 6163 6865 7229  cher(FileCacher)
+00008a30: 3a0a 2020 2020 6361 6368 655f 7061 7468  :.    cache_path
+00008a40: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
+00008a50: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00008a60: 2020 2020 2020 2073 656c 662c 2070 6174         self, pat
+00008a70: 683a 2073 7472 2c20 6361 6368 655f 7061  h: str, cache_pa
+00008a80: 7468 3a20 4f70 7469 6f6e 616c 5b73 7472  th: Optional[str
+00008a90: 5d20 3d20 4e6f 6e65 2c20 6d6f 6465 3a20  ] = None, mode: 
+00008aa0: 7374 7220 3d20 2772 2729 3a0a 2020 2020  str = 'r'):.    
+00008ab0: 2020 2020 6966 206d 6f64 6520 6e6f 7420      if mode not 
+00008ac0: 696e 2028 2772 272c 2027 7727 2c20 2761  in ('r', 'w', 'a
+00008ad0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+00008ae0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00008af0: 2827 756e 6163 6365 7074 6162 6c65 206d  ('unacceptable m
+00008b00: 6f64 653a 2025 7227 2025 206d 6f64 6529  ode: %r' % mode)
+00008b10: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+00008b20: 2069 6e20 2827 7227 2c20 2761 2729 3a0a   in ('r', 'a'):.
+00008b30: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00008b40: 6163 6865 5f70 6174 6820 6973 204e 6f6e  ache_path is Non
+00008b50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008b60: 2020 2063 6163 6865 5f70 6174 6820 3d20     cache_path = 
+00008b70: 6765 6e65 7261 7465 5f63 6163 6865 5f70  generate_cache_p
+00008b80: 6174 6828 7061 7468 290a 2020 2020 2020  ath(path).      
+00008b90: 2020 2020 2020 7333 5f64 6f77 6e6c 6f61        s3_downloa
+00008ba0: 6428 7061 7468 2c20 6361 6368 655f 7061  d(path, cache_pa
+00008bb0: 7468 290a 2020 2020 2020 2020 7365 6c66  th).        self
+00008bc0: 2e6e 616d 6520 3d20 7061 7468 0a20 2020  .name = path.   
+00008bd0: 2020 2020 2073 656c 662e 6d6f 6465 203d       self.mode =
+00008be0: 206d 6f64 650a 2020 2020 2020 2020 7365   mode.        se
+00008bf0: 6c66 2e63 6163 6865 5f70 6174 6820 3d20  lf.cache_path = 
+00008c00: 6361 6368 655f 7061 7468 0a0a 2020 2020  cache_path..    
+00008c10: 6465 6620 5f63 6c6f 7365 2873 656c 6629  def _close(self)
+00008c20: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00008c30: 662e 6361 6368 655f 7061 7468 2069 7320  f.cache_path is 
+00008c40: 6e6f 7420 4e6f 6e65 2061 6e64 205c 0a20  not None and \. 
+00008c50: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+00008c60: 7468 2e65 7869 7374 7328 7365 6c66 2e63  th.exists(self.c
+00008c70: 6163 6865 5f70 6174 6829 3a0a 2020 2020  ache_path):.    
+00008c80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00008c90: 6d6f 6465 2069 6e20 2827 7727 2c20 2761  mode in ('w', 'a
+00008ca0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+00008cb0: 2020 2020 7333 5f75 706c 6f61 6428 7365      s3_upload(se
+00008cc0: 6c66 2e63 6163 6865 5f70 6174 682c 2073  lf.cache_path, s
+00008cd0: 656c 662e 6e61 6d65 290a 2020 2020 2020  elf.name).      
+00008ce0: 2020 2020 2020 6f73 2e75 6e6c 696e 6b28        os.unlink(
+00008cf0: 7365 6c66 2e63 6163 6865 5f70 6174 6829  self.cache_path)
+00008d00: 0a0a 0a64 6566 2073 335f 676c 6f62 280a  ...def s3_glob(.
+00008d10: 2020 2020 2020 2020 7061 7468 3a20 5061          path: Pa
+00008d20: 7468 4c69 6b65 2c0a 2020 2020 2020 2020  thLike,.        
+00008d30: 7265 6375 7273 6976 653a 2062 6f6f 6c20  recursive: bool 
+00008d40: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+00008d50: 6d69 7373 696e 675f 6f6b 3a20 626f 6f6c  missing_ok: bool
+00008d60: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+00008d70: 2066 6f6c 6c6f 776c 696e 6b73 3a20 626f   followlinks: bo
+00008d80: 6f6c 203d 2046 616c 7365 2c0a 2920 2d3e  ol = False,.) ->
+00008d90: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
+00008da0: 2727 2752 6574 7572 6e20 7333 2070 6174  '''Return s3 pat
+00008db0: 6820 6c69 7374 2069 6e20 6173 6365 6e64  h list in ascend
+00008dc0: 696e 6720 616c 7068 6162 6574 6963 616c  ing alphabetical
+00008dd0: 206f 7264 6572 2c20 696e 2077 6869 6368   order, in which
+00008de0: 2070 6174 6820 6d61 7463 6865 7320 676c   path matches gl
+00008df0: 6f62 2070 6174 7465 726e 0a20 2020 204e  ob pattern.    N
+00008e00: 6f74 6573 3a20 4f6e 6c79 2067 6c6f 6220  otes: Only glob 
+00008e10: 696e 2062 7563 6b65 742e 2049 6620 7472  in bucket. If tr
+00008e20: 7969 6e67 2074 6f20 6d61 7463 6820 6275  ying to match bu
+00008e30: 636b 6574 2077 6974 6820 7769 6c64 6361  cket with wildca
+00008e40: 7264 2063 6861 7261 6374 6572 732c 2072  rd characters, r
+00008e50: 6169 7365 2055 6e73 7570 706f 7274 6564  aise Unsupported
+00008e60: 4572 726f 720a 0a20 2020 203a 7061 7261  Error..    :para
+00008e70: 6d20 7265 6375 7273 6976 653a 2049 6620  m recursive: If 
+00008e80: 4661 6c73 652c 2060 2a2a 6020 7769 6c6c  False, `**` will
+00008e90: 206e 6f74 2073 6561 7263 6820 6469 7265   not search dire
+00008ea0: 6374 6f72 7920 7265 6375 7273 6976 656c  ctory recursivel
+00008eb0: 790a 2020 2020 3a70 6172 616d 206d 6973  y.    :param mis
+00008ec0: 7369 6e67 5f6f 6b3a 2049 6620 4661 6c73  sing_ok: If Fals
+00008ed0: 6520 616e 6420 7461 7267 6574 2070 6174  e and target pat
+00008ee0: 6820 646f 6573 6e27 7420 6d61 7463 6820  h doesn't match 
+00008ef0: 616e 7920 6669 6c65 2c20 7261 6973 6520  any file, raise 
+00008f00: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
+00008f10: 720a 2020 2020 3a72 6169 7365 733a 2055  r.    :raises: U
+00008f20: 6e73 7570 706f 7274 6564 4572 726f 722c  nsupportedError,
+00008f30: 2077 6865 6e20 6275 636b 6574 2070 6172   when bucket par
+00008f40: 7420 636f 6e74 6169 6e73 2077 696c 6463  t contains wildc
+00008f50: 6172 6420 6368 6172 6163 7465 7273 0a20  ard characters. 
+00008f60: 2020 203a 7265 7475 726e 733a 2041 206c     :returns: A l
+00008f70: 6973 7420 636f 6e74 6169 6e73 2070 6174  ist contains pat
+00008f80: 6873 206d 6174 6368 2060 7333 5f70 6174  hs match `s3_pat
+00008f90: 686e 616d 6560 0a20 2020 2027 2727 0a20  hname`.    '''. 
+00008fa0: 2020 2072 6574 7572 6e20 6c69 7374 280a     return list(.
+00008fb0: 2020 2020 2020 2020 7333 5f69 676c 6f62          s3_iglob
+00008fc0: 280a 2020 2020 2020 2020 2020 2020 7061  (.            pa
+00008fd0: 7468 3d70 6174 682c 0a20 2020 2020 2020  th=path,.       
+00008fe0: 2020 2020 2072 6563 7572 7369 7665 3d72       recursive=r
+00008ff0: 6563 7572 7369 7665 2c0a 2020 2020 2020  ecursive,.      
+00009000: 2020 2020 2020 6d69 7373 696e 675f 6f6b        missing_ok
+00009010: 3d6d 6973 7369 6e67 5f6f 6b2c 0a20 2020  =missing_ok,.   
+00009020: 2020 2020 2020 2020 2066 6f6c 6c6f 776c           followl
+00009030: 696e 6b73 3d66 6f6c 6c6f 776c 696e 6b73  inks=followlinks
+00009040: 2929 0a0a 0a64 6566 2073 335f 676c 6f62  ))...def s3_glob
+00009050: 5f73 7461 7428 0a20 2020 2020 2020 2070  _stat(.        p
+00009060: 6174 683a 2050 6174 684c 696b 652c 0a20  ath: PathLike,. 
+00009070: 2020 2020 2020 2072 6563 7572 7369 7665         recursive
+00009080: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+00009090: 2020 2020 2020 206d 6973 7369 6e67 5f6f         missing_o
+000090a0: 6b3a 2062 6f6f 6c20 3d20 5472 7565 2c0a  k: bool = True,.
+000090b0: 2020 2020 2020 2020 666f 6c6c 6f77 6c69          followli
+000090c0: 6e6b 733a 2062 6f6f 6c20 3d20 4661 6c73  nks: bool = Fals
+000090d0: 6529 202d 3e20 4974 6572 6174 6f72 5b46  e) -> Iterator[F
+000090e0: 696c 6545 6e74 7279 5d3a 0a20 2020 2027  ileEntry]:.    '
+000090f0: 2727 5265 7475 726e 2061 2067 656e 6572  ''Return a gener
+00009100: 6174 6f72 2063 6f6e 7461 696e 7320 7475  ator contains tu
+00009110: 706c 6573 206f 6620 7061 7468 2061 6e64  ples of path and
+00009120: 2066 696c 6520 7374 6174 2c20 696e 2061   file stat, in a
+00009130: 7363 656e 6469 6e67 2061 6c70 6861 6265  scending alphabe
+00009140: 7469 6361 6c20 6f72 6465 722c 2069 6e20  tical order, in 
+00009150: 7768 6963 6820 7061 7468 206d 6174 6368  which path match
+00009160: 6573 2067 6c6f 6220 7061 7474 6572 6e0a  es glob pattern.
+00009170: 2020 2020 4e6f 7465 733a 204f 6e6c 7920      Notes: Only 
+00009180: 676c 6f62 2069 6e20 6275 636b 6574 2e20  glob in bucket. 
+00009190: 4966 2074 7279 696e 6720 746f 206d 6174  If trying to mat
+000091a0: 6368 2062 7563 6b65 7420 7769 7468 2077  ch bucket with w
+000091b0: 696c 6463 6172 6420 6368 6172 6163 7465  ildcard characte
+000091c0: 7273 2c20 7261 6973 6520 556e 7375 7070  rs, raise Unsupp
+000091d0: 6f72 7465 6445 7272 6f72 0a0a 2020 2020  ortedError..    
+000091e0: 3a70 6172 616d 2072 6563 7572 7369 7665  :param recursive
+000091f0: 3a20 4966 2046 616c 7365 2c20 602a 2a60  : If False, `**`
+00009200: 2077 696c 6c20 6e6f 7420 7365 6172 6368   will not search
+00009210: 2064 6972 6563 746f 7279 2072 6563 7572   directory recur
+00009220: 7369 7665 6c79 0a20 2020 203a 7061 7261  sively.    :para
+00009230: 6d20 6d69 7373 696e 675f 6f6b 3a20 4966  m missing_ok: If
+00009240: 2046 616c 7365 2061 6e64 2074 6172 6765   False and targe
+00009250: 7420 7061 7468 2064 6f65 736e 2774 206d  t path doesn't m
+00009260: 6174 6368 2061 6e79 2066 696c 652c 2072  atch any file, r
+00009270: 6169 7365 2046 696c 654e 6f74 466f 756e  aise FileNotFoun
+00009280: 6445 7272 6f72 0a20 2020 203a 7261 6973  dError.    :rais
+00009290: 6573 3a20 556e 7375 7070 6f72 7465 6445  es: UnsupportedE
+000092a0: 7272 6f72 2c20 7768 656e 2062 7563 6b65  rror, when bucke
+000092b0: 7420 7061 7274 2063 6f6e 7461 696e 7320  t part contains 
+000092c0: 7769 6c64 6361 7264 2063 6861 7261 6374  wildcard charact
+000092d0: 6572 730a 2020 2020 3a72 6574 7572 6e73  ers.    :returns
+000092e0: 3a20 4120 6765 6e65 7261 746f 7220 636f  : A generator co
+000092f0: 6e74 6169 6e73 2074 7570 6c65 7320 6f66  ntains tuples of
+00009300: 2070 6174 6820 616e 6420 6669 6c65 2073   path and file s
+00009310: 7461 742c 2069 6e20 7768 6963 6820 7061  tat, in which pa
+00009320: 7468 7320 6d61 7463 6820 6073 335f 7061  ths match `s3_pa
+00009330: 7468 6e61 6d65 600a 2020 2020 2727 270a  thname`.    '''.
+00009340: 2020 2020 7265 7475 726e 2053 3350 6174      return S3Pat
+00009350: 6828 7061 7468 292e 676c 6f62 5f73 7461  h(path).glob_sta
+00009360: 7428 0a20 2020 2020 2020 2070 6174 7465  t(.        patte
+00009370: 726e 3d22 222c 0a20 2020 2020 2020 2072  rn="",.        r
+00009380: 6563 7572 7369 7665 3d72 6563 7572 7369  ecursive=recursi
+00009390: 7665 2c0a 2020 2020 2020 2020 6d69 7373  ve,.        miss
+000093a0: 696e 675f 6f6b 3d6d 6973 7369 6e67 5f6f  ing_ok=missing_o
+000093b0: 6b2c 0a20 2020 2020 2020 2066 6f6c 6c6f  k,.        follo
+000093c0: 776c 696e 6b73 3d66 6f6c 6c6f 776c 696e  wlinks=followlin
+000093d0: 6b73 290a 0a0a 6465 6620 7333 5f69 676c  ks)...def s3_igl
+000093e0: 6f62 280a 2020 2020 2020 2020 7061 7468  ob(.        path
+000093f0: 3a20 5061 7468 4c69 6b65 2c0a 2020 2020  : PathLike,.    
+00009400: 2020 2020 7265 6375 7273 6976 653a 2062      recursive: b
+00009410: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+00009420: 2020 2020 6d69 7373 696e 675f 6f6b 3a20      missing_ok: 
+00009430: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+00009440: 2020 2020 2066 6f6c 6c6f 776c 696e 6b73       followlinks
+00009450: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00009460: 2920 2d3e 2049 7465 7261 746f 725b 7374  ) -> Iterator[st
+00009470: 725d 3a0a 2020 2020 2727 2752 6574 7572  r]:.    '''Retur
+00009480: 6e20 7333 2070 6174 6820 6974 6572 6174  n s3 path iterat
+00009490: 6f72 2069 6e20 6173 6365 6e64 696e 6720  or in ascending 
+000094a0: 616c 7068 6162 6574 6963 616c 206f 7264  alphabetical ord
+000094b0: 6572 2c20 696e 2077 6869 6368 2070 6174  er, in which pat
+000094c0: 6820 6d61 7463 6865 7320 676c 6f62 2070  h matches glob p
+000094d0: 6174 7465 726e 0a20 2020 204e 6f74 6573  attern.    Notes
+000094e0: 3a20 4f6e 6c79 2067 6c6f 6220 696e 2062  : Only glob in b
+000094f0: 7563 6b65 742e 2049 6620 7472 7969 6e67  ucket. If trying
+00009500: 2074 6f20 6d61 7463 6820 6275 636b 6574   to match bucket
+00009510: 2077 6974 6820 7769 6c64 6361 7264 2063   with wildcard c
+00009520: 6861 7261 6374 6572 732c 2072 6169 7365  haracters, raise
+00009530: 2055 6e73 7570 706f 7274 6564 4572 726f   UnsupportedErro
+00009540: 720a 0a20 2020 203a 7061 7261 6d20 7265  r..    :param re
+00009550: 6375 7273 6976 653a 2049 6620 4661 6c73  cursive: If Fals
+00009560: 652c 2060 2a2a 6020 7769 6c6c 206e 6f74  e, `**` will not
+00009570: 2073 6561 7263 6820 6469 7265 6374 6f72   search director
+00009580: 7920 7265 6375 7273 6976 656c 790a 2020  y recursively.  
+00009590: 2020 3a70 6172 616d 206d 6973 7369 6e67    :param missing
+000095a0: 5f6f 6b3a 2049 6620 4661 6c73 6520 616e  _ok: If False an
+000095b0: 6420 7461 7267 6574 2070 6174 6820 646f  d target path do
+000095c0: 6573 6e27 7420 6d61 7463 6820 616e 7920  esn't match any 
+000095d0: 6669 6c65 2c20 7261 6973 6520 4669 6c65  file, raise File
+000095e0: 4e6f 7446 6f75 6e64 4572 726f 720a 2020  NotFoundError.  
+000095f0: 2020 3a72 6169 7365 733a 2055 6e73 7570    :raises: Unsup
+00009600: 706f 7274 6564 4572 726f 722c 2077 6865  portedError, whe
+00009610: 6e20 6275 636b 6574 2070 6172 7420 636f  n bucket part co
+00009620: 6e74 6169 6e73 2077 696c 6463 6172 6420  ntains wildcard 
+00009630: 6368 6172 6163 7465 7273 0a20 2020 203a  characters.    :
+00009640: 7265 7475 726e 733a 2041 6e20 6974 6572  returns: An iter
+00009650: 6174 6f72 2063 6f6e 7461 696e 7320 7061  ator contains pa
+00009660: 7468 7320 6d61 7463 6820 6073 335f 7061  ths match `s3_pa
+00009670: 7468 6e61 6d65 600a 2020 2020 2727 270a  thname`.    '''.
+00009680: 2020 2020 666f 7220 7061 7468 5f6f 626a      for path_obj
+00009690: 2069 6e20 5333 5061 7468 2870 6174 6829   in S3Path(path)
+000096a0: 2e69 676c 6f62 2870 6174 7465 726e 3d22  .iglob(pattern="
+000096b0: 222c 2072 6563 7572 7369 7665 3d72 6563  ", recursive=rec
+000096c0: 7572 7369 7665 2c0a 2020 2020 2020 2020  ursive,.        
+000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000096f0: 6973 7369 6e67 5f6f 6b3d 6d69 7373 696e  issing_ok=missin
+00009700: 675f 6f6b 2c0a 2020 2020 2020 2020 2020  g_ok,.          
+00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009720: 2020 2020 2020 2020 2020 2020 2066 6f6c               fol
+00009730: 6c6f 776c 696e 6b73 3d66 6f6c 6c6f 776c  lowlinks=followl
+00009740: 696e 6b73 293a 0a20 2020 2020 2020 2079  inks):.        y
+00009750: 6965 6c64 2070 6174 685f 6f62 6a2e 7061  ield path_obj.pa
+00009760: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
+00009770: 0a0a 0a64 6566 2073 335f 6d61 6b65 6469  ...def s3_makedi
+00009780: 7273 2870 6174 683a 2050 6174 684c 696b  rs(path: PathLik
+00009790: 652c 2065 7869 7374 5f6f 6b3a 2062 6f6f  e, exist_ok: boo
+000097a0: 6c20 3d20 4661 6c73 6529 3a0a 2020 2020  l = False):.    
+000097b0: 2727 270a 2020 2020 4372 6561 7465 2061  '''.    Create a
+000097c0: 6e20 7333 2064 6972 6563 746f 7279 2e0a  n s3 directory..
+000097d0: 2020 2020 5075 7265 6c79 2063 7265 6174      Purely creat
+000097e0: 696e 6720 6469 7265 6374 6f72 7920 6973  ing directory is
+000097f0: 2069 6e76 616c 6964 2062 6563 6175 7365   invalid because
+00009800: 2069 7427 7320 756e 6176 6169 6c61 626c   it's unavailabl
+00009810: 6520 6f6e 204f 5353 2e0a 2020 2020 5468  e on OSS..    Th
+00009820: 6973 2066 756e 6374 696f 6e20 6973 2074  is function is t
+00009830: 6f20 7465 7374 2074 6865 2074 6172 6765  o test the targe
+00009840: 7420 6275 636b 6574 2068 6176 6520 5752  t bucket have WR
+00009850: 4954 4520 6163 6365 7373 2e0a 0a20 2020  ITE access...   
+00009860: 203a 7061 7261 6d20 7061 7468 3a20 4769   :param path: Gi
+00009870: 7665 6e20 7061 7468 0a20 2020 203a 7061  ven path.    :pa
+00009880: 7261 6d20 6578 6973 745f 6f6b 3a20 4966  ram exist_ok: If
+00009890: 2046 616c 7365 2061 6e64 2074 6172 6765   False and targe
+000098a0: 7420 6469 7265 6374 6f72 7920 6578 6973  t directory exis
+000098b0: 7473 2c20 7261 6973 6520 5333 4669 6c65  ts, raise S3File
+000098c0: 4578 6973 7473 4572 726f 720a 2020 2020  ExistsError.    
+000098d0: 3a72 6169 7365 733a 2053 3342 7563 6b65  :raises: S3Bucke
+000098e0: 744e 6f74 466f 756e 6445 7272 6f72 2c20  tNotFoundError, 
+000098f0: 5333 4669 6c65 4578 6973 7473 4572 726f  S3FileExistsErro
+00009900: 720a 2020 2020 2727 270a 2020 2020 7265  r.    '''.    re
+00009910: 7475 726e 2053 3350 6174 6828 7061 7468  turn S3Path(path
+00009920: 292e 6d6b 6469 7228 7061 7265 6e74 733d  ).mkdir(parents=
+00009930: 5472 7565 2c20 6578 6973 745f 6f6b 3d65  True, exist_ok=e
+00009940: 7869 7374 5f6f 6b29 0a0a 0a64 6566 205f  xist_ok)...def _
+00009950: 6772 6f75 705f 7372 635f 7061 7468 735f  group_src_paths_
+00009960: 6279 5f62 6c6f 636b 280a 2020 2020 2020  by_block(.      
+00009970: 2020 7372 635f 7061 7468 733a 204c 6973    src_paths: Lis
+00009980: 745b 5061 7468 4c69 6b65 5d2c 2062 6c6f  t[PathLike], blo
+00009990: 636b 5f73 697a 653a 2069 6e74 203d 2044  ck_size: int = D
+000099a0: 4546 4155 4c54 5f42 4c4f 434b 5f53 495a  EFAULT_BLOCK_SIZ
+000099b0: 450a 2920 2d3e 204c 6973 745b 4c69 7374  E.) -> List[List
+000099c0: 5b54 7570 6c65 5b50 6174 684c 696b 652c  [Tuple[PathLike,
+000099d0: 204f 7074 696f 6e61 6c5b 7374 725d 5d5d   Optional[str]]]
+000099e0: 5d3a 0a20 2020 2067 726f 7570 7320 3d20  ]:.    groups = 
+000099f0: 5b5d 0a20 2020 2063 7572 7265 6e74 5f67  [].    current_g
+00009a00: 726f 7570 2c20 6375 7272 656e 745f 6772  roup, current_gr
+00009a10: 6f75 705f 7369 7a65 203d 205b 5d2c 2030  oup_size = [], 0
+00009a20: 0a20 2020 2066 6f72 2073 7263 5f70 6174  .    for src_pat
+00009a30: 6820 696e 2073 7263 5f70 6174 6873 3a0a  h in src_paths:.
+00009a40: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00009a50: 6669 6c65 5f73 697a 6520 3d20 5333 5061  file_size = S3Pa
+00009a60: 7468 2873 7263 5f70 6174 6829 2e73 7461  th(src_path).sta
+00009a70: 7428 292e 7369 7a65 0a20 2020 2020 2020  t().size.       
+00009a80: 2069 6620 6375 7272 656e 745f 6669 6c65   if current_file
+00009a90: 5f73 697a 6520 3d3d 2030 3a20 2023 2070  _size == 0:  # p
+00009aa0: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+00009ab0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00009ac0: 696e 7565 0a0a 2020 2020 2020 2020 6966  inue..        if
+00009ad0: 2063 7572 7265 6e74 5f66 696c 655f 7369   current_file_si
+00009ae0: 7a65 203e 3d20 626c 6f63 6b5f 7369 7a65  ze >= block_size
+00009af0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00009b00: 206c 656e 2867 726f 7570 7329 203d 3d20   len(groups) == 
+00009b10: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00009b20: 2020 2069 6620 6375 7272 656e 745f 6772     if current_gr
+00009b30: 6f75 705f 7369 7a65 202b 2063 7572 7265  oup_size + curre
+00009b40: 6e74 5f66 696c 655f 7369 7a65 203e 2032  nt_file_size > 2
+00009b50: 202a 2062 6c6f 636b 5f73 697a 653a 0a20   * block_size:. 
+00009b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b70: 2020 2067 726f 7570 5f6c 6163 6b5f 7369     group_lack_si
+00009b80: 7a65 203d 2062 6c6f 636b 5f73 697a 6520  ze = block_size 
+00009b90: 2d20 6375 7272 656e 745f 6772 6f75 705f  - current_group_
+00009ba0: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
+00009bb0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00009bc0: 5f67 726f 7570 2e61 7070 656e 6428 0a20  _group.append(. 
+00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009be0: 2020 2020 2020 2028 7372 635f 7061 7468         (src_path
+00009bf0: 2c20 6627 6279 7465 733d 302d 7b67 726f  , f'bytes=0-{gro
+00009c00: 7570 5f6c 6163 6b5f 7369 7a65 2d31 7d27  up_lack_size-1}'
+00009c10: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00009c20: 2020 2020 2020 2067 726f 7570 732e 6578         groups.ex
+00009c30: 7465 6e64 280a 2020 2020 2020 2020 2020  tend(.          
+00009c40: 2020 2020 2020 2020 2020 2020 2020 5b0a                [.
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00009c70: 656e 745f 6772 6f75 702c 0a20 2020 2020  ent_group,.     
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c90: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cb0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009ce0: 7263 5f70 6174 682c 0a20 2020 2020 2020  rc_path,.       
+00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d00: 2020 2020 2020 2020 2020 2020 2066 2762               f'b
+00009d10: 7974 6573 3d7b 6772 6f75 705f 6c61 636b  ytes={group_lack
+00009d20: 5f73 697a 657d 2d7b 6375 7272 656e 745f  _size}-{current_
+00009d30: 6669 6c65 5f73 697a 652d 317d 270a 2020  file_size-1}'.  
+00009d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d50: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d70: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d90: 2020 2020 2020 5d29 0a20 2020 2020 2020        ]).       
+00009da0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dc0: 2020 2063 7572 7265 6e74 5f67 726f 7570     current_group
+00009dd0: 2e61 7070 656e 6428 2873 7263 5f70 6174  .append((src_pat
+00009de0: 682c 204e 6f6e 6529 290a 2020 2020 2020  h, None)).      
+00009df0: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+00009e00: 6f75 7073 2e61 7070 656e 6428 6375 7272  oups.append(curr
+00009e10: 656e 745f 6772 6f75 7029 0a20 2020 2020  ent_group).     
+00009e20: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00009e30: 2020 2020 2020 2020 2020 2020 2067 726f               gro
+00009e40: 7570 735b 2d31 5d2e 6578 7465 6e64 2863  ups[-1].extend(c
+00009e50: 7572 7265 6e74 5f67 726f 7570 290a 2020  urrent_group).  
+00009e60: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+00009e70: 6f75 7073 2e61 7070 656e 6428 5b28 7372  oups.append([(sr
+00009e80: 635f 7061 7468 2c20 4e6f 6e65 295d 290a  c_path, None)]).
+00009e90: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00009ea0: 656e 745f 6772 6f75 702c 2063 7572 7265  ent_group, curre
+00009eb0: 6e74 5f67 726f 7570 5f73 697a 6520 3d20  nt_group_size = 
+00009ec0: 5b5d 2c20 300a 2020 2020 2020 2020 656c  [], 0.        el
+00009ed0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009ee0: 6375 7272 656e 745f 6772 6f75 702e 6170  current_group.ap
+00009ef0: 7065 6e64 2828 7372 635f 7061 7468 2c20  pend((src_path, 
+00009f00: 4e6f 6e65 2929 0a20 2020 2020 2020 2020  None)).         
+00009f10: 2020 2063 7572 7265 6e74 5f67 726f 7570     current_group
+00009f20: 5f73 697a 6520 2b3d 2063 7572 7265 6e74  _size += current
+00009f30: 5f66 696c 655f 7369 7a65 0a20 2020 2020  _file_size.     
+00009f40: 2020 2020 2020 2069 6620 6375 7272 656e         if curren
+00009f50: 745f 6772 6f75 705f 7369 7a65 203e 3d20  t_group_size >= 
+00009f60: 626c 6f63 6b5f 7369 7a65 3a0a 2020 2020  block_size:.    
+00009f70: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+00009f80: 7073 2e61 7070 656e 6428 6375 7272 656e  ps.append(curren
+00009f90: 745f 6772 6f75 7029 0a20 2020 2020 2020  t_group).       
+00009fa0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00009fb0: 5f67 726f 7570 2c20 6375 7272 656e 745f  _group, current_
+00009fc0: 6772 6f75 705f 7369 7a65 203d 205b 5d2c  group_size = [],
+00009fd0: 2030 0a20 2020 2069 6620 6375 7272 656e   0.    if curren
+00009fe0: 745f 6772 6f75 703a 0a20 2020 2020 2020  t_group:.       
+00009ff0: 2067 726f 7570 732e 6170 7065 6e64 2863   groups.append(c
+0000a000: 7572 7265 6e74 5f67 726f 7570 290a 2020  urrent_group).  
+0000a010: 2020 7265 7475 726e 2067 726f 7570 730a    return groups.
+0000a020: 0a0a 6465 6620 7333 5f63 6f6e 6361 7428  ..def s3_concat(
+0000a030: 0a20 2020 2020 2020 2073 7263 5f70 6174  .        src_pat
+0000a040: 6873 3a20 4c69 7374 5b50 6174 684c 696b  hs: List[PathLik
+0000a050: 655d 2c0a 2020 2020 2020 2020 6473 745f  e],.        dst_
+0000a060: 7061 7468 3a20 5061 7468 4c69 6b65 2c0a  path: PathLike,.
+0000a070: 2020 2020 2020 2020 626c 6f63 6b5f 7369          block_si
+0000a080: 7a65 3a20 696e 7420 3d20 4445 4641 554c  ze: int = DEFAUL
+0000a090: 545f 424c 4f43 4b5f 5349 5a45 2c0a 2020  T_BLOCK_SIZE,.  
+0000a0a0: 2020 2020 2020 6d61 785f 776f 726b 6572        max_worker
+0000a0b0: 733a 2069 6e74 203d 2047 4c4f 4241 4c5f  s: int = GLOBAL_
+0000a0c0: 4d41 585f 574f 524b 4552 5329 202d 3e20  MAX_WORKERS) -> 
+0000a0d0: 4e6f 6e65 3a0a 2020 2020 2727 2743 6f6e  None:.    '''Con
+0000a0e0: 6361 7465 6e61 7465 2073 3320 6669 6c65  catenate s3 file
+0000a0f0: 7320 746f 206f 6e65 2066 696c 652e 0a0a  s to one file...
+0000a100: 2020 2020 3a70 6172 616d 2073 7263 5f70      :param src_p
+0000a110: 6174 6873 3a20 4769 7665 6e20 736f 7572  aths: Given sour
+0000a120: 6365 2070 6174 6873 0a20 2020 203a 7061  ce paths.    :pa
+0000a130: 7261 6d20 6473 745f 7061 7468 3a20 4769  ram dst_path: Gi
+0000a140: 7665 6e20 6465 7374 696e 6174 696f 6e20  ven destination 
+0000a150: 7061 7468 0a20 2020 2027 2727 0a20 2020  path.    '''.   
+0000a160: 2063 6c69 656e 7420 3d20 5333 5061 7468   client = S3Path
+0000a170: 2864 7374 5f70 6174 6829 2e5f 636c 6965  (dst_path)._clie
+0000a180: 6e74 0a20 2020 2077 6974 6820 7261 6973  nt.    with rais
+0000a190: 655f 7333 5f65 7272 6f72 2864 7374 5f70  e_s3_error(dst_p
+0000a1a0: 6174 6829 3a0a 2020 2020 2020 2020 6966  ath):.        if
+0000a1b0: 2062 6c6f 636b 5f73 697a 6520 3d3d 2030   block_size == 0
+0000a1c0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+0000a1d0: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+0000a1e0: 2020 6772 6f75 7073 203d 205b 5b28 7372    groups = [[(sr
+0000a1f0: 635f 7061 7468 2c20 4e6f 6e65 295d 2066  c_path, None)] f
+0000a200: 6f72 2073 7263 5f70 6174 6820 696e 2073  or src_path in s
+0000a210: 7263 5f70 6174 6873 5d0a 2020 2020 2020  rc_paths].      
+0000a220: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a230: 2020 2020 6772 6f75 7073 203d 205f 6772      groups = _gr
+0000a240: 6f75 705f 7372 635f 7061 7468 735f 6279  oup_src_paths_by
+0000a250: 5f62 6c6f 636b 2873 7263 5f70 6174 6873  _block(src_paths
+0000a260: 2c20 626c 6f63 6b5f 7369 7a65 3d62 6c6f  , block_size=blo
+0000a270: 636b 5f73 697a 6529 0a0a 2020 2020 2020  ck_size)..      
+0000a280: 2020 7769 7468 204d 756c 7469 5061 7274    with MultiPart
+0000a290: 5772 6974 6572 2863 6c69 656e 742c 2064  Writer(client, d
+0000a2a0: 7374 5f70 6174 6829 2061 7320 7772 6974  st_path) as writ
+0000a2b0: 6572 2c20 5468 7265 6164 506f 6f6c 4578  er, ThreadPoolEx
+0000a2c0: 6563 7574 6f72 280a 2020 2020 2020 2020  ecutor(.        
+0000a2d0: 2020 2020 2020 2020 6d61 785f 776f 726b          max_work
+0000a2e0: 6572 733d 6d61 785f 776f 726b 6572 7329  ers=max_workers)
+0000a2f0: 2061 7320 6578 6563 7574 6f72 3a0a 2020   as executor:.  
+0000a300: 2020 2020 2020 2020 2020 666f 7220 696e            for in
+0000a310: 6465 782c 2067 726f 7570 2069 6e20 656e  dex, group in en
+0000a320: 756d 6572 6174 6528 6772 6f75 7073 2c20  umerate(groups, 
+0000a330: 7374 6172 743d 3129 3a0a 2020 2020 2020  start=1):.      
+0000a340: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000a350: 2867 726f 7570 2920 3d3d 2031 3a0a 2020  (group) == 1:.  
+0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a370: 2020 6578 6563 7574 6f72 2e73 7562 6d69    executor.submi
+0000a380: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000a390: 2020 2020 2020 2020 2020 2077 7269 7465             write
+0000a3a0: 722e 7570 6c6f 6164 5f70 6172 745f 636f  r.upload_part_co
+0000a3b0: 7079 2c20 696e 6465 782c 2067 726f 7570  py, index, group
+0000a3c0: 5b30 5d5b 305d 2c0a 2020 2020 2020 2020  [0][0],.        
+0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3e0: 6772 6f75 705b 305d 5b31 5d29 0a20 2020  group[0][1]).   
+0000a3f0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000a400: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000a410: 2020 2020 2020 2065 7865 6375 746f 722e         executor.
+0000a420: 7375 626d 6974 2877 7269 7465 722e 7570  submit(writer.up
+0000a430: 6c6f 6164 5f70 6172 745f 6279 5f70 6174  load_part_by_pat
+0000a440: 6873 2c20 696e 6465 782c 2067 726f 7570  hs, index, group
+0000a450: 290a 0a0a 4053 6d61 7274 5061 7468 2e72  )...@SmartPath.r
+0000a460: 6567 6973 7465 720a 636c 6173 7320 5333  egister.class S3
+0000a470: 5061 7468 2855 5249 5061 7468 293a 0a0a  Path(URIPath):..
+0000a480: 2020 2020 7072 6f74 6f63 6f6c 203d 2022      protocol = "
+0000a490: 7333 220a 0a20 2020 2064 6566 205f 5f69  s3"..    def __i
+0000a4a0: 6e69 745f 5f28 7365 6c66 2c20 7061 7468  nit__(self, path
+0000a4b0: 3a20 2250 6174 684c 696b 6522 2c20 2a6f  : "PathLike", *o
+0000a4c0: 7468 6572 5f70 6174 6873 3a20 2250 6174  ther_paths: "Pat
+0000a4d0: 684c 696b 6522 293a 0a20 2020 2020 2020  hLike"):.       
+0000a4e0: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+0000a4f0: 5f28 7061 7468 2c20 2a6f 7468 6572 5f70  _(path, *other_p
+0000a500: 6174 6873 290a 2020 2020 2020 2020 7072  aths).        pr
+0000a510: 6f74 6f63 6f6c 203d 2067 6574 5f75 726c  otocol = get_url
+0000a520: 5f73 6368 656d 6528 7365 6c66 2e70 6174  _scheme(self.pat
+0000a530: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
+0000a540: 5f70 726f 746f 636f 6c5f 7769 7468 5f70  _protocol_with_p
+0000a550: 726f 6669 6c65 203d 2073 656c 662e 7072  rofile = self.pr
+0000a560: 6f74 6f63 6f6c 0a20 2020 2020 2020 2073  otocol.        s
+0000a570: 656c 662e 5f70 726f 6669 6c65 5f6e 616d  elf._profile_nam
+0000a580: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
+0000a590: 2069 6620 7072 6f74 6f63 6f6c 2e73 7461   if protocol.sta
+0000a5a0: 7274 7377 6974 6828 2773 332b 2729 3a0a  rtswith('s3+'):.
+0000a5b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a5c0: 2e5f 7072 6f74 6f63 6f6c 5f77 6974 685f  ._protocol_with_
+0000a5d0: 7072 6f66 696c 6520 3d20 7072 6f74 6f63  profile = protoc
+0000a5e0: 6f6c 0a20 2020 2020 2020 2020 2020 2073  ol.            s
+0000a5f0: 656c 662e 5f70 726f 6669 6c65 5f6e 616d  elf._profile_nam
+0000a600: 6520 3d20 7072 6f74 6f63 6f6c 5b33 3a5d  e = protocol[3:]
+0000a610: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000a620: 662e 5f73 335f 7061 7468 203d 2066 2273  f._s3_path = f"s
+0000a630: 333a 2f2f 7b73 656c 662e 7061 7468 5b6c  3://{self.path[l
+0000a640: 656e 2870 726f 746f 636f 6c29 2b33 3a5d  en(protocol)+3:]
+0000a650: 7d22 0a20 2020 2020 2020 2065 6c69 6620  }".        elif 
+0000a660: 6e6f 7420 7072 6f74 6f63 6f6c 3a0a 2020  not protocol:.  
+0000a670: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a680: 7333 5f70 6174 6820 3d20 6622 7333 3a2f  s3_path = f"s3:/
+0000a690: 2f7b 7365 6c66 2e70 6174 682e 6c73 7472  /{self.path.lstr
+0000a6a0: 6970 2827 2f27 297d 220a 2020 2020 2020  ip('/')}".      
+0000a6b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a6c0: 2020 2020 7365 6c66 2e5f 7333 5f70 6174      self._s3_pat
+0000a6d0: 6820 3d20 7365 6c66 2e70 6174 680a 0a20  h = self.path.. 
+0000a6e0: 2020 2040 6361 6368 6564 7072 6f70 6572     @cachedproper
+0000a6f0: 7479 0a20 2020 2064 6566 2070 6174 685f  ty.    def path_
+0000a700: 7769 7468 5f70 726f 746f 636f 6c28 7365  with_protocol(se
+0000a710: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+0000a720: 2020 2020 2727 2752 6574 7572 6e20 7061      '''Return pa
+0000a730: 7468 2077 6974 6820 7072 6f74 6f63 6f6c  th with protocol
+0000a740: 2c20 6c69 6b65 2066 696c 653a 2f2f 2f72  , like file:///r
+0000a750: 6f6f 742c 2073 333a 2f2f 6275 636b 6574  oot, s3://bucket
+0000a760: 2f6b 6579 2727 270a 2020 2020 2020 2020  /key'''.        
+0000a770: 7061 7468 203d 2073 656c 662e 7061 7468  path = self.path
+0000a780: 0a20 2020 2020 2020 2070 726f 746f 636f  .        protoco
+0000a790: 6c5f 7072 6566 6978 203d 2073 656c 662e  l_prefix = self.
+0000a7a0: 5f70 726f 746f 636f 6c5f 7769 7468 5f70  _protocol_with_p
+0000a7b0: 726f 6669 6c65 202b 2022 3a2f 2f22 0a20  rofile + "://". 
+0000a7c0: 2020 2020 2020 2069 6620 7061 7468 2e73         if path.s
+0000a7d0: 7461 7274 7377 6974 6828 7072 6f74 6f63  tartswith(protoc
+0000a7e0: 6f6c 5f70 7265 6669 7829 3a0a 2020 2020  ol_prefix):.    
+0000a7f0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+0000a800: 6174 680a 2020 2020 2020 2020 7265 7475  ath.        retu
+0000a810: 726e 2070 726f 746f 636f 6c5f 7072 6566  rn protocol_pref
+0000a820: 6978 202b 2070 6174 682e 6c73 7472 6970  ix + path.lstrip
+0000a830: 2827 2f27 290a 0a20 2020 2040 6361 6368  ('/')..    @cach
+0000a840: 6564 7072 6f70 6572 7479 0a20 2020 2064  edproperty.    d
+0000a850: 6566 2070 6174 685f 7769 7468 6f75 745f  ef path_without_
+0000a860: 7072 6f74 6f63 6f6c 2873 656c 6629 202d  protocol(self) -
+0000a870: 3e20 7374 723a 0a20 2020 2020 2020 2027  > str:.        '
+0000a880: 2727 5265 7475 726e 2070 6174 6820 7769  ''Return path wi
+0000a890: 7468 6f75 7420 7072 6f74 6f63 6f6c 2c20  thout protocol, 
+0000a8a0: 6578 616d 706c 653a 2069 6620 7061 7468  example: if path
+0000a8b0: 2069 7320 7333 3a2f 2f62 7563 6b65 742f   is s3://bucket/
+0000a8c0: 6b65 792c 2072 6574 7572 6e20 6275 636b  key, return buck
+0000a8d0: 6574 2f6b 6579 2727 270a 2020 2020 2020  et/key'''.      
+0000a8e0: 2020 7061 7468 203d 2073 656c 662e 7061    path = self.pa
+0000a8f0: 7468 0a20 2020 2020 2020 2070 726f 746f  th.        proto
+0000a900: 636f 6c5f 7072 6566 6978 203d 2073 656c  col_prefix = sel
+0000a910: 662e 5f70 726f 746f 636f 6c5f 7769 7468  f._protocol_with
+0000a920: 5f70 726f 6669 6c65 202b 2022 3a2f 2f22  _profile + "://"
+0000a930: 0a20 2020 2020 2020 2069 6620 7061 7468  .        if path
+0000a940: 2e73 7461 7274 7377 6974 6828 7072 6f74  .startswith(prot
+0000a950: 6f63 6f6c 5f70 7265 6669 7829 3a0a 2020  ocol_prefix):.  
+0000a960: 2020 2020 2020 2020 2020 7061 7468 203d            path =
+0000a970: 2070 6174 685b 6c65 6e28 7072 6f74 6f63   path[len(protoc
+0000a980: 6f6c 5f70 7265 6669 7829 3a5d 0a20 2020  ol_prefix):].   
+0000a990: 2020 2020 2072 6574 7572 6e20 7061 7468       return path
+0000a9a0: 0a0a 2020 2020 4063 6163 6865 6470 726f  ..    @cachedpro
+0000a9b0: 7065 7274 790a 2020 2020 6465 6620 5f63  perty.    def _c
+0000a9c0: 6c69 656e 7428 7365 6c66 293a 0a20 2020  lient(self):.   
+0000a9d0: 2020 2020 2072 6574 7572 6e20 6765 745f       return get_
+0000a9e0: 7333 5f63 6c69 656e 7428 7072 6f66 696c  s3_client(profil
+0000a9f0: 655f 6e61 6d65 3d73 656c 662e 5f70 726f  e_name=self._pro
+0000aa00: 6669 6c65 5f6e 616d 6529 0a0a 2020 2020  file_name)..    
+0000aa10: 6465 6620 5f73 335f 6765 745f 6d65 7461  def _s3_get_meta
+0000aa20: 6461 7461 2873 656c 6629 202d 3e20 6469  data(self) -> di
+0000aa30: 6374 3a0a 2020 2020 2020 2020 2727 270a  ct:.        '''.
+0000aa40: 2020 2020 2020 2020 4765 7420 6f62 6a65          Get obje
+0000aa50: 6374 206d 6574 6164 6174 610a 0a20 2020  ct metadata..   
+0000aa60: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
+0000aa70: 3a20 4f62 6a65 6374 2070 6174 680a 2020  : Object path.  
+0000aa80: 2020 2020 2020 3a72 6574 7572 6e73 3a20        :returns: 
+0000aa90: 4f62 6a65 6374 206d 6574 6164 6174 610a  Object metadata.
+0000aaa0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000aab0: 2020 2020 6275 636b 6574 2c20 6b65 7920      bucket, key 
+0000aac0: 3d20 7061 7273 655f 7333 5f75 726c 2873  = parse_s3_url(s
+0000aad0: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
+0000aae0: 6f74 6f63 6f6c 290a 2020 2020 2020 2020  otocol).        
+0000aaf0: 6966 206e 6f74 2062 7563 6b65 743a 0a20  if not bucket:. 
+0000ab00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ab10: 6e20 7b7d 0a20 2020 2020 2020 2069 6620  n {}.        if 
+0000ab20: 6e6f 7420 6b65 7920 6f72 206b 6579 2e65  not key or key.e
+0000ab30: 6e64 7377 6974 6828 272f 2729 3a0a 2020  ndswith('/'):.  
+0000ab40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ab50: 207b 7d0a 2020 2020 2020 2020 7472 793a   {}.        try:
+0000ab60: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000ab70: 6820 7261 6973 655f 7333 5f65 7272 6f72  h raise_s3_error
+0000ab80: 2873 656c 662e 7061 7468 5f77 6974 685f  (self.path_with_
+0000ab90: 7072 6f74 6f63 6f6c 293a 0a20 2020 2020  protocol):.     
+0000aba0: 2020 2020 2020 2020 2020 2072 6573 7020             resp 
+0000abb0: 3d20 7365 6c66 2e5f 636c 6965 6e74 2e68  = self._client.h
+0000abc0: 6561 645f 6f62 6a65 6374 2842 7563 6b65  ead_object(Bucke
+0000abd0: 743d 6275 636b 6574 2c20 4b65 793d 6b65  t=bucket, Key=ke
+0000abe0: 7929 0a20 2020 2020 2020 2020 2020 2072  y).            r
+0000abf0: 6574 7572 6e20 6469 6374 280a 2020 2020  eturn dict(.    
+0000ac00: 2020 2020 2020 2020 2020 2020 286b 6579              (key
+0000ac10: 2e6c 6f77 6572 2829 2c20 7661 6c75 6529  .lower(), value)
+0000ac20: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+0000ac30: 696e 2072 6573 705b 274d 6574 6164 6174  in resp['Metadat
+0000ac40: 6127 5d2e 6974 656d 7328 2929 0a20 2020  a'].items()).   
+0000ac50: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0000ac60: 7074 696f 6e20 6173 2065 7272 6f72 3a0a  ption as error:.
+0000ac70: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000ac80: 7369 6e73 7461 6e63 6528 6572 726f 722c  sinstance(error,
+0000ac90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aca0: 2020 2020 2020 2020 2020 2028 5333 556e             (S3Un
+0000acb0: 6b6e 6f77 6e45 7272 6f72 2c20 5333 436f  knownError, S3Co
+0000acc0: 6e66 6967 4572 726f 722c 2053 3350 6572  nfigError, S3Per
+0000acd0: 6d69 7373 696f 6e45 7272 6f72 2929 3a0a  missionError)):.
+0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acf0: 7261 6973 6520 6572 726f 720a 2020 2020  raise error.    
+0000ad00: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+0000ad10: 7d0a 0a20 2020 2064 6566 2061 6363 6573  }..    def acces
+0000ad20: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
+0000ad30: 656c 662c 206d 6f64 653a 2041 6363 6573  elf, mode: Acces
+0000ad40: 7320 3d20 4163 6365 7373 2e52 4541 442c  s = Access.READ,
+0000ad50: 0a20 2020 2020 2020 2020 2020 2066 6f6c  .            fol
+0000ad60: 6c6f 776c 696e 6b73 3a20 626f 6f6c 203d  lowlinks: bool =
+0000ad70: 2046 616c 7365 2920 2d3e 2062 6f6f 6c3a   False) -> bool:
+0000ad80: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+0000ad90: 2020 2020 2054 6573 7420 6966 2070 6174       Test if pat
+0000ada0: 6820 6861 7320 6163 6365 7373 2070 6572  h has access per
+0000adb0: 6d69 7373 696f 6e20 6465 7363 7269 6265  mission describe
+0000adc0: 6420 6279 206d 6f64 650a 2020 2020 2020  d by mode.      
+0000add0: 2020 5573 696e 6720 6865 6164 5f62 7563    Using head_buc
+0000ade0: 6b65 7428 292c 206e 6f77 2052 4541 442f  ket(), now READ/
+0000adf0: 5752 4954 4520 6172 6520 7361 6d65 2e0a  WRITE are same..
+0000ae00: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000ae10: 6d6f 6465 3a20 6163 6365 7373 206d 6f64  mode: access mod
+0000ae20: 650a 2020 2020 2020 2020 3a72 6574 7572  e.        :retur
+0000ae30: 6e73 3a20 626f 6f6c 2c20 6966 2074 6865  ns: bool, if the
+0000ae40: 2062 7563 6b65 7420 6f66 2073 335f 7572   bucket of s3_ur
+0000ae50: 6c20 6861 7320 7265 6164 2f77 7269 7465  l has read/write
+0000ae60: 2061 6363 6573 732e 0a20 2020 2020 2020   access..       
+0000ae70: 2027 2727 0a20 2020 2020 2020 2073 335f   '''.        s3_
+0000ae80: 7572 6c20 3d20 7365 6c66 2e70 6174 685f  url = self.path_
+0000ae90: 7769 7468 5f70 726f 746f 636f 6c0a 2020  with_protocol.  
+0000aea0: 2020 2020 2020 6966 2066 6f6c 6c6f 776c        if followl
+0000aeb0: 696e 6b73 3a0a 2020 2020 2020 2020 2020  inks:.          
+0000aec0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000aed0: 2020 2020 2020 2073 335f 7572 6c20 3d20         s3_url = 
+0000aee0: 7365 6c66 2e72 6561 646c 696e 6b28 292e  self.readlink().
+0000aef0: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
+0000af00: 6f6c 0a20 2020 2020 2020 2020 2020 2065  ol.            e
+0000af10: 7863 6570 7420 5333 4e6f 7441 4c69 6e6b  xcept S3NotALink
+0000af20: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+0000af30: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+0000af40: 2020 2020 6275 636b 6574 2c20 5f20 3d20      bucket, _ = 
+0000af50: 7061 7273 655f 7333 5f75 726c 2873 335f  parse_s3_url(s3_
+0000af60: 7572 6c29 2020 2320 6f6e 6c79 2063 6865  url)  # only che
+0000af70: 636b 2062 7563 6b65 7420 6163 6365 7373  ck bucket access
+0000af80: 6962 696c 6974 790a 2020 2020 2020 2020  ibility.        
+0000af90: 6966 206e 6f74 2062 7563 6b65 743a 0a20  if not bucket:. 
+0000afa0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000afb0: 2045 7863 6570 7469 6f6e 2822 4e6f 2061   Exception("No a
+0000afc0: 7661 696c 6162 6c65 2062 7563 6b65 7422  vailable bucket"
+0000afd0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+0000afe0: 2069 7369 6e73 7461 6e63 6528 6d6f 6465   isinstance(mode
+0000aff0: 2c20 4163 6365 7373 293a 0a20 2020 2020  , Access):.     
+0000b000: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0000b010: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0000b020: 2020 2020 2020 2020 2755 6e73 7570 706f          'Unsuppo
+0000b030: 7274 6564 206d 6f64 653a 207b 7d20 2d2d  rted mode: {} --
+0000b040: 204d 6f64 6520 7368 6f75 6c64 2075 7365   Mode should use
+0000b050: 206f 6e65 206f 6620 7468 6520 656e 756d   one of the enum
+0000b060: 7320 6265 6c6f 6e67 696e 6720 746f 3a20  s belonging to: 
+0000b070: 207b 7d27 0a20 2020 2020 2020 2020 2020   {}'.           
+0000b080: 2020 2020 202e 666f 726d 6174 286d 6f64       .format(mod
+0000b090: 652c 2027 2c20 272e 6a6f 696e 285b 7374  e, ', '.join([st
+0000b0a0: 7228 6129 2066 6f72 2061 2069 6e20 4163  r(a) for a in Ac
+0000b0b0: 6365 7373 5d29 2929 0a20 2020 2020 2020  cess]))).       
+0000b0c0: 2069 6620 6d6f 6465 206e 6f74 2069 6e20   if mode not in 
+0000b0d0: 2841 6363 6573 732e 5245 4144 2c20 4163  (Access.READ, Ac
+0000b0e0: 6365 7373 2e57 5249 5445 293a 0a20 2020  cess.WRITE):.   
+0000b0f0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+0000b100: 7970 6545 7272 6f72 2827 556e 7375 7070  ypeError('Unsupp
+0000b110: 6f72 7465 6420 6d6f 6465 3a20 7b7d 272e  orted mode: {}'.
+0000b120: 666f 726d 6174 286d 6f64 6529 290a 2020  format(mode)).  
+0000b130: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000b140: 2020 2020 2020 2073 656c 662e 5f63 6c69         self._cli
+0000b150: 656e 742e 6865 6164 5f62 7563 6b65 7428  ent.head_bucket(
+0000b160: 4275 636b 6574 3d62 7563 6b65 7429 0a20  Bucket=bucket). 
+0000b170: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+0000b180: 6365 7074 696f 6e20 6173 2065 7272 6f72  ception as error
+0000b190: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
+0000b1a0: 726f 7220 3d20 7472 616e 736c 6174 655f  ror = translate_
+0000b1b0: 7333 5f65 7272 6f72 2865 7272 6f72 2c20  s3_error(error, 
+0000b1c0: 7333 5f75 726c 290a 2020 2020 2020 2020  s3_url).        
+0000b1d0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000b1e0: 6528 6572 726f 722c 2028 5333 5065 726d  e(error, (S3Perm
+0000b1f0: 6973 7369 6f6e 4572 726f 722c 2053 3346  issionError, S3F
+0000b200: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
+0000b210: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 2020 2020 5333 4275 636b 6574 4e6f 7446      S3BucketNotF
+0000b240: 6f75 6e64 4572 726f 7229 293a 0a20 2020  oundError)):.   
+0000b250: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000b260: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+0000b270: 2020 2020 2020 7261 6973 6520 6572 726f        raise erro
+0000b280: 720a 2020 2020 2020 2020 7265 7475 726e  r.        return
+0000b290: 2054 7275 650a 0a20 2020 2064 6566 2065   True..    def e
+0000b2a0: 7869 7374 7328 7365 6c66 2c20 666f 6c6c  xists(self, foll
+0000b2b0: 6f77 6c69 6e6b 733a 2062 6f6f 6c20 3d20  owlinks: bool = 
+0000b2c0: 4661 6c73 6529 202d 3e20 626f 6f6c 3a0a  False) -> bool:.
+0000b2d0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000b2e0: 2020 2020 5465 7374 2069 6620 7333 5f75      Test if s3_u
+0000b2f0: 726c 2065 7869 7374 730a 0a20 2020 2020  rl exists..     
+0000b300: 2020 2049 6620 7468 6520 6275 636b 6574     If the bucket
+0000b310: 206f 6620 7333 5f75 726c 2061 7265 206e   of s3_url are n
+0000b320: 6f74 2070 6572 6d69 7474 6564 2074 6f20  ot permitted to 
+0000b330: 7265 6164 2c20 7265 7475 726e 2046 616c  read, return Fal
+0000b340: 7365 0a0a 2020 2020 2020 2020 3a72 6574  se..        :ret
+0000b350: 7572 6e73 3a20 5472 7565 2069 6620 7333  urns: True if s3
+0000b360: 5f75 726c 2065 6978 7374 732c 2065 6c73  _url eixsts, els
+0000b370: 6520 4661 6c73 650a 2020 2020 2020 2020  e False.        
+0000b380: 2727 270a 2020 2020 2020 2020 6275 636b  '''.        buck
+0000b390: 6574 2c20 6b65 7920 3d20 7061 7273 655f  et, key = parse_
+0000b3a0: 7333 5f75 726c 2873 656c 662e 7061 7468  s3_url(self.path
+0000b3b0: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
+0000b3c0: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
+0000b3d0: 7563 6b65 743a 2020 2320 7333 3a2f 2f20  ucket:  # s3:// 
+0000b3e0: 3d3e 2054 7275 652c 2073 333a 2f2f 2f6b  => True, s3:///k
+0000b3f0: 6579 203d 3e20 4661 6c73 650a 2020 2020  ey => False.    
+0000b400: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+0000b410: 6f74 206b 6579 0a0a 2020 2020 2020 2020  ot key..        
+0000b420: 7265 7475 726e 2073 656c 662e 6973 5f64  return self.is_d
+0000b430: 6972 2829 206f 7220 7365 6c66 2e69 735f  ir() or self.is_
+0000b440: 6669 6c65 2866 6f6c 6c6f 776c 696e 6b73  file(followlinks
+0000b450: 290a 0a20 2020 2064 6566 2067 6574 6d74  )..    def getmt
+0000b460: 696d 6528 7365 6c66 2c20 666f 6c6c 6f77  ime(self, follow
+0000b470: 5f73 796d 6c69 6e6b 733a 2062 6f6f 6c20  _symlinks: bool 
+0000b480: 3d20 4661 6c73 6529 202d 3e20 666c 6f61  = False) -> floa
+0000b490: 743a 0a20 2020 2020 2020 2027 2727 0a20  t:.        '''. 
+0000b4a0: 2020 2020 2020 2047 6574 206c 6173 742d         Get last-
+0000b4b0: 6d6f 6469 6669 6564 2074 696d 6520 6f66  modified time of
+0000b4c0: 2074 6865 2066 696c 6520 6f6e 2074 6865   the file on the
+0000b4d0: 2067 6976 656e 2073 335f 7572 6c20 7061   given s3_url pa
+0000b4e0: 7468 2028 696e 2055 6e69 7820 7469 6d65  th (in Unix time
+0000b4f0: 7374 616d 7020 666f 726d 6174 292e 0a20  stamp format).. 
+0000b500: 2020 2020 2020 2049 6620 7468 6520 7061         If the pa
+0000b510: 7468 2069 7320 616e 2065 7869 7374 656e  th is an existen
+0000b520: 7420 6469 7265 6374 6f72 792c 2072 6574  t directory, ret
+0000b530: 7572 6e20 7468 6520 6c61 7465 7374 206d  urn the latest m
+0000b540: 6f64 6966 6965 6420 7469 6d65 206f 6620  odified time of 
+0000b550: 616c 6c20 6669 6c65 2069 6e20 6974 2e20  all file in it. 
+0000b560: 5468 6520 6d74 696d 6520 6f66 2065 6d70  The mtime of emp
+0000b570: 7479 2064 6972 6563 746f 7279 2069 7320  ty directory is 
+0000b580: 3139 3730 2d30 312d 3031 2030 303a 3030  1970-01-01 00:00
+0000b590: 3a30 300a 0a20 2020 2020 2020 2049 6620  :00..        If 
+0000b5a0: 7333 5f75 726c 2069 7320 6e6f 7420 616e  s3_url is not an
+0000b5b0: 2065 7869 7374 656e 7420 7061 7468 2c20   existent path, 
+0000b5c0: 7768 6963 6820 6d65 616e 7320 7333 5f65  which means s3_e
+0000b5d0: 7869 7374 2873 335f 7572 6c29 2072 6574  xist(s3_url) ret
+0000b5e0: 7572 6e73 2046 616c 7365 2c20 7468 656e  urns False, then
+0000b5f0: 2072 6169 7365 2053 3346 696c 654e 6f74   raise S3FileNot
+0000b600: 466f 756e 6445 7272 6f72 0a0a 2020 2020  FoundError..    
+0000b610: 2020 2020 3a72 6574 7572 6e73 3a20 4c61      :returns: La
+0000b620: 7374 2d6d 6f64 6966 6965 6420 7469 6d65  st-modified time
+0000b630: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+0000b640: 3a20 5333 4669 6c65 4e6f 7446 6f75 6e64  : S3FileNotFound
+0000b650: 4572 726f 722c 2055 6e73 7570 706f 7274  Error, Unsupport
+0000b660: 6564 4572 726f 720a 2020 2020 2020 2020  edError.        
+0000b670: 2727 270a 2020 2020 2020 2020 7265 7475  '''.        retu
+0000b680: 726e 2073 656c 662e 7374 6174 2866 6f6c  rn self.stat(fol
+0000b690: 6c6f 775f 7379 6d6c 696e 6b73 3d66 6f6c  low_symlinks=fol
+0000b6a0: 6c6f 775f 7379 6d6c 696e 6b73 292e 6d74  low_symlinks).mt
+0000b6b0: 696d 650a 0a20 2020 2064 6566 2067 6574  ime..    def get
+0000b6c0: 7369 7a65 2873 656c 662c 2066 6f6c 6c6f  size(self, follo
+0000b6d0: 775f 7379 6d6c 696e 6b73 3a20 626f 6f6c  w_symlinks: bool
+0000b6e0: 203d 2046 616c 7365 2920 2d3e 2069 6e74   = False) -> int
+0000b6f0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+0000b700: 2020 2020 2020 4765 7420 6669 6c65 2073        Get file s
+0000b710: 697a 6520 6f6e 2074 6865 2067 6976 656e  ize on the given
+0000b720: 2073 335f 7572 6c20 7061 7468 2028 696e   s3_url path (in
+0000b730: 2062 7974 6573 292e 0a20 2020 2020 2020   bytes)..       
+0000b740: 2049 6620 7468 6520 7061 7468 2069 6e20   If the path in 
+0000b750: 6120 6469 7265 6374 6f72 792c 2072 6574  a directory, ret
+0000b760: 7572 6e20 7468 6520 7375 6d20 6f66 2061  urn the sum of a
+0000b770: 6c6c 2066 696c 6520 7369 7a65 2069 6e20  ll file size in 
+0000b780: 6974 2c20 696e 636c 7564 696e 6720 6669  it, including fi
+0000b790: 6c65 2069 6e20 7375 6264 6972 6563 746f  le in subdirecto
+0000b7a0: 7269 6573 2028 6966 2065 7869 7374 292e  ries (if exist).
+0000b7b0: 0a20 2020 2020 2020 2054 6865 2072 6573  .        The res
+0000b7c0: 756c 7420 6578 636c 7564 6573 2074 6865  ult excludes the
+0000b7d0: 2073 697a 6520 6f66 2064 6972 6563 746f   size of directo
+0000b7e0: 7279 2069 7473 656c 662e 2049 6e20 6f74  ry itself. In ot
+0000b7f0: 6865 7220 776f 7264 732c 2072 6574 7572  her words, retur
+0000b800: 6e20 3020 4279 7465 206f 6e20 616e 2065  n 0 Byte on an e
+0000b810: 6d70 7479 2064 6972 6563 746f 7279 2070  mpty directory p
+0000b820: 6174 682e 0a0a 2020 2020 2020 2020 4966  ath...        If
+0000b830: 2073 335f 7572 6c20 6973 206e 6f74 2061   s3_url is not a
+0000b840: 6e20 6578 6973 7465 6e74 2070 6174 682c  n existent path,
+0000b850: 2077 6869 6368 206d 6561 6e73 2073 335f   which means s3_
+0000b860: 6578 6973 7428 7333 5f75 726c 2920 7265  exist(s3_url) re
+0000b870: 7475 726e 7320 4661 6c73 652c 2074 6865  turns False, the
+0000b880: 6e20 7261 6973 6520 5333 4669 6c65 4e6f  n raise S3FileNo
+0000b890: 7446 6f75 6e64 4572 726f 720a 0a20 2020  tFoundError..   
+0000b8a0: 2020 2020 203a 7265 7475 726e 733a 2046       :returns: F
+0000b8b0: 696c 6520 7369 7a65 0a20 2020 2020 2020  ile size.       
+0000b8c0: 203a 7261 6973 6573 3a20 5333 4669 6c65   :raises: S3File
+0000b8d0: 4e6f 7446 6f75 6e64 4572 726f 722c 2055  NotFoundError, U
+0000b8e0: 6e73 7570 706f 7274 6564 4572 726f 720a  nsupportedError.
+0000b8f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000b900: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000b910: 7374 6174 2866 6f6c 6c6f 775f 7379 6d6c  stat(follow_syml
+0000b920: 696e 6b73 3d66 6f6c 6c6f 775f 7379 6d6c  inks=follow_syml
+0000b930: 696e 6b73 292e 7369 7a65 0a0a 2020 2020  inks).size..    
+0000b940: 6465 6620 676c 6f62 280a 2020 2020 2020  def glob(.      
+0000b950: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000b960: 2020 2020 2020 2020 7061 7474 6572 6e2c          pattern,
+0000b970: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+0000b980: 7572 7369 7665 3a20 626f 6f6c 203d 2054  ursive: bool = T
+0000b990: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0000b9a0: 206d 6973 7369 6e67 5f6f 6b3a 2062 6f6f   missing_ok: boo
+0000b9b0: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+0000b9c0: 2020 2020 2020 666f 6c6c 6f77 6c69 6e6b        followlink
+0000b9d0: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
+0000b9e0: 0a20 2020 2029 202d 3e20 4c69 7374 5b27  .    ) -> List['
+0000b9f0: 5333 5061 7468 275d 3a0a 2020 2020 2020  S3Path']:.      
+0000ba00: 2020 2727 2752 6574 7572 6e20 7333 2070    '''Return s3 p
+0000ba10: 6174 6820 6c69 7374 2069 6e20 6173 6365  ath list in asce
+0000ba20: 6e64 696e 6720 616c 7068 6162 6574 6963  nding alphabetic
+0000ba30: 616c 206f 7264 6572 2c20 696e 2077 6869  al order, in whi
+0000ba40: 6368 2070 6174 6820 6d61 7463 6865 7320  ch path matches 
+0000ba50: 676c 6f62 2070 6174 7465 726e 0a20 2020  glob pattern.   
+0000ba60: 2020 2020 204e 6f74 6573 3a20 4f6e 6c79       Notes: Only
+0000ba70: 2067 6c6f 6220 696e 2062 7563 6b65 742e   glob in bucket.
+0000ba80: 2049 6620 7472 7969 6e67 2074 6f20 6d61   If trying to ma
+0000ba90: 7463 6820 6275 636b 6574 2077 6974 6820  tch bucket with 
+0000baa0: 7769 6c64 6361 7264 2063 6861 7261 6374  wildcard charact
+0000bab0: 6572 732c 2072 6169 7365 2055 6e73 7570  ers, raise Unsup
+0000bac0: 706f 7274 6564 4572 726f 720a 0a20 2020  portedError..   
+0000bad0: 2020 2020 203a 7061 7261 6d20 7061 7474       :param patt
+0000bae0: 6572 6e3a 2047 6c6f 6220 7468 6520 6769  ern: Glob the gi
+0000baf0: 7665 6e20 7265 6c61 7469 7665 2070 6174  ven relative pat
+0000bb00: 7465 726e 2069 6e20 7468 6520 6469 7265  tern in the dire
+0000bb10: 6374 6f72 7920 7265 7072 6573 656e 7465  ctory represente
+0000bb20: 6420 6279 2074 6869 7320 7061 7468 0a20  d by this path. 
+0000bb30: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
+0000bb40: 6375 7273 6976 653a 2049 6620 4661 6c73  cursive: If Fals
+0000bb50: 652c 2060 2a2a 6020 7769 6c6c 206e 6f74  e, `**` will not
+0000bb60: 2073 6561 7263 6820 6469 7265 6374 6f72   search director
+0000bb70: 7920 7265 6375 7273 6976 656c 790a 2020  y recursively.  
+0000bb80: 2020 2020 2020 3a70 6172 616d 206d 6973        :param mis
+0000bb90: 7369 6e67 5f6f 6b3a 2049 6620 4661 6c73  sing_ok: If Fals
+0000bba0: 6520 616e 6420 7461 7267 6574 2070 6174  e and target pat
+0000bbb0: 6820 646f 6573 6e27 7420 6d61 7463 6820  h doesn't match 
+0000bbc0: 616e 7920 6669 6c65 2c20 7261 6973 6520  any file, raise 
+0000bbd0: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
+0000bbe0: 720a 2020 2020 2020 2020 3a72 6169 7365  r.        :raise
+0000bbf0: 733a 2055 6e73 7570 706f 7274 6564 4572  s: UnsupportedEr
+0000bc00: 726f 722c 2077 6865 6e20 6275 636b 6574  ror, when bucket
+0000bc10: 2070 6172 7420 636f 6e74 6169 6e73 2077   part contains w
+0000bc20: 696c 6463 6172 6420 6368 6172 6163 7465  ildcard characte
+0000bc30: 7273 0a20 2020 2020 2020 203a 7265 7475  rs.        :retu
+0000bc40: 726e 733a 2041 206c 6973 7420 636f 6e74  rns: A list cont
+0000bc50: 6169 6e73 2070 6174 6873 206d 6174 6368  ains paths match
+0000bc60: 2060 7333 5f70 6174 686e 616d 6560 0a20   `s3_pathname`. 
+0000bc70: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000bc80: 2020 2072 6574 7572 6e20 6c69 7374 280a     return list(.
+0000bc90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000bca0: 2e69 676c 6f62 280a 2020 2020 2020 2020  .iglob(.        
+0000bcb0: 2020 2020 2020 2020 7061 7474 6572 6e3d          pattern=
+0000bcc0: 7061 7474 6572 6e2c 0a20 2020 2020 2020  pattern,.       
+0000bcd0: 2020 2020 2020 2020 2072 6563 7572 7369           recursi
+0000bce0: 7665 3d72 6563 7572 7369 7665 2c0a 2020  ve=recursive,.  
+0000bcf0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+0000bd00: 7373 696e 675f 6f6b 3d6d 6973 7369 6e67  ssing_ok=missing
+0000bd10: 5f6f 6b2c 0a20 2020 2020 2020 2020 2020  _ok,.           
+0000bd20: 2020 2020 2066 6f6c 6c6f 776c 696e 6b73       followlinks
+0000bd30: 3d66 6f6c 6c6f 776c 696e 6b73 2929 0a0a  =followlinks))..
+0000bd40: 2020 2020 6465 6620 676c 6f62 5f73 7461      def glob_sta
+0000bd50: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
+0000bd60: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000bd70: 2070 6174 7465 726e 2c0a 2020 2020 2020   pattern,.      
+0000bd80: 2020 2020 2020 7265 6375 7273 6976 653a        recursive:
+0000bd90: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
+0000bda0: 2020 2020 2020 2020 2020 6d69 7373 696e            missin
+0000bdb0: 675f 6f6b 3a20 626f 6f6c 203d 2054 7275  g_ok: bool = Tru
+0000bdc0: 652c 0a20 2020 2020 2020 2020 2020 2066  e,.            f
+0000bdd0: 6f6c 6c6f 776c 696e 6b73 3a20 626f 6f6c  ollowlinks: bool
+0000bde0: 203d 2046 616c 7365 2920 2d3e 2049 7465   = False) -> Ite
+0000bdf0: 7261 746f 725b 4669 6c65 456e 7472 795d  rator[FileEntry]
+0000be00: 3a0a 2020 2020 2020 2020 2727 2752 6574  :.        '''Ret
+0000be10: 7572 6e20 6120 6765 6e65 7261 746f 7220  urn a generator 
+0000be20: 636f 6e74 6169 6e73 2074 7570 6c65 7320  contains tuples 
+0000be30: 6f66 2070 6174 6820 616e 6420 6669 6c65  of path and file
+0000be40: 2073 7461 742c 2069 6e20 6173 6365 6e64   stat, in ascend
+0000be50: 696e 6720 616c 7068 6162 6574 6963 616c  ing alphabetical
+0000be60: 206f 7264 6572 2c20 696e 2077 6869 6368   order, in which
+0000be70: 2070 6174 6820 6d61 7463 6865 7320 676c   path matches gl
+0000be80: 6f62 2070 6174 7465 726e 0a20 2020 2020  ob pattern.     
+0000be90: 2020 204e 6f74 6573 3a20 4f6e 6c79 2067     Notes: Only g
+0000bea0: 6c6f 6220 696e 2062 7563 6b65 742e 2049  lob in bucket. I
+0000beb0: 6620 7472 7969 6e67 2074 6f20 6d61 7463  f trying to matc
+0000bec0: 6820 6275 636b 6574 2077 6974 6820 7769  h bucket with wi
+0000bed0: 6c64 6361 7264 2063 6861 7261 6374 6572  ldcard character
+0000bee0: 732c 2072 6169 7365 2055 6e73 7570 706f  s, raise Unsuppo
+0000bef0: 7274 6564 4572 726f 720a 0a20 2020 2020  rtedError..     
+0000bf00: 2020 203a 7061 7261 6d20 7061 7474 6572     :param patter
+0000bf10: 6e3a 2047 6c6f 6220 7468 6520 6769 7665  n: Glob the give
+0000bf20: 6e20 7265 6c61 7469 7665 2070 6174 7465  n relative patte
+0000bf30: 726e 2069 6e20 7468 6520 6469 7265 6374  rn in the direct
+0000bf40: 6f72 7920 7265 7072 6573 656e 7465 6420  ory represented 
+0000bf50: 6279 2074 6869 7320 7061 7468 0a20 2020  by this path.   
+0000bf60: 2020 2020 203a 7061 7261 6d20 7265 6375       :param recu
+0000bf70: 7273 6976 653a 2049 6620 4661 6c73 652c  rsive: If False,
+0000bf80: 2060 2a2a 6020 7769 6c6c 206e 6f74 2073   `**` will not s
+0000bf90: 6561 7263 6820 6469 7265 6374 6f72 7920  earch directory 
+0000bfa0: 7265 6375 7273 6976 656c 790a 2020 2020  recursively.    
+0000bfb0: 2020 2020 3a70 6172 616d 206d 6973 7369      :param missi
+0000bfc0: 6e67 5f6f 6b3a 2049 6620 4661 6c73 6520  ng_ok: If False 
+0000bfd0: 616e 6420 7461 7267 6574 2070 6174 6820  and target path 
+0000bfe0: 646f 6573 6e27 7420 6d61 7463 6820 616e  doesn't match an
+0000bff0: 7920 6669 6c65 2c20 7261 6973 6520 4669  y file, raise Fi
+0000c000: 6c65 4e6f 7446 6f75 6e64 4572 726f 720a  leNotFoundError.
+0000c010: 2020 2020 2020 2020 3a72 6169 7365 733a          :raises:
+0000c020: 2055 6e73 7570 706f 7274 6564 4572 726f   UnsupportedErro
+0000c030: 722c 2077 6865 6e20 6275 636b 6574 2070  r, when bucket p
+0000c040: 6172 7420 636f 6e74 6169 6e73 2077 696c  art contains wil
+0000c050: 6463 6172 6420 6368 6172 6163 7465 7273  dcard characters
+0000c060: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000c070: 733a 2041 2067 656e 6572 6174 6f72 2063  s: A generator c
+0000c080: 6f6e 7461 696e 7320 7475 706c 6573 206f  ontains tuples o
+0000c090: 6620 7061 7468 2061 6e64 2066 696c 6520  f path and file 
+0000c0a0: 7374 6174 2c20 696e 2077 6869 6368 2070  stat, in which p
+0000c0b0: 6174 6873 206d 6174 6368 2060 7333 5f70  aths match `s3_p
+0000c0c0: 6174 686e 616d 6560 0a20 2020 2020 2020  athname`.       
+0000c0d0: 2027 2727 0a20 2020 2020 2020 2067 6c6f   '''.        glo
+0000c0e0: 625f 7061 7468 203d 2073 656c 662e 5f73  b_path = self._s
+0000c0f0: 335f 7061 7468 0a20 2020 2020 2020 2069  3_path.        i
+0000c100: 6620 7061 7474 6572 6e3a 0a20 2020 2020  f pattern:.     
+0000c110: 2020 2020 2020 2067 6c6f 625f 7061 7468         glob_path
+0000c120: 203d 2073 656c 662e 6a6f 696e 7061 7468   = self.joinpath
+0000c130: 2870 6174 7465 726e 292e 5f73 335f 7061  (pattern)._s3_pa
+0000c140: 7468 2020 2320 7079 7479 7065 3a20 6469  th  # pytype: di
+0000c150: 7361 626c 653d 6174 7472 6962 7574 652d  sable=attribute-
+0000c160: 6572 726f 720a 2020 2020 2020 2020 7333  error.        s3
+0000c170: 5f70 6174 686e 616d 6520 3d20 6673 7061  _pathname = fspa
+0000c180: 7468 2867 6c6f 625f 7061 7468 290a 0a20  th(glob_path).. 
+0000c190: 2020 2020 2020 2064 6566 2063 7265 6174         def creat
+0000c1a0: 655f 6765 6e65 7261 746f 7228 293a 0a20  e_generator():. 
+0000c1b0: 2020 2020 2020 2020 2020 2066 6f72 2067             for g
+0000c1c0: 726f 7570 5f73 335f 7061 7468 6e61 6d65  roup_s3_pathname
+0000c1d0: 5f31 2069 6e20 5f67 726f 7570 5f73 3370  _1 in _group_s3p
+0000c1e0: 6174 685f 6279 5f62 7563 6b65 7428 0a20  ath_by_bucket(. 
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 2020 2073 335f 7061 7468 6e61 6d65 2c20     s3_pathname, 
+0000c210: 7365 6c66 2e5f 7072 6f66 696c 655f 6e61  self._profile_na
+0000c220: 6d65 293a 0a20 2020 2020 2020 2020 2020  me):.           
+0000c230: 2020 2020 2066 6f72 2067 726f 7570 5f73       for group_s
+0000c240: 335f 7061 7468 6e61 6d65 5f32 2069 6e20  3_pathname_2 in 
+0000c250: 5f67 726f 7570 5f73 3370 6174 685f 6279  _group_s3path_by
+0000c260: 5f70 7265 6669 7828 0a20 2020 2020 2020  _prefix(.       
+0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c280: 2067 726f 7570 5f73 335f 7061 7468 6e61   group_s3_pathna
+0000c290: 6d65 5f31 293a 0a20 2020 2020 2020 2020  me_1):.         
+0000c2a0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+0000c2b0: 696c 655f 656e 7472 7920 696e 205f 7333  ile_entry in _s3
+0000c2c0: 5f67 6c6f 625f 7374 6174 5f73 696e 676c  _glob_stat_singl
+0000c2d0: 655f 7061 7468 280a 2020 2020 2020 2020  e_path(.        
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2f0: 2020 2020 6772 6f75 705f 7333 5f70 6174      group_s3_pat
+0000c300: 686e 616d 655f 322c 2072 6563 7572 7369  hname_2, recursi
+0000c310: 7665 2c20 6d69 7373 696e 675f 6f6b 2c0a  ve, missing_ok,.
+0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c330: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
+0000c340: 6f77 6c69 6e6b 733d 666f 6c6c 6f77 6c69  owlinks=followli
+0000c350: 6e6b 732c 0a20 2020 2020 2020 2020 2020  nks,.           
 0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c370: 2020 2066 6f72 2066 696c 655f 656e 7472     for file_entr
-0000c380: 7920 696e 205f 7333 5f67 6c6f 625f 7374  y in _s3_glob_st
-0000c390: 6174 5f73 696e 676c 655f 7061 7468 280a  at_single_path(.
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-0000c3c0: 705f 7333 5f70 6174 686e 616d 655f 322c  p_s3_pathname_2,
-0000c3d0: 2072 6563 7572 7369 7665 2c20 6d69 7373   recursive, miss
-0000c3e0: 696e 675f 6f6b 2c0a 2020 2020 2020 2020  ing_ok,.        
-0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c400: 2020 2020 666f 6c6c 6f77 6c69 6e6b 733d      followlinks=
-0000c410: 666f 6c6c 6f77 6c69 6e6b 732c 0a20 2020  followlinks,.   
-0000c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c430: 2020 2020 2020 2020 2070 726f 6669 6c65           profile
-0000c440: 5f6e 616d 653d 7365 6c66 2e5f 7072 6f66  _name=self._prof
-0000c450: 696c 655f 6e61 6d65 293a 0a20 2020 2020  ile_name):.     
-0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c470: 2020 2069 6620 7365 6c66 2e5f 7072 6f66     if self._prof
-0000c480: 696c 655f 6e61 6d65 3a0a 2020 2020 2020  ile_name:.      
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 2020 6669 6c65 5f65 6e74 7279        file_entry
-0000c4b0: 203d 2066 696c 655f 656e 7472 792e 5f72   = file_entry._r
-0000c4c0: 6570 6c61 6365 280a 2020 2020 2020 2020  eplace(.        
-0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4e0: 2020 2020 2020 2020 7061 7468 3d0a 2020          path=.  
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c500: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000c510: 7b73 656c 662e 5f70 726f 746f 636f 6c5f  {self._protocol_
-0000c520: 7769 7468 5f70 726f 6669 6c65 7d3a 2f2f  with_profile}://
-0000c530: 7b66 696c 655f 656e 7472 792e 7061 7468  {file_entry.path
-0000c540: 5b35 3a5d 7d22 0a20 2020 2020 2020 2020  [5:]}".         
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000c570: 2020 2020 2020 2020 2020 2020 2079 6965               yie
-0000c580: 6c64 2066 696c 655f 656e 7472 790a 0a20  ld file_entry.. 
-0000c590: 2020 2020 2020 2072 6574 7572 6e20 5f63         return _c
-0000c5a0: 7265 6174 655f 6d69 7373 696e 675f 6f6b  reate_missing_ok
-0000c5b0: 5f67 656e 6572 6174 6f72 280a 2020 2020  _generator(.    
-0000c5c0: 2020 2020 2020 2020 6372 6561 7465 5f67          create_g
-0000c5d0: 656e 6572 6174 6f72 2829 2c20 6d69 7373  enerator(), miss
-0000c5e0: 696e 675f 6f6b 2c0a 2020 2020 2020 2020  ing_ok,.        
-0000c5f0: 2020 2020 5333 4669 6c65 4e6f 7446 6f75      S3FileNotFou
-0000c600: 6e64 4572 726f 7228 274e 6f20 6d61 7463  ndError('No matc
-0000c610: 6820 6669 6c65 3a20 2572 2720 2520 7333  h file: %r' % s3
-0000c620: 5f70 6174 686e 616d 6529 290a 0a20 2020  _pathname))..   
-0000c630: 2064 6566 2069 676c 6f62 280a 2020 2020   def iglob(.    
-0000c640: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000c650: 2020 2020 2020 2020 2020 7061 7474 6572            patter
-0000c660: 6e2c 0a20 2020 2020 2020 2020 2020 2072  n,.            r
-0000c670: 6563 7572 7369 7665 3a20 626f 6f6c 203d  ecursive: bool =
-0000c680: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-0000c690: 2020 206d 6973 7369 6e67 5f6f 6b3a 2062     missing_ok: b
-0000c6a0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-0000c6b0: 2020 2020 2020 2020 666f 6c6c 6f77 6c69          followli
-0000c6c0: 6e6b 733a 2062 6f6f 6c20 3d20 4661 6c73  nks: bool = Fals
-0000c6d0: 652c 0a20 2020 2029 202d 3e20 4974 6572  e,.    ) -> Iter
-0000c6e0: 6174 6f72 5b27 5333 5061 7468 275d 3a0a  ator['S3Path']:.
-0000c6f0: 2020 2020 2020 2020 2727 2752 6574 7572          '''Retur
-0000c700: 6e20 7333 2070 6174 6820 6974 6572 6174  n s3 path iterat
-0000c710: 6f72 2069 6e20 6173 6365 6e64 696e 6720  or in ascending 
-0000c720: 616c 7068 6162 6574 6963 616c 206f 7264  alphabetical ord
-0000c730: 6572 2c20 696e 2077 6869 6368 2070 6174  er, in which pat
-0000c740: 6820 6d61 7463 6865 7320 676c 6f62 2070  h matches glob p
-0000c750: 6174 7465 726e 0a20 2020 2020 2020 204e  attern.        N
-0000c760: 6f74 6573 3a20 4f6e 6c79 2067 6c6f 6220  otes: Only glob 
-0000c770: 696e 2062 7563 6b65 742e 2049 6620 7472  in bucket. If tr
-0000c780: 7969 6e67 2074 6f20 6d61 7463 6820 6275  ying to match bu
-0000c790: 636b 6574 2077 6974 6820 7769 6c64 6361  cket with wildca
-0000c7a0: 7264 2063 6861 7261 6374 6572 732c 2072  rd characters, r
-0000c7b0: 6169 7365 2055 6e73 7570 706f 7274 6564  aise Unsupported
-0000c7c0: 4572 726f 720a 0a20 2020 2020 2020 203a  Error..        :
-0000c7d0: 7061 7261 6d20 7061 7474 6572 6e3a 2047  param pattern: G
-0000c7e0: 6c6f 6220 7468 6520 6769 7665 6e20 7265  lob the given re
-0000c7f0: 6c61 7469 7665 2070 6174 7465 726e 2069  lative pattern i
-0000c800: 6e20 7468 6520 6469 7265 6374 6f72 7920  n the directory 
-0000c810: 7265 7072 6573 656e 7465 6420 6279 2074  represented by t
-0000c820: 6869 7320 7061 7468 0a20 2020 2020 2020  his path.       
-0000c830: 203a 7061 7261 6d20 7265 6375 7273 6976   :param recursiv
-0000c840: 653a 2049 6620 4661 6c73 652c 2060 2a2a  e: If False, `**
-0000c850: 6020 7769 6c6c 206e 6f74 2073 6561 7263  ` will not searc
-0000c860: 6820 6469 7265 6374 6f72 7920 7265 6375  h directory recu
-0000c870: 7273 6976 656c 790a 2020 2020 2020 2020  rsively.        
-0000c880: 3a70 6172 616d 206d 6973 7369 6e67 5f6f  :param missing_o
-0000c890: 6b3a 2049 6620 4661 6c73 6520 616e 6420  k: If False and 
-0000c8a0: 7461 7267 6574 2070 6174 6820 646f 6573  target path does
-0000c8b0: 6e27 7420 6d61 7463 6820 616e 7920 6669  n't match any fi
-0000c8c0: 6c65 2c20 7261 6973 6520 4669 6c65 4e6f  le, raise FileNo
-0000c8d0: 7446 6f75 6e64 4572 726f 720a 2020 2020  tFoundError.    
-0000c8e0: 2020 2020 3a72 6169 7365 733a 2055 6e73      :raises: Uns
-0000c8f0: 7570 706f 7274 6564 4572 726f 722c 2077  upportedError, w
-0000c900: 6865 6e20 6275 636b 6574 2070 6172 7420  hen bucket part 
-0000c910: 636f 6e74 6169 6e73 2077 696c 6463 6172  contains wildcar
-0000c920: 6420 6368 6172 6163 7465 7273 0a20 2020  d characters.   
-0000c930: 2020 2020 203a 7265 7475 726e 733a 2041       :returns: A
-0000c940: 6e20 6974 6572 6174 6f72 2063 6f6e 7461  n iterator conta
-0000c950: 696e 7320 7061 7468 7320 6d61 7463 6820  ins paths match 
-0000c960: 6073 335f 7061 7468 6e61 6d65 600a 2020  `s3_pathname`.  
-0000c970: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000c980: 2020 666f 7220 6669 6c65 5f65 6e74 7279    for file_entry
-0000c990: 2069 6e20 7365 6c66 2e67 6c6f 625f 7374   in self.glob_st
-0000c9a0: 6174 2870 6174 7465 726e 3d70 6174 7465  at(pattern=patte
-0000c9b0: 726e 2c20 7265 6375 7273 6976 653d 7265  rn, recursive=re
-0000c9c0: 6375 7273 6976 652c 0a20 2020 2020 2020  cursive,.       
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9f0: 2020 6d69 7373 696e 675f 6f6b 3d6d 6973    missing_ok=mis
-0000ca00: 7369 6e67 5f6f 6b2c 0a20 2020 2020 2020  sing_ok,.       
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca30: 2020 666f 6c6c 6f77 6c69 6e6b 733d 666f    followlinks=fo
-0000ca40: 6c6c 6f77 6c69 6e6b 7329 3a0a 2020 2020  llowlinks):.    
-0000ca50: 2020 2020 2020 2020 7969 656c 6420 7365          yield se
-0000ca60: 6c66 2e66 726f 6d5f 7061 7468 2866 696c  lf.from_path(fil
-0000ca70: 655f 656e 7472 792e 7061 7468 290a 0a20  e_entry.path).. 
-0000ca80: 2020 2064 6566 2069 735f 6469 7228 7365     def is_dir(se
-0000ca90: 6c66 2c20 666f 6c6c 6f77 6c69 6e6b 733a  lf, followlinks:
-0000caa0: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
-0000cab0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0000cac0: 2727 270a 2020 2020 2020 2020 5465 7374  '''.        Test
-0000cad0: 2069 6620 616e 2073 3320 7572 6c20 6973   if an s3 url is
-0000cae0: 2064 6972 6563 746f 7279 0a20 2020 2020   directory.     
-0000caf0: 2020 2053 7065 6369 6669 6320 7072 6f63     Specific proc
-0000cb00: 6564 7572 6573 2061 7265 2061 7320 666f  edures are as fo
-0000cb10: 6c6c 6f77 733a 0a20 2020 2020 2020 2049  llows:.        I
-0000cb20: 6620 7468 6572 6520 6578 6973 7473 2061  f there exists a
-0000cb30: 2073 7566 6669 782c 206f 6620 7768 6963   suffix, of whic
-0000cb40: 6820 6060 6f73 2e70 6174 682e 6a6f 696e  h ``os.path.join
-0000cb50: 2873 335f 7572 6c2c 2073 7566 6669 7829  (s3_url, suffix)
-0000cb60: 6060 2069 7320 6120 6669 6c65 0a20 2020  `` is a file.   
-0000cb70: 2020 2020 2049 6620 7468 6520 7572 6c20       If the url 
-0000cb80: 6973 2065 6d70 7479 2062 7563 6b65 7420  is empty bucket 
-0000cb90: 6f72 2073 333a 2f2f 0a0a 2020 2020 2020  or s3://..      
-0000cba0: 2020 3a70 6172 616d 2066 6f6c 6c6f 776c    :param followl
-0000cbb0: 696e 6b73 3a20 7768 6574 6865 7220 666f  inks: whether fo
-0000cbc0: 6c6c 6f77 6c69 6e6b 7320 6973 2054 7275  llowlinks is Tru
-0000cbd0: 6520 6f72 2046 616c 7365 2c20 7265 7375  e or False, resu
-0000cbe0: 6c74 2069 7320 7468 6520 7361 6d65 2e20  lt is the same. 
-0000cbf0: 4265 6361 7573 6520 7333 2073 796d 6c69  Because s3 symli
-0000cc00: 6e6b 206e 6f74 2073 7570 706f 7274 2064  nk not support d
-0000cc10: 6972 2e0a 2020 2020 2020 2020 3a72 6574  ir..        :ret
-0000cc20: 7572 6e73 3a20 5472 7565 2069 6620 7061  urns: True if pa
-0000cc30: 7468 2069 7320 7333 2064 6972 6563 746f  th is s3 directo
-0000cc40: 7279 2c20 656c 7365 2046 616c 7365 0a20  ry, else False. 
-0000cc50: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0000cc60: 2020 2062 7563 6b65 742c 206b 6579 203d     bucket, key =
-0000cc70: 2070 6172 7365 5f73 335f 7572 6c28 7365   parse_s3_url(se
-0000cc80: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
-0000cc90: 746f 636f 6c29 0a20 2020 2020 2020 2069  tocol).        i
-0000cca0: 6620 6e6f 7420 6275 636b 6574 3a20 2023  f not bucket:  #
-0000ccb0: 2073 333a 2f2f 203d 3e20 5472 7565 2c20   s3:// => True, 
-0000ccc0: 7333 3a2f 2f2f 6b65 7920 3d3e 2046 616c  s3:///key => Fal
-0000ccd0: 7365 0a20 2020 2020 2020 2020 2020 2072  se.            r
-0000cce0: 6574 7572 6e20 6e6f 7420 6b65 790a 2020  eturn not key.  
-0000ccf0: 2020 2020 2020 7072 6566 6978 203d 205f        prefix = _
-0000cd00: 6265 636f 6d65 5f70 7265 6669 7828 6b65  become_prefix(ke
-0000cd10: 7929 0a20 2020 2020 2020 2074 7279 3a0a  y).        try:.
-0000cd20: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-0000cd30: 203d 2073 656c 662e 5f63 6c69 656e 742e   = self._client.
-0000cd40: 6c69 7374 5f6f 626a 6563 7473 5f76 3228  list_objects_v2(
-0000cd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd60: 2042 7563 6b65 743d 6275 636b 6574 2c20   Bucket=bucket, 
-0000cd70: 5072 6566 6978 3d70 7265 6669 782c 2044  Prefix=prefix, D
-0000cd80: 656c 696d 6974 6572 3d27 2f27 2c20 4d61  elimiter='/', Ma
-0000cd90: 784b 6579 733d 3129 0a20 2020 2020 2020  xKeys=1).       
-0000cda0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0000cdb0: 6e20 6173 2065 7272 6f72 3a0a 2020 2020  n as error:.    
-0000cdc0: 2020 2020 2020 2020 6572 726f 7220 3d20          error = 
-0000cdd0: 7472 616e 736c 6174 655f 7333 5f65 7272  translate_s3_err
-0000cde0: 6f72 2865 7272 6f72 2c20 7365 6c66 2e70  or(error, self.p
-0000cdf0: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
-0000ce00: 6c29 0a20 2020 2020 2020 2020 2020 2069  l).            i
-0000ce10: 6620 6973 696e 7374 616e 6365 2865 7272  f isinstance(err
-0000ce20: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-0000ce30: 2020 2020 2020 2020 2020 2020 2020 2853                (S
-0000ce40: 3355 6e6b 6e6f 776e 4572 726f 722c 2053  3UnknownError, S
-0000ce50: 3343 6f6e 6669 6745 7272 6f72 2c20 5333  3ConfigError, S3
-0000ce60: 5065 726d 6973 7369 6f6e 4572 726f 7229  PermissionError)
-0000ce70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ce80: 2020 2072 6169 7365 2065 7272 6f72 0a20     raise error. 
-0000ce90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000cea0: 6e20 4661 6c73 650a 0a20 2020 2020 2020  n False..       
-0000ceb0: 2069 6620 6e6f 7420 6b65 793a 2020 2320   if not key:  # 
-0000cec0: 6275 636b 6574 2069 7320 6163 6365 7373  bucket is access
-0000ced0: 6962 6c65 0a20 2020 2020 2020 2020 2020  ible.           
-0000cee0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-0000cef0: 2020 2020 2020 6966 2027 4b65 7943 6f75        if 'KeyCou
-0000cf00: 6e74 2720 696e 2072 6573 703a 0a20 2020  nt' in resp:.   
-0000cf10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000cf20: 7265 7370 5b27 4b65 7943 6f75 6e74 275d  resp['KeyCount']
-0000cf30: 203e 2030 0a0a 2020 2020 2020 2020 7265   > 0..        re
-0000cf40: 7475 726e 206c 656e 2872 6573 702e 6765  turn len(resp.ge
-0000cf50: 7428 2743 6f6e 7465 6e74 7327 2c20 5b5d  t('Contents', []
-0000cf60: 2929 203e 2030 206f 7220 5c0a 2020 2020  )) > 0 or \.    
-0000cf70: 2020 2020 2020 2020 6c65 6e28 7265 7370          len(resp
-0000cf80: 2e67 6574 2827 436f 6d6d 6f6e 5072 6566  .get('CommonPref
-0000cf90: 6978 6573 272c 205b 5d29 2920 3e20 300a  ixes', [])) > 0.
-0000cfa0: 0a20 2020 2064 6566 2069 735f 6669 6c65  .    def is_file
-0000cfb0: 2873 656c 662c 2066 6f6c 6c6f 776c 696e  (self, followlin
-0000cfc0: 6b73 3a20 626f 6f6c 203d 2046 616c 7365  ks: bool = False
-0000cfd0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-0000cfe0: 2020 2027 2727 0a20 2020 2020 2020 2054     '''.        T
-0000cff0: 6573 7420 6966 2061 6e20 7333 5f75 726c  est if an s3_url
-0000d000: 2069 7320 6669 6c65 0a0a 2020 2020 2020   is file..      
-0000d010: 2020 3a72 6574 7572 6e73 3a20 5472 7565    :returns: True
-0000d020: 2069 6620 7061 7468 2069 7320 7333 2066   if path is s3 f
-0000d030: 696c 652c 2065 6c73 6520 4661 6c73 650a  ile, else False.
-0000d040: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000d050: 2020 2020 7333 5f75 726c 203d 2073 656c      s3_url = sel
-0000d060: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
-0000d070: 6f63 6f6c 0a20 2020 2020 2020 2069 6620  ocol.        if 
-0000d080: 666f 6c6c 6f77 6c69 6e6b 733a 0a20 2020  followlinks:.   
-0000d090: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 7333                s3
-0000d0b0: 5f75 726c 203d 2073 656c 662e 7265 6164  _url = self.read
-0000d0c0: 6c69 6e6b 2829 2e70 6174 685f 7769 7468  link().path_with
-0000d0d0: 5f70 726f 746f 636f 6c0a 2020 2020 2020  _protocol.      
-0000d0e0: 2020 2020 2020 6578 6365 7074 2053 334e        except S3N
-0000d0f0: 6f74 414c 696e 6b45 7272 6f72 3a0a 2020  otALinkError:.  
-0000d100: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000d110: 7373 0a20 2020 2020 2020 2062 7563 6b65  ss.        bucke
-0000d120: 742c 206b 6579 203d 2070 6172 7365 5f73  t, key = parse_s
-0000d130: 335f 7572 6c28 7333 5f75 726c 290a 2020  3_url(s3_url).  
-0000d140: 2020 2020 2020 6966 206e 6f74 2062 7563        if not buc
-0000d150: 6b65 7420 6f72 206e 6f74 206b 6579 206f  ket or not key o
-0000d160: 7220 6b65 792e 656e 6473 7769 7468 2827  r key.endswith('
-0000d170: 2f27 293a 0a20 2020 2020 2020 2020 2020  /'):.           
-0000d180: 2023 2073 333a 2f2f 2c20 7333 3a2f 2f2f   # s3://, s3:///
-0000d190: 6b65 792c 2073 333a 2f2f 6275 636b 6574  key, s3://bucket
-0000d1a0: 2c20 7333 3a2f 2f62 7563 6b65 742f 7072  , s3://bucket/pr
-0000d1b0: 6566 6978 2f0a 2020 2020 2020 2020 2020  efix/.          
-0000d1c0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-0000d1d0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0000d1e0: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
-0000d1f0: 6965 6e74 2e68 6561 645f 6f62 6a65 6374  ient.head_object
-0000d200: 2842 7563 6b65 743d 6275 636b 6574 2c20  (Bucket=bucket, 
-0000d210: 4b65 793d 6b65 7929 0a20 2020 2020 2020  Key=key).       
-0000d220: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0000d230: 6e20 6173 2065 7272 6f72 3a0a 2020 2020  n as error:.    
-0000d240: 2020 2020 2020 2020 6572 726f 7220 3d20          error = 
-0000d250: 7472 616e 736c 6174 655f 7333 5f65 7272  translate_s3_err
-0000d260: 6f72 2865 7272 6f72 2c20 7333 5f75 726c  or(error, s3_url
-0000d270: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000d280: 2069 7369 6e73 7461 6e63 6528 6572 726f   isinstance(erro
-0000d290: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000d2a0: 2020 2020 2020 2020 2020 2020 2028 5333               (S3
-0000d2b0: 556e 6b6e 6f77 6e45 7272 6f72 2c20 5333  UnknownError, S3
-0000d2c0: 436f 6e66 6967 4572 726f 722c 2053 3350  ConfigError, S3P
-0000d2d0: 6572 6d69 7373 696f 6e45 7272 6f72 2929  ermissionError))
-0000d2e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d2f0: 2020 7261 6973 6520 6572 726f 720a 2020    raise error.  
-0000d300: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d310: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
-0000d320: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-0000d330: 6465 6620 6c69 7374 6469 7228 7365 6c66  def listdir(self
-0000d340: 2c20 666f 6c6c 6f77 6c69 6e6b 733a 2062  , followlinks: b
-0000d350: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
-0000d360: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
-0000d370: 2020 2027 2727 0a20 2020 2020 2020 2047     '''.        G
-0000d380: 6574 2061 6c6c 2063 6f6e 7465 6e74 7320  et all contents 
-0000d390: 6f66 2067 6976 656e 2073 335f 7572 6c2e  of given s3_url.
-0000d3a0: 2054 6865 2072 6573 756c 7420 6973 2069   The result is i
-0000d3b0: 6e20 6163 7365 6e64 696e 6720 616c 7068  n acsending alph
-0000d3c0: 6162 6574 6963 616c 206f 7264 6572 2e0a  abetical order..
-0000d3d0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0000d3e0: 733a 2041 6c6c 2063 6f6e 7465 6e74 7320  s: All contents 
-0000d3f0: 6861 7665 2070 7265 6669 7820 6f66 2073  have prefix of s
-0000d400: 335f 7572 6c20 696e 2061 6373 656e 6469  3_url in acsendi
-0000d410: 6e67 2061 6c70 6861 6265 7469 6361 6c20  ng alphabetical 
-0000d420: 6f72 6465 720a 2020 2020 2020 2020 3a72  order.        :r
-0000d430: 6169 7365 733a 2053 3346 696c 654e 6f74  aises: S3FileNot
-0000d440: 466f 756e 6445 7272 6f72 2c20 5333 4e6f  FoundError, S3No
-0000d450: 7441 4469 7265 6374 6f72 7945 7272 6f72  tADirectoryError
-0000d460: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0000d470: 2020 2020 2065 6e74 7269 6573 203d 206c       entries = l
-0000d480: 6973 7428 7365 6c66 2e73 6361 6e64 6972  ist(self.scandir
-0000d490: 2866 6f6c 6c6f 776c 696e 6b73 3d66 6f6c  (followlinks=fol
-0000d4a0: 6c6f 776c 696e 6b73 2929 0a20 2020 2020  lowlinks)).     
-0000d4b0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-0000d4c0: 285b 656e 7472 792e 6e61 6d65 2066 6f72  ([entry.name for
-0000d4d0: 2065 6e74 7279 2069 6e20 656e 7472 6965   entry in entrie
-0000d4e0: 735d 290a 0a20 2020 2064 6566 2069 7465  s])..    def ite
-0000d4f0: 7264 6972 2873 656c 662c 2066 6f6c 6c6f  rdir(self, follo
-0000d500: 776c 696e 6b73 3a20 626f 6f6c 203d 2046  wlinks: bool = F
-0000d510: 616c 7365 2920 2d3e 2049 7465 7261 746f  alse) -> Iterato
-0000d520: 725b 2753 3350 6174 6827 5d3a 0a20 2020  r['S3Path']:.   
-0000d530: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-0000d540: 2047 6574 2061 6c6c 2063 6f6e 7465 6e74   Get all content
-0000d550: 7320 6f66 2067 6976 656e 2073 335f 7572  s of given s3_ur
-0000d560: 6c2e 2054 6865 2072 6573 756c 7420 6973  l. The result is
-0000d570: 2069 6e20 6163 7365 6e64 696e 6720 616c   in acsending al
-0000d580: 7068 6162 6574 6963 616c 206f 7264 6572  phabetical order
-0000d590: 2e0a 0a20 2020 2020 2020 203a 7265 7475  ...        :retu
-0000d5a0: 726e 733a 2041 6c6c 2063 6f6e 7465 6e74  rns: All content
-0000d5b0: 7320 6861 7665 2070 7265 6669 7820 6f66  s have prefix of
-0000d5c0: 2073 335f 7572 6c20 696e 2061 6373 656e   s3_url in acsen
-0000d5d0: 6469 6e67 2061 6c70 6861 6265 7469 6361  ding alphabetica
-0000d5e0: 6c20 6f72 6465 720a 2020 2020 2020 2020  l order.        
-0000d5f0: 3a72 6169 7365 733a 2053 3346 696c 654e  :raises: S3FileN
-0000d600: 6f74 466f 756e 6445 7272 6f72 2c20 5333  otFoundError, S3
-0000d610: 4e6f 7441 4469 7265 6374 6f72 7945 7272  NotADirectoryErr
-0000d620: 6f72 0a20 2020 2020 2020 2027 2727 0a20  or.        '''. 
-0000d630: 2020 2020 2020 2066 6f72 2070 6174 6820         for path 
-0000d640: 696e 2073 656c 662e 6c69 7374 6469 7228  in self.listdir(
-0000d650: 666f 6c6c 6f77 6c69 6e6b 733d 666f 6c6c  followlinks=foll
-0000d660: 6f77 6c69 6e6b 7329 3a0a 2020 2020 2020  owlinks):.      
-0000d670: 2020 2020 2020 7969 656c 6420 7365 6c66        yield self
-0000d680: 2e6a 6f69 6e70 6174 6828 7061 7468 2920  .joinpath(path) 
-0000d690: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
-0000d6a0: 0a20 2020 2064 6566 206c 6f61 6428 7365  .    def load(se
-0000d6b0: 6c66 2c20 666f 6c6c 6f77 6c69 6e6b 733a  lf, followlinks:
-0000d6c0: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
-0000d6d0: 3e20 4269 6e61 7279 494f 3a0a 2020 2020  > BinaryIO:.    
-0000d6e0: 2020 2020 2727 2752 6561 6420 616c 6c20      '''Read all 
-0000d6f0: 636f 6e74 656e 7420 696e 2062 696e 6172  content in binar
-0000d700: 7920 6f6e 2073 7065 6369 6669 6564 2070  y on specified p
-0000d710: 6174 6820 616e 6420 7772 6974 6520 696e  ath and write in
-0000d720: 746f 206d 656d 6f72 790a 0a20 2020 2020  to memory..     
-0000d730: 2020 2055 7365 7220 7368 6f75 6c64 2063     User should c
-0000d740: 6c6f 7365 2074 6865 2042 696e 6172 7949  lose the BinaryI
-0000d750: 4f20 6d61 6e75 616c 6c79 0a0a 2020 2020  O manually..    
-0000d760: 2020 2020 3a72 6574 7572 6e73 3a20 4269      :returns: Bi
-0000d770: 6e61 7279 494f 0a20 2020 2020 2020 2027  naryIO.        '
-0000d780: 2727 0a20 2020 2020 2020 2073 335f 7572  ''.        s3_ur
-0000d790: 6c20 3d20 7365 6c66 2e70 6174 685f 7769  l = self.path_wi
-0000d7a0: 7468 5f70 726f 746f 636f 6c0a 2020 2020  th_protocol.    
-0000d7b0: 2020 2020 6966 2066 6f6c 6c6f 776c 696e      if followlin
-0000d7c0: 6b73 3a0a 2020 2020 2020 2020 2020 2020  ks:.            
-0000d7d0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000d7e0: 2020 2020 2073 335f 7572 6c20 3d20 7365       s3_url = se
-0000d7f0: 6c66 2e72 6561 646c 696e 6b28 292e 7061  lf.readlink().pa
-0000d800: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
-0000d810: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-0000d820: 6570 7420 5333 4e6f 7441 4c69 6e6b 4572  ept S3NotALinkEr
-0000d830: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-0000d840: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-0000d850: 2020 6275 636b 6574 2c20 6b65 7920 3d20    bucket, key = 
-0000d860: 7061 7273 655f 7333 5f75 726c 2873 335f  parse_s3_url(s3_
-0000d870: 7572 6c29 0a20 2020 2020 2020 2069 6620  url).        if 
-0000d880: 6e6f 7420 6275 636b 6574 3a0a 2020 2020  not bucket:.    
-0000d890: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
-0000d8a0: 4275 636b 6574 4e6f 7446 6f75 6e64 4572  BucketNotFoundEr
-0000d8b0: 726f 7228 2745 6d70 7479 2062 7563 6b65  ror('Empty bucke
-0000d8c0: 7420 6e61 6d65 3a20 2572 2720 2520 7333  t name: %r' % s3
-0000d8d0: 5f75 726c 290a 2020 2020 2020 2020 6966  _url).        if
-0000d8e0: 206e 6f74 206b 6579 206f 7220 6b65 792e   not key or key.
-0000d8f0: 656e 6473 7769 7468 2827 2f27 293a 0a20  endswith('/'):. 
-0000d900: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000d910: 2053 3349 7341 4469 7265 6374 6f72 7945   S3IsADirectoryE
-0000d920: 7272 6f72 2827 4973 2061 2064 6972 6563  rror('Is a direc
-0000d930: 746f 7279 3a20 2572 2720 2520 7333 5f75  tory: %r' % s3_u
-0000d940: 726c 290a 0a20 2020 2020 2020 2062 7566  rl)..        buf
-0000d950: 6665 7220 3d20 696f 2e42 7974 6573 494f  fer = io.BytesIO
-0000d960: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
-0000d970: 7261 6973 655f 7333 5f65 7272 6f72 2873  raise_s3_error(s
-0000d980: 335f 7572 6c29 3a0a 2020 2020 2020 2020  3_url):.        
-0000d990: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
-0000d9a0: 2e64 6f77 6e6c 6f61 645f 6669 6c65 6f62  .download_fileob
-0000d9b0: 6a28 6275 636b 6574 2c20 6b65 792c 2062  j(bucket, key, b
-0000d9c0: 7566 6665 7229 0a20 2020 2020 2020 2062  uffer).        b
-0000d9d0: 7566 6665 722e 7365 656b 2830 290a 2020  uffer.seek(0).  
-0000d9e0: 2020 2020 2020 7265 7475 726e 2062 7566        return buf
-0000d9f0: 6665 720a 0a20 2020 2064 6566 2068 6173  fer..    def has
-0000da00: 6275 636b 6574 2873 656c 6629 202d 3e20  bucket(self) -> 
-0000da10: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
-0000da20: 270a 2020 2020 2020 2020 5465 7374 2069  '.        Test i
-0000da30: 6620 7468 6520 6275 636b 6574 206f 6620  f the bucket of 
-0000da40: 7333 5f75 726c 2065 7869 7374 730a 0a20  s3_url exists.. 
-0000da50: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
-0000da60: 2054 7275 6520 6966 2062 7563 6b65 7420   True if bucket 
-0000da70: 6f66 2073 335f 7572 6c20 6569 7873 7473  of s3_url eixsts
-0000da80: 2c20 656c 7365 2046 616c 7365 0a20 2020  , else False.   
-0000da90: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-0000daa0: 2062 7563 6b65 742c 205f 203d 2070 6172   bucket, _ = par
-0000dab0: 7365 5f73 335f 7572 6c28 7365 6c66 2e70  se_s3_url(self.p
-0000dac0: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
-0000dad0: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
-0000dae0: 7420 6275 636b 6574 3a0a 2020 2020 2020  t bucket:.      
-0000daf0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000db00: 7365 0a0a 2020 2020 2020 2020 7472 793a  se..        try:
-0000db10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000db20: 662e 5f63 6c69 656e 742e 6865 6164 5f62  f._client.head_b
-0000db30: 7563 6b65 7428 4275 636b 6574 3d62 7563  ucket(Bucket=buc
-0000db40: 6b65 7429 0a20 2020 2020 2020 2065 7863  ket).        exc
-0000db50: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-0000db60: 2065 7272 6f72 3a0a 2020 2020 2020 2020   error:.        
-0000db70: 2020 2020 6572 726f 7220 3d20 7472 616e      error = tran
-0000db80: 736c 6174 655f 7333 5f65 7272 6f72 2865  slate_s3_error(e
-0000db90: 7272 6f72 2c20 7365 6c66 2e70 6174 685f  rror, self.path_
-0000dba0: 7769 7468 5f70 726f 746f 636f 6c29 0a20  with_protocol). 
-0000dbb0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0000dbc0: 696e 7374 616e 6365 2865 7272 6f72 2c0a  instance(error,.
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 2020 2020 2020 2020 2020 2853 3355 6e6b            (S3Unk
-0000dbf0: 6e6f 776e 4572 726f 722c 2053 3343 6f6e  nownError, S3Con
-0000dc00: 6669 6745 7272 6f72 2c20 5333 5065 726d  figError, S3Perm
-0000dc10: 6973 7369 6f6e 4572 726f 7229 293a 0a20  issionError)):. 
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000dc30: 6169 7365 2065 7272 6f72 0a20 2020 2020  aise error.     
-0000dc40: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0000dc50: 616e 6365 2865 7272 6f72 2c20 5333 4669  ance(error, S3Fi
-0000dc60: 6c65 4e6f 7446 6f75 6e64 4572 726f 7229  leNotFoundError)
-0000dc70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000dc80: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-0000dc90: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000dca0: 7275 650a 0a20 2020 2064 6566 206d 6b64  rue..    def mkd
-0000dcb0: 6972 2873 656c 662c 206d 6f64 653d 306f  ir(self, mode=0o
-0000dcc0: 3737 372c 2070 6172 656e 7473 3a20 626f  777, parents: bo
-0000dcd0: 6f6c 203d 2046 616c 7365 2c20 6578 6973  ol = False, exis
-0000dce0: 745f 6f6b 3a20 626f 6f6c 203d 2046 616c  t_ok: bool = Fal
-0000dcf0: 7365 293a 0a20 2020 2020 2020 2027 2727  se):.        '''
-0000dd00: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
-0000dd10: 616e 2073 3320 6469 7265 6374 6f72 792e  an s3 directory.
-0000dd20: 0a20 2020 2020 2020 2050 7572 656c 7920  .        Purely 
-0000dd30: 6372 6561 7469 6e67 2064 6972 6563 746f  creating directo
-0000dd40: 7279 2069 7320 696e 7661 6c69 6420 6265  ry is invalid be
-0000dd50: 6361 7573 6520 6974 2773 2075 6e61 7661  cause it's unava
-0000dd60: 696c 6162 6c65 206f 6e20 4f53 532e 0a20  ilable on OSS.. 
-0000dd70: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
-0000dd80: 7469 6f6e 2069 7320 746f 2074 6573 7420  tion is to test 
-0000dd90: 7468 6520 7461 7267 6574 2062 7563 6b65  the target bucke
-0000dda0: 7420 6861 7665 2057 5249 5445 2061 6363  t have WRITE acc
-0000ddb0: 6573 732e 0a0a 2020 2020 2020 2020 3a70  ess...        :p
-0000ddc0: 6172 616d 206d 6f64 653a 206d 6f64 6520  aram mode: mode 
-0000ddd0: 6973 2069 676e 6f72 6564 2c20 6f6e 6c79  is ignored, only
-0000dde0: 2062 6520 636f 6d70 6174 6962 6c65 2077   be compatible w
-0000ddf0: 6974 6820 7061 7468 6c69 622e 5061 7468  ith pathlib.Path
-0000de00: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000de10: 7061 7265 6e74 733a 2070 6172 656e 7473  parents: parents
-0000de20: 2069 7320 6967 6e6f 7265 642c 206f 6e6c   is ignored, onl
-0000de30: 7920 6265 2063 6f6d 7061 7469 626c 6520  y be compatible 
-0000de40: 7769 7468 2070 6174 686c 6962 2e50 6174  with pathlib.Pat
-0000de50: 680a 2020 2020 2020 2020 3a70 6172 616d  h.        :param
-0000de60: 2065 7869 7374 5f6f 6b3a 2049 6620 4661   exist_ok: If Fa
-0000de70: 6c73 6520 616e 6420 7461 7267 6574 2064  lse and target d
-0000de80: 6972 6563 746f 7279 2065 7869 7374 732c  irectory exists,
-0000de90: 2072 6169 7365 2053 3346 696c 6545 7869   raise S3FileExi
-0000dea0: 7374 7345 7272 6f72 0a20 2020 2020 2020  stsError.       
-0000deb0: 203a 7261 6973 6573 3a20 5333 4275 636b   :raises: S3Buck
-0000dec0: 6574 4e6f 7446 6f75 6e64 4572 726f 722c  etNotFoundError,
-0000ded0: 2053 3346 696c 6545 7869 7374 7345 7272   S3FileExistsErr
-0000dee0: 6f72 0a20 2020 2020 2020 2027 2727 0a20  or.        '''. 
-0000def0: 2020 2020 2020 2062 7563 6b65 742c 205f         bucket, _
-0000df00: 203d 2070 6172 7365 5f73 335f 7572 6c28   = parse_s3_url(
-0000df10: 7365 6c66 2e70 6174 685f 7769 7468 5f70  self.path_with_p
-0000df20: 726f 746f 636f 6c29 0a20 2020 2020 2020  rotocol).       
-0000df30: 2069 6620 6e6f 7420 6275 636b 6574 3a0a   if not bucket:.
-0000df40: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000df50: 6520 5333 4275 636b 6574 4e6f 7446 6f75  e S3BucketNotFou
-0000df60: 6e64 4572 726f 7228 0a20 2020 2020 2020  ndError(.       
-0000df70: 2020 2020 2020 2020 2027 456d 7074 7920           'Empty 
-0000df80: 6275 636b 6574 206e 616d 653a 2025 7227  bucket name: %r'
-0000df90: 2025 2073 656c 662e 7061 7468 5f77 6974   % self.path_wit
-0000dfa0: 685f 7072 6f74 6f63 6f6c 290a 2020 2020  h_protocol).    
-0000dfb0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0000dfc0: 6861 7362 7563 6b65 7428 293a 0a20 2020  hasbucket():.   
-0000dfd0: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-0000dfe0: 3342 7563 6b65 744e 6f74 466f 756e 6445  3BucketNotFoundE
-0000dff0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000e000: 2020 2020 2020 274e 6f20 7375 6368 2062        'No such b
-0000e010: 7563 6b65 743a 2025 7227 2025 2073 656c  ucket: %r' % sel
-0000e020: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
-0000e030: 6f63 6f6c 290a 2020 2020 2020 2020 6966  ocol).        if
-0000e040: 2065 7869 7374 5f6f 6b3a 0a20 2020 2020   exist_ok:.     
-0000e050: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-0000e060: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
-0000e070: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000e080: 5333 4669 6c65 4578 6973 7473 4572 726f  S3FileExistsErro
-0000e090: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000e0a0: 2020 2020 2020 2027 4669 6c65 2065 7869         'File exi
-0000e0b0: 7374 733a 2025 7227 2025 2073 656c 662e  sts: %r' % self.
-0000e0c0: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
-0000e0d0: 6f6c 290a 2020 2020 2020 2020 2020 2020  ol).            
-0000e0e0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000e0f0: 6620 7365 6c66 2e65 7869 7374 7328 293a  f self.exists():
-0000e100: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000e110: 7365 2053 3346 696c 6545 7869 7374 7345  se S3FileExistsE
-0000e120: 7272 6f72 2827 4669 6c65 2065 7869 7374  rror('File exist
-0000e130: 733a 2025 7227 2025 2073 656c 662e 7061  s: %r' % self.pa
-0000e140: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
-0000e150: 290a 0a20 2020 2064 6566 206d 6f76 6528  )..    def move(
-0000e160: 7365 6c66 2c20 6473 745f 7572 6c3a 2050  self, dst_url: P
-0000e170: 6174 684c 696b 6529 202d 3e20 4e6f 6e65  athLike) -> None
-0000e180: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-0000e190: 2020 2020 2020 4d6f 7665 2066 696c 652f        Move file/
-0000e1a0: 6469 7265 6374 6f72 7920 7061 7468 2066  directory path f
-0000e1b0: 726f 6d20 7372 635f 7572 6c20 746f 2064  rom src_url to d
-0000e1c0: 7374 5f75 726c 0a0a 2020 2020 2020 2020  st_url..        
-0000e1d0: 3a70 6172 616d 2064 7374 5f75 726c 3a20  :param dst_url: 
-0000e1e0: 4769 7665 6e20 6465 7374 696e 6174 696f  Given destinatio
-0000e1f0: 6e20 7061 7468 0a20 2020 2020 2020 2027  n path.        '
-0000e200: 2727 0a20 2020 2020 2020 2066 6f72 2073  ''.        for s
-0000e210: 7263 5f66 696c 655f 7061 7468 2c20 6473  rc_file_path, ds
-0000e220: 745f 6669 6c65 5f70 6174 6820 696e 205f  t_file_path in _
-0000e230: 7333 5f73 6361 6e5f 7061 6972 7328 0a20  s3_scan_pairs(. 
-0000e240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e250: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
-0000e260: 6f74 6f63 6f6c 2c20 6473 745f 7572 6c29  otocol, dst_url)
-0000e270: 3a0a 2020 2020 2020 2020 2020 2020 5333  :.            S3
-0000e280: 5061 7468 2873 7263 5f66 696c 655f 7061  Path(src_file_pa
-0000e290: 7468 292e 7265 6e61 6d65 2864 7374 5f66  th).rename(dst_f
-0000e2a0: 696c 655f 7061 7468 290a 0a20 2020 2064  ile_path)..    d
-0000e2b0: 6566 2072 656d 6f76 6528 7365 6c66 2c20  ef remove(self, 
-0000e2c0: 6d69 7373 696e 675f 6f6b 3a20 626f 6f6c  missing_ok: bool
-0000e2d0: 203d 2046 616c 7365 2920 2d3e 204e 6f6e   = False) -> Non
-0000e2e0: 653a 0a20 2020 2020 2020 2027 2727 0a20  e:.        '''. 
-0000e2f0: 2020 2020 2020 2052 656d 6f76 6520 7468         Remove th
-0000e300: 6520 6669 6c65 206f 7220 6469 7265 6374  e file or direct
-0000e310: 6f72 7920 6f6e 2073 332c 2060 7333 3a2f  ory on s3, `s3:/
-0000e320: 2f60 2061 6e64 2060 7333 3a2f 2f62 7563  /` and `s3://buc
-0000e330: 6b65 7460 2061 7265 206e 6f74 2070 6572  ket` are not per
-0000e340: 6d69 7474 6564 2074 6f20 7265 6d6f 7665  mitted to remove
-0000e350: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000e360: 206d 6973 7369 6e67 5f6f 6b3a 2069 6620   missing_ok: if 
-0000e370: 4661 6c73 6520 616e 6420 7461 7267 6574  False and target
-0000e380: 2066 696c 652f 6469 7265 6374 6f72 7920   file/directory 
-0000e390: 6e6f 7420 6578 6973 7473 2c20 7261 6973  not exists, rais
-0000e3a0: 6520 5333 4669 6c65 4e6f 7446 6f75 6e64  e S3FileNotFound
-0000e3b0: 4572 726f 720a 2020 2020 2020 2020 3a72  Error.        :r
-0000e3c0: 6169 7365 733a 2053 3350 6572 6d69 7373  aises: S3Permiss
-0000e3d0: 696f 6e45 7272 6f72 2c20 5333 4669 6c65  ionError, S3File
-0000e3e0: 4e6f 7446 6f75 6e64 4572 726f 722c 2055  NotFoundError, U
-0000e3f0: 6e73 7570 706f 7274 6564 4572 726f 720a  nsupportedError.
-0000e400: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000e410: 2020 2020 6275 636b 6574 2c20 6b65 7920      bucket, key 
-0000e420: 3d20 7061 7273 655f 7333 5f75 726c 2873  = parse_s3_url(s
-0000e430: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
-0000e440: 6f74 6f63 6f6c 290a 2020 2020 2020 2020  otocol).        
-0000e450: 6966 206e 6f74 2062 7563 6b65 743a 0a20  if not bucket:. 
-0000e460: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000e470: 7420 6b65 793a 0a20 2020 2020 2020 2020  t key:.         
-0000e480: 2020 2020 2020 2072 6169 7365 2055 6e73         raise Uns
-0000e490: 7570 706f 7274 6564 4572 726f 7228 0a20  upportedError(. 
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4b0: 2020 2027 5265 6d6f 7665 2077 686f 6c65     'Remove whole
-0000e4c0: 2073 3327 2c20 7365 6c66 2e70 6174 685f   s3', self.path_
-0000e4d0: 7769 7468 5f70 726f 746f 636f 6c29 0a20  with_protocol). 
-0000e4e0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000e4f0: 2053 3342 7563 6b65 744e 6f74 466f 756e   S3BucketNotFoun
-0000e500: 6445 7272 6f72 280a 2020 2020 2020 2020  dError(.        
-0000e510: 2020 2020 2020 2020 2745 6d70 7479 2062          'Empty b
-0000e520: 7563 6b65 7420 6e61 6d65 3a20 2572 2720  ucket name: %r' 
-0000e530: 2520 7365 6c66 2e70 6174 685f 7769 7468  % self.path_with
-0000e540: 5f70 726f 746f 636f 6c29 0a20 2020 2020  _protocol).     
-0000e550: 2020 2069 6620 6e6f 7420 6b65 793a 0a20     if not key:. 
-0000e560: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000e570: 2055 6e73 7570 706f 7274 6564 4572 726f   UnsupportedErro
-0000e580: 7228 2752 656d 6f76 6520 6275 636b 6574  r('Remove bucket
-0000e590: 272c 2073 656c 662e 7061 7468 5f77 6974  ', self.path_wit
-0000e5a0: 685f 7072 6f74 6f63 6f6c 290a 2020 2020  h_protocol).    
-0000e5b0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0000e5c0: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-0000e5d0: 2020 2020 2020 6966 206d 6973 7369 6e67        if missing
-0000e5e0: 5f6f 6b3a 0a20 2020 2020 2020 2020 2020  _ok:.           
-0000e5f0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000e600: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
-0000e610: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
-0000e620: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000e630: 2020 2027 4e6f 2073 7563 6820 6669 6c65     'No such file
-0000e640: 206f 7220 6469 7265 6374 6f72 793a 2025   or directory: %
-0000e650: 7227 2025 2073 656c 662e 7061 7468 5f77  r' % self.path_w
-0000e660: 6974 685f 7072 6f74 6f63 6f6c 290a 0a20  ith_protocol).. 
-0000e670: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
-0000e680: 7365 6c66 2e5f 636c 6965 6e74 0a20 2020  self._client.   
-0000e690: 2020 2020 2077 6974 6820 7261 6973 655f       with raise_
-0000e6a0: 7333 5f65 7272 6f72 2873 656c 662e 7061  s3_error(self.pa
-0000e6b0: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
-0000e6c0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-0000e6d0: 6620 7365 6c66 2e69 735f 6669 6c65 2829  f self.is_file()
-0000e6e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e6f0: 2020 636c 6965 6e74 2e64 656c 6574 655f    client.delete_
-0000e700: 6f62 6a65 6374 2842 7563 6b65 743d 6275  object(Bucket=bu
-0000e710: 636b 6574 2c20 4b65 793d 6b65 7929 0a20  cket, Key=key). 
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e730: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-0000e740: 2020 7072 6566 6978 203d 205f 6265 636f    prefix = _beco
-0000e750: 6d65 5f70 7265 6669 7828 6b65 7929 0a20  me_prefix(key). 
-0000e760: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-0000e770: 5f63 6f75 6e74 2c20 6572 726f 725f 636f  _count, error_co
-0000e780: 756e 7420 3d20 302c 2030 0a20 2020 2020  unt = 0, 0.     
-0000e790: 2020 2020 2020 2066 6f72 2072 6573 7020         for resp 
-0000e7a0: 696e 205f 6c69 7374 5f6f 626a 6563 7473  in _list_objects
-0000e7b0: 5f72 6563 7572 7369 7665 2863 6c69 656e  _recursive(clien
-0000e7c0: 742c 2062 7563 6b65 742c 2070 7265 6669  t, bucket, prefi
-0000e7d0: 7829 3a0a 2020 2020 2020 2020 2020 2020  x):.            
-0000e7e0: 2020 2020 6966 2027 436f 6e74 656e 7473      if 'Contents
-0000e7f0: 2720 696e 2072 6573 703a 0a20 2020 2020  ' in resp:.     
-0000e800: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-0000e810: 6579 7320 3d20 5b0a 2020 2020 2020 2020  eys = [.        
-0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e830: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0000e840: 2020 2020 2020 2020 2020 2020 2020 274b                'K
-0000e850: 6579 273a 2063 6f6e 7465 6e74 5b27 4b65  ey': content['Ke
-0000e860: 7927 5d0a 2020 2020 2020 2020 2020 2020  y'].            
-0000e870: 2020 2020 2020 2020 2020 2020 7d20 666f              } fo
-0000e880: 7220 636f 6e74 656e 7420 696e 2072 6573  r content in res
-0000e890: 705b 2743 6f6e 7465 6e74 7327 5d0a 2020  p['Contents'].  
-0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8b0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-0000e8c0: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
-0000e8d0: 756e 7420 2b3d 206c 656e 286b 6579 7329  unt += len(keys)
-0000e8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e8f0: 2020 2020 2065 7272 6f72 7320 3d20 5b5d       errors = []
-0000e900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e910: 2020 2020 2072 6574 7269 6573 203d 2032       retries = 2
-0000e920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e930: 2020 2020 2072 6574 7279 5f69 6e74 6572       retry_inter
-0000e940: 7661 6c20 3d20 6d69 6e28 302e 3120 2a20  val = min(0.1 * 
-0000e950: 322a 2a72 6574 7269 6573 2c20 3330 290a  2**retries, 30).
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000e980: 6765 2872 6574 7269 6573 293a 0a20 2020  ge(retries):.   
-0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9a0: 2020 2020 2023 2064 6f63 3a20 6874 7470       # doc: http
-0000e9b0: 733a 2f2f 626f 746f 332e 616d 617a 6f6e  s://boto3.amazon
-0000e9c0: 6177 732e 636f 6d2f 7631 2f64 6f63 756d  aws.com/v1/docum
-0000e9d0: 656e 7461 7469 6f6e 2f61 7069 2f6c 6174  entation/api/lat
-0000e9e0: 6573 742f 7265 6665 7265 6e63 652f 7365  est/reference/se
-0000e9f0: 7276 6963 6573 2f73 332e 6874 6d6c 2353  rvices/s3.html#S
-0000ea00: 332e 436c 6965 6e74 2e64 656c 6574 655f  3.Client.delete_
-0000ea10: 6f62 6a65 6374 730a 2020 2020 2020 2020  objects.        
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 6966 206e 6f74 206b 6579 733a 0a20 2020  if not keys:.   
+0000c370: 2070 726f 6669 6c65 5f6e 616d 653d 7365   profile_name=se
+0000c380: 6c66 2e5f 7072 6f66 696c 655f 6e61 6d65  lf._profile_name
+0000c390: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000c3a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c3b0: 6c66 2e5f 7072 6f66 696c 655f 6e61 6d65  lf._profile_name
+0000c3c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000c3e0: 6c65 5f65 6e74 7279 203d 2066 696c 655f  le_entry = file_
+0000c3f0: 656e 7472 792e 5f72 6570 6c61 6365 280a  entry._replace(.
+0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c420: 7061 7468 3d0a 2020 2020 2020 2020 2020  path=.          
+0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c440: 2020 2020 2020 6622 7b73 656c 662e 5f70        f"{self._p
+0000c450: 726f 746f 636f 6c5f 7769 7468 5f70 726f  rotocol_with_pro
+0000c460: 6669 6c65 7d3a 2f2f 7b66 696c 655f 656e  file}://{file_en
+0000c470: 7472 792e 7061 7468 5b35 3a5d 7d22 0a20  try.path[5:]}". 
+0000c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c490: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4b0: 2020 2020 2079 6965 6c64 2066 696c 655f       yield file_
+0000c4c0: 656e 7472 790a 0a20 2020 2020 2020 2072  entry..        r
+0000c4d0: 6574 7572 6e20 5f63 7265 6174 655f 6d69  eturn _create_mi
+0000c4e0: 7373 696e 675f 6f6b 5f67 656e 6572 6174  ssing_ok_generat
+0000c4f0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000c500: 6372 6561 7465 5f67 656e 6572 6174 6f72  create_generator
+0000c510: 2829 2c20 6d69 7373 696e 675f 6f6b 2c0a  (), missing_ok,.
+0000c520: 2020 2020 2020 2020 2020 2020 5333 4669              S3Fi
+0000c530: 6c65 4e6f 7446 6f75 6e64 4572 726f 7228  leNotFoundError(
+0000c540: 274e 6f20 6d61 7463 6820 6669 6c65 3a20  'No match file: 
+0000c550: 2572 2720 2520 7333 5f70 6174 686e 616d  %r' % s3_pathnam
+0000c560: 6529 290a 0a20 2020 2064 6566 2069 676c  e))..    def igl
+0000c570: 6f62 280a 2020 2020 2020 2020 2020 2020  ob(.            
+0000c580: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+0000c590: 2020 7061 7474 6572 6e2c 0a20 2020 2020    pattern,.     
+0000c5a0: 2020 2020 2020 2072 6563 7572 7369 7665         recursive
+0000c5b0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+0000c5c0: 2020 2020 2020 2020 2020 206d 6973 7369             missi
+0000c5d0: 6e67 5f6f 6b3a 2062 6f6f 6c20 3d20 5472  ng_ok: bool = Tr
+0000c5e0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000c5f0: 666f 6c6c 6f77 6c69 6e6b 733a 2062 6f6f  followlinks: boo
+0000c600: 6c20 3d20 4661 6c73 652c 0a20 2020 2029  l = False,.    )
+0000c610: 202d 3e20 4974 6572 6174 6f72 5b27 5333   -> Iterator['S3
+0000c620: 5061 7468 275d 3a0a 2020 2020 2020 2020  Path']:.        
+0000c630: 2727 2752 6574 7572 6e20 7333 2070 6174  '''Return s3 pat
+0000c640: 6820 6974 6572 6174 6f72 2069 6e20 6173  h iterator in as
+0000c650: 6365 6e64 696e 6720 616c 7068 6162 6574  cending alphabet
+0000c660: 6963 616c 206f 7264 6572 2c20 696e 2077  ical order, in w
+0000c670: 6869 6368 2070 6174 6820 6d61 7463 6865  hich path matche
+0000c680: 7320 676c 6f62 2070 6174 7465 726e 0a20  s glob pattern. 
+0000c690: 2020 2020 2020 204e 6f74 6573 3a20 4f6e         Notes: On
+0000c6a0: 6c79 2067 6c6f 6220 696e 2062 7563 6b65  ly glob in bucke
+0000c6b0: 742e 2049 6620 7472 7969 6e67 2074 6f20  t. If trying to 
+0000c6c0: 6d61 7463 6820 6275 636b 6574 2077 6974  match bucket wit
+0000c6d0: 6820 7769 6c64 6361 7264 2063 6861 7261  h wildcard chara
+0000c6e0: 6374 6572 732c 2072 6169 7365 2055 6e73  cters, raise Uns
+0000c6f0: 7570 706f 7274 6564 4572 726f 720a 0a20  upportedError.. 
+0000c700: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
+0000c710: 7474 6572 6e3a 2047 6c6f 6220 7468 6520  ttern: Glob the 
+0000c720: 6769 7665 6e20 7265 6c61 7469 7665 2070  given relative p
+0000c730: 6174 7465 726e 2069 6e20 7468 6520 6469  attern in the di
+0000c740: 7265 6374 6f72 7920 7265 7072 6573 656e  rectory represen
+0000c750: 7465 6420 6279 2074 6869 7320 7061 7468  ted by this path
+0000c760: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000c770: 7265 6375 7273 6976 653a 2049 6620 4661  recursive: If Fa
+0000c780: 6c73 652c 2060 2a2a 6020 7769 6c6c 206e  lse, `**` will n
+0000c790: 6f74 2073 6561 7263 6820 6469 7265 6374  ot search direct
+0000c7a0: 6f72 7920 7265 6375 7273 6976 656c 790a  ory recursively.
+0000c7b0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
+0000c7c0: 6973 7369 6e67 5f6f 6b3a 2049 6620 4661  issing_ok: If Fa
+0000c7d0: 6c73 6520 616e 6420 7461 7267 6574 2070  lse and target p
+0000c7e0: 6174 6820 646f 6573 6e27 7420 6d61 7463  ath doesn't matc
+0000c7f0: 6820 616e 7920 6669 6c65 2c20 7261 6973  h any file, rais
+0000c800: 6520 4669 6c65 4e6f 7446 6f75 6e64 4572  e FileNotFoundEr
+0000c810: 726f 720a 2020 2020 2020 2020 3a72 6169  ror.        :rai
+0000c820: 7365 733a 2055 6e73 7570 706f 7274 6564  ses: Unsupported
+0000c830: 4572 726f 722c 2077 6865 6e20 6275 636b  Error, when buck
+0000c840: 6574 2070 6172 7420 636f 6e74 6169 6e73  et part contains
+0000c850: 2077 696c 6463 6172 6420 6368 6172 6163   wildcard charac
+0000c860: 7465 7273 0a20 2020 2020 2020 203a 7265  ters.        :re
+0000c870: 7475 726e 733a 2041 6e20 6974 6572 6174  turns: An iterat
+0000c880: 6f72 2063 6f6e 7461 696e 7320 7061 7468  or contains path
+0000c890: 7320 6d61 7463 6820 6073 335f 7061 7468  s match `s3_path
+0000c8a0: 6e61 6d65 600a 2020 2020 2020 2020 2727  name`.        ''
+0000c8b0: 270a 2020 2020 2020 2020 666f 7220 6669  '.        for fi
+0000c8c0: 6c65 5f65 6e74 7279 2069 6e20 7365 6c66  le_entry in self
+0000c8d0: 2e67 6c6f 625f 7374 6174 2870 6174 7465  .glob_stat(patte
+0000c8e0: 726e 3d70 6174 7465 726e 2c20 7265 6375  rn=pattern, recu
+0000c8f0: 7273 6976 653d 7265 6375 7273 6976 652c  rsive=recursive,
+0000c900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c920: 2020 2020 2020 2020 2020 6d69 7373 696e            missin
+0000c930: 675f 6f6b 3d6d 6973 7369 6e67 5f6f 6b2c  g_ok=missing_ok,
+0000c940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c960: 2020 2020 2020 2020 2020 666f 6c6c 6f77            follow
+0000c970: 6c69 6e6b 733d 666f 6c6c 6f77 6c69 6e6b  links=followlink
+0000c980: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000c990: 7969 656c 6420 7365 6c66 2e66 726f 6d5f  yield self.from_
+0000c9a0: 7061 7468 2866 696c 655f 656e 7472 792e  path(file_entry.
+0000c9b0: 7061 7468 290a 0a20 2020 2064 6566 2069  path)..    def i
+0000c9c0: 735f 6469 7228 7365 6c66 2c20 666f 6c6c  s_dir(self, foll
+0000c9d0: 6f77 6c69 6e6b 733a 2062 6f6f 6c20 3d20  owlinks: bool = 
+0000c9e0: 4661 6c73 6529 202d 3e20 626f 6f6c 3a0a  False) -> bool:.
+0000c9f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000ca00: 2020 2020 5465 7374 2069 6620 616e 2073      Test if an s
+0000ca10: 3320 7572 6c20 6973 2064 6972 6563 746f  3 url is directo
+0000ca20: 7279 0a20 2020 2020 2020 2053 7065 6369  ry.        Speci
+0000ca30: 6669 6320 7072 6f63 6564 7572 6573 2061  fic procedures a
+0000ca40: 7265 2061 7320 666f 6c6c 6f77 733a 0a20  re as follows:. 
+0000ca50: 2020 2020 2020 2049 6620 7468 6572 6520         If there 
+0000ca60: 6578 6973 7473 2061 2073 7566 6669 782c  exists a suffix,
+0000ca70: 206f 6620 7768 6963 6820 6060 6f73 2e70   of which ``os.p
+0000ca80: 6174 682e 6a6f 696e 2873 335f 7572 6c2c  ath.join(s3_url,
+0000ca90: 2073 7566 6669 7829 6060 2069 7320 6120   suffix)`` is a 
+0000caa0: 6669 6c65 0a20 2020 2020 2020 2049 6620  file.        If 
+0000cab0: 7468 6520 7572 6c20 6973 2065 6d70 7479  the url is empty
+0000cac0: 2062 7563 6b65 7420 6f72 2073 333a 2f2f   bucket or s3://
+0000cad0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000cae0: 2066 6f6c 6c6f 776c 696e 6b73 3a20 7768   followlinks: wh
+0000caf0: 6574 6865 7220 666f 6c6c 6f77 6c69 6e6b  ether followlink
+0000cb00: 7320 6973 2054 7275 6520 6f72 2046 616c  s is True or Fal
+0000cb10: 7365 2c20 7265 7375 6c74 2069 7320 7468  se, result is th
+0000cb20: 6520 7361 6d65 2e20 4265 6361 7573 6520  e same. Because 
+0000cb30: 7333 2073 796d 6c69 6e6b 206e 6f74 2073  s3 symlink not s
+0000cb40: 7570 706f 7274 2064 6972 2e0a 2020 2020  upport dir..    
+0000cb50: 2020 2020 3a72 6574 7572 6e73 3a20 5472      :returns: Tr
+0000cb60: 7565 2069 6620 7061 7468 2069 7320 7333  ue if path is s3
+0000cb70: 2064 6972 6563 746f 7279 2c20 656c 7365   directory, else
+0000cb80: 2046 616c 7365 0a20 2020 2020 2020 2027   False.        '
+0000cb90: 2727 0a20 2020 2020 2020 2062 7563 6b65  ''.        bucke
+0000cba0: 742c 206b 6579 203d 2070 6172 7365 5f73  t, key = parse_s
+0000cbb0: 335f 7572 6c28 7365 6c66 2e70 6174 685f  3_url(self.path_
+0000cbc0: 7769 7468 5f70 726f 746f 636f 6c29 0a20  with_protocol). 
+0000cbd0: 2020 2020 2020 2069 6620 6e6f 7420 6275         if not bu
+0000cbe0: 636b 6574 3a20 2023 2073 333a 2f2f 203d  cket:  # s3:// =
+0000cbf0: 3e20 5472 7565 2c20 7333 3a2f 2f2f 6b65  > True, s3:///ke
+0000cc00: 7920 3d3e 2046 616c 7365 0a20 2020 2020  y => False.     
+0000cc10: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
+0000cc20: 7420 6b65 790a 2020 2020 2020 2020 7072  t key.        pr
+0000cc30: 6566 6978 203d 205f 6265 636f 6d65 5f70  efix = _become_p
+0000cc40: 7265 6669 7828 6b65 7929 0a20 2020 2020  refix(key).     
+0000cc50: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000cc60: 2020 2020 7265 7370 203d 2073 656c 662e      resp = self.
+0000cc70: 5f63 6c69 656e 742e 6c69 7374 5f6f 626a  _client.list_obj
+0000cc80: 6563 7473 5f76 3228 0a20 2020 2020 2020  ects_v2(.       
+0000cc90: 2020 2020 2020 2020 2042 7563 6b65 743d           Bucket=
+0000cca0: 6275 636b 6574 2c20 5072 6566 6978 3d70  bucket, Prefix=p
+0000ccb0: 7265 6669 782c 2044 656c 696d 6974 6572  refix, Delimiter
+0000ccc0: 3d27 2f27 2c20 4d61 784b 6579 733d 3129  ='/', MaxKeys=1)
+0000ccd0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000cce0: 4578 6365 7074 696f 6e20 6173 2065 7272  Exception as err
+0000ccf0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0000cd00: 6572 726f 7220 3d20 7472 616e 736c 6174  error = translat
+0000cd10: 655f 7333 5f65 7272 6f72 2865 7272 6f72  e_s3_error(error
+0000cd20: 2c20 7365 6c66 2e70 6174 685f 7769 7468  , self.path_with
+0000cd30: 5f70 726f 746f 636f 6c29 0a20 2020 2020  _protocol).     
+0000cd40: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000cd50: 616e 6365 2865 7272 6f72 2c0a 2020 2020  ance(error,.    
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 2020 2853 3355 6e6b 6e6f 776e        (S3Unknown
+0000cd80: 4572 726f 722c 2053 3343 6f6e 6669 6745  Error, S3ConfigE
+0000cd90: 7272 6f72 2c20 5333 5065 726d 6973 7369  rror, S3Permissi
+0000cda0: 6f6e 4572 726f 7229 293a 0a20 2020 2020  onError)):.     
+0000cdb0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000cdc0: 2065 7272 6f72 0a20 2020 2020 2020 2020   error.         
+0000cdd0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0000cde0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000cdf0: 6b65 793a 2020 2320 6275 636b 6574 2069  key:  # bucket i
+0000ce00: 7320 6163 6365 7373 6962 6c65 0a20 2020  s accessible.   
+0000ce10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000ce20: 5472 7565 0a0a 2020 2020 2020 2020 6966  True..        if
+0000ce30: 2027 4b65 7943 6f75 6e74 2720 696e 2072   'KeyCount' in r
+0000ce40: 6573 703a 0a20 2020 2020 2020 2020 2020  esp:.           
+0000ce50: 2072 6574 7572 6e20 7265 7370 5b27 4b65   return resp['Ke
+0000ce60: 7943 6f75 6e74 275d 203e 2030 0a0a 2020  yCount'] > 0..  
+0000ce70: 2020 2020 2020 7265 7475 726e 206c 656e        return len
+0000ce80: 2872 6573 702e 6765 7428 2743 6f6e 7465  (resp.get('Conte
+0000ce90: 6e74 7327 2c20 5b5d 2929 203e 2030 206f  nts', [])) > 0 o
+0000cea0: 7220 5c0a 2020 2020 2020 2020 2020 2020  r \.            
+0000ceb0: 6c65 6e28 7265 7370 2e67 6574 2827 436f  len(resp.get('Co
+0000cec0: 6d6d 6f6e 5072 6566 6978 6573 272c 205b  mmonPrefixes', [
+0000ced0: 5d29 2920 3e20 300a 0a20 2020 2064 6566  ])) > 0..    def
+0000cee0: 2069 735f 6669 6c65 2873 656c 662c 2066   is_file(self, f
+0000cef0: 6f6c 6c6f 776c 696e 6b73 3a20 626f 6f6c  ollowlinks: bool
+0000cf00: 203d 2046 616c 7365 2920 2d3e 2062 6f6f   = False) -> boo
+0000cf10: 6c3a 0a20 2020 2020 2020 2027 2727 0a20  l:.        '''. 
+0000cf20: 2020 2020 2020 2054 6573 7420 6966 2061         Test if a
+0000cf30: 6e20 7333 5f75 726c 2069 7320 6669 6c65  n s3_url is file
+0000cf40: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+0000cf50: 6e73 3a20 5472 7565 2069 6620 7061 7468  ns: True if path
+0000cf60: 2069 7320 7333 2066 696c 652c 2065 6c73   is s3 file, els
+0000cf70: 6520 4661 6c73 650a 2020 2020 2020 2020  e False.        
+0000cf80: 2727 270a 2020 2020 2020 2020 7333 5f75  '''.        s3_u
+0000cf90: 726c 203d 2073 656c 662e 7061 7468 5f77  rl = self.path_w
+0000cfa0: 6974 685f 7072 6f74 6f63 6f6c 0a20 2020  ith_protocol.   
+0000cfb0: 2020 2020 2069 6620 666f 6c6c 6f77 6c69       if followli
+0000cfc0: 6e6b 733a 0a20 2020 2020 2020 2020 2020  nks:.           
+0000cfd0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000cfe0: 2020 2020 2020 7333 5f75 726c 203d 2073        s3_url = s
+0000cff0: 656c 662e 7265 6164 6c69 6e6b 2829 2e70  elf.readlink().p
+0000d000: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
+0000d010: 6c0a 2020 2020 2020 2020 2020 2020 6578  l.            ex
+0000d020: 6365 7074 2053 334e 6f74 414c 696e 6b45  cept S3NotALinkE
+0000d030: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+0000d040: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+0000d050: 2020 2062 7563 6b65 742c 206b 6579 203d     bucket, key =
+0000d060: 2070 6172 7365 5f73 335f 7572 6c28 7333   parse_s3_url(s3
+0000d070: 5f75 726c 290a 2020 2020 2020 2020 6966  _url).        if
+0000d080: 206e 6f74 2062 7563 6b65 7420 6f72 206e   not bucket or n
+0000d090: 6f74 206b 6579 206f 7220 6b65 792e 656e  ot key or key.en
+0000d0a0: 6473 7769 7468 2827 2f27 293a 0a20 2020  dswith('/'):.   
+0000d0b0: 2020 2020 2020 2020 2023 2073 333a 2f2f           # s3://
+0000d0c0: 2c20 7333 3a2f 2f2f 6b65 792c 2073 333a  , s3:///key, s3:
+0000d0d0: 2f2f 6275 636b 6574 2c20 7333 3a2f 2f62  //bucket, s3://b
+0000d0e0: 7563 6b65 742f 7072 6566 6978 2f0a 2020  ucket/prefix/.  
+0000d0f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000d100: 2046 616c 7365 0a20 2020 2020 2020 2074   False.        t
+0000d110: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000d120: 7365 6c66 2e5f 636c 6965 6e74 2e68 6561  self._client.hea
+0000d130: 645f 6f62 6a65 6374 2842 7563 6b65 743d  d_object(Bucket=
+0000d140: 6275 636b 6574 2c20 4b65 793d 6b65 7929  bucket, Key=key)
+0000d150: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000d160: 4578 6365 7074 696f 6e20 6173 2065 7272  Exception as err
+0000d170: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0000d180: 6572 726f 7220 3d20 7472 616e 736c 6174  error = translat
+0000d190: 655f 7333 5f65 7272 6f72 2865 7272 6f72  e_s3_error(error
+0000d1a0: 2c20 7333 5f75 726c 290a 2020 2020 2020  , s3_url).      
+0000d1b0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000d1c0: 6e63 6528 6572 726f 722c 0a20 2020 2020  nce(error,.     
+0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1e0: 2020 2020 2028 5333 556e 6b6e 6f77 6e45       (S3UnknownE
+0000d1f0: 7272 6f72 2c20 5333 436f 6e66 6967 4572  rror, S3ConfigEr
+0000d200: 726f 722c 2053 3350 6572 6d69 7373 696f  ror, S3Permissio
+0000d210: 6e45 7272 6f72 2929 3a0a 2020 2020 2020  nError)):.      
+0000d220: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d230: 6572 726f 720a 2020 2020 2020 2020 2020  error.          
+0000d240: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+0000d250: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0000d260: 7565 0a0a 2020 2020 6465 6620 6c69 7374  ue..    def list
+0000d270: 6469 7228 7365 6c66 2c20 666f 6c6c 6f77  dir(self, follow
+0000d280: 6c69 6e6b 733a 2062 6f6f 6c20 3d20 4661  links: bool = Fa
+0000d290: 6c73 6529 202d 3e20 4c69 7374 5b73 7472  lse) -> List[str
+0000d2a0: 5d3a 0a20 2020 2020 2020 2027 2727 0a20  ]:.        '''. 
+0000d2b0: 2020 2020 2020 2047 6574 2061 6c6c 2063         Get all c
+0000d2c0: 6f6e 7465 6e74 7320 6f66 2067 6976 656e  ontents of given
+0000d2d0: 2073 335f 7572 6c2e 2054 6865 2072 6573   s3_url. The res
+0000d2e0: 756c 7420 6973 2069 6e20 6163 7365 6e64  ult is in acsend
+0000d2f0: 696e 6720 616c 7068 6162 6574 6963 616c  ing alphabetical
+0000d300: 206f 7264 6572 2e0a 0a20 2020 2020 2020   order...       
+0000d310: 203a 7265 7475 726e 733a 2041 6c6c 2063   :returns: All c
+0000d320: 6f6e 7465 6e74 7320 6861 7665 2070 7265  ontents have pre
+0000d330: 6669 7820 6f66 2073 335f 7572 6c20 696e  fix of s3_url in
+0000d340: 2061 6373 656e 6469 6e67 2061 6c70 6861   acsending alpha
+0000d350: 6265 7469 6361 6c20 6f72 6465 720a 2020  betical order.  
+0000d360: 2020 2020 2020 3a72 6169 7365 733a 2053        :raises: S
+0000d370: 3346 696c 654e 6f74 466f 756e 6445 7272  3FileNotFoundErr
+0000d380: 6f72 2c20 5333 4e6f 7441 4469 7265 6374  or, S3NotADirect
+0000d390: 6f72 7945 7272 6f72 0a20 2020 2020 2020  oryError.       
+0000d3a0: 2027 2727 0a20 2020 2020 2020 2065 6e74   '''.        ent
+0000d3b0: 7269 6573 203d 206c 6973 7428 7365 6c66  ries = list(self
+0000d3c0: 2e73 6361 6e64 6972 2866 6f6c 6c6f 776c  .scandir(followl
+0000d3d0: 696e 6b73 3d66 6f6c 6c6f 776c 696e 6b73  inks=followlinks
+0000d3e0: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
+0000d3f0: 6e20 736f 7274 6564 285b 656e 7472 792e  n sorted([entry.
+0000d400: 6e61 6d65 2066 6f72 2065 6e74 7279 2069  name for entry i
+0000d410: 6e20 656e 7472 6965 735d 290a 0a20 2020  n entries])..   
+0000d420: 2064 6566 2069 7465 7264 6972 2873 656c   def iterdir(sel
+0000d430: 662c 2066 6f6c 6c6f 776c 696e 6b73 3a20  f, followlinks: 
+0000d440: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
+0000d450: 2049 7465 7261 746f 725b 2753 3350 6174   Iterator['S3Pat
+0000d460: 6827 5d3a 0a20 2020 2020 2020 2027 2727  h']:.        '''
+0000d470: 0a20 2020 2020 2020 2047 6574 2061 6c6c  .        Get all
+0000d480: 2063 6f6e 7465 6e74 7320 6f66 2067 6976   contents of giv
+0000d490: 656e 2073 335f 7572 6c2e 2054 6865 2072  en s3_url. The r
+0000d4a0: 6573 756c 7420 6973 2069 6e20 6163 7365  esult is in acse
+0000d4b0: 6e64 696e 6720 616c 7068 6162 6574 6963  nding alphabetic
+0000d4c0: 616c 206f 7264 6572 2e0a 0a20 2020 2020  al order...     
+0000d4d0: 2020 203a 7265 7475 726e 733a 2041 6c6c     :returns: All
+0000d4e0: 2063 6f6e 7465 6e74 7320 6861 7665 2070   contents have p
+0000d4f0: 7265 6669 7820 6f66 2073 335f 7572 6c20  refix of s3_url 
+0000d500: 696e 2061 6373 656e 6469 6e67 2061 6c70  in acsending alp
+0000d510: 6861 6265 7469 6361 6c20 6f72 6465 720a  habetical order.
+0000d520: 2020 2020 2020 2020 3a72 6169 7365 733a          :raises:
+0000d530: 2053 3346 696c 654e 6f74 466f 756e 6445   S3FileNotFoundE
+0000d540: 7272 6f72 2c20 5333 4e6f 7441 4469 7265  rror, S3NotADire
+0000d550: 6374 6f72 7945 7272 6f72 0a20 2020 2020  ctoryError.     
+0000d560: 2020 2027 2727 0a20 2020 2020 2020 2066     '''.        f
+0000d570: 6f72 2070 6174 6820 696e 2073 656c 662e  or path in self.
+0000d580: 6c69 7374 6469 7228 666f 6c6c 6f77 6c69  listdir(followli
+0000d590: 6e6b 733d 666f 6c6c 6f77 6c69 6e6b 7329  nks=followlinks)
+0000d5a0: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
+0000d5b0: 656c 6420 7365 6c66 2e6a 6f69 6e70 6174  eld self.joinpat
+0000d5c0: 6828 7061 7468 2920 2023 2074 7970 653a  h(path)  # type:
+0000d5d0: 2069 676e 6f72 650a 0a20 2020 2064 6566   ignore..    def
+0000d5e0: 206c 6f61 6428 7365 6c66 2c20 666f 6c6c   load(self, foll
+0000d5f0: 6f77 6c69 6e6b 733a 2062 6f6f 6c20 3d20  owlinks: bool = 
+0000d600: 4661 6c73 6529 202d 3e20 4269 6e61 7279  False) -> Binary
+0000d610: 494f 3a0a 2020 2020 2020 2020 2727 2752  IO:.        '''R
+0000d620: 6561 6420 616c 6c20 636f 6e74 656e 7420  ead all content 
+0000d630: 696e 2062 696e 6172 7920 6f6e 2073 7065  in binary on spe
+0000d640: 6369 6669 6564 2070 6174 6820 616e 6420  cified path and 
+0000d650: 7772 6974 6520 696e 746f 206d 656d 6f72  write into memor
+0000d660: 790a 0a20 2020 2020 2020 2055 7365 7220  y..        User 
+0000d670: 7368 6f75 6c64 2063 6c6f 7365 2074 6865  should close the
+0000d680: 2042 696e 6172 7949 4f20 6d61 6e75 616c   BinaryIO manual
+0000d690: 6c79 0a0a 2020 2020 2020 2020 3a72 6574  ly..        :ret
+0000d6a0: 7572 6e73 3a20 4269 6e61 7279 494f 0a20  urns: BinaryIO. 
+0000d6b0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000d6c0: 2020 2073 335f 7572 6c20 3d20 7365 6c66     s3_url = self
+0000d6d0: 2e70 6174 685f 7769 7468 5f70 726f 746f  .path_with_proto
+0000d6e0: 636f 6c0a 2020 2020 2020 2020 6966 2066  col.        if f
+0000d6f0: 6f6c 6c6f 776c 696e 6b73 3a0a 2020 2020  ollowlinks:.    
+0000d700: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0000d710: 2020 2020 2020 2020 2020 2020 2073 335f               s3_
+0000d720: 7572 6c20 3d20 7365 6c66 2e72 6561 646c  url = self.readl
+0000d730: 696e 6b28 292e 7061 7468 5f77 6974 685f  ink().path_with_
+0000d740: 7072 6f74 6f63 6f6c 0a20 2020 2020 2020  protocol.       
+0000d750: 2020 2020 2065 7863 6570 7420 5333 4e6f       except S3No
+0000d760: 7441 4c69 6e6b 4572 726f 723a 0a20 2020  tALinkError:.   
+0000d770: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+0000d780: 730a 2020 2020 2020 2020 6275 636b 6574  s.        bucket
+0000d790: 2c20 6b65 7920 3d20 7061 7273 655f 7333  , key = parse_s3
+0000d7a0: 5f75 726c 2873 335f 7572 6c29 0a20 2020  _url(s3_url).   
+0000d7b0: 2020 2020 2069 6620 6e6f 7420 6275 636b       if not buck
+0000d7c0: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+0000d7d0: 7261 6973 6520 5333 4275 636b 6574 4e6f  raise S3BucketNo
+0000d7e0: 7446 6f75 6e64 4572 726f 7228 2745 6d70  tFoundError('Emp
+0000d7f0: 7479 2062 7563 6b65 7420 6e61 6d65 3a20  ty bucket name: 
+0000d800: 2572 2720 2520 7333 5f75 726c 290a 2020  %r' % s3_url).  
+0000d810: 2020 2020 2020 6966 206e 6f74 206b 6579        if not key
+0000d820: 206f 7220 6b65 792e 656e 6473 7769 7468   or key.endswith
+0000d830: 2827 2f27 293a 0a20 2020 2020 2020 2020  ('/'):.         
+0000d840: 2020 2072 6169 7365 2053 3349 7341 4469     raise S3IsADi
+0000d850: 7265 6374 6f72 7945 7272 6f72 2827 4973  rectoryError('Is
+0000d860: 2061 2064 6972 6563 746f 7279 3a20 2572   a directory: %r
+0000d870: 2720 2520 7333 5f75 726c 290a 0a20 2020  ' % s3_url)..   
+0000d880: 2020 2020 2062 7566 6665 7220 3d20 696f       buffer = io
+0000d890: 2e42 7974 6573 494f 2829 0a20 2020 2020  .BytesIO().     
+0000d8a0: 2020 2077 6974 6820 7261 6973 655f 7333     with raise_s3
+0000d8b0: 5f65 7272 6f72 2873 335f 7572 6c29 3a0a  _error(s3_url):.
+0000d8c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d8d0: 2e5f 636c 6965 6e74 2e64 6f77 6e6c 6f61  ._client.downloa
+0000d8e0: 645f 6669 6c65 6f62 6a28 6275 636b 6574  d_fileobj(bucket
+0000d8f0: 2c20 6b65 792c 2062 7566 6665 7229 0a20  , key, buffer). 
+0000d900: 2020 2020 2020 2062 7566 6665 722e 7365         buffer.se
+0000d910: 656b 2830 290a 2020 2020 2020 2020 7265  ek(0).        re
+0000d920: 7475 726e 2062 7566 6665 720a 0a20 2020  turn buffer..   
+0000d930: 2064 6566 2068 6173 6275 636b 6574 2873   def hasbucket(s
+0000d940: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0000d950: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0000d960: 2020 5465 7374 2069 6620 7468 6520 6275    Test if the bu
+0000d970: 636b 6574 206f 6620 7333 5f75 726c 2065  cket of s3_url e
+0000d980: 7869 7374 730a 0a20 2020 2020 2020 203a  xists..        :
+0000d990: 7265 7475 726e 733a 2054 7275 6520 6966  returns: True if
+0000d9a0: 2062 7563 6b65 7420 6f66 2073 335f 7572   bucket of s3_ur
+0000d9b0: 6c20 6569 7873 7473 2c20 656c 7365 2046  l eixsts, else F
+0000d9c0: 616c 7365 0a20 2020 2020 2020 2027 2727  alse.        '''
+0000d9d0: 0a20 2020 2020 2020 2062 7563 6b65 742c  .        bucket,
+0000d9e0: 205f 203d 2070 6172 7365 5f73 335f 7572   _ = parse_s3_ur
+0000d9f0: 6c28 7365 6c66 2e70 6174 685f 7769 7468  l(self.path_with
+0000da00: 5f70 726f 746f 636f 6c29 0a20 2020 2020  _protocol).     
+0000da10: 2020 2069 6620 6e6f 7420 6275 636b 6574     if not bucket
+0000da20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000da30: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+0000da40: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000da50: 2020 2020 2073 656c 662e 5f63 6c69 656e       self._clien
+0000da60: 742e 6865 6164 5f62 7563 6b65 7428 4275  t.head_bucket(Bu
+0000da70: 636b 6574 3d62 7563 6b65 7429 0a20 2020  cket=bucket).   
+0000da80: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0000da90: 7074 696f 6e20 6173 2065 7272 6f72 3a0a  ption as error:.
+0000daa0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+0000dab0: 7220 3d20 7472 616e 736c 6174 655f 7333  r = translate_s3
+0000dac0: 5f65 7272 6f72 2865 7272 6f72 2c20 7365  _error(error, se
+0000dad0: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
+0000dae0: 746f 636f 6c29 0a20 2020 2020 2020 2020  tocol).         
+0000daf0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000db00: 2865 7272 6f72 2c0a 2020 2020 2020 2020  (error,.        
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db20: 2020 2853 3355 6e6b 6e6f 776e 4572 726f    (S3UnknownErro
+0000db30: 722c 2053 3343 6f6e 6669 6745 7272 6f72  r, S3ConfigError
+0000db40: 2c20 5333 5065 726d 6973 7369 6f6e 4572  , S3PermissionEr
+0000db50: 726f 7229 293a 0a20 2020 2020 2020 2020  ror)):.         
+0000db60: 2020 2020 2020 2072 6169 7365 2065 7272         raise err
+0000db70: 6f72 0a20 2020 2020 2020 2020 2020 2069  or.            i
+0000db80: 6620 6973 696e 7374 616e 6365 2865 7272  f isinstance(err
+0000db90: 6f72 2c20 5333 4669 6c65 4e6f 7446 6f75  or, S3FileNotFou
+0000dba0: 6e64 4572 726f 7229 3a0a 2020 2020 2020  ndError):.      
+0000dbb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000dbc0: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+0000dbd0: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+0000dbe0: 2064 6566 206d 6b64 6972 2873 656c 662c   def mkdir(self,
+0000dbf0: 206d 6f64 653d 306f 3737 372c 2070 6172   mode=0o777, par
+0000dc00: 656e 7473 3a20 626f 6f6c 203d 2046 616c  ents: bool = Fal
+0000dc10: 7365 2c20 6578 6973 745f 6f6b 3a20 626f  se, exist_ok: bo
+0000dc20: 6f6c 203d 2046 616c 7365 293a 0a20 2020  ol = False):.   
+0000dc30: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0000dc40: 2043 7265 6174 6520 616e 2073 3320 6469   Create an s3 di
+0000dc50: 7265 6374 6f72 792e 0a20 2020 2020 2020  rectory..       
+0000dc60: 2050 7572 656c 7920 6372 6561 7469 6e67   Purely creating
+0000dc70: 2064 6972 6563 746f 7279 2069 7320 696e   directory is in
+0000dc80: 7661 6c69 6420 6265 6361 7573 6520 6974  valid because it
+0000dc90: 2773 2075 6e61 7661 696c 6162 6c65 206f  's unavailable o
+0000dca0: 6e20 4f53 532e 0a20 2020 2020 2020 2054  n OSS..        T
+0000dcb0: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
+0000dcc0: 746f 2074 6573 7420 7468 6520 7461 7267  to test the targ
+0000dcd0: 6574 2062 7563 6b65 7420 6861 7665 2057  et bucket have W
+0000dce0: 5249 5445 2061 6363 6573 732e 0a0a 2020  RITE access...  
+0000dcf0: 2020 2020 2020 3a70 6172 616d 206d 6f64        :param mod
+0000dd00: 653a 206d 6f64 6520 6973 2069 676e 6f72  e: mode is ignor
+0000dd10: 6564 2c20 6f6e 6c79 2062 6520 636f 6d70  ed, only be comp
+0000dd20: 6174 6962 6c65 2077 6974 6820 7061 7468  atible with path
+0000dd30: 6c69 622e 5061 7468 0a20 2020 2020 2020  lib.Path.       
+0000dd40: 203a 7061 7261 6d20 7061 7265 6e74 733a   :param parents:
+0000dd50: 2070 6172 656e 7473 2069 7320 6967 6e6f   parents is igno
+0000dd60: 7265 642c 206f 6e6c 7920 6265 2063 6f6d  red, only be com
+0000dd70: 7061 7469 626c 6520 7769 7468 2070 6174  patible with pat
+0000dd80: 686c 6962 2e50 6174 680a 2020 2020 2020  hlib.Path.      
+0000dd90: 2020 3a70 6172 616d 2065 7869 7374 5f6f    :param exist_o
+0000dda0: 6b3a 2049 6620 4661 6c73 6520 616e 6420  k: If False and 
+0000ddb0: 7461 7267 6574 2064 6972 6563 746f 7279  target directory
+0000ddc0: 2065 7869 7374 732c 2072 6169 7365 2053   exists, raise S
+0000ddd0: 3346 696c 6545 7869 7374 7345 7272 6f72  3FileExistsError
+0000dde0: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+0000ddf0: 3a20 5333 4275 636b 6574 4e6f 7446 6f75  : S3BucketNotFou
+0000de00: 6e64 4572 726f 722c 2053 3346 696c 6545  ndError, S3FileE
+0000de10: 7869 7374 7345 7272 6f72 0a20 2020 2020  xistsError.     
+0000de20: 2020 2027 2727 0a20 2020 2020 2020 2062     '''.        b
+0000de30: 7563 6b65 742c 205f 203d 2070 6172 7365  ucket, _ = parse
+0000de40: 5f73 335f 7572 6c28 7365 6c66 2e70 6174  _s3_url(self.pat
+0000de50: 685f 7769 7468 5f70 726f 746f 636f 6c29  h_with_protocol)
+0000de60: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000de70: 6275 636b 6574 3a0a 2020 2020 2020 2020  bucket:.        
+0000de80: 2020 2020 7261 6973 6520 5333 4275 636b      raise S3Buck
+0000de90: 6574 4e6f 7446 6f75 6e64 4572 726f 7228  etNotFoundError(
+0000dea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000deb0: 2027 456d 7074 7920 6275 636b 6574 206e   'Empty bucket n
+0000dec0: 616d 653a 2025 7227 2025 2073 656c 662e  ame: %r' % self.
+0000ded0: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
+0000dee0: 6f6c 290a 2020 2020 2020 2020 6966 206e  ol).        if n
+0000def0: 6f74 2073 656c 662e 6861 7362 7563 6b65  ot self.hasbucke
+0000df00: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000df10: 2072 6169 7365 2053 3342 7563 6b65 744e   raise S3BucketN
+0000df20: 6f74 466f 756e 6445 7272 6f72 280a 2020  otFoundError(.  
+0000df30: 2020 2020 2020 2020 2020 2020 2020 274e                'N
+0000df40: 6f20 7375 6368 2062 7563 6b65 743a 2025  o such bucket: %
+0000df50: 7227 2025 2073 656c 662e 7061 7468 5f77  r' % self.path_w
+0000df60: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
+0000df70: 2020 2020 2020 6966 2065 7869 7374 5f6f        if exist_o
+0000df80: 6b3a 0a20 2020 2020 2020 2020 2020 2069  k:.            i
+0000df90: 6620 7365 6c66 2e69 735f 6669 6c65 2829  f self.is_file()
+0000dfa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000dfb0: 2020 7261 6973 6520 5333 4669 6c65 4578    raise S3FileEx
+0000dfc0: 6973 7473 4572 726f 7228 0a20 2020 2020  istsError(.     
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000dfe0: 4669 6c65 2065 7869 7374 733a 2025 7227  File exists: %r'
+0000dff0: 2025 2073 656c 662e 7061 7468 5f77 6974   % self.path_wit
+0000e000: 685f 7072 6f74 6f63 6f6c 290a 2020 2020  h_protocol).    
+0000e010: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000e020: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+0000e030: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
+0000e040: 2020 2020 2072 6169 7365 2053 3346 696c       raise S3Fil
+0000e050: 6545 7869 7374 7345 7272 6f72 2827 4669  eExistsError('Fi
+0000e060: 6c65 2065 7869 7374 733a 2025 7227 2025  le exists: %r' %
+0000e070: 2073 656c 662e 7061 7468 5f77 6974 685f   self.path_with_
+0000e080: 7072 6f74 6f63 6f6c 290a 0a20 2020 2064  protocol)..    d
+0000e090: 6566 206d 6f76 6528 7365 6c66 2c20 6473  ef move(self, ds
+0000e0a0: 745f 7572 6c3a 2050 6174 684c 696b 6529  t_url: PathLike)
+0000e0b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000e0c0: 2020 2727 270a 2020 2020 2020 2020 4d6f    '''.        Mo
+0000e0d0: 7665 2066 696c 652f 6469 7265 6374 6f72  ve file/director
+0000e0e0: 7920 7061 7468 2066 726f 6d20 7372 635f  y path from src_
+0000e0f0: 7572 6c20 746f 2064 7374 5f75 726c 0a0a  url to dst_url..
+0000e100: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+0000e110: 7374 5f75 726c 3a20 4769 7665 6e20 6465  st_url: Given de
+0000e120: 7374 696e 6174 696f 6e20 7061 7468 0a20  stination path. 
+0000e130: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000e140: 2020 2066 6f72 2073 7263 5f66 696c 655f     for src_file_
+0000e150: 7061 7468 2c20 6473 745f 6669 6c65 5f70  path, dst_file_p
+0000e160: 6174 6820 696e 205f 7333 5f73 6361 6e5f  ath in _s3_scan_
+0000e170: 7061 6972 7328 0a20 2020 2020 2020 2020  pairs(.         
+0000e180: 2020 2020 2020 2073 656c 662e 7061 7468         self.path
+0000e190: 5f77 6974 685f 7072 6f74 6f63 6f6c 2c20  _with_protocol, 
+0000e1a0: 6473 745f 7572 6c29 3a0a 2020 2020 2020  dst_url):.      
+0000e1b0: 2020 2020 2020 5333 5061 7468 2873 7263        S3Path(src
+0000e1c0: 5f66 696c 655f 7061 7468 292e 7265 6e61  _file_path).rena
+0000e1d0: 6d65 2864 7374 5f66 696c 655f 7061 7468  me(dst_file_path
+0000e1e0: 290a 0a20 2020 2064 6566 2072 656d 6f76  )..    def remov
+0000e1f0: 6528 7365 6c66 2c20 6d69 7373 696e 675f  e(self, missing_
+0000e200: 6f6b 3a20 626f 6f6c 203d 2046 616c 7365  ok: bool = False
+0000e210: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000e220: 2020 2027 2727 0a20 2020 2020 2020 2052     '''.        R
+0000e230: 656d 6f76 6520 7468 6520 6669 6c65 206f  emove the file o
+0000e240: 7220 6469 7265 6374 6f72 7920 6f6e 2073  r directory on s
+0000e250: 332c 2060 7333 3a2f 2f60 2061 6e64 2060  3, `s3://` and `
+0000e260: 7333 3a2f 2f62 7563 6b65 7460 2061 7265  s3://bucket` are
+0000e270: 206e 6f74 2070 6572 6d69 7474 6564 2074   not permitted t
+0000e280: 6f20 7265 6d6f 7665 0a0a 2020 2020 2020  o remove..      
+0000e290: 2020 3a70 6172 616d 206d 6973 7369 6e67    :param missing
+0000e2a0: 5f6f 6b3a 2069 6620 4661 6c73 6520 616e  _ok: if False an
+0000e2b0: 6420 7461 7267 6574 2066 696c 652f 6469  d target file/di
+0000e2c0: 7265 6374 6f72 7920 6e6f 7420 6578 6973  rectory not exis
+0000e2d0: 7473 2c20 7261 6973 6520 5333 4669 6c65  ts, raise S3File
+0000e2e0: 4e6f 7446 6f75 6e64 4572 726f 720a 2020  NotFoundError.  
+0000e2f0: 2020 2020 2020 3a72 6169 7365 733a 2053        :raises: S
+0000e300: 3350 6572 6d69 7373 696f 6e45 7272 6f72  3PermissionError
+0000e310: 2c20 5333 4669 6c65 4e6f 7446 6f75 6e64  , S3FileNotFound
+0000e320: 4572 726f 722c 2055 6e73 7570 706f 7274  Error, Unsupport
+0000e330: 6564 4572 726f 720a 2020 2020 2020 2020  edError.        
+0000e340: 2727 270a 2020 2020 2020 2020 6275 636b  '''.        buck
+0000e350: 6574 2c20 6b65 7920 3d20 7061 7273 655f  et, key = parse_
+0000e360: 7333 5f75 726c 2873 656c 662e 7061 7468  s3_url(self.path
+0000e370: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
+0000e380: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
+0000e390: 7563 6b65 743a 0a20 2020 2020 2020 2020  ucket:.         
+0000e3a0: 2020 2069 6620 6e6f 7420 6b65 793a 0a20     if not key:. 
+0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000e3c0: 6169 7365 2055 6e73 7570 706f 7274 6564  aise Unsupported
+0000e3d0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000e3e0: 2020 2020 2020 2020 2020 2027 5265 6d6f             'Remo
+0000e3f0: 7665 2077 686f 6c65 2073 3327 2c20 7365  ve whole s3', se
+0000e400: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
+0000e410: 746f 636f 6c29 0a20 2020 2020 2020 2020  tocol).         
+0000e420: 2020 2072 6169 7365 2053 3342 7563 6b65     raise S3Bucke
+0000e430: 744e 6f74 466f 756e 6445 7272 6f72 280a  tNotFoundError(.
+0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e450: 2745 6d70 7479 2062 7563 6b65 7420 6e61  'Empty bucket na
+0000e460: 6d65 3a20 2572 2720 2520 7365 6c66 2e70  me: %r' % self.p
+0000e470: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
+0000e480: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
+0000e490: 7420 6b65 793a 0a20 2020 2020 2020 2020  t key:.         
+0000e4a0: 2020 2072 6169 7365 2055 6e73 7570 706f     raise Unsuppo
+0000e4b0: 7274 6564 4572 726f 7228 2752 656d 6f76  rtedError('Remov
+0000e4c0: 6520 6275 636b 6574 272c 2073 656c 662e  e bucket', self.
+0000e4d0: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
+0000e4e0: 6f6c 290a 2020 2020 2020 2020 6966 206e  ol).        if n
+0000e4f0: 6f74 2073 656c 662e 6578 6973 7473 2829  ot self.exists()
+0000e500: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000e510: 206d 6973 7369 6e67 5f6f 6b3a 0a20 2020   missing_ok:.   
+0000e520: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000e530: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+0000e540: 7261 6973 6520 5333 4669 6c65 4e6f 7446  raise S3FileNotF
+0000e550: 6f75 6e64 4572 726f 7228 0a20 2020 2020  oundError(.     
+0000e560: 2020 2020 2020 2020 2020 2027 4e6f 2073             'No s
+0000e570: 7563 6820 6669 6c65 206f 7220 6469 7265  uch file or dire
+0000e580: 6374 6f72 793a 2025 7227 2025 2073 656c  ctory: %r' % sel
+0000e590: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
+0000e5a0: 6f63 6f6c 290a 0a20 2020 2020 2020 2063  ocol)..        c
+0000e5b0: 6c69 656e 7420 3d20 7365 6c66 2e5f 636c  lient = self._cl
+0000e5c0: 6965 6e74 0a20 2020 2020 2020 2077 6974  ient.        wit
+0000e5d0: 6820 7261 6973 655f 7333 5f65 7272 6f72  h raise_s3_error
+0000e5e0: 2873 656c 662e 7061 7468 5f77 6974 685f  (self.path_with_
+0000e5f0: 7072 6f74 6f63 6f6c 293a 0a20 2020 2020  protocol):.     
+0000e600: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+0000e610: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
+0000e620: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+0000e630: 2e64 656c 6574 655f 6f62 6a65 6374 2842  .delete_object(B
+0000e640: 7563 6b65 743d 6275 636b 6574 2c20 4b65  ucket=bucket, Ke
+0000e650: 793d 6b65 7929 0a20 2020 2020 2020 2020  y=key).         
+0000e660: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000e670: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
+0000e680: 203d 205f 6265 636f 6d65 5f70 7265 6669   = _become_prefi
+0000e690: 7828 6b65 7929 0a20 2020 2020 2020 2020  x(key).         
+0000e6a0: 2020 2074 6f74 616c 5f63 6f75 6e74 2c20     total_count, 
+0000e6b0: 6572 726f 725f 636f 756e 7420 3d20 302c  error_count = 0,
+0000e6c0: 2030 0a20 2020 2020 2020 2020 2020 2066   0.            f
+0000e6d0: 6f72 2072 6573 7020 696e 205f 6c69 7374  or resp in _list
+0000e6e0: 5f6f 626a 6563 7473 5f72 6563 7572 7369  _objects_recursi
+0000e6f0: 7665 2863 6c69 656e 742c 2062 7563 6b65  ve(client, bucke
+0000e700: 742c 2070 7265 6669 7829 3a0a 2020 2020  t, prefix):.    
+0000e710: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+0000e720: 436f 6e74 656e 7473 2720 696e 2072 6573  Contents' in res
+0000e730: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+0000e740: 2020 2020 2020 206b 6579 7320 3d20 5b0a         keys = [.
+0000e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e760: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e780: 2020 2020 2020 274b 6579 273a 2063 6f6e        'Key': con
+0000e790: 7465 6e74 5b27 4b65 7927 5d0a 2020 2020  tent['Key'].    
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7b0: 2020 2020 7d20 666f 7220 636f 6e74 656e      } for conten
+0000e7c0: 7420 696e 2072 6573 705b 2743 6f6e 7465  t in resp['Conte
+0000e7d0: 6e74 7327 5d0a 2020 2020 2020 2020 2020  nts'].          
+0000e7e0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e800: 746f 7461 6c5f 636f 756e 7420 2b3d 206c  total_count += l
+0000e810: 656e 286b 6579 7329 0a20 2020 2020 2020  en(keys).       
+0000e820: 2020 2020 2020 2020 2020 2020 2065 7272               err
+0000e830: 6f72 7320 3d20 5b5d 0a20 2020 2020 2020  ors = [].       
+0000e840: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000e850: 7269 6573 203d 2032 0a20 2020 2020 2020  ries = 2.       
+0000e860: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000e870: 7279 5f69 6e74 6572 7661 6c20 3d20 6d69  ry_interval = mi
+0000e880: 6e28 302e 3120 2a20 322a 2a72 6574 7269  n(0.1 * 2**retri
+0000e890: 6573 2c20 3330 290a 2020 2020 2020 2020  es, 30).        
+0000e8a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000e8b0: 6920 696e 2072 616e 6765 2872 6574 7269  i in range(retri
+0000e8c0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+0000e8d0: 2020 2020 2020 2020 2020 2020 2023 2064               # d
+0000e8e0: 6f63 3a20 6874 7470 733a 2f2f 626f 746f  oc: https://boto
+0000e8f0: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
+0000e900: 7631 2f64 6f63 756d 656e 7461 7469 6f6e  v1/documentation
+0000e910: 2f61 7069 2f6c 6174 6573 742f 7265 6665  /api/latest/refe
+0000e920: 7265 6e63 652f 7365 7276 6963 6573 2f73  rence/services/s
+0000e930: 332e 6874 6d6c 2353 332e 436c 6965 6e74  3.html#S3.Client
+0000e940: 2e64 656c 6574 655f 6f62 6a65 6374 730a  .delete_objects.
+0000e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e960: 2020 2020 2020 2020 6966 206e 6f74 206b          if not k
+0000e970: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e990: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000e9b0: 6573 706f 6e73 6520 3d20 636c 6965 6e74  esponse = client
+0000e9c0: 2e64 656c 6574 655f 6f62 6a65 6374 7328  .delete_objects(
+0000e9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e9e0: 2020 2020 2020 2020 2020 2020 2042 7563               Buc
+0000e9f0: 6b65 743d 6275 636b 6574 2c20 4465 6c65  ket=bucket, Dele
+0000ea00: 7465 3d7b 274f 626a 6563 7473 273a 206b  te={'Objects': k
+0000ea10: 6579 737d 290a 2020 2020 2020 2020 2020  eys}).          
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
+0000ea30: 7973 203d 205b 5d0a 2020 2020 2020 2020  ys = [].        
 0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea70: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0000ea80: 3d20 636c 6965 6e74 2e64 656c 6574 655f  = client.delete_
-0000ea90: 6f62 6a65 6374 7328 0a20 2020 2020 2020  objects(.       
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2020 2020 2042 7563 6b65 743d 6275 636b       Bucket=buck
-0000eac0: 6574 2c20 4465 6c65 7465 3d7b 274f 626a  et, Delete={'Obj
-0000ead0: 6563 7473 273a 206b 6579 737d 290a 2020  ects': keys}).  
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 2020 2020 2020 6b65 7973 203d 205b 5d0a        keys = [].
+0000ea50: 666f 7220 6572 726f 725f 696e 666f 2069  for error_info i
+0000ea60: 6e20 7265 7370 6f6e 7365 2e67 6574 2827  n response.get('
+0000ea70: 4572 726f 7273 272c 205b 5d29 3a0a 2020  Errors', []):.  
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea90: 2020 2020 2020 2020 2020 6966 2073 335f            if s3_
+0000eaa0: 6572 726f 725f 636f 6465 5f73 686f 756c  error_code_shoul
+0000eab0: 645f 7265 7472 7928 0a20 2020 2020 2020  d_retry(.       
+0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ead0: 2020 2020 2020 2020 2020 2020 2065 7272               err
+0000eae0: 6f72 5f69 6e66 6f2e 6765 7428 2743 6f64  or_info.get('Cod
+0000eaf0: 6527 2929 3a0a 2020 2020 2020 2020 2020  e')):.          
 0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 2020 2020 2020 666f 7220 6572 726f          for erro
-0000eb20: 725f 696e 666f 2069 6e20 7265 7370 6f6e  r_info in respon
-0000eb30: 7365 2e67 6574 2827 4572 726f 7273 272c  se.get('Errors',
-0000eb40: 205b 5d29 3a0a 2020 2020 2020 2020 2020   []):.          
-0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb60: 2020 6966 2073 335f 6572 726f 725f 636f    if s3_error_co
-0000eb70: 6465 5f73 686f 756c 645f 7265 7472 7928  de_should_retry(
-0000eb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb10: 2020 2020 2020 6572 726f 725f 6c6f 6767        error_logg
+0000eb20: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
+0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb50: 2272 6574 7279 2025 7320 7469 6d65 732c  "retry %s times,
+0000eb60: 2072 656d 6f76 696e 6720 6669 6c65 3a20   removing file: 
+0000eb70: 2573 2c20 7769 7468 2065 7272 6f72 2025  %s, with error %
+0000eb80: 733a 2025 7322 0a20 2020 2020 2020 2020  s: %s".         
 0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eba0: 2020 2020 2065 7272 6f72 5f69 6e66 6f2e       error_info.
-0000ebb0: 6765 7428 2743 6f64 6527 2929 3a0a 2020  get('Code')):.  
+0000eba0: 2020 2020 2020 2020 2020 2025 2028 0a20             % (. 
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebd0: 2020 2020 2020 2020 2020 2020 2020 6572                er
-0000ebe0: 726f 725f 6c6f 6767 6572 2e77 6172 6e69  ror_logger.warni
-0000ebf0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000ebd0: 2020 2020 2020 2069 202b 2031 2c20 6572         i + 1, er
+0000ebe0: 726f 725f 696e 666f 5b27 4b65 7927 5d2c  ror_info['Key'],
+0000ebf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec10: 2020 2020 2020 2020 2272 6574 7279 2025          "retry %
-0000ec20: 7320 7469 6d65 732c 2072 656d 6f76 696e  s times, removin
-0000ec30: 6720 6669 6c65 3a20 2573 2c20 7769 7468  g file: %s, with
-0000ec40: 2065 7272 6f72 2025 733a 2025 7322 0a20   error %s: %s". 
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec70: 2020 2025 2028 0a20 2020 2020 2020 2020     % (.         
-0000ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000eca0: 202b 2031 2c20 6572 726f 725f 696e 666f   + 1, error_info
-0000ecb0: 5b27 4b65 7927 5d2c 0a20 2020 2020 2020  ['Key'],.       
+0000ec10: 2020 2020 2020 2020 2065 7272 6f72 5f69           error_i
+0000ec20: 6e66 6f5b 2743 6f64 6527 5d2c 0a20 2020  nfo['Code'],.   
+0000ec30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec50: 2020 2020 2065 7272 6f72 5f69 6e66 6f5b       error_info[
+0000ec60: 274d 6573 7361 6765 275d 2929 0a20 2020  'Message'])).   
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec80: 2020 2020 2020 2020 2020 2020 206b 6579               key
+0000ec90: 732e 6170 7065 6e64 287b 274b 6579 273a  s.append({'Key':
+0000eca0: 2065 7272 6f72 5f69 6e66 6f5b 274b 6579   error_info['Key
+0000ecb0: 275d 7d29 0a20 2020 2020 2020 2020 2020  ']}).           
 0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 2065 7272 6f72 5f69 6e66 6f5b 2743 6f64   error_info['Cod
-0000ecf0: 6527 5d2c 0a20 2020 2020 2020 2020 2020  e'],.           
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed10: 2020 2020 2020 2020 2020 2020 2065 7272               err
-0000ed20: 6f72 5f69 6e66 6f5b 274d 6573 7361 6765  or_info['Message
-0000ed30: 275d 2929 0a20 2020 2020 2020 2020 2020  '])).           
-0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed50: 2020 2020 206b 6579 732e 6170 7065 6e64       keys.append
-0000ed60: 287b 274b 6579 273a 2065 7272 6f72 5f69  ({'Key': error_i
-0000ed70: 6e66 6f5b 274b 6579 275d 7d29 0a20 2020  nfo['Key']}).   
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000ecd0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecf0: 2020 2020 2020 2065 7272 6f72 732e 6170         errors.ap
+0000ed00: 7065 6e64 2865 7272 6f72 5f69 6e66 6f29  pend(error_info)
+0000ed10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ed20: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
+0000ed30: 6565 7028 7265 7472 795f 696e 7465 7276  eep(retry_interv
+0000ed40: 616c 290a 2020 2020 2020 2020 2020 2020  al).            
+0000ed50: 2020 2020 2020 2020 666f 7220 6572 726f          for erro
+0000ed60: 725f 696e 666f 2069 6e20 6572 726f 7273  r_info in errors
+0000ed70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ed80: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+0000ed90: 6c6f 6767 6572 2e65 7272 6f72 280a 2020  logger.error(.  
 0000eda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000edc0: 7272 6f72 732e 6170 7065 6e64 2865 7272  rrors.append(err
-0000edd0: 6f72 5f69 6e66 6f29 0a20 2020 2020 2020  or_info).       
-0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edf0: 2074 696d 652e 736c 6565 7028 7265 7472   time.sleep(retr
-0000ee00: 795f 696e 7465 7276 616c 290a 2020 2020  y_interval).    
-0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee20: 666f 7220 6572 726f 725f 696e 666f 2069  for error_info i
-0000ee30: 6e20 6572 726f 7273 3a0a 2020 2020 2020  n errors:.      
+0000edb0: 2020 2020 2020 2020 2020 2266 6169 6c65            "faile
+0000edc0: 6420 7265 6d6f 7665 2066 696c 653a 2025  d remove file: %
+0000edd0: 732c 2077 6974 6820 6572 726f 7220 2573  s, with error %s
+0000ede0: 3a20 2573 2220 2520 280a 2020 2020 2020  : %s" % (.      
+0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee00: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+0000ee10: 696e 666f 5b27 4b65 7927 5d2c 2065 7272  info['Key'], err
+0000ee20: 6f72 5f69 6e66 6f5b 2743 6f64 6527 5d2c  or_info['Code'],
+0000ee30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 2020 6572 726f 725f 6c6f 6767 6572 2e65    error_logger.e
-0000ee60: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee80: 2020 2266 6169 6c65 6420 7265 6d6f 7665    "failed remove
-0000ee90: 2066 696c 653a 2025 732c 2077 6974 6820   file: %s, with 
-0000eea0: 6572 726f 7220 2573 3a20 2573 2220 2520  error %s: %s" % 
-0000eeb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eed0: 2020 6572 726f 725f 696e 666f 5b27 4b65    error_info['Ke
-0000eee0: 7927 5d2c 2065 7272 6f72 5f69 6e66 6f5b  y'], error_info[
-0000eef0: 2743 6f64 6527 5d2c 0a20 2020 2020 2020  'Code'],.       
-0000ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef10: 2020 2020 2020 2020 2065 7272 6f72 5f69           error_i
-0000ef20: 6e66 6f5b 274d 6573 7361 6765 275d 2929  nfo['Message']))
-0000ef30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ef40: 2020 2020 2065 7272 6f72 5f63 6f75 6e74       error_count
-0000ef50: 202b 3d20 6c65 6e28 6572 726f 7273 290a   += len(errors).
-0000ef60: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-0000ef70: 7272 6f72 5f63 6f75 6e74 203e 2030 3a0a  rror_count > 0:.
-0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef90: 6572 726f 725f 6d73 6720 3d20 2266 6169  error_msg = "fai
-0000efa0: 6c65 6420 7265 6d6f 7665 2070 6174 683a  led remove path:
-0000efb0: 2025 732c 2074 6f74 616c 2066 696c 6520   %s, total file 
-0000efc0: 636f 756e 743a 2025 732c 2066 6169 6c65  count: %s, faile
-0000efd0: 6420 636f 756e 743a 2025 7322 2025 2028  d count: %s" % (
-0000efe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eff0: 2020 2020 2073 656c 662e 7061 7468 5f77       self.path_w
-0000f000: 6974 685f 7072 6f74 6f63 6f6c 2c20 746f  ith_protocol, to
-0000f010: 7461 6c5f 636f 756e 742c 2065 7272 6f72  tal_count, error
-0000f020: 5f63 6f75 6e74 290a 2020 2020 2020 2020  _count).        
-0000f030: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
-0000f040: 556e 6b6e 6f77 6e45 7272 6f72 280a 2020  UnknownError(.  
-0000f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f060: 2020 4578 6365 7074 696f 6e28 6572 726f    Exception(erro
-0000f070: 725f 6d73 6729 2c20 7365 6c66 2e70 6174  r_msg), self.pat
-0000f080: 685f 7769 7468 5f70 726f 746f 636f 6c29  h_with_protocol)
-0000f090: 0a0a 2020 2020 6465 6620 7265 6e61 6d65  ..    def rename
-0000f0a0: 2873 656c 662c 2064 7374 5f70 6174 683a  (self, dst_path:
-0000f0b0: 2050 6174 684c 696b 6529 202d 3e20 2753   PathLike) -> 'S
-0000f0c0: 3350 6174 6827 3a0a 2020 2020 2020 2020  3Path':.        
-0000f0d0: 2727 270a 2020 2020 2020 2020 4d6f 7665  '''.        Move
-0000f0e0: 2073 3320 6669 6c65 2070 6174 6820 6672   s3 file path fr
-0000f0f0: 6f6d 2073 7263 5f75 726c 2074 6f20 6473  om src_url to ds
-0000f100: 745f 7572 6c0a 0a20 2020 2020 2020 203a  t_url..        :
-0000f110: 7061 7261 6d20 6473 745f 7061 7468 3a20  param dst_path: 
-0000f120: 4769 7665 6e20 6465 7374 696e 6174 696f  Given destinatio
-0000f130: 6e20 7061 7468 0a20 2020 2020 2020 2027  n path.        '
-0000f140: 2727 0a20 2020 2020 2020 2073 335f 7265  ''.        s3_re
-0000f150: 6e61 6d65 2873 656c 662e 7061 7468 5f77  name(self.path_w
-0000f160: 6974 685f 7072 6f74 6f63 6f6c 2c20 6473  ith_protocol, ds
-0000f170: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
-0000f180: 7265 7475 726e 2073 656c 662e 6672 6f6d  return self.from
-0000f190: 5f70 6174 6828 6473 745f 7061 7468 290a  _path(dst_path).
-0000f1a0: 0a20 2020 2064 6566 2073 6361 6e28 7365  .    def scan(se
-0000f1b0: 6c66 2c20 6d69 7373 696e 675f 6f6b 3a20  lf, missing_ok: 
-0000f1c0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-0000f1d0: 2020 2020 2020 2020 2020 666f 6c6c 6f77            follow
-0000f1e0: 6c69 6e6b 733a 2062 6f6f 6c20 3d20 4661  links: bool = Fa
-0000f1f0: 6c73 6529 202d 3e20 4974 6572 6174 6f72  lse) -> Iterator
-0000f200: 5b73 7472 5d3a 0a20 2020 2020 2020 2027  [str]:.        '
-0000f210: 2727 0a20 2020 2020 2020 2049 7465 7261  ''.        Itera
-0000f220: 7469 7665 6c79 2074 7261 7665 7273 6520  tively traverse 
-0000f230: 6f6e 6c79 2066 696c 6573 2069 6e20 6769  only files in gi
-0000f240: 7665 6e20 7333 2064 6972 6563 746f 7279  ven s3 directory
-0000f250: 2c20 696e 2061 6c70 6861 6265 7469 6361  , in alphabetica
-0000f260: 6c20 6f72 6465 722e 0a20 2020 2020 2020  l order..       
-0000f270: 2045 7665 7279 2069 7465 7261 7469 6f6e   Every iteration
-0000f280: 206f 6e20 6765 6e65 7261 746f 7220 7969   on generator yi
-0000f290: 656c 6473 2061 2070 6174 6820 7374 7269  elds a path stri
-0000f2a0: 6e67 2e0a 0a20 2020 2020 2020 2049 6620  ng...        If 
-0000f2b0: 7333 5f75 726c 2069 7320 6120 6669 6c65  s3_url is a file
-0000f2c0: 2070 6174 682c 2079 6965 6c64 7320 7468   path, yields th
-0000f2d0: 6520 6669 6c65 206f 6e6c 790a 2020 2020  e file only.    
-0000f2e0: 2020 2020 4966 2073 335f 7572 6c20 6973      If s3_url is
-0000f2f0: 2061 206e 6f6e 2d65 7869 7374 656e 7420   a non-existent 
-0000f300: 7061 7468 2c20 7265 7475 726e 2061 6e20  path, return an 
-0000f310: 656d 7074 7920 6765 6e65 7261 746f 720a  empty generator.
-0000f320: 2020 2020 2020 2020 4966 2073 335f 7572          If s3_ur
-0000f330: 6c20 6973 2061 2062 7563 6b65 7420 7061  l is a bucket pa
-0000f340: 7468 2c20 7265 7475 726e 2061 6c6c 2066  th, return all f
-0000f350: 696c 6520 7061 7468 7320 696e 2074 6865  ile paths in the
-0000f360: 2062 7563 6b65 740a 2020 2020 2020 2020   bucket.        
-0000f370: 4966 2073 335f 7572 6c20 6973 2061 6e20  If s3_url is an 
-0000f380: 656d 7074 7920 6275 636b 6574 2c20 7265  empty bucket, re
-0000f390: 7475 726e 2061 6e20 656d 7074 7920 6765  turn an empty ge
-0000f3a0: 6e65 7261 746f 720a 2020 2020 2020 2020  nerator.        
-0000f3b0: 4966 2073 335f 7572 6c20 646f 6573 6e27  If s3_url doesn'
-0000f3c0: 7420 636f 6e74 6169 6e20 616e 7920 6275  t contain any bu
-0000f3d0: 636b 6574 2c20 7768 6963 6820 6973 2073  cket, which is s
-0000f3e0: 335f 7572 6c20 3d3d 2027 7333 3a2f 2f27  3_url == 's3://'
-0000f3f0: 2c20 7261 6973 6520 556e 7375 7070 6f72  , raise Unsuppor
-0000f400: 7465 6445 7272 6f72 2e20 7761 6c6b 2829  tedError. walk()
-0000f410: 206f 6e20 636f 6d70 6c65 7465 2073 3320   on complete s3 
-0000f420: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-0000f430: 2069 6e20 6d65 6766 696c 650a 0a20 2020   in megfile..   
-0000f440: 2020 2020 203a 7061 7261 6d20 6d69 7373       :param miss
-0000f450: 696e 675f 6f6b 3a20 4966 2046 616c 7365  ing_ok: If False
-0000f460: 2061 6e64 2074 6865 7265 2773 206e 6f20   and there's no 
-0000f470: 6669 6c65 2069 6e20 7468 6520 6469 7265  file in the dire
-0000f480: 6374 6f72 792c 2072 6169 7365 2046 696c  ctory, raise Fil
-0000f490: 654e 6f74 466f 756e 6445 7272 6f72 0a20  eNotFoundError. 
-0000f4a0: 2020 2020 2020 203a 7261 6973 6573 3a20         :raises: 
-0000f4b0: 556e 7375 7070 6f72 7465 6445 7272 6f72  UnsupportedError
-0000f4c0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0000f4d0: 733a 2041 2066 696c 6520 7061 7468 2067  s: A file path g
-0000f4e0: 656e 6572 6174 6f72 0a20 2020 2020 2020  enerator.       
-0000f4f0: 2027 2727 0a20 2020 2020 2020 2073 6361   '''.        sca
-0000f500: 6e5f 7374 6174 5f69 7465 7220 3d20 7365  n_stat_iter = se
-0000f510: 6c66 2e73 6361 6e5f 7374 6174 280a 2020  lf.scan_stat(.  
-0000f520: 2020 2020 2020 2020 2020 6d69 7373 696e            missin
-0000f530: 675f 6f6b 3d6d 6973 7369 6e67 5f6f 6b2c  g_ok=missing_ok,
-0000f540: 2066 6f6c 6c6f 776c 696e 6b73 3d66 6f6c   followlinks=fol
-0000f550: 6c6f 776c 696e 6b73 290a 0a20 2020 2020  lowlinks)..     
-0000f560: 2020 2064 6566 2063 7265 6174 655f 6765     def create_ge
-0000f570: 6e65 7261 746f 7228 2920 2d3e 2049 7465  nerator() -> Ite
-0000f580: 7261 746f 725b 7374 725d 3a0a 2020 2020  rator[str]:.    
-0000f590: 2020 2020 2020 2020 666f 7220 6669 6c65          for file
-0000f5a0: 5f65 6e74 7279 2069 6e20 7363 616e 5f73  _entry in scan_s
-0000f5b0: 7461 745f 6974 6572 3a0a 2020 2020 2020  tat_iter:.      
-0000f5c0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-0000f5d0: 6669 6c65 5f65 6e74 7279 2e70 6174 680a  file_entry.path.
-0000f5e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000f5f0: 6372 6561 7465 5f67 656e 6572 6174 6f72  create_generator
-0000f600: 2829 0a0a 2020 2020 6465 6620 7363 616e  ()..    def scan
-0000f610: 5f73 7461 7428 7365 6c66 2c20 6d69 7373  _stat(self, miss
-0000f620: 696e 675f 6f6b 3a20 626f 6f6c 203d 2054  ing_ok: bool = T
-0000f630: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0000f640: 2020 2020 2020 2066 6f6c 6c6f 776c 696e         followlin
-0000f650: 6b73 3a20 626f 6f6c 203d 2046 616c 7365  ks: bool = False
-0000f660: 2920 2d3e 2049 7465 7261 746f 725b 4669  ) -> Iterator[Fi
-0000f670: 6c65 456e 7472 795d 3a0a 2020 2020 2020  leEntry]:.      
-0000f680: 2020 2727 270a 2020 2020 2020 2020 4974    '''.        It
-0000f690: 6572 6174 6976 656c 7920 7472 6176 6572  eratively traver
-0000f6a0: 7365 206f 6e6c 7920 6669 6c65 7320 696e  se only files in
-0000f6b0: 2067 6976 656e 2064 6972 6563 746f 7279   given directory
-0000f6c0: 2c20 696e 2061 6c70 6861 6265 7469 6361  , in alphabetica
-0000f6d0: 6c20 6f72 6465 722e 0a20 2020 2020 2020  l order..       
-0000f6e0: 2045 7665 7279 2069 7465 7261 7469 6f6e   Every iteration
-0000f6f0: 206f 6e20 6765 6e65 7261 746f 7220 7969   on generator yi
-0000f700: 656c 6473 2061 2074 7570 6c65 206f 6620  elds a tuple of 
-0000f710: 7061 7468 2073 7472 696e 6720 616e 6420  path string and 
-0000f720: 6669 6c65 2073 7461 740a 0a20 2020 2020  file stat..     
-0000f730: 2020 203a 7061 7261 6d20 6d69 7373 696e     :param missin
-0000f740: 675f 6f6b 3a20 4966 2046 616c 7365 2061  g_ok: If False a
-0000f750: 6e64 2074 6865 7265 2773 206e 6f20 6669  nd there's no fi
-0000f760: 6c65 2069 6e20 7468 6520 6469 7265 6374  le in the direct
-0000f770: 6f72 792c 2072 6169 7365 2046 696c 654e  ory, raise FileN
-0000f780: 6f74 466f 756e 6445 7272 6f72 0a20 2020  otFoundError.   
-0000f790: 2020 2020 203a 7261 6973 6573 3a20 556e       :raises: Un
-0000f7a0: 7375 7070 6f72 7465 6445 7272 6f72 0a20  supportedError. 
-0000f7b0: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
-0000f7c0: 2041 2066 696c 6520 7061 7468 2067 656e   A file path gen
-0000f7d0: 6572 6174 6f72 0a20 2020 2020 2020 2027  erator.        '
-0000f7e0: 2727 0a20 2020 2020 2020 2062 7563 6b65  ''.        bucke
-0000f7f0: 742c 206b 6579 203d 2070 6172 7365 5f73  t, key = parse_s
-0000f800: 335f 7572 6c28 7365 6c66 2e70 6174 685f  3_url(self.path_
-0000f810: 7769 7468 5f70 726f 746f 636f 6c29 0a20  with_protocol). 
-0000f820: 2020 2020 2020 2069 6620 6e6f 7420 6275         if not bu
-0000f830: 636b 6574 3a0a 2020 2020 2020 2020 2020  cket:.          
-0000f840: 2020 7261 6973 6520 556e 7375 7070 6f72    raise Unsuppor
-0000f850: 7465 6445 7272 6f72 2827 5363 616e 2077  tedError('Scan w
-0000f860: 686f 6c65 2073 3327 2c20 7365 6c66 2e70  hole s3', self.p
-0000f870: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
-0000f880: 6c29 0a0a 2020 2020 2020 2020 6465 6620  l)..        def 
-0000f890: 6372 6561 7465 5f67 656e 6572 6174 6f72  create_generator
-0000f8a0: 2829 202d 3e20 4974 6572 6174 6f72 5b46  () -> Iterator[F
-0000f8b0: 696c 6545 6e74 7279 5d3a 0a20 2020 2020  ileEntry]:.     
-0000f8c0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000f8d0: 6c66 2e69 735f 6469 7228 293a 0a20 2020  lf.is_dir():.   
-0000f8e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f8f0: 7365 6c66 2e69 735f 6669 6c65 2829 3a0a  self.is_file():.
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 2020 2020 2320 4f6e 2073 332c 2066 696c      # On s3, fil
-0000f920: 6520 616e 6420 6469 7265 6374 6f72 7920  e and directory 
-0000f930: 6d61 7920 6265 206f 6620 7361 6d65 206e  may be of same n
-0000f940: 616d 6520 616e 6420 6c65 7665 6c2c 2073  ame and level, s
-0000f950: 6f20 6e65 6564 2074 6f20 7465 7374 2074  o need to test t
-0000f960: 6865 2070 6174 6820 6973 2066 696c 6520  he path is file 
-0000f970: 6f72 2064 6972 6563 746f 7279 0a20 2020  or directory.   
-0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f990: 2079 6965 6c64 2046 696c 6545 6e74 7279   yield FileEntry
-0000f9a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f9b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000f9c0: 616d 652c 2066 7370 6174 6828 7365 6c66  ame, fspath(self
-0000f9d0: 2e70 6174 685f 7769 7468 5f70 726f 746f  .path_with_proto
-0000f9e0: 636f 6c29 2c0a 2020 2020 2020 2020 2020  col),.          
-0000f9f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fa00: 6c66 2e73 7461 7428 666f 6c6c 6f77 5f73  lf.stat(follow_s
-0000fa10: 796d 6c69 6e6b 733d 666f 6c6c 6f77 6c69  ymlinks=followli
-0000fa20: 6e6b 7329 290a 2020 2020 2020 2020 2020  nks)).          
-0000fa30: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-0000fa40: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000fa50: 206b 6579 2e65 6e64 7377 6974 6828 272f   key.endswith('/
-0000fa60: 2729 2061 6e64 2073 656c 662e 6973 5f66  ') and self.is_f
-0000fa70: 696c 6528 293a 0a20 2020 2020 2020 2020  ile():.         
-0000fa80: 2020 2020 2020 2079 6965 6c64 2046 696c         yield Fil
-0000fa90: 6545 6e74 7279 280a 2020 2020 2020 2020  eEntry(.        
-0000faa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fab0: 2e6e 616d 652c 2066 7370 6174 6828 7365  .name, fspath(se
-0000fac0: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
-0000fad0: 746f 636f 6c29 2c0a 2020 2020 2020 2020  tocol),.        
-0000fae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000faf0: 2e73 7461 7428 666f 6c6c 6f77 5f73 796d  .stat(follow_sym
-0000fb00: 6c69 6e6b 733d 666f 6c6c 6f77 6c69 6e6b  links=followlink
-0000fb10: 7329 290a 0a20 2020 2020 2020 2020 2020  s))..           
-0000fb20: 2070 7265 6669 7820 3d20 5f62 6563 6f6d   prefix = _becom
-0000fb30: 655f 7072 6566 6978 286b 6579 290a 2020  e_prefix(key).  
-0000fb40: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-0000fb50: 203d 2073 656c 662e 5f63 6c69 656e 740a   = self._client.
-0000fb60: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000fb70: 2072 6169 7365 5f73 335f 6572 726f 7228   raise_s3_error(
-0000fb80: 7365 6c66 2e70 6174 685f 7769 7468 5f70  self.path_with_p
-0000fb90: 726f 746f 636f 6c29 3a0a 2020 2020 2020  rotocol):.      
-0000fba0: 2020 2020 2020 2020 2020 666f 7220 7265            for re
-0000fbb0: 7370 2069 6e20 5f6c 6973 745f 6f62 6a65  sp in _list_obje
-0000fbc0: 6374 735f 7265 6375 7273 6976 6528 636c  cts_recursive(cl
-0000fbd0: 6965 6e74 2c20 6275 636b 6574 2c20 7072  ient, bucket, pr
-0000fbe0: 6566 6978 293a 0a20 2020 2020 2020 2020  efix):.         
-0000fbf0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-0000fc00: 6f6e 7465 6e74 2069 6e20 7265 7370 2e67  ontent in resp.g
-0000fc10: 6574 2827 436f 6e74 656e 7473 272c 205b  et('Contents', [
-0000fc20: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-0000fc30: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
-0000fc40: 5f70 6174 6820 3d20 7333 5f70 6174 685f  _path = s3_path_
-0000fc50: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc70: 2020 6627 7b73 656c 662e 5f70 726f 746f    f'{self._proto
-0000fc80: 636f 6c5f 7769 7468 5f70 726f 6669 6c65  col_with_profile
-0000fc90: 7d3a 2f2f 272c 2062 7563 6b65 742c 0a20  }://', bucket,. 
-0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcb0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-0000fcc0: 6e74 5b27 4b65 7927 5d29 0a20 2020 2020  nt['Key']).     
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fce0: 2020 2079 6965 6c64 2046 696c 6545 6e74     yield FileEnt
-0000fcf0: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd10: 5333 5061 7468 2866 756c 6c5f 7061 7468  S3Path(full_path
-0000fd20: 292e 6e61 6d65 2c20 6675 6c6c 5f70 6174  ).name, full_pat
-0000fd30: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-0000fd50: 6d61 6b65 5f73 7461 7428 636f 6e74 656e  make_stat(conten
-0000fd60: 7429 290a 0a20 2020 2020 2020 2072 6574  t))..        ret
-0000fd70: 7572 6e20 5f63 7265 6174 655f 6d69 7373  urn _create_miss
-0000fd80: 696e 675f 6f6b 5f67 656e 6572 6174 6f72  ing_ok_generator
-0000fd90: 280a 2020 2020 2020 2020 2020 2020 6372  (.            cr
-0000fda0: 6561 7465 5f67 656e 6572 6174 6f72 2829  eate_generator()
-0000fdb0: 2c20 6d69 7373 696e 675f 6f6b 2c0a 2020  , missing_ok,.  
-0000fdc0: 2020 2020 2020 2020 2020 5333 4669 6c65            S3File
-0000fdd0: 4e6f 7446 6f75 6e64 4572 726f 7228 274e  NotFoundError('N
-0000fde0: 6f20 6d61 7463 6820 6669 6c65 3a20 2572  o match file: %r
-0000fdf0: 2720 2520 7365 6c66 2e70 6174 685f 7769  ' % self.path_wi
-0000fe00: 7468 5f70 726f 746f 636f 6c29 290a 0a20  th_protocol)).. 
-0000fe10: 2020 2064 6566 2073 6361 6e64 6972 2873     def scandir(s
-0000fe20: 656c 662c 2066 6f6c 6c6f 776c 696e 6b73  elf, followlinks
-0000fe30: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-0000fe40: 2d3e 2049 7465 7261 746f 725b 4669 6c65  -> Iterator[File
-0000fe50: 456e 7472 795d 3a0a 2020 2020 2020 2020  Entry]:.        
-0000fe60: 2727 270a 2020 2020 2020 2020 4765 7420  '''.        Get 
-0000fe70: 616c 6c20 636f 6e74 656e 7473 206f 6620  all contents of 
-0000fe80: 6769 7665 6e20 7333 5f75 726c 2c20 7468  given s3_url, th
-0000fe90: 6520 6f72 6465 7220 6f66 2072 6573 756c  e order of resul
-0000fea0: 7420 6973 206e 6f74 2067 7561 7261 6e74  t is not guarant
-0000feb0: 6565 642e 0a0a 2020 2020 2020 2020 3a72  eed...        :r
-0000fec0: 6574 7572 6e73 3a20 416c 6c20 636f 6e74  eturns: All cont
-0000fed0: 656e 7473 2068 6176 6520 7072 6566 6978  ents have prefix
-0000fee0: 206f 6620 7333 5f75 726c 0a20 2020 2020   of s3_url.     
-0000fef0: 2020 203a 7261 6973 6573 3a20 5333 4669     :raises: S3Fi
-0000ff00: 6c65 4e6f 7446 6f75 6e64 4572 726f 722c  leNotFoundError,
-0000ff10: 2053 334e 6f74 4144 6972 6563 746f 7279   S3NotADirectory
-0000ff20: 4572 726f 720a 2020 2020 2020 2020 2727  Error.        ''
-0000ff30: 270a 2020 2020 2020 2020 6275 636b 6574  '.        bucket
-0000ff40: 2c20 6b65 7920 3d20 7061 7273 655f 7333  , key = parse_s3
-0000ff50: 5f75 726c 2873 656c 662e 7061 7468 5f77  _url(self.path_w
-0000ff60: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
-0000ff70: 2020 2020 2020 6966 206e 6f74 2062 7563        if not buc
-0000ff80: 6b65 7420 616e 6420 6b65 793a 0a20 2020  ket and key:.   
-0000ff90: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-0000ffa0: 3342 7563 6b65 744e 6f74 466f 756e 6445  3BucketNotFoundE
-0000ffb0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000ffc0: 2020 2020 2020 2745 6d70 7479 2062 7563        'Empty buc
-0000ffd0: 6b65 7420 6e61 6d65 3a20 2572 2720 2520  ket name: %r' % 
-0000ffe0: 7365 6c66 2e70 6174 685f 7769 7468 5f70  self.path_with_p
-0000fff0: 726f 746f 636f 6c29 0a0a 2020 2020 2020  rotocol)..      
-00010000: 2020 6966 2073 656c 662e 6973 5f66 696c    if self.is_fil
-00010010: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
-00010020: 2072 6169 7365 2053 334e 6f74 4144 6972   raise S3NotADir
-00010030: 6563 746f 7279 4572 726f 7228 0a20 2020  ectoryError(.   
-00010040: 2020 2020 2020 2020 2020 2020 2027 4e6f               'No
-00010050: 7420 6120 6469 7265 6374 6f72 793a 2025  t a directory: %
-00010060: 7227 2025 2073 656c 662e 7061 7468 5f77  r' % self.path_w
-00010070: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
-00010080: 2020 2020 2020 656c 6966 206e 6f74 2073        elif not s
-00010090: 656c 662e 6973 5f64 6972 2829 3a0a 2020  elf.is_dir():.  
-000100a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000100b0: 5333 4669 6c65 4e6f 7446 6f75 6e64 4572  S3FileNotFoundEr
-000100c0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-000100d0: 2020 2020 2027 4e6f 2073 7563 6820 6469       'No such di
-000100e0: 7265 6374 6f72 793a 2025 7227 2025 2073  rectory: %r' % s
-000100f0: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
-00010100: 6f74 6f63 6f6c 290a 2020 2020 2020 2020  otocol).        
-00010110: 7072 6566 6978 203d 205f 6265 636f 6d65  prefix = _become
-00010120: 5f70 7265 6669 7828 6b65 7929 0a20 2020  _prefix(key).   
-00010130: 2020 2020 2063 6c69 656e 7420 3d20 7365       client = se
-00010140: 6c66 2e5f 636c 6965 6e74 0a0a 2020 2020  lf._client..    
-00010150: 2020 2020 2320 496e 206f 7264 6572 2074      # In order t
-00010160: 6f20 646f 2063 6865 636b 206f 6e20 6372  o do check on cr
-00010170: 6561 7469 6f6e 2c0a 2020 2020 2020 2020  eation,.        
-00010180: 2320 7765 206e 6565 6420 746f 2077 7261  # we need to wra
-00010190: 7020 7468 6520 6974 6572 6174 6f72 2069  p the iterator i
-000101a0: 6e20 616e 6f74 6865 7220 6675 6e63 7469  n another functi
-000101b0: 6f6e 0a20 2020 2020 2020 2064 6566 2063  on.        def c
-000101c0: 7265 6174 655f 6765 6e65 7261 746f 7228  reate_generator(
-000101d0: 2920 2d3e 2049 7465 7261 746f 725b 4669  ) -> Iterator[Fi
-000101e0: 6c65 456e 7472 795d 3a0a 2020 2020 2020  leEntry]:.      
-000101f0: 2020 2020 2020 7769 7468 2072 6169 7365        with raise
-00010200: 5f73 335f 6572 726f 7228 7365 6c66 2e70  _s3_error(self.p
-00010210: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
-00010220: 6c29 3a0a 0a20 2020 2020 2020 2020 2020  l):..           
-00010230: 2020 2020 2064 6566 2067 656e 6572 6174       def generat
-00010240: 655f 7333 5f70 6174 6828 0a20 2020 2020  e_s3_path(.     
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2070 726f 746f 636f 6c3a 2073 7472     protocol: str
-00010270: 2c20 6275 636b 6574 3a20 7374 722c 206b  , bucket: str, k
-00010280: 6579 3a20 7374 7229 202d 3e20 7374 723a  ey: str) -> str:
-00010290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000102a0: 2020 2020 2072 6574 7572 6e20 2225 733a       return "%s:
-000102b0: 2f2f 2573 2f25 7322 2025 2028 7072 6f74  //%s/%s" % (prot
-000102c0: 6f63 6f6c 2c20 6275 636b 6574 2c20 6b65  ocol, bucket, ke
-000102d0: 7929 0a0a 2020 2020 2020 2020 2020 2020  y)..            
-000102e0: 2020 2020 6966 206e 6f74 2062 7563 6b65      if not bucke
-000102f0: 7420 616e 6420 6e6f 7420 6b65 793a 2020  t and not key:  
-00010300: 2320 6c69 7374 2062 7563 6b65 7473 0a20  # list buckets. 
-00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010320: 2020 2072 6573 706f 6e73 6520 3d20 636c     response = cl
-00010330: 6965 6e74 2e6c 6973 745f 6275 636b 6574  ient.list_bucket
-00010340: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00010350: 2020 2020 2020 2020 666f 7220 636f 6e74          for cont
-00010360: 656e 7420 696e 2072 6573 706f 6e73 655b  ent in response[
-00010370: 2742 7563 6b65 7473 275d 3a0a 2020 2020  'Buckets']:.    
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 2020 7969 656c 6420 4669 6c65 456e      yield FileEn
-000103a0: 7472 7928 0a20 2020 2020 2020 2020 2020  try(.           
-000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103c0: 2063 6f6e 7465 6e74 5b27 4e61 6d65 275d   content['Name']
-000103d0: 2c20 6622 7333 3a2f 2f7b 636f 6e74 656e  , f"s3://{conten
-000103e0: 745b 274e 616d 6527 5d7d 222c 0a20 2020  t['Name']}",.   
-000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010400: 2020 2020 2020 2020 2053 7461 7452 6573           StatRes
-00010410: 756c 7428 0a20 2020 2020 2020 2020 2020  ult(.           
-00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010430: 2020 2020 2063 7469 6d65 3d63 6f6e 7465       ctime=conte
-00010440: 6e74 5b27 4372 6561 7469 6f6e 4461 7465  nt['CreationDate
-00010450: 275d 2e74 696d 6573 7461 6d70 2829 2c0a  '].timestamp(),.
-00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 6973 6469 723d 5472 7565 2c0a 2020 2020  isdir=True,.    
+0000ee50: 2065 7272 6f72 5f69 6e66 6f5b 274d 6573   error_info['Mes
+0000ee60: 7361 6765 275d 2929 0a20 2020 2020 2020  sage'])).       
+0000ee70: 2020 2020 2020 2020 2020 2020 2065 7272               err
+0000ee80: 6f72 5f63 6f75 6e74 202b 3d20 6c65 6e28  or_count += len(
+0000ee90: 6572 726f 7273 290a 2020 2020 2020 2020  errors).        
+0000eea0: 2020 2020 6966 2065 7272 6f72 5f63 6f75      if error_cou
+0000eeb0: 6e74 203e 2030 3a0a 2020 2020 2020 2020  nt > 0:.        
+0000eec0: 2020 2020 2020 2020 6572 726f 725f 6d73          error_ms
+0000eed0: 6720 3d20 2266 6169 6c65 6420 7265 6d6f  g = "failed remo
+0000eee0: 7665 2070 6174 683a 2025 732c 2074 6f74  ve path: %s, tot
+0000eef0: 616c 2066 696c 6520 636f 756e 743a 2025  al file count: %
+0000ef00: 732c 2066 6169 6c65 6420 636f 756e 743a  s, failed count:
+0000ef10: 2025 7322 2025 2028 0a20 2020 2020 2020   %s" % (.       
+0000ef20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ef30: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
+0000ef40: 6f63 6f6c 2c20 746f 7461 6c5f 636f 756e  ocol, total_coun
+0000ef50: 742c 2065 7272 6f72 5f63 6f75 6e74 290a  t, error_count).
+0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef70: 7261 6973 6520 5333 556e 6b6e 6f77 6e45  raise S3UnknownE
+0000ef80: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000ef90: 2020 2020 2020 2020 2020 4578 6365 7074            Except
+0000efa0: 696f 6e28 6572 726f 725f 6d73 6729 2c20  ion(error_msg), 
+0000efb0: 7365 6c66 2e70 6174 685f 7769 7468 5f70  self.path_with_p
+0000efc0: 726f 746f 636f 6c29 0a0a 2020 2020 6465  rotocol)..    de
+0000efd0: 6620 7265 6e61 6d65 2873 656c 662c 2064  f rename(self, d
+0000efe0: 7374 5f70 6174 683a 2050 6174 684c 696b  st_path: PathLik
+0000eff0: 6529 202d 3e20 2753 3350 6174 6827 3a0a  e) -> 'S3Path':.
+0000f000: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000f010: 2020 2020 4d6f 7665 2073 3320 6669 6c65      Move s3 file
+0000f020: 2070 6174 6820 6672 6f6d 2073 7263 5f75   path from src_u
+0000f030: 726c 2074 6f20 6473 745f 7572 6c0a 0a20  rl to dst_url.. 
+0000f040: 2020 2020 2020 203a 7061 7261 6d20 6473         :param ds
+0000f050: 745f 7061 7468 3a20 4769 7665 6e20 6465  t_path: Given de
+0000f060: 7374 696e 6174 696f 6e20 7061 7468 0a20  stination path. 
+0000f070: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000f080: 2020 2073 335f 7265 6e61 6d65 2873 656c     s3_rename(sel
+0000f090: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
+0000f0a0: 6f63 6f6c 2c20 6473 745f 7061 7468 290a  ocol, dst_path).
+0000f0b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000f0c0: 656c 662e 6672 6f6d 5f70 6174 6828 6473  elf.from_path(ds
+0000f0d0: 745f 7061 7468 290a 0a20 2020 2064 6566  t_path)..    def
+0000f0e0: 2073 6361 6e28 7365 6c66 2c20 6d69 7373   scan(self, miss
+0000f0f0: 696e 675f 6f6b 3a20 626f 6f6c 203d 2054  ing_ok: bool = T
+0000f100: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0000f110: 2020 666f 6c6c 6f77 6c69 6e6b 733a 2062    followlinks: b
+0000f120: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
+0000f130: 4974 6572 6174 6f72 5b73 7472 5d3a 0a20  Iterator[str]:. 
+0000f140: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000f150: 2020 2049 7465 7261 7469 7665 6c79 2074     Iteratively t
+0000f160: 7261 7665 7273 6520 6f6e 6c79 2066 696c  raverse only fil
+0000f170: 6573 2069 6e20 6769 7665 6e20 7333 2064  es in given s3 d
+0000f180: 6972 6563 746f 7279 2c20 696e 2061 6c70  irectory, in alp
+0000f190: 6861 6265 7469 6361 6c20 6f72 6465 722e  habetical order.
+0000f1a0: 0a20 2020 2020 2020 2045 7665 7279 2069  .        Every i
+0000f1b0: 7465 7261 7469 6f6e 206f 6e20 6765 6e65  teration on gene
+0000f1c0: 7261 746f 7220 7969 656c 6473 2061 2070  rator yields a p
+0000f1d0: 6174 6820 7374 7269 6e67 2e0a 0a20 2020  ath string...   
+0000f1e0: 2020 2020 2049 6620 7333 5f75 726c 2069       If s3_url i
+0000f1f0: 7320 6120 6669 6c65 2070 6174 682c 2079  s a file path, y
+0000f200: 6965 6c64 7320 7468 6520 6669 6c65 206f  ields the file o
+0000f210: 6e6c 790a 2020 2020 2020 2020 4966 2073  nly.        If s
+0000f220: 335f 7572 6c20 6973 2061 206e 6f6e 2d65  3_url is a non-e
+0000f230: 7869 7374 656e 7420 7061 7468 2c20 7265  xistent path, re
+0000f240: 7475 726e 2061 6e20 656d 7074 7920 6765  turn an empty ge
+0000f250: 6e65 7261 746f 720a 2020 2020 2020 2020  nerator.        
+0000f260: 4966 2073 335f 7572 6c20 6973 2061 2062  If s3_url is a b
+0000f270: 7563 6b65 7420 7061 7468 2c20 7265 7475  ucket path, retu
+0000f280: 726e 2061 6c6c 2066 696c 6520 7061 7468  rn all file path
+0000f290: 7320 696e 2074 6865 2062 7563 6b65 740a  s in the bucket.
+0000f2a0: 2020 2020 2020 2020 4966 2073 335f 7572          If s3_ur
+0000f2b0: 6c20 6973 2061 6e20 656d 7074 7920 6275  l is an empty bu
+0000f2c0: 636b 6574 2c20 7265 7475 726e 2061 6e20  cket, return an 
+0000f2d0: 656d 7074 7920 6765 6e65 7261 746f 720a  empty generator.
+0000f2e0: 2020 2020 2020 2020 4966 2073 335f 7572          If s3_ur
+0000f2f0: 6c20 646f 6573 6e27 7420 636f 6e74 6169  l doesn't contai
+0000f300: 6e20 616e 7920 6275 636b 6574 2c20 7768  n any bucket, wh
+0000f310: 6963 6820 6973 2073 335f 7572 6c20 3d3d  ich is s3_url ==
+0000f320: 2027 7333 3a2f 2f27 2c20 7261 6973 6520   's3://', raise 
+0000f330: 556e 7375 7070 6f72 7465 6445 7272 6f72  UnsupportedError
+0000f340: 2e20 7761 6c6b 2829 206f 6e20 636f 6d70  . walk() on comp
+0000f350: 6c65 7465 2073 3320 6973 206e 6f74 2073  lete s3 is not s
+0000f360: 7570 706f 7274 6564 2069 6e20 6d65 6766  upported in megf
+0000f370: 696c 650a 0a20 2020 2020 2020 203a 7061  ile..        :pa
+0000f380: 7261 6d20 6d69 7373 696e 675f 6f6b 3a20  ram missing_ok: 
+0000f390: 4966 2046 616c 7365 2061 6e64 2074 6865  If False and the
+0000f3a0: 7265 2773 206e 6f20 6669 6c65 2069 6e20  re's no file in 
+0000f3b0: 7468 6520 6469 7265 6374 6f72 792c 2072  the directory, r
+0000f3c0: 6169 7365 2046 696c 654e 6f74 466f 756e  aise FileNotFoun
+0000f3d0: 6445 7272 6f72 0a20 2020 2020 2020 203a  dError.        :
+0000f3e0: 7261 6973 6573 3a20 556e 7375 7070 6f72  raises: Unsuppor
+0000f3f0: 7465 6445 7272 6f72 0a20 2020 2020 2020  tedError.       
+0000f400: 203a 7265 7475 726e 733a 2041 2066 696c   :returns: A fil
+0000f410: 6520 7061 7468 2067 656e 6572 6174 6f72  e path generator
+0000f420: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+0000f430: 2020 2020 2073 6361 6e5f 7374 6174 5f69       scan_stat_i
+0000f440: 7465 7220 3d20 7365 6c66 2e73 6361 6e5f  ter = self.scan_
+0000f450: 7374 6174 280a 2020 2020 2020 2020 2020  stat(.          
+0000f460: 2020 6d69 7373 696e 675f 6f6b 3d6d 6973    missing_ok=mis
+0000f470: 7369 6e67 5f6f 6b2c 2066 6f6c 6c6f 776c  sing_ok, followl
+0000f480: 696e 6b73 3d66 6f6c 6c6f 776c 696e 6b73  inks=followlinks
+0000f490: 290a 0a20 2020 2020 2020 2064 6566 2063  )..        def c
+0000f4a0: 7265 6174 655f 6765 6e65 7261 746f 7228  reate_generator(
+0000f4b0: 2920 2d3e 2049 7465 7261 746f 725b 7374  ) -> Iterator[st
+0000f4c0: 725d 3a0a 2020 2020 2020 2020 2020 2020  r]:.            
+0000f4d0: 666f 7220 6669 6c65 5f65 6e74 7279 2069  for file_entry i
+0000f4e0: 6e20 7363 616e 5f73 7461 745f 6974 6572  n scan_stat_iter
+0000f4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f500: 2020 7969 656c 6420 6669 6c65 5f65 6e74    yield file_ent
+0000f510: 7279 2e70 6174 680a 0a20 2020 2020 2020  ry.path..       
+0000f520: 2072 6574 7572 6e20 6372 6561 7465 5f67   return create_g
+0000f530: 656e 6572 6174 6f72 2829 0a0a 2020 2020  enerator()..    
+0000f540: 6465 6620 7363 616e 5f73 7461 7428 7365  def scan_stat(se
+0000f550: 6c66 2c20 6d69 7373 696e 675f 6f6b 3a20  lf, missing_ok: 
+0000f560: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+0000f570: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f580: 6f6c 6c6f 776c 696e 6b73 3a20 626f 6f6c  ollowlinks: bool
+0000f590: 203d 2046 616c 7365 2920 2d3e 2049 7465   = False) -> Ite
+0000f5a0: 7261 746f 725b 4669 6c65 456e 7472 795d  rator[FileEntry]
+0000f5b0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+0000f5c0: 2020 2020 2020 4974 6572 6174 6976 656c        Iterativel
+0000f5d0: 7920 7472 6176 6572 7365 206f 6e6c 7920  y traverse only 
+0000f5e0: 6669 6c65 7320 696e 2067 6976 656e 2064  files in given d
+0000f5f0: 6972 6563 746f 7279 2c20 696e 2061 6c70  irectory, in alp
+0000f600: 6861 6265 7469 6361 6c20 6f72 6465 722e  habetical order.
+0000f610: 0a20 2020 2020 2020 2045 7665 7279 2069  .        Every i
+0000f620: 7465 7261 7469 6f6e 206f 6e20 6765 6e65  teration on gene
+0000f630: 7261 746f 7220 7969 656c 6473 2061 2074  rator yields a t
+0000f640: 7570 6c65 206f 6620 7061 7468 2073 7472  uple of path str
+0000f650: 696e 6720 616e 6420 6669 6c65 2073 7461  ing and file sta
+0000f660: 740a 0a20 2020 2020 2020 203a 7061 7261  t..        :para
+0000f670: 6d20 6d69 7373 696e 675f 6f6b 3a20 4966  m missing_ok: If
+0000f680: 2046 616c 7365 2061 6e64 2074 6865 7265   False and there
+0000f690: 2773 206e 6f20 6669 6c65 2069 6e20 7468  's no file in th
+0000f6a0: 6520 6469 7265 6374 6f72 792c 2072 6169  e directory, rai
+0000f6b0: 7365 2046 696c 654e 6f74 466f 756e 6445  se FileNotFoundE
+0000f6c0: 7272 6f72 0a20 2020 2020 2020 203a 7261  rror.        :ra
+0000f6d0: 6973 6573 3a20 556e 7375 7070 6f72 7465  ises: Unsupporte
+0000f6e0: 6445 7272 6f72 0a20 2020 2020 2020 203a  dError.        :
+0000f6f0: 7265 7475 726e 733a 2041 2066 696c 6520  returns: A file 
+0000f700: 7061 7468 2067 656e 6572 6174 6f72 0a20  path generator. 
+0000f710: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000f720: 2020 2062 7563 6b65 742c 206b 6579 203d     bucket, key =
+0000f730: 2070 6172 7365 5f73 335f 7572 6c28 7365   parse_s3_url(se
+0000f740: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
+0000f750: 746f 636f 6c29 0a20 2020 2020 2020 2069  tocol).        i
+0000f760: 6620 6e6f 7420 6275 636b 6574 3a0a 2020  f not bucket:.  
+0000f770: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000f780: 556e 7375 7070 6f72 7465 6445 7272 6f72  UnsupportedError
+0000f790: 2827 5363 616e 2077 686f 6c65 2073 3327  ('Scan whole s3'
+0000f7a0: 2c20 7365 6c66 2e70 6174 685f 7769 7468  , self.path_with
+0000f7b0: 5f70 726f 746f 636f 6c29 0a0a 2020 2020  _protocol)..    
+0000f7c0: 2020 2020 6465 6620 6372 6561 7465 5f67      def create_g
+0000f7d0: 656e 6572 6174 6f72 2829 202d 3e20 4974  enerator() -> It
+0000f7e0: 6572 6174 6f72 5b46 696c 6545 6e74 7279  erator[FileEntry
+0000f7f0: 5d3a 0a20 2020 2020 2020 2020 2020 2069  ]:.            i
+0000f800: 6620 6e6f 7420 7365 6c66 2e69 735f 6469  f not self.is_di
+0000f810: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
+0000f820: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+0000f830: 6669 6c65 2829 3a0a 2020 2020 2020 2020  file():.        
+0000f840: 2020 2020 2020 2020 2020 2020 2320 4f6e              # On
+0000f850: 2073 332c 2066 696c 6520 616e 6420 6469   s3, file and di
+0000f860: 7265 6374 6f72 7920 6d61 7920 6265 206f  rectory may be o
+0000f870: 6620 7361 6d65 206e 616d 6520 616e 6420  f same name and 
+0000f880: 6c65 7665 6c2c 2073 6f20 6e65 6564 2074  level, so need t
+0000f890: 6f20 7465 7374 2074 6865 2070 6174 6820  o test the path 
+0000f8a0: 6973 2066 696c 6520 6f72 2064 6972 6563  is file or direc
+0000f8b0: 746f 7279 0a20 2020 2020 2020 2020 2020  tory.           
+0000f8c0: 2020 2020 2020 2020 2079 6965 6c64 2046           yield F
+0000f8d0: 696c 6545 6e74 7279 280a 2020 2020 2020  ileEntry(.      
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8f0: 2020 7365 6c66 2e6e 616d 652c 2066 7370    self.name, fsp
+0000f900: 6174 6828 7365 6c66 2e70 6174 685f 7769  ath(self.path_wi
+0000f910: 7468 5f70 726f 746f 636f 6c29 2c0a 2020  th_protocol),.  
+0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f930: 2020 2020 2020 7365 6c66 2e73 7461 7428        self.stat(
+0000f940: 666f 6c6c 6f77 5f73 796d 6c69 6e6b 733d  follow_symlinks=
+0000f950: 666f 6c6c 6f77 6c69 6e6b 7329 290a 2020  followlinks)).  
+0000f960: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000f970: 7475 726e 0a0a 2020 2020 2020 2020 2020  turn..          
+0000f980: 2020 6966 206e 6f74 206b 6579 2e65 6e64    if not key.end
+0000f990: 7377 6974 6828 272f 2729 2061 6e64 2073  swith('/') and s
+0000f9a0: 656c 662e 6973 5f66 696c 6528 293a 0a20  elf.is_file():. 
+0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+0000f9c0: 6965 6c64 2046 696c 6545 6e74 7279 280a  ield FileEntry(.
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 2020 2020 7365 6c66 2e6e 616d 652c 2066      self.name, f
+0000f9f0: 7370 6174 6828 7365 6c66 2e70 6174 685f  spath(self.path_
+0000fa00: 7769 7468 5f70 726f 746f 636f 6c29 2c0a  with_protocol),.
+0000fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa20: 2020 2020 7365 6c66 2e73 7461 7428 666f      self.stat(fo
+0000fa30: 6c6c 6f77 5f73 796d 6c69 6e6b 733d 666f  llow_symlinks=fo
+0000fa40: 6c6c 6f77 6c69 6e6b 7329 290a 0a20 2020  llowlinks))..   
+0000fa50: 2020 2020 2020 2020 2070 7265 6669 7820           prefix 
+0000fa60: 3d20 5f62 6563 6f6d 655f 7072 6566 6978  = _become_prefix
+0000fa70: 286b 6579 290a 2020 2020 2020 2020 2020  (key).          
+0000fa80: 2020 636c 6965 6e74 203d 2073 656c 662e    client = self.
+0000fa90: 5f63 6c69 656e 740a 2020 2020 2020 2020  _client.        
+0000faa0: 2020 2020 7769 7468 2072 6169 7365 5f73      with raise_s
+0000fab0: 335f 6572 726f 7228 7365 6c66 2e70 6174  3_error(self.pat
+0000fac0: 685f 7769 7468 5f70 726f 746f 636f 6c29  h_with_protocol)
+0000fad0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fae0: 2020 666f 7220 7265 7370 2069 6e20 5f6c    for resp in _l
+0000faf0: 6973 745f 6f62 6a65 6374 735f 7265 6375  ist_objects_recu
+0000fb00: 7273 6976 6528 636c 6965 6e74 2c20 6275  rsive(client, bu
+0000fb10: 636b 6574 2c20 7072 6566 6978 293a 0a20  cket, prefix):. 
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 2020 2066 6f72 2063 6f6e 7465 6e74 2069     for content i
+0000fb40: 6e20 7265 7370 2e67 6574 2827 436f 6e74  n resp.get('Cont
+0000fb50: 656e 7473 272c 205b 5d29 3a0a 2020 2020  ents', []):.    
+0000fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb70: 2020 2020 6675 6c6c 5f70 6174 6820 3d20      full_path = 
+0000fb80: 7333 5f70 6174 685f 6a6f 696e 280a 2020  s3_path_join(.  
+0000fb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fba0: 2020 2020 2020 2020 2020 6627 7b73 656c            f'{sel
+0000fbb0: 662e 5f70 726f 746f 636f 6c5f 7769 7468  f._protocol_with
+0000fbc0: 5f70 726f 6669 6c65 7d3a 2f2f 272c 2062  _profile}://', b
+0000fbd0: 7563 6b65 742c 0a20 2020 2020 2020 2020  ucket,.         
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbf0: 2020 2063 6f6e 7465 6e74 5b27 4b65 7927     content['Key'
+0000fc00: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000fc10: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+0000fc20: 2046 696c 6545 6e74 7279 280a 2020 2020   FileEntry(.    
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc40: 2020 2020 2020 2020 5333 5061 7468 2866          S3Path(f
+0000fc50: 756c 6c5f 7061 7468 292e 6e61 6d65 2c20  ull_path).name, 
+0000fc60: 6675 6c6c 5f70 6174 682c 0a20 2020 2020  full_path,.     
+0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc80: 2020 2020 2020 205f 6d61 6b65 5f73 7461         _make_sta
+0000fc90: 7428 636f 6e74 656e 7429 290a 0a20 2020  t(content))..   
+0000fca0: 2020 2020 2072 6574 7572 6e20 5f63 7265       return _cre
+0000fcb0: 6174 655f 6d69 7373 696e 675f 6f6b 5f67  ate_missing_ok_g
+0000fcc0: 656e 6572 6174 6f72 280a 2020 2020 2020  enerator(.      
+0000fcd0: 2020 2020 2020 6372 6561 7465 5f67 656e        create_gen
+0000fce0: 6572 6174 6f72 2829 2c20 6d69 7373 696e  erator(), missin
+0000fcf0: 675f 6f6b 2c0a 2020 2020 2020 2020 2020  g_ok,.          
+0000fd00: 2020 5333 4669 6c65 4e6f 7446 6f75 6e64    S3FileNotFound
+0000fd10: 4572 726f 7228 274e 6f20 6d61 7463 6820  Error('No match 
+0000fd20: 6669 6c65 3a20 2572 2720 2520 7365 6c66  file: %r' % self
+0000fd30: 2e70 6174 685f 7769 7468 5f70 726f 746f  .path_with_proto
+0000fd40: 636f 6c29 290a 0a20 2020 2064 6566 2073  col))..    def s
+0000fd50: 6361 6e64 6972 2873 656c 662c 2066 6f6c  candir(self, fol
+0000fd60: 6c6f 776c 696e 6b73 3a20 626f 6f6c 203d  lowlinks: bool =
+0000fd70: 2046 616c 7365 2920 2d3e 2049 7465 7261   False) -> Itera
+0000fd80: 746f 725b 4669 6c65 456e 7472 795d 3a0a  tor[FileEntry]:.
+0000fd90: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000fda0: 2020 2020 4765 7420 616c 6c20 636f 6e74      Get all cont
+0000fdb0: 656e 7473 206f 6620 6769 7665 6e20 7333  ents of given s3
+0000fdc0: 5f75 726c 2c20 7468 6520 6f72 6465 7220  _url, the order 
+0000fdd0: 6f66 2072 6573 756c 7420 6973 206e 6f74  of result is not
+0000fde0: 2067 7561 7261 6e74 6565 642e 0a0a 2020   guaranteed...  
+0000fdf0: 2020 2020 2020 3a72 6574 7572 6e73 3a20        :returns: 
+0000fe00: 416c 6c20 636f 6e74 656e 7473 2068 6176  All contents hav
+0000fe10: 6520 7072 6566 6978 206f 6620 7333 5f75  e prefix of s3_u
+0000fe20: 726c 0a20 2020 2020 2020 203a 7261 6973  rl.        :rais
+0000fe30: 6573 3a20 5333 4669 6c65 4e6f 7446 6f75  es: S3FileNotFou
+0000fe40: 6e64 4572 726f 722c 2053 334e 6f74 4144  ndError, S3NotAD
+0000fe50: 6972 6563 746f 7279 4572 726f 720a 2020  irectoryError.  
+0000fe60: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0000fe70: 2020 6275 636b 6574 2c20 6b65 7920 3d20    bucket, key = 
+0000fe80: 7061 7273 655f 7333 5f75 726c 2873 656c  parse_s3_url(sel
+0000fe90: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
+0000fea0: 6f63 6f6c 290a 2020 2020 2020 2020 6966  ocol).        if
+0000feb0: 206e 6f74 2062 7563 6b65 7420 616e 6420   not bucket and 
+0000fec0: 6b65 793a 0a20 2020 2020 2020 2020 2020  key:.           
+0000fed0: 2072 6169 7365 2053 3342 7563 6b65 744e   raise S3BucketN
+0000fee0: 6f74 466f 756e 6445 7272 6f72 280a 2020  otFoundError(.  
+0000fef0: 2020 2020 2020 2020 2020 2020 2020 2745                'E
+0000ff00: 6d70 7479 2062 7563 6b65 7420 6e61 6d65  mpty bucket name
+0000ff10: 3a20 2572 2720 2520 7365 6c66 2e70 6174  : %r' % self.pat
+0000ff20: 685f 7769 7468 5f70 726f 746f 636f 6c29  h_with_protocol)
+0000ff30: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000ff40: 662e 6973 5f66 696c 6528 293a 0a20 2020  f.is_file():.   
+0000ff50: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+0000ff60: 334e 6f74 4144 6972 6563 746f 7279 4572  3NotADirectoryEr
+0000ff70: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000ff80: 2020 2020 2027 4e6f 7420 6120 6469 7265       'Not a dire
+0000ff90: 6374 6f72 793a 2025 7227 2025 2073 656c  ctory: %r' % sel
+0000ffa0: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
+0000ffb0: 6f63 6f6c 290a 2020 2020 2020 2020 656c  ocol).        el
+0000ffc0: 6966 206e 6f74 2073 656c 662e 6973 5f64  if not self.is_d
+0000ffd0: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
+0000ffe0: 2020 7261 6973 6520 5333 4669 6c65 4e6f    raise S3FileNo
+0000fff0: 7446 6f75 6e64 4572 726f 7228 0a20 2020  tFoundError(.   
+00010000: 2020 2020 2020 2020 2020 2020 2027 4e6f               'No
+00010010: 2073 7563 6820 6469 7265 6374 6f72 793a   such directory:
+00010020: 2025 7227 2025 2073 656c 662e 7061 7468   %r' % self.path
+00010030: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
+00010040: 2020 2020 2020 2020 7072 6566 6978 203d          prefix =
+00010050: 205f 6265 636f 6d65 5f70 7265 6669 7828   _become_prefix(
+00010060: 6b65 7929 0a20 2020 2020 2020 2063 6c69  key).        cli
+00010070: 656e 7420 3d20 7365 6c66 2e5f 636c 6965  ent = self._clie
+00010080: 6e74 0a0a 2020 2020 2020 2020 2320 496e  nt..        # In
+00010090: 206f 7264 6572 2074 6f20 646f 2063 6865   order to do che
+000100a0: 636b 206f 6e20 6372 6561 7469 6f6e 2c0a  ck on creation,.
+000100b0: 2020 2020 2020 2020 2320 7765 206e 6565          # we nee
+000100c0: 6420 746f 2077 7261 7020 7468 6520 6974  d to wrap the it
+000100d0: 6572 6174 6f72 2069 6e20 616e 6f74 6865  erator in anothe
+000100e0: 7220 6675 6e63 7469 6f6e 0a20 2020 2020  r function.     
+000100f0: 2020 2064 6566 2063 7265 6174 655f 6765     def create_ge
+00010100: 6e65 7261 746f 7228 2920 2d3e 2049 7465  nerator() -> Ite
+00010110: 7261 746f 725b 4669 6c65 456e 7472 795d  rator[FileEntry]
+00010120: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00010130: 7468 2072 6169 7365 5f73 335f 6572 726f  th raise_s3_erro
+00010140: 7228 7365 6c66 2e70 6174 685f 7769 7468  r(self.path_with
+00010150: 5f70 726f 746f 636f 6c29 3a0a 0a20 2020  _protocol):..   
+00010160: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00010170: 2067 656e 6572 6174 655f 7333 5f70 6174   generate_s3_pat
+00010180: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
+00010190: 2020 2020 2020 2020 2020 2070 726f 746f             proto
+000101a0: 636f 6c3a 2073 7472 2c20 6275 636b 6574  col: str, bucket
+000101b0: 3a20 7374 722c 206b 6579 3a20 7374 7229  : str, key: str)
+000101c0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+000101d0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000101e0: 7572 6e20 2225 733a 2f2f 2573 2f25 7322  urn "%s://%s/%s"
+000101f0: 2025 2028 7072 6f74 6f63 6f6c 2c20 6275   % (protocol, bu
+00010200: 636b 6574 2c20 6b65 7929 0a0a 2020 2020  cket, key)..    
+00010210: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00010220: 6f74 2062 7563 6b65 7420 616e 6420 6e6f  ot bucket and no
+00010230: 7420 6b65 793a 2020 2320 6c69 7374 2062  t key:  # list b
+00010240: 7563 6b65 7473 0a20 2020 2020 2020 2020  uckets.         
+00010250: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+00010260: 6e73 6520 3d20 636c 6965 6e74 2e6c 6973  nse = client.lis
+00010270: 745f 6275 636b 6574 7328 290a 2020 2020  t_buckets().    
+00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010290: 666f 7220 636f 6e74 656e 7420 696e 2072  for content in r
+000102a0: 6573 706f 6e73 655b 2742 7563 6b65 7473  esponse['Buckets
+000102b0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+000102c0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+000102d0: 6420 4669 6c65 456e 7472 7928 0a20 2020  d FileEntry(.   
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+00010300: 5b27 4e61 6d65 275d 2c20 6622 7333 3a2f  ['Name'], f"s3:/
+00010310: 2f7b 636f 6e74 656e 745b 274e 616d 6527  /{content['Name'
+00010320: 5d7d 222c 0a20 2020 2020 2020 2020 2020  ]}",.           
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 2053 7461 7452 6573 756c 7428 0a20 2020   StatResult(.   
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 2020 2020 2020 2020 2020 2063 7469               cti
+00010370: 6d65 3d63 6f6e 7465 6e74 5b27 4372 6561  me=content['Crea
+00010380: 7469 6f6e 4461 7465 275d 2e74 696d 6573  tionDate'].times
+00010390: 7461 6d70 2829 2c0a 2020 2020 2020 2020  tamp(),.        
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2020 2020 2020 2020 6973 6469 723d 5472          isdir=Tr
+000103c0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 2020 2020 6578 7472 613d 636f 6e74 656e      extra=conten
+000103f0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00010400: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010410: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010420: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00010430: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010440: 7220 7265 7370 2069 6e20 5f6c 6973 745f  r resp in _list_
+00010450: 6f62 6a65 6374 735f 7265 6375 7273 6976  objects_recursiv
+00010460: 6528 636c 6965 6e74 2c20 6275 636b 6574  e(client, bucket
+00010470: 2c20 7072 6566 6978 2c0a 2020 2020 2020  , prefix,.      
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2020 2020 2020 2020 2020 6578 7472              extr
-000104b0: 613d 636f 6e74 656e 742c 0a20 2020 2020  a=content,.     
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2020 2020 2020 2029 290a 2020 2020 2020         )).      
-000104e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000104f0: 7475 726e 0a0a 2020 2020 2020 2020 2020  turn..          
-00010500: 2020 2020 2020 666f 7220 7265 7370 2069        for resp i
-00010510: 6e20 5f6c 6973 745f 6f62 6a65 6374 735f  n _list_objects_
-00010520: 7265 6375 7273 6976 6528 636c 6965 6e74  recursive(client
-00010530: 2c20 6275 636b 6574 2c20 7072 6566 6978  , bucket, prefix
-00010540: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 2020 2020 272f 2729 3a0a 2020 2020        '/'):.    
-00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 666f 7220 636f 6d6d 6f6e 5f70 7265 6669  for common_prefi
-000105a0: 7820 696e 2072 6573 702e 6765 7428 2743  x in resp.get('C
-000105b0: 6f6d 6d6f 6e50 7265 6669 7865 7327 2c20  ommonPrefixes', 
-000105c0: 5b5d 293a 0a20 2020 2020 2020 2020 2020  []):.           
-000105d0: 2020 2020 2020 2020 2020 2020 2079 6965               yie
-000105e0: 6c64 2046 696c 6545 6e74 7279 280a 2020  ld FileEntry(.  
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2020 2020 2020 2020 636f 6d6d 6f6e            common
-00010610: 5f70 7265 6669 785b 2750 7265 6669 7827  _prefix['Prefix'
-00010620: 5d5b 6c65 6e28 7072 6566 6978 293a 2d31  ][len(prefix):-1
-00010630: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00010640: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00010650: 656e 6572 6174 655f 7333 5f70 6174 6828  enerate_s3_path(
+000104a0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+000104b0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+000104c0: 2020 2020 2020 2020 666f 7220 636f 6d6d          for comm
+000104d0: 6f6e 5f70 7265 6669 7820 696e 2072 6573  on_prefix in res
+000104e0: 702e 6765 7428 2743 6f6d 6d6f 6e50 7265  p.get('CommonPre
+000104f0: 6669 7865 7327 2c20 5b5d 293a 0a20 2020  fixes', []):.   
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 2020 2020 2079 6965 6c64 2046 696c 6545       yield FileE
+00010520: 6e74 7279 280a 2020 2020 2020 2020 2020  ntry(.          
+00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010540: 2020 636f 6d6d 6f6e 5f70 7265 6669 785b    common_prefix[
+00010550: 2750 7265 6669 7827 5d5b 6c65 6e28 7072  'Prefix'][len(pr
+00010560: 6566 6978 293a 2d31 5d2c 0a20 2020 2020  efix):-1],.     
+00010570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010580: 2020 2020 2020 2067 656e 6572 6174 655f         generate_
+00010590: 7333 5f70 6174 6828 0a20 2020 2020 2020  s3_path(.       
+000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105b0: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+000105c0: 726f 746f 636f 6c5f 7769 7468 5f70 726f  rotocol_with_pro
+000105d0: 6669 6c65 2c20 6275 636b 6574 2c0a 2020  file, bucket,.  
+000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00010600: 6d6d 6f6e 5f70 7265 6669 785b 2750 7265  mmon_prefix['Pre
+00010610: 6669 7827 5d29 2c0a 2020 2020 2020 2020  fix']),.        
+00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010630: 2020 2020 5374 6174 5265 7375 6c74 2869      StatResult(i
+00010640: 7364 6972 3d54 7275 652c 2065 7874 7261  sdir=True, extra
+00010650: 3d63 6f6d 6d6f 6e5f 7072 6566 6978 2929  =common_prefix))
 00010660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 2073 656c 662e 5f70 726f 746f 636f 6c5f   self._protocol_
-00010690: 7769 7468 5f70 726f 6669 6c65 2c20 6275  with_profile, bu
-000106a0: 636b 6574 2c0a 2020 2020 2020 2020 2020  cket,.          
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2020 2020 636f 6d6d 6f6e 5f70 7265        common_pre
-000106d0: 6669 785b 2750 7265 6669 7827 5d29 2c0a  fix['Prefix']),.
-000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106f0: 2020 2020 2020 2020 2020 2020 5374 6174              Stat
-00010700: 5265 7375 6c74 2869 7364 6972 3d54 7275  Result(isdir=Tru
-00010710: 652c 2065 7874 7261 3d63 6f6d 6d6f 6e5f  e, extra=common_
-00010720: 7072 6566 6978 2929 0a20 2020 2020 2020  prefix)).       
-00010730: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00010740: 2063 6f6e 7465 6e74 2069 6e20 7265 7370   content in resp
-00010750: 2e67 6574 2827 436f 6e74 656e 7473 272c  .get('Contents',
-00010760: 205b 5d29 3a0a 2020 2020 2020 2020 2020   []):.          
-00010770: 2020 2020 2020 2020 2020 2020 2020 7372                sr
-00010780: 635f 7572 6c20 3d20 6765 6e65 7261 7465  c_url = generate
-00010790: 5f73 335f 7061 7468 280a 2020 2020 2020  _s3_path(.      
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2020 2020 7365 6c66 2e5f 7072 6f74        self._prot
-000107c0: 6f63 6f6c 5f77 6974 685f 7072 6f66 696c  ocol_with_profil
-000107d0: 652c 2062 7563 6b65 742c 2063 6f6e 7465  e, bucket, conte
-000107e0: 6e74 5b27 4b65 7927 5d29 0a0a 2020 2020  nt['Key'])..    
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 2020 2020 6966 2066 6f6c 6c6f 776c 696e      if followlin
-00010810: 6b73 2061 6e64 2053 3350 6174 6828 7372  ks and S3Path(sr
-00010820: 635f 7572 6c29 2e69 735f 7379 6d6c 696e  c_url).is_symlin
-00010830: 6b28 293a 0a20 2020 2020 2020 2020 2020  k():.           
-00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010850: 2063 6f6e 7465 6e74 5b27 6973 6c6e 6b27   content['islnk'
-00010860: 5d20 3d20 5472 7565 0a0a 2020 2020 2020  ] = True..      
-00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010880: 2020 7969 656c 6420 4669 6c65 456e 7472    yield FileEntr
-00010890: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000108b0: 6f6e 7465 6e74 5b27 4b65 7927 5d5b 6c65  ontent['Key'][le
-000108c0: 6e28 7072 6566 6978 293a 5d2c 2073 7263  n(prefix):], src
-000108d0: 5f75 726c 2c0a 2020 2020 2020 2020 2020  _url,.          
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 2020 5f6d 616b 655f 7374 6174 2863 6f6e    _make_stat(con
-00010900: 7465 6e74 2929 0a0a 2020 2020 2020 2020  tent))..        
-00010910: 7265 7475 726e 2043 6f6e 7465 7874 4974  return ContextIt
-00010920: 6572 6174 6f72 2863 7265 6174 655f 6765  erator(create_ge
-00010930: 6e65 7261 746f 7228 2929 0a0a 2020 2020  nerator())..    
-00010940: 6465 6620 5f67 6574 6469 7273 7461 7428  def _getdirstat(
-00010950: 7365 6c66 2920 2d3e 2053 7461 7452 6573  self) -> StatRes
-00010960: 756c 743a 0a20 2020 2020 2020 2027 2727  ult:.        '''
-00010970: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-00010980: 5374 6174 5265 7375 6c74 206f 6620 6769  StatResult of gi
-00010990: 7665 6e20 7333 5f75 726c 2064 6972 6563  ven s3_url direc
-000109a0: 746f 7279 2c20 696e 636c 7564 696e 673a  tory, including:
-000109b0: 200a 0a20 2020 2020 2020 2031 2e20 4469   ..        1. Di
-000109c0: 7265 6374 6f72 7920 7369 7a65 3a20 7468  rectory size: th
-000109d0: 6520 7375 6d20 6f66 2061 6c6c 2066 696c  e sum of all fil
-000109e0: 6520 7369 7a65 2069 6e20 6974 2c20 696e  e size in it, in
-000109f0: 636c 7564 696e 6720 6669 6c65 2069 6e20  cluding file in 
-00010a00: 7375 6264 6972 6563 746f 7269 6573 2028  subdirectories (
-00010a10: 6966 2065 7869 7374 292e 0a20 2020 2020  if exist)..     
-00010a20: 2020 2054 6865 2072 6573 756c 7420 6578     The result ex
-00010a30: 636c 7564 6573 2074 6865 2073 697a 6520  cludes the size 
-00010a40: 6f66 2064 6972 6563 746f 7279 2069 7473  of directory its
-00010a50: 656c 662e 2049 6e20 6f74 6865 7220 776f  elf. In other wo
-00010a60: 7264 732c 2072 6574 7572 6e20 3020 4279  rds, return 0 By
-00010a70: 7465 206f 6e20 616e 2065 6d70 7479 2064  te on an empty d
-00010a80: 6972 6563 746f 7279 2070 6174 680a 2020  irectory path.  
-00010a90: 2020 2020 2020 322e 204c 6173 742d 6d6f        2. Last-mo
-00010aa0: 6469 6669 6564 2074 696d 6520 6f66 2064  dified time of d
-00010ab0: 6972 6563 746f 7279 3a20 7265 7475 726e  irectory: return
-00010ac0: 2074 6865 206c 6174 6573 7420 6d6f 6469   the latest modi
-00010ad0: 6669 6564 2074 696d 6520 6f66 2061 6c6c  fied time of all
-00010ae0: 2066 696c 6520 696e 2069 742e 2054 6865   file in it. The
-00010af0: 206d 7469 6d65 206f 6620 656d 7074 7920   mtime of empty 
-00010b00: 6469 7265 6374 6f72 7920 6973 2031 3937  directory is 197
-00010b10: 302d 3031 2d30 3120 3030 3a30 303a 3030  0-01-01 00:00:00
-00010b20: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00010b30: 6e73 3a20 416e 2069 6e74 2069 6e64 6963  ns: An int indic
-00010b40: 6174 6573 2073 697a 6520 696e 2042 7974  ates size in Byt
-00010b50: 6573 0a20 2020 2020 2020 2027 2727 0a20  es.        '''. 
-00010b60: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00010b70: 6c66 2e69 735f 6469 7228 293a 0a20 2020  lf.is_dir():.   
-00010b80: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-00010b90: 3346 696c 654e 6f74 466f 756e 6445 7272  3FileNotFoundErr
-00010ba0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00010bb0: 2020 2020 274e 6f20 7375 6368 2066 696c      'No such fil
-00010bc0: 6520 6f72 2064 6972 6563 746f 7279 3a20  e or directory: 
-00010bd0: 2572 2720 2520 7365 6c66 2e70 6174 685f  %r' % self.path_
-00010be0: 7769 7468 5f70 726f 746f 636f 6c29 0a0a  with_protocol)..
-00010bf0: 2020 2020 2020 2020 6275 636b 6574 2c20          bucket, 
-00010c00: 6b65 7920 3d20 7061 7273 655f 7333 5f75  key = parse_s3_u
-00010c10: 726c 2873 656c 662e 7061 7468 5f77 6974  rl(self.path_wit
-00010c20: 685f 7072 6f74 6f63 6f6c 290a 2020 2020  h_protocol).    
-00010c30: 2020 2020 7072 6566 6978 203d 205f 6265      prefix = _be
-00010c40: 636f 6d65 5f70 7265 6669 7828 6b65 7929  come_prefix(key)
-00010c50: 0a20 2020 2020 2020 2063 6c69 656e 7420  .        client 
-00010c60: 3d20 7365 6c66 2e5f 636c 6965 6e74 0a20  = self._client. 
-00010c70: 2020 2020 2020 2073 697a 6520 3d20 300a         size = 0.
-00010c80: 2020 2020 2020 2020 6d74 696d 6520 3d20          mtime = 
-00010c90: 302e 300a 2020 2020 2020 2020 7769 7468  0.0.        with
-00010ca0: 2072 6169 7365 5f73 335f 6572 726f 7228   raise_s3_error(
-00010cb0: 7365 6c66 2e70 6174 685f 7769 7468 5f70  self.path_with_p
-00010cc0: 726f 746f 636f 6c29 3a0a 2020 2020 2020  rotocol):.      
-00010cd0: 2020 2020 2020 666f 7220 7265 7370 2069        for resp i
-00010ce0: 6e20 5f6c 6973 745f 6f62 6a65 6374 735f  n _list_objects_
-00010cf0: 7265 6375 7273 6976 6528 636c 6965 6e74  recursive(client
-00010d00: 2c20 6275 636b 6574 2c20 7072 6566 6978  , bucket, prefix
-00010d10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010d20: 2020 2066 6f72 2063 6f6e 7465 6e74 2069     for content i
-00010d30: 6e20 7265 7370 2e67 6574 2827 436f 6e74  n resp.get('Cont
-00010d40: 656e 7473 272c 205b 5d29 3a0a 2020 2020  ents', []):.    
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 7369 7a65 202b 3d20 636f 6e74 656e 745b  size += content[
-00010d70: 2753 697a 6527 5d0a 2020 2020 2020 2020  'Size'].        
-00010d80: 2020 2020 2020 2020 2020 2020 6c61 7374              last
-00010d90: 5f6d 6f64 6966 6965 6420 3d20 636f 6e74  _modified = cont
-00010da0: 656e 745b 274c 6173 744d 6f64 6966 6965  ent['LastModifie
-00010db0: 6427 5d2e 7469 6d65 7374 616d 7028 290a  d'].timestamp().
-00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dd0: 2020 2020 6966 206d 7469 6d65 203c 206c      if mtime < l
-00010de0: 6173 745f 6d6f 6469 6669 6564 3a0a 2020  ast_modified:.  
-00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 2020 2020 2020 6d74 696d 6520 3d20 6c61        mtime = la
-00010e10: 7374 5f6d 6f64 6966 6965 640a 0a20 2020  st_modified..   
-00010e20: 2020 2020 2072 6574 7572 6e20 5374 6174       return Stat
-00010e30: 5265 7375 6c74 2873 697a 653d 7369 7a65  Result(size=size
-00010e40: 2c20 6d74 696d 653d 6d74 696d 652c 2069  , mtime=mtime, i
-00010e50: 7364 6972 3d54 7275 6529 0a0a 2020 2020  sdir=True)..    
-00010e60: 6465 6620 7374 6174 2873 656c 662c 2066  def stat(self, f
-00010e70: 6f6c 6c6f 775f 7379 6d6c 696e 6b73 3d54  ollow_symlinks=T
-00010e80: 7275 6529 202d 3e20 5374 6174 5265 7375  rue) -> StatResu
-00010e90: 6c74 3a0a 2020 2020 2020 2020 2727 270a  lt:.        '''.
-00010ea0: 2020 2020 2020 2020 4765 7420 5374 6174          Get Stat
-00010eb0: 5265 7375 6c74 206f 6620 7333 5f75 726c  Result of s3_url
-00010ec0: 2066 696c 652c 2069 6e63 6c75 6469 6e67   file, including
-00010ed0: 2066 696c 6520 7369 7a65 2061 6e64 206d   file size and m
-00010ee0: 7469 6d65 2c20 7265 6665 7272 696e 6720  time, referring 
-00010ef0: 746f 2073 335f 6765 7473 697a 6520 616e  to s3_getsize an
-00010f00: 6420 7333 5f67 6574 6d74 696d 650a 0a20  d s3_getmtime.. 
-00010f10: 2020 2020 2020 2049 6620 7333 5f75 726c         If s3_url
-00010f20: 2069 7320 6e6f 7420 616e 2065 7869 7374   is not an exist
-00010f30: 656e 7420 7061 7468 2c20 7768 6963 6820  ent path, which 
-00010f40: 6d65 616e 7320 7333 5f65 7869 7374 2873  means s3_exist(s
-00010f50: 335f 7572 6c29 2072 6574 7572 6e73 2046  3_url) returns F
-00010f60: 616c 7365 2c20 7468 656e 2072 6169 7365  alse, then raise
-00010f70: 2053 3346 696c 654e 6f74 466f 756e 6445   S3FileNotFoundE
-00010f80: 7272 6f72 0a20 2020 2020 2020 2049 6620  rror.        If 
-00010f90: 6174 7465 6d70 7420 746f 2067 6574 2053  attempt to get S
-00010fa0: 7461 7452 6573 756c 7420 6f66 2063 6f6d  tatResult of com
-00010fb0: 706c 6574 6520 7333 2c20 7375 6368 2061  plete s3, such a
-00010fc0: 7320 7333 5f64 6972 5f75 726c 203d 3d20  s s3_dir_url == 
-00010fd0: 2773 333a 2f2f 272c 2072 6169 7365 2053  's3://', raise S
-00010fe0: 3342 7563 6b65 744e 6f74 466f 756e 6445  3BucketNotFoundE
-00010ff0: 7272 6f72 0a0a 2020 2020 2020 2020 3a72  rror..        :r
-00011000: 6574 7572 6e73 3a20 5374 6174 5265 7375  eturns: StatResu
-00011010: 6c74 0a20 2020 2020 2020 203a 7261 6973  lt.        :rais
-00011020: 6573 3a20 5333 4669 6c65 4e6f 7446 6f75  es: S3FileNotFou
-00011030: 6e64 4572 726f 722c 2053 3342 7563 6b65  ndError, S3Bucke
-00011040: 744e 6f74 466f 756e 6445 7272 6f72 0a20  tNotFoundError. 
-00011050: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00011060: 2020 2069 736c 6e6b 203d 2046 616c 7365     islnk = False
-00011070: 0a20 2020 2020 2020 2062 7563 6b65 742c  .        bucket,
-00011080: 206b 6579 203d 2070 6172 7365 5f73 335f   key = parse_s3_
-00011090: 7572 6c28 7365 6c66 2e70 6174 685f 7769  url(self.path_wi
-000110a0: 7468 5f70 726f 746f 636f 6c29 0a20 2020  th_protocol).   
-000110b0: 2020 2020 2069 6620 6e6f 7420 6275 636b       if not buck
-000110c0: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-000110d0: 7261 6973 6520 5333 4275 636b 6574 4e6f  raise S3BucketNo
-000110e0: 7446 6f75 6e64 4572 726f 7228 0a20 2020  tFoundError(.   
-000110f0: 2020 2020 2020 2020 2020 2020 2027 456d               'Em
-00011100: 7074 7920 6275 636b 6574 206e 616d 653a  pty bucket name:
-00011110: 2025 7227 2025 2073 656c 662e 7061 7468   %r' % self.path
-00011120: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
-00011130: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00011140: 7365 6c66 2e69 735f 6669 6c65 2829 3a0a  self.is_file():.
-00011150: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011160: 726e 2073 656c 662e 5f67 6574 6469 7273  rn self._getdirs
-00011170: 7461 7428 290a 0a20 2020 2020 2020 2063  tat()..        c
-00011180: 6c69 656e 7420 3d20 7365 6c66 2e5f 636c  lient = self._cl
-00011190: 6965 6e74 0a20 2020 2020 2020 2077 6974  ient.        wit
-000111a0: 6820 7261 6973 655f 7333 5f65 7272 6f72  h raise_s3_error
-000111b0: 2873 656c 662e 7061 7468 5f77 6974 685f  (self.path_with_
-000111c0: 7072 6f74 6f63 6f6c 293a 0a20 2020 2020  protocol):.     
-000111d0: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-000111e0: 2063 6c69 656e 742e 6865 6164 5f6f 626a   client.head_obj
-000111f0: 6563 7428 4275 636b 6574 3d62 7563 6b65  ect(Bucket=bucke
-00011200: 742c 204b 6579 3d6b 6579 290a 2020 2020  t, Key=key).    
-00011210: 2020 2020 2020 2020 6966 2027 4d65 7461          if 'Meta
-00011220: 6461 7461 2720 696e 2063 6f6e 7465 6e74  data' in content
-00011230: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011240: 2020 6d65 7461 6461 7461 203d 2064 6963    metadata = dic
-00011250: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00011260: 2020 2020 2020 2028 6b65 792e 6c6f 7765         (key.lowe
-00011270: 7228 292c 2076 616c 7565 290a 2020 2020  r(), value).    
-00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011290: 666f 7220 6b65 792c 2076 616c 7565 2069  for key, value i
-000112a0: 6e20 636f 6e74 656e 745b 274d 6574 6164  n content['Metad
-000112b0: 6174 6127 5d2e 6974 656d 7328 2929 0a20  ata'].items()). 
-000112c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000112d0: 6620 6d65 7461 6461 7461 2061 6e64 2027  f metadata and '
-000112e0: 7379 6d6c 696e 6b5f 746f 2720 696e 206d  symlink_to' in m
-000112f0: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
-00011300: 2020 2020 2020 2020 2020 2020 2069 736c               isl
-00011310: 6e6b 203d 2054 7275 650a 2020 2020 2020  nk = True.      
-00011320: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011330: 2069 736c 6e6b 2061 6e64 2066 6f6c 6c6f   islnk and follo
-00011340: 775f 7379 6d6c 696e 6b73 3a0a 2020 2020  w_symlinks:.    
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2020 7333 5f75 726c 203d 206d 6574      s3_url = met
-00011370: 6164 6174 615b 2773 796d 6c69 6e6b 5f74  adata['symlink_t
-00011380: 6f27 5d0a 2020 2020 2020 2020 2020 2020  o'].            
-00011390: 2020 2020 2020 2020 2020 2020 6275 636b              buck
-000113a0: 6574 2c20 6b65 7920 3d20 7061 7273 655f  et, key = parse_
-000113b0: 7333 5f75 726c 2873 335f 7572 6c29 0a20  s3_url(s3_url). 
-000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113d0: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-000113e0: 2063 6c69 656e 742e 6865 6164 5f6f 626a   client.head_obj
-000113f0: 6563 7428 4275 636b 6574 3d62 7563 6b65  ect(Bucket=bucke
-00011400: 742c 204b 6579 3d6b 6579 290a 2020 2020  t, Key=key).    
-00011410: 2020 2020 2020 2020 7374 6174 5f72 6563          stat_rec
-00011420: 6f72 6420 3d20 5374 6174 5265 7375 6c74  ord = StatResult
-00011430: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011440: 2020 6973 6c6e 6b3d 6973 6c6e 6b2c 0a20    islnk=islnk,. 
-00011450: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011460: 697a 653d 636f 6e74 656e 745b 2743 6f6e  ize=content['Con
-00011470: 7465 6e74 4c65 6e67 7468 275d 2c0a 2020  tentLength'],.  
-00011480: 2020 2020 2020 2020 2020 2020 2020 6d74                mt
-00011490: 696d 653d 636f 6e74 656e 745b 274c 6173  ime=content['Las
-000114a0: 744d 6f64 6966 6965 6427 5d2e 7469 6d65  tModified'].time
-000114b0: 7374 616d 7028 292c 0a20 2020 2020 2020  stamp(),.       
-000114c0: 2020 2020 2020 2020 2065 7874 7261 3d63           extra=c
-000114d0: 6f6e 7465 6e74 290a 2020 2020 2020 2020  ontent).        
-000114e0: 7265 7475 726e 2073 7461 745f 7265 636f  return stat_reco
-000114f0: 7264 0a0a 2020 2020 6465 6620 6c73 7461  rd..    def lsta
-00011500: 7428 7365 6c66 2920 2d3e 2053 7461 7452  t(self) -> StatR
-00011510: 6573 756c 743a 0a20 2020 2020 2020 2027  esult:.        '
-00011520: 2727 4c69 6b65 2050 6174 682e 7374 6174  ''Like Path.stat
-00011530: 2829 2062 7574 2c20 6966 2074 6865 2070  () but, if the p
-00011540: 6174 6820 706f 696e 7473 2074 6f20 6120  ath points to a 
-00011550: 7379 6d62 6f6c 6963 206c 696e 6b2c 2072  symbolic link, r
-00011560: 6574 7572 6e20 7468 6520 7379 6d62 6f6c  eturn the symbol
-00011570: 6963 206c 696e 6be2 8099 7320 696e 666f  ic link...s info
-00011580: 726d 6174 696f 6e20 7261 7468 6572 2074  rmation rather t
-00011590: 6861 6e20 6974 7320 7461 7267 6574 e280  han its target..
-000115a0: 9973 2e27 2727 0a20 2020 2020 2020 2072  .s.'''.        r
-000115b0: 6574 7572 6e20 7365 6c66 2e73 7461 7428  eturn self.stat(
-000115c0: 666f 6c6c 6f77 5f73 796d 6c69 6e6b 733d  follow_symlinks=
-000115d0: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
-000115e0: 756e 6c69 6e6b 2873 656c 662c 206d 6973  unlink(self, mis
-000115f0: 7369 6e67 5f6f 6b3a 2062 6f6f 6c20 3d20  sing_ok: bool = 
-00011600: 4661 6c73 6529 202d 3e20 4e6f 6e65 3a0a  False) -> None:.
-00011610: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00011620: 2020 2020 5265 6d6f 7665 2074 6865 2066      Remove the f
-00011630: 696c 6520 6f6e 2073 330a 0a20 2020 2020  ile on s3..     
-00011640: 2020 203a 7061 7261 6d20 6d69 7373 696e     :param missin
-00011650: 675f 6f6b 3a20 6966 2046 616c 7365 2061  g_ok: if False a
-00011660: 6e64 2074 6172 6765 7420 6669 6c65 206e  nd target file n
-00011670: 6f74 2065 7869 7374 732c 2072 6169 7365  ot exists, raise
-00011680: 2053 3346 696c 654e 6f74 466f 756e 6445   S3FileNotFoundE
-00011690: 7272 6f72 0a20 2020 2020 2020 203a 7261  rror.        :ra
-000116a0: 6973 6573 3a20 5333 5065 726d 6973 7369  ises: S3Permissi
-000116b0: 6f6e 4572 726f 722c 2053 3346 696c 654e  onError, S3FileN
-000116c0: 6f74 466f 756e 6445 7272 6f72 2c20 5333  otFoundError, S3
-000116d0: 4973 4144 6972 6563 746f 7279 4572 726f  IsADirectoryErro
-000116e0: 720a 2020 2020 2020 2020 2727 270a 2020  r.        '''.  
-000116f0: 2020 2020 2020 6275 636b 6574 2c20 6b65        bucket, ke
-00011700: 7920 3d20 7061 7273 655f 7333 5f75 726c  y = parse_s3_url
-00011710: 2873 656c 662e 7061 7468 5f77 6974 685f  (self.path_with_
-00011720: 7072 6f74 6f63 6f6c 290a 2020 2020 2020  protocol).      
-00011730: 2020 6966 206e 6f74 2062 7563 6b65 7420    if not bucket 
-00011740: 6f72 206e 6f74 206b 6579 206f 7220 6b65  or not key or ke
-00011750: 792e 656e 6473 7769 7468 2827 2f27 293a  y.endswith('/'):
-00011760: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00011770: 7365 2053 3349 7341 4469 7265 6374 6f72  se S3IsADirector
-00011780: 7945 7272 6f72 280a 2020 2020 2020 2020  yError(.        
-00011790: 2020 2020 2020 2020 2749 7320 6120 6469          'Is a di
-000117a0: 7265 6374 6f72 793a 2025 7227 2025 2073  rectory: %r' % s
-000117b0: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
-000117c0: 6f74 6f63 6f6c 290a 2020 2020 2020 2020  otocol).        
-000117d0: 6966 206e 6f74 2073 656c 662e 6973 5f66  if not self.is_f
-000117e0: 696c 6528 293a 0a20 2020 2020 2020 2020  ile():.         
-000117f0: 2020 2069 6620 6d69 7373 696e 675f 6f6b     if missing_ok
-00011800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011810: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00011820: 2020 2020 2072 6169 7365 2053 3346 696c       raise S3Fil
-00011830: 654e 6f74 466f 756e 6445 7272 6f72 280a  eNotFoundError(.
-00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011850: 274e 6f20 7375 6368 2066 696c 653a 2025  'No such file: %
-00011860: 7227 2025 2073 656c 662e 7061 7468 5f77  r' % self.path_w
-00011870: 6974 685f 7072 6f74 6f63 6f6c 290a 0a20  ith_protocol).. 
-00011880: 2020 2020 2020 2077 6974 6820 7261 6973         with rais
-00011890: 655f 7333 5f65 7272 6f72 2873 656c 662e  e_s3_error(self.
-000118a0: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
-000118b0: 6f6c 293a 0a20 2020 2020 2020 2020 2020  ol):.           
-000118c0: 2073 656c 662e 5f63 6c69 656e 742e 6465   self._client.de
-000118d0: 6c65 7465 5f6f 626a 6563 7428 4275 636b  lete_object(Buck
-000118e0: 6574 3d62 7563 6b65 742c 204b 6579 3d6b  et=bucket, Key=k
-000118f0: 6579 290a 0a20 2020 2064 6566 2077 616c  ey)..    def wal
-00011900: 6b28 7365 6c66 2c20 666f 6c6c 6f77 6c69  k(self, followli
-00011910: 6e6b 733a 2062 6f6f 6c20 3d20 4661 6c73  nks: bool = Fals
-00011920: 650a 2020 2020 2020 2020 2020 2020 2920  e.            ) 
-00011930: 2d3e 2049 7465 7261 746f 725b 5475 706c  -> Iterator[Tupl
-00011940: 655b 7374 722c 204c 6973 745b 7374 725d  e[str, List[str]
-00011950: 2c20 4c69 7374 5b73 7472 5d5d 5d3a 0a20  , List[str]]]:. 
-00011960: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00011970: 2020 2049 7465 7261 7469 7665 6c79 2074     Iteratively t
-00011980: 7261 7665 7273 6520 7468 6520 6769 7665  raverse the give
-00011990: 6e20 7333 2064 6972 6563 746f 7279 2c20  n s3 directory, 
-000119a0: 696e 2074 6f70 2d62 6f74 746f 6d20 6f72  in top-bottom or
-000119b0: 6465 722e 2049 6e20 6f74 6865 7220 776f  der. In other wo
-000119c0: 7264 732c 2066 6972 7374 6c79 2074 7261  rds, firstly tra
-000119d0: 7665 7273 6520 7061 7265 6e74 2064 6972  verse parent dir
-000119e0: 6563 746f 7279 2c20 6966 2073 7562 6469  ectory, if subdi
-000119f0: 7265 6374 6f72 6965 7320 6578 6973 742c  rectories exist,
-00011a00: 2074 7261 7665 7273 6520 7468 6520 7375   traverse the su
-00011a10: 6264 6972 6563 746f 7269 6573 2069 6e20  bdirectories in 
-00011a20: 616c 7068 6162 6574 6963 616c 206f 7264  alphabetical ord
-00011a30: 6572 2e0a 2020 2020 2020 2020 4576 6572  er..        Ever
-00011a40: 7920 6974 6572 6174 696f 6e20 6f6e 2067  y iteration on g
-00011a50: 656e 6572 6174 6f72 2079 6965 6c64 7320  enerator yields 
-00011a60: 6120 332d 7475 706c 653a 2028 726f 6f74  a 3-tuple: (root
-00011a70: 2c20 6469 7273 2c20 6669 6c65 7329 0a0a  , dirs, files)..
-00011a80: 2020 2020 2020 2020 2d20 726f 6f74 3a20          - root: 
-00011a90: 4375 7272 656e 7420 7333 2070 6174 683b  Current s3 path;
-00011aa0: 0a20 2020 2020 2020 202d 2064 6972 733a  .        - dirs:
-00011ab0: 204e 616d 6520 6c69 7374 206f 6620 7375   Name list of su
-00011ac0: 6264 6972 6563 746f 7269 6573 2069 6e20  bdirectories in 
-00011ad0: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
-00011ae0: 792e 2054 6865 206c 6973 7420 6973 2073  y. The list is s
-00011af0: 6f72 7465 6420 6279 206e 616d 6520 696e  orted by name in
-00011b00: 2061 7363 656e 6469 6e67 2061 6c70 6861   ascending alpha
-00011b10: 6265 7469 6361 6c20 6f72 6465 723b 0a20  betical order;. 
-00011b20: 2020 2020 2020 202d 2066 696c 6573 3a20         - files: 
-00011b30: 4e61 6d65 206c 6973 7420 6f66 2066 696c  Name list of fil
-00011b40: 6573 2069 6e20 6375 7272 656e 7420 6469  es in current di
-00011b50: 7265 6374 6f72 792e 2054 6865 206c 6973  rectory. The lis
-00011b60: 7420 6973 2073 6f72 7465 6420 6279 206e  t is sorted by n
-00011b70: 616d 6520 696e 2061 7363 656e 6469 6e67  ame in ascending
-00011b80: 2061 6c70 6861 6265 7469 6361 6c20 6f72   alphabetical or
-00011b90: 6465 723b 0a0a 2020 2020 2020 2020 4966  der;..        If
-00011ba0: 2073 335f 7572 6c20 6973 2061 2066 696c   s3_url is a fil
-00011bb0: 6520 7061 7468 2c20 7265 7475 726e 2061  e path, return a
-00011bc0: 6e20 656d 7074 7920 6765 6e65 7261 746f  n empty generato
-00011bd0: 720a 2020 2020 2020 2020 4966 2073 335f  r.        If s3_
-00011be0: 7572 6c20 6973 2061 206e 6f6e 2d65 7869  url is a non-exi
-00011bf0: 7374 656e 7420 7061 7468 2c20 7265 7475  stent path, retu
-00011c00: 726e 2061 6e20 656d 7074 7920 6765 6e65  rn an empty gene
-00011c10: 7261 746f 720a 2020 2020 2020 2020 4966  rator.        If
-00011c20: 2073 335f 7572 6c20 6973 2061 2062 7563   s3_url is a buc
-00011c30: 6b65 7420 7061 7468 2c20 6275 636b 6574  ket path, bucket
-00011c40: 2077 696c 6c20 6265 2074 6865 2074 6f70   will be the top
-00011c50: 2064 6972 6563 746f 7279 2c20 616e 6420   directory, and 
-00011c60: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
-00011c70: 2061 7420 6669 7273 7420 6974 6572 6174   at first iterat
-00011c80: 696f 6e20 6f66 2067 656e 6572 6174 6f72  ion of generator
-00011c90: 0a20 2020 2020 2020 2049 6620 7333 5f75  .        If s3_u
-00011ca0: 726c 2069 7320 616e 2065 6d70 7479 2062  rl is an empty b
-00011cb0: 7563 6b65 742c 206f 6e6c 7920 7969 656c  ucket, only yiel
-00011cc0: 6420 6f6e 6520 332d 7475 706c 6520 286e  d one 3-tuple (n
-00011cd0: 6f74 6573 3a20 7333 2064 6f65 736e 2774  otes: s3 doesn't
-00011ce0: 2068 6176 6520 656d 7074 7920 6469 7265   have empty dire
-00011cf0: 6374 6f72 7929 0a20 2020 2020 2020 2049  ctory).        I
-00011d00: 6620 7333 5f75 726c 2064 6f65 736e 2774  f s3_url doesn't
-00011d10: 2063 6f6e 7461 696e 2061 6e79 2062 7563   contain any buc
-00011d20: 6b65 742c 2077 6869 6368 2069 7320 7333  ket, which is s3
-00011d30: 5f75 726c 203d 3d20 2773 333a 2f2f 272c  _url == 's3://',
-00011d40: 2072 6169 7365 2055 6e73 7570 706f 7274   raise Unsupport
-00011d50: 6564 4572 726f 722e 2077 616c 6b28 2920  edError. walk() 
-00011d60: 6f6e 2063 6f6d 706c 6574 6520 7333 2069  on complete s3 i
-00011d70: 7320 6e6f 7420 7375 7070 6f72 7465 6420  s not supported 
-00011d80: 696e 206d 6567 6669 6c65 0a0a 2020 2020  in megfile..    
-00011d90: 2020 2020 3a70 6172 616d 2066 6f6c 6c6f      :param follo
-00011da0: 776c 696e 6b73 3a20 7768 6574 6865 7220  wlinks: whether 
-00011db0: 666f 6c6c 6f77 6c69 6e6b 7320 6973 2054  followlinks is T
-00011dc0: 7275 6520 6f72 2046 616c 7365 2c20 7265  rue or False, re
-00011dd0: 7375 6c74 2069 7320 7468 6520 7361 6d65  sult is the same
-00011de0: 2e20 4265 6361 7573 6520 7333 2073 796d  . Because s3 sym
-00011df0: 6c69 6e6b 206e 6f74 2073 7570 706f 7274  link not support
-00011e00: 2064 6972 2e0a 2020 2020 2020 2020 3a72   dir..        :r
-00011e10: 6169 7365 733a 2055 6e73 7570 706f 7274  aises: Unsupport
-00011e20: 6564 4572 726f 720a 2020 2020 2020 2020  edError.        
-00011e30: 3a72 6574 7572 6e73 3a20 4120 332d 7475  :returns: A 3-tu
-00011e40: 706c 6520 6765 6e65 7261 746f 720a 2020  ple generator.  
-00011e50: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00011e60: 2020 6275 636b 6574 2c20 6b65 7920 3d20    bucket, key = 
-00011e70: 7061 7273 655f 7333 5f75 726c 2873 656c  parse_s3_url(sel
-00011e80: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
-00011e90: 6f63 6f6c 290a 2020 2020 2020 2020 6966  ocol).        if
-00011ea0: 206e 6f74 2062 7563 6b65 743a 0a20 2020   not bucket:.   
-00011eb0: 2020 2020 2020 2020 2072 6169 7365 2055           raise U
-00011ec0: 6e73 7570 706f 7274 6564 4572 726f 7228  nsupportedError(
-00011ed0: 2757 616c 6b20 7768 6f6c 6520 7333 272c  'Walk whole s3',
-00011ee0: 2073 656c 662e 7061 7468 5f77 6974 685f   self.path_with_
-00011ef0: 7072 6f74 6f63 6f6c 290a 0a20 2020 2020  protocol)..     
-00011f00: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
-00011f10: 735f 6469 7228 293a 0a20 2020 2020 2020  s_dir():.       
-00011f20: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00011f30: 2020 2020 2073 7461 636b 203d 205b 6b65       stack = [ke
-00011f40: 795d 0a20 2020 2020 2020 2063 6c69 656e  y].        clien
-00011f50: 7420 3d20 7365 6c66 2e5f 636c 6965 6e74  t = self._client
-00011f60: 0a20 2020 2020 2020 2077 6869 6c65 206c  .        while l
-00011f70: 656e 2873 7461 636b 2920 3e20 303a 0a20  en(stack) > 0:. 
-00011f80: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00011f90: 6e74 203d 205f 6265 636f 6d65 5f70 7265  nt = _become_pre
-00011fa0: 6669 7828 7374 6163 6b2e 706f 7028 2929  fix(stack.pop())
-00011fb0: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-00011fc0: 732c 2066 696c 6573 203d 205b 5d2c 205b  s, files = [], [
-00011fd0: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00011fe0: 7220 7265 7370 2069 6e20 5f6c 6973 745f  r resp in _list_
-00011ff0: 6f62 6a65 6374 735f 7265 6375 7273 6976  objects_recursiv
-00012000: 6528 636c 6965 6e74 2c20 6275 636b 6574  e(client, bucket
-00012010: 2c20 6375 7272 656e 742c 2027 2f27 293a  , current, '/'):
-00012020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012030: 2066 6f72 2063 6f6d 6d6f 6e5f 7072 6566   for common_pref
-00012040: 6978 2069 6e20 7265 7370 2e67 6574 2827  ix in resp.get('
-00012050: 436f 6d6d 6f6e 5072 6566 6978 6573 272c  CommonPrefixes',
-00012060: 205b 5d29 3a0a 2020 2020 2020 2020 2020   []):.          
-00012070: 2020 2020 2020 2020 2020 6469 7273 2e61            dirs.a
-00012080: 7070 656e 6428 636f 6d6d 6f6e 5f70 7265  ppend(common_pre
-00012090: 6669 785b 2750 7265 6669 7827 5d5b 3a2d  fix['Prefix'][:-
-000120a0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-000120b0: 2020 2020 666f 7220 636f 6e74 656e 7420      for content 
-000120c0: 696e 2072 6573 702e 6765 7428 2743 6f6e  in resp.get('Con
-000120d0: 7465 6e74 7327 2c20 5b5d 293a 0a20 2020  tents', []):.   
-000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120f0: 2066 696c 6573 2e61 7070 656e 6428 636f   files.append(co
-00012100: 6e74 656e 745b 274b 6579 275d 290a 0a20  ntent['Key']).. 
-00012110: 2020 2020 2020 2020 2020 2064 6972 7320             dirs 
-00012120: 3d20 736f 7274 6564 2864 6972 7329 0a20  = sorted(dirs). 
-00012130: 2020 2020 2020 2020 2020 2073 7461 636b             stack
-00012140: 2e65 7874 656e 6428 7265 7665 7273 6564  .extend(reversed
-00012150: 2864 6972 7329 290a 0a20 2020 2020 2020  (dirs))..       
-00012160: 2020 2020 2072 6f6f 7420 3d20 7333 5f70       root = s3_p
-00012170: 6174 685f 6a6f 696e 280a 2020 2020 2020  ath_join(.      
-00012180: 2020 2020 2020 2020 2020 6627 7b73 656c            f'{sel
-00012190: 662e 5f70 726f 746f 636f 6c5f 7769 7468  f._protocol_with
-000121a0: 5f70 726f 6669 6c65 7d3a 2f2f 272c 2062  _profile}://', b
-000121b0: 7563 6b65 742c 2063 7572 7265 6e74 295b  ucket, current)[
-000121c0: 3a2d 315d 0a20 2020 2020 2020 2020 2020  :-1].           
-000121d0: 2064 6972 7320 3d20 5b70 6174 685b 6c65   dirs = [path[le
-000121e0: 6e28 6375 7272 656e 7429 3a5d 2066 6f72  n(current):] for
-000121f0: 2070 6174 6820 696e 2064 6972 735d 0a20   path in dirs]. 
-00012200: 2020 2020 2020 2020 2020 2066 696c 6573             files
-00012210: 203d 2073 6f72 7465 6428 7061 7468 5b6c   = sorted(path[l
-00012220: 656e 2863 7572 7265 6e74 293a 5d20 666f  en(current):] fo
-00012230: 7220 7061 7468 2069 6e20 6669 6c65 7329  r path in files)
-00012240: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
-00012250: 6c64 2072 6f6f 742c 2064 6972 732c 2066  ld root, dirs, f
-00012260: 696c 6573 0a0a 2020 2020 6465 6620 6d64  iles..    def md
-00012270: 3528 7365 6c66 2c20 7265 6361 6c63 756c  5(self, recalcul
-00012280: 6174 653a 2062 6f6f 6c20 3d20 4661 6c73  ate: bool = Fals
-00012290: 652c 2066 6f6c 6c6f 776c 696e 6b73 3a20  e, followlinks: 
-000122a0: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
-000122b0: 2073 7472 3a0a 2020 2020 2020 2020 2727   str:.        ''
-000122c0: 270a 2020 2020 2020 2020 4765 7420 6d64  '.        Get md
-000122d0: 3520 6d65 7461 2069 6e66 6f20 696e 2066  5 meta info in f
-000122e0: 696c 6573 2074 6861 7420 7570 6c6f 6164  iles that upload
-000122f0: 6564 2f63 6f70 6965 6420 7669 6120 6d65  ed/copied via me
-00012300: 6766 696c 650a 0a20 2020 2020 2020 2049  gfile..        I
-00012310: 6620 6d65 7461 2069 6e66 6f20 6973 206c  f meta info is l
-00012320: 6f73 7420 6f72 206e 6f6e 2d65 7869 7374  ost or non-exist
-00012330: 656e 742c 2072 6574 7572 6e20 4e6f 6e65  ent, return None
-00012340: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00012350: 2072 6563 616c 6375 6c61 7465 3a20 6361   recalculate: ca
-00012360: 6c63 756c 6174 6520 6d64 3520 696e 2072  lculate md5 in r
-00012370: 6561 6c2d 7469 6d65 206f 7220 7265 7475  eal-time or retu
-00012380: 726e 2073 3320 6574 6167 0a20 2020 2020  rn s3 etag.     
-00012390: 2020 203a 7061 7261 6d20 666f 6c6c 6f77     :param follow
-000123a0: 6c69 6e6b 733a 2049 6620 6973 2054 7275  links: If is Tru
-000123b0: 652c 2063 616c 6375 6c61 7465 206d 6435  e, calculate md5
-000123c0: 2066 6f72 2072 6561 6c20 6669 6c65 0a20   for real file. 
-000123d0: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
-000123e0: 206d 6435 206d 6574 6120 696e 666f 0a20   md5 meta info. 
-000123f0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00012400: 2020 2062 7563 6b65 742c 205f 203d 2070     bucket, _ = p
-00012410: 6172 7365 5f73 335f 7572 6c28 7365 6c66  arse_s3_url(self
-00012420: 2e70 6174 685f 7769 7468 5f70 726f 746f  .path_with_proto
-00012430: 636f 6c29 0a20 2020 2020 2020 2069 6620  col).        if 
-00012440: 6e6f 7420 6275 636b 6574 3a0a 2020 2020  not bucket:.    
-00012450: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
-00012460: 4275 636b 6574 4e6f 7446 6f75 6e64 4572  BucketNotFoundEr
-00012470: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00012480: 2020 2020 2027 456d 7074 7920 6275 636b       'Empty buck
-00012490: 6574 206e 616d 653a 2025 7227 2025 2073  et name: %r' % s
-000124a0: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
-000124b0: 6f74 6f63 6f6c 290a 2020 2020 2020 2020  otocol).        
-000124c0: 7374 6174 203d 2073 656c 662e 7374 6174  stat = self.stat
-000124d0: 2866 6f6c 6c6f 775f 7379 6d6c 696e 6b73  (follow_symlinks
-000124e0: 3d66 6f6c 6c6f 776c 696e 6b73 290a 2020  =followlinks).  
-000124f0: 2020 2020 2020 6966 2073 7461 742e 6973        if stat.is
-00012500: 6469 723a 0a20 2020 2020 2020 2020 2020  dir:.           
-00012510: 2068 6173 685f 6d64 3520 3d20 6861 7368   hash_md5 = hash
-00012520: 6c69 622e 6d64 3528 2920 2023 206e 6f73  lib.md5()  # nos
-00012530: 6563 0a20 2020 2020 2020 2020 2020 2066  ec.            f
-00012540: 6f72 2066 696c 655f 6e61 6d65 2069 6e20  or file_name in 
-00012550: 7365 6c66 2e6c 6973 7464 6972 2829 3a0a  self.listdir():.
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 6368 756e 6b20 3d20 5333 5061 7468 280a  chunk = S3Path(.
-00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012590: 2020 2020 7333 5f70 6174 685f 6a6f 696e      s3_path_join
-000125a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000125b0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000125c0: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
-000125d0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-000125e0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-000125f0: 6e61 6d65 2929 2e6d 6435 2872 6563 616c  name)).md5(recal
-00012600: 6375 6c61 7465 3d72 6563 616c 6375 6c61  culate=recalcula
-00012610: 7465 292e 656e 636f 6465 2829 0a20 2020  te).encode().   
-00012620: 2020 2020 2020 2020 2020 2020 2068 6173               has
-00012630: 685f 6d64 352e 7570 6461 7465 2863 6875  h_md5.update(chu
-00012640: 6e6b 290a 2020 2020 2020 2020 2020 2020  nk).            
-00012650: 7265 7475 726e 2068 6173 685f 6d64 352e  return hash_md5.
-00012660: 6865 7864 6967 6573 7428 290a 2020 2020  hexdigest().    
-00012670: 2020 2020 6966 2072 6563 616c 6375 6c61      if recalcula
-00012680: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-00012690: 7061 7468 5f69 6e73 7461 6e63 6520 3d20  path_instance = 
-000126a0: 7365 6c66 0a20 2020 2020 2020 2020 2020  self.           
-000126b0: 2069 6620 666f 6c6c 6f77 6c69 6e6b 733a   if followlinks:
-000126c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000126d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000126e0: 2020 2020 2020 2020 2020 7061 7468 5f69            path_i
-000126f0: 6e73 7461 6e63 6520 3d20 7365 6c66 2e72  nstance = self.r
-00012700: 6561 646c 696e 6b28 290a 2020 2020 2020  eadlink().      
-00012710: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00012720: 2053 334e 6f74 414c 696e 6b45 7272 6f72   S3NotALinkError
-00012730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012740: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00012750: 2020 2020 2020 2077 6974 6820 7061 7468         with path
-00012760: 5f69 6e73 7461 6e63 652e 6f70 656e 2827  _instance.open('
-00012770: 7262 2729 2061 7320 663a 0a20 2020 2020  rb') as f:.     
-00012780: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00012790: 6e20 6361 6c63 756c 6174 655f 6d64 3528  n calculate_md5(
-000127a0: 6629 0a20 2020 2020 2020 2072 6574 7572  f).        retur
-000127b0: 6e20 7374 6174 2e65 7874 7261 2e67 6574  n stat.extra.get
-000127c0: 2827 4554 6167 272c 2027 2729 5b31 3a2d  ('ETag', '')[1:-
-000127d0: 315d 0a0a 2020 2020 6465 6620 636f 7079  1]..    def copy
-000127e0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-000127f0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00012800: 6473 745f 7572 6c3a 2050 6174 684c 696b  dst_url: PathLik
-00012810: 652c 0a20 2020 2020 2020 2020 2020 2066  e,.            f
-00012820: 6f6c 6c6f 776c 696e 6b73 3a20 626f 6f6c  ollowlinks: bool
-00012830: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00012840: 2020 2020 2020 6361 6c6c 6261 636b 3a20        callback: 
-00012850: 4f70 7469 6f6e 616c 5b43 616c 6c61 626c  Optional[Callabl
-00012860: 655b 5b69 6e74 5d2c 204e 6f6e 655d 5d20  e[[int], None]] 
-00012870: 3d20 4e6f 6e65 2920 2d3e 204e 6f6e 653a  = None) -> None:
-00012880: 0a20 2020 2020 2020 2027 2727 2046 696c  .        ''' Fil
-00012890: 6520 636f 7079 206f 6e20 5333 0a20 2020  e copy on S3.   
-000128a0: 2020 2020 2043 6f70 7920 636f 6e74 656e       Copy conten
-000128b0: 7420 6f66 2066 696c 6520 6f6e 2060 7372  t of file on `sr
-000128c0: 635f 7061 7468 6020 746f 2060 6473 745f  c_path` to `dst_
-000128d0: 7061 7468 602e 0a20 2020 2020 2020 2049  path`..        I
-000128e0: 7427 7320 6361 6c6c 6572 2773 2072 6573  t's caller's res
-000128f0: 706f 6e73 6562 696c 6974 7920 746f 2065  ponsebility to e
-00012900: 6e73 7572 6520 7468 6520 7333 5f69 7366  nsure the s3_isf
-00012910: 696c 6528 7372 635f 7572 6c29 203d 3d20  ile(src_url) == 
-00012920: 5472 7565 0a0a 2020 2020 2020 2020 3a70  True..        :p
-00012930: 6172 616d 2064 7374 5f70 6174 683a 2054  aram dst_path: T
-00012940: 6172 6765 7420 6669 6c65 2070 6174 680a  arget file path.
-00012950: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-00012960: 616c 6c62 6163 6b3a 2043 616c 6c65 6420  allback: Called 
-00012970: 7065 7269 6f64 6963 616c 6c79 2064 7572  periodically dur
-00012980: 696e 6720 636f 7079 2c20 616e 6420 7468  ing copy, and th
-00012990: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
-000129a0: 7220 6973 2074 6865 2064 6174 6120 7369  r is the data si
-000129b0: 7a65 2028 696e 2062 7974 6573 2920 6f66  ze (in bytes) of
-000129c0: 2063 6f70 7920 7369 6e63 6520 7468 6520   copy since the 
-000129d0: 6c61 7374 2063 616c 6c0a 2020 2020 2020  last call.      
-000129e0: 2020 2727 270a 2020 2020 2020 2020 7372    '''.        sr
-000129f0: 635f 7572 6c20 3d20 7365 6c66 2e70 6174  c_url = self.pat
-00012a00: 685f 7769 7468 5f70 726f 746f 636f 6c0a  h_with_protocol.
-00012a10: 2020 2020 2020 2020 7372 635f 6275 636b          src_buck
-00012a20: 6574 2c20 7372 635f 6b65 7920 3d20 7061  et, src_key = pa
-00012a30: 7273 655f 7333 5f75 726c 2873 7263 5f75  rse_s3_url(src_u
-00012a40: 726c 290a 2020 2020 2020 2020 6473 745f  rl).        dst_
-00012a50: 6275 636b 6574 2c20 6473 745f 6b65 7920  bucket, dst_key 
-00012a60: 3d20 7061 7273 655f 7333 5f75 726c 2864  = parse_s3_url(d
-00012a70: 7374 5f75 726c 290a 0a20 2020 2020 2020  st_url)..       
-00012a80: 2069 6620 6e6f 7420 7372 635f 6275 636b   if not src_buck
-00012a90: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-00012aa0: 7261 6973 6520 5333 4275 636b 6574 4e6f  raise S3BucketNo
-00012ab0: 7446 6f75 6e64 4572 726f 7228 2745 6d70  tFoundError('Emp
-00012ac0: 7479 2062 7563 6b65 7420 6e61 6d65 3a20  ty bucket name: 
-00012ad0: 2572 2720 2520 7372 635f 7572 6c29 0a20  %r' % src_url). 
-00012ae0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00012af0: 735f 6469 7228 293a 0a20 2020 2020 2020  s_dir():.       
-00012b00: 2020 2020 2072 6169 7365 2053 3349 7341       raise S3IsA
-00012b10: 4469 7265 6374 6f72 7945 7272 6f72 2827  DirectoryError('
-00012b20: 4973 2061 2064 6972 6563 746f 7279 3a20  Is a directory: 
-00012b30: 2572 2720 2520 7372 635f 7572 6c29 0a0a  %r' % src_url)..
-00012b40: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
-00012b50: 7374 5f62 7563 6b65 743a 0a20 2020 2020  st_bucket:.     
-00012b60: 2020 2020 2020 2072 6169 7365 2053 3342         raise S3B
-00012b70: 7563 6b65 744e 6f74 466f 756e 6445 7272  ucketNotFoundErr
-00012b80: 6f72 2827 456d 7074 7920 6275 636b 6574  or('Empty bucket
-00012b90: 206e 616d 653a 2025 7227 2025 2064 7374   name: %r' % dst
-00012ba0: 5f75 726c 290a 2020 2020 2020 2020 6966  _url).        if
-00012bb0: 206e 6f74 2064 7374 5f6b 6579 206f 7220   not dst_key or 
-00012bc0: 6473 745f 6b65 792e 656e 6473 7769 7468  dst_key.endswith
-00012bd0: 2827 2f27 293a 0a20 2020 2020 2020 2020  ('/'):.         
-00012be0: 2020 2072 6169 7365 2053 3349 7341 4469     raise S3IsADi
-00012bf0: 7265 6374 6f72 7945 7272 6f72 2827 4973  rectoryError('Is
-00012c00: 2061 2064 6972 6563 746f 7279 3a20 2572   a directory: %r
-00012c10: 2720 2520 6473 745f 7572 6c29 0a0a 2020  ' % dst_url)..  
-00012c20: 2020 2020 2020 6966 2066 6f6c 6c6f 776c        if followl
-00012c30: 696e 6b73 3a0a 2020 2020 2020 2020 2020  inks:.          
-00012c40: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00012c50: 2020 2020 2020 2073 335f 7572 6c20 3d20         s3_url = 
-00012c60: 7365 6c66 2e72 6561 646c 696e 6b28 292e  self.readlink().
-00012c70: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-00012c80: 2020 2020 2073 7263 5f62 7563 6b65 742c       src_bucket,
-00012c90: 2073 7263 5f6b 6579 203d 2070 6172 7365   src_key = parse
-00012ca0: 5f73 335f 7572 6c28 7333 5f75 726c 290a  _s3_url(s3_url).
-00012cb0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00012cc0: 7074 2053 334e 6f74 414c 696e 6b45 7272  pt S3NotALinkErr
-00012cd0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00012ce0: 2020 2020 7061 7373 0a0a 2020 2020 2020      pass..      
-00012cf0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00012d00: 2020 2073 656c 662e 5f63 6c69 656e 742e     self._client.
-00012d10: 636f 7079 280a 2020 2020 2020 2020 2020  copy(.          
-00012d20: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00012d30: 2020 2020 2020 2020 2020 2020 2742 7563              'Buc
-00012d40: 6b65 7427 3a20 7372 635f 6275 636b 6574  ket': src_bucket
-00012d50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012d60: 2020 2020 2020 274b 6579 273a 2073 7263        'Key': src
-00012d70: 5f6b 6579 2c0a 2020 2020 2020 2020 2020  _key,.          
-00012d80: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00012d90: 2020 2020 2020 2020 2042 7563 6b65 743d           Bucket=
-00012da0: 6473 745f 6275 636b 6574 2c0a 2020 2020  dst_bucket,.    
-00012db0: 2020 2020 2020 2020 2020 2020 4b65 793d              Key=
-00012dc0: 6473 745f 6b65 792c 0a20 2020 2020 2020  dst_key,.       
-00012dd0: 2020 2020 2020 2020 2043 616c 6c62 6163           Callbac
-00012de0: 6b3d 6361 6c6c 6261 636b 290a 2020 2020  k=callback).    
-00012df0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00012e00: 7469 6f6e 2061 7320 6572 726f 723a 0a20  tion as error:. 
-00012e10: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00012e20: 203d 2074 7261 6e73 6c61 7465 5f73 335f   = translate_s3_
-00012e30: 6572 726f 7228 6572 726f 722c 2064 7374  error(error, dst
-00012e40: 5f75 726c 290a 2020 2020 2020 2020 2020  _url).          
-00012e50: 2020 2320 4572 726f 7220 6361 6e27 7420    # Error can't 
-00012e60: 6865 6c70 2074 656c 6c20 7768 6963 6820  help tell which 
-00012e70: 6973 2070 726f 626c 656d 6174 6963 0a20  is problematic. 
-00012e80: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00012e90: 696e 7374 616e 6365 2865 7272 6f72 2c20  instance(error, 
-00012ea0: 5333 4275 636b 6574 4e6f 7446 6f75 6e64  S3BucketNotFound
-00012eb0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00012ec0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00012ed0: 656c 662e 6861 7362 7563 6b65 7428 293a  elf.hasbucket():
-00012ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ef0: 2020 2020 2072 6169 7365 2053 3342 7563       raise S3Buc
-00012f00: 6b65 744e 6f74 466f 756e 6445 7272 6f72  ketNotFoundError
-00012f10: 2827 4e6f 2073 7563 6820 6275 636b 6574  ('No such bucket
-00012f20: 3a20 2572 2720 2520 7372 635f 7572 6c29  : %r' % src_url)
-00012f30: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00012f40: 6620 6973 696e 7374 616e 6365 2865 7272  f isinstance(err
-00012f50: 6f72 2c20 5333 4669 6c65 4e6f 7446 6f75  or, S3FileNotFou
-00012f60: 6e64 4572 726f 7229 3a0a 2020 2020 2020  ndError):.      
-00012f70: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00012f80: 2073 656c 662e 6973 5f66 696c 6528 293a   self.is_file():
-00012f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012fa0: 2020 2020 2072 6169 7365 2053 3346 696c       raise S3Fil
-00012fb0: 654e 6f74 466f 756e 6445 7272 6f72 2827  eNotFoundError('
-00012fc0: 4e6f 2073 7563 6820 6669 6c65 3a20 2572  No such file: %r
-00012fd0: 2720 2520 7372 635f 7572 6c29 0a20 2020  ' % src_url).   
-00012fe0: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
-00012ff0: 7272 6f72 0a0a 2020 2020 6465 6620 7379  rror..    def sy
-00013000: 6e63 2873 656c 662c 2064 7374 5f75 726c  nc(self, dst_url
-00013010: 3a20 5061 7468 4c69 6b65 2c20 666f 6c6c  : PathLike, foll
-00013020: 6f77 6c69 6e6b 733a 2062 6f6f 6c20 3d20  owlinks: bool = 
-00013030: 4661 6c73 6529 202d 3e20 4e6f 6e65 3a0a  False) -> None:.
-00013040: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00013050: 2020 2020 436f 7079 2066 696c 652f 6469      Copy file/di
-00013060: 7265 6374 6f72 7920 6f6e 2073 7263 5f75  rectory on src_u
-00013070: 726c 2074 6f20 6473 745f 7572 6c0a 0a20  rl to dst_url.. 
-00013080: 2020 2020 2020 203a 7061 7261 6d20 6473         :param ds
-00013090: 745f 7572 6c3a 2047 6976 656e 2064 6573  t_url: Given des
-000130a0: 7469 6e61 7469 6f6e 2070 6174 680a 2020  tination path.  
-000130b0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000130c0: 2020 666f 7220 7372 635f 6669 6c65 5f70    for src_file_p
-000130d0: 6174 682c 2064 7374 5f66 696c 655f 7061  ath, dst_file_pa
-000130e0: 7468 2069 6e20 5f73 335f 7363 616e 5f70  th in _s3_scan_p
-000130f0: 6169 7273 280a 2020 2020 2020 2020 2020  airs(.          
-00013100: 2020 2020 2020 7365 6c66 2e70 6174 685f        self.path_
-00013110: 7769 7468 5f70 726f 746f 636f 6c2c 2064  with_protocol, d
-00013120: 7374 5f75 726c 293a 0a20 2020 2020 2020  st_url):.       
-00013130: 2020 2020 2073 7263 5f66 696c 655f 7061       src_file_pa
-00013140: 7468 203d 2073 656c 662e 6672 6f6d 5f70  th = self.from_p
-00013150: 6174 6828 7372 635f 6669 6c65 5f70 6174  ath(src_file_pat
-00013160: 6829 0a20 2020 2020 2020 2020 2020 2064  h).            d
-00013170: 7374 5f66 696c 655f 7061 7468 203d 2073  st_file_path = s
-00013180: 656c 662e 6672 6f6d 5f70 6174 6828 6473  elf.from_path(ds
-00013190: 745f 6669 6c65 5f70 6174 6829 0a20 2020  t_file_path).   
-000131a0: 2020 2020 2020 2020 2069 6620 6473 745f           if dst_
-000131b0: 6669 6c65 5f70 6174 682e 6578 6973 7473  file_path.exists
-000131c0: 2829 2061 6e64 2069 735f 7361 6d65 5f66  () and is_same_f
-000131d0: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
-000131e0: 2020 2020 2020 2020 2073 7263 5f66 696c           src_fil
-000131f0: 655f 7061 7468 2e73 7461 7428 292c 2064  e_path.stat(), d
-00013200: 7374 5f66 696c 655f 7061 7468 2e73 7461  st_file_path.sta
-00013210: 7428 292c 2027 636f 7079 2729 3a0a 2020  t(), 'copy'):.  
-00013220: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00013230: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-00013240: 2020 2073 7263 5f66 696c 655f 7061 7468     src_file_path
-00013250: 2e63 6f70 7928 6473 745f 6669 6c65 5f70  .copy(dst_file_p
-00013260: 6174 682c 2066 6f6c 6c6f 776c 696e 6b73  ath, followlinks
-00013270: 3d66 6f6c 6c6f 776c 696e 6b73 290a 0a20  =followlinks).. 
-00013280: 2020 2064 6566 2073 796d 6c69 6e6b 2873     def symlink(s
-00013290: 656c 662c 2064 7374 5f70 6174 683a 2050  elf, dst_path: P
-000132a0: 6174 684c 696b 6529 202d 3e20 4e6f 6e65  athLike) -> None
-000132b0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-000132c0: 2020 2020 2020 4372 6561 7465 2061 2073        Create a s
-000132d0: 796d 626f 6c69 6320 6c69 6e6b 2070 6f69  ymbolic link poi
-000132e0: 6e74 696e 6720 746f 2073 7263 5f70 6174  nting to src_pat
-000132f0: 6820 6e61 6d65 6420 6473 745f 7061 7468  h named dst_path
-00013300: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00013310: 6d20 6473 745f 7061 7468 3a20 4465 7369  m dst_path: Desi
-00013320: 6e61 7469 6f6e 2070 6174 680a 2020 2020  nation path.    
-00013330: 2020 2020 3a72 6169 7365 733a 2053 334e      :raises: S3N
-00013340: 616d 6554 6f6f 4c6f 6e67 4572 726f 722c  ameTooLongError,
-00013350: 2053 3342 7563 6b65 744e 6f74 466f 756e   S3BucketNotFoun
-00013360: 6445 7272 6f72 2c20 5333 4973 4144 6972  dError, S3IsADir
-00013370: 6563 746f 7279 4572 726f 720a 2020 2020  ectoryError.    
-00013380: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00013390: 6966 206c 656e 2873 7472 2873 656c 662e  if len(str(self.
-000133a0: 5f73 335f 7061 7468 292e 656e 636f 6465  _s3_path).encode
-000133b0: 2829 2920 3e20 3130 3234 3a0a 2020 2020  ()) > 1024:.    
-000133c0: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
-000133d0: 4e61 6d65 546f 6f4c 6f6e 6745 7272 6f72  NameTooLongError
-000133e0: 2827 4669 6c65 206e 616d 6520 746f 6f20  ('File name too 
-000133f0: 6c6f 6e67 3a20 2572 2720 2520 6473 745f  long: %r' % dst_
-00013400: 7061 7468 290a 2020 2020 2020 2020 7372  path).        sr
-00013410: 635f 6275 636b 6574 2c20 7372 635f 6b65  c_bucket, src_ke
-00013420: 7920 3d20 7061 7273 655f 7333 5f75 726c  y = parse_s3_url
-00013430: 2873 656c 662e 7061 7468 5f77 6974 685f  (self.path_with_
-00013440: 7072 6f74 6f63 6f6c 290a 2020 2020 2020  protocol).      
-00013450: 2020 6473 745f 6275 636b 6574 2c20 6473    dst_bucket, ds
-00013460: 745f 6b65 7920 3d20 7061 7273 655f 7333  t_key = parse_s3
-00013470: 5f75 726c 2864 7374 5f70 6174 6829 0a0a  _url(dst_path)..
-00013480: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00013490: 7263 5f62 7563 6b65 743a 0a20 2020 2020  rc_bucket:.     
-000134a0: 2020 2020 2020 2072 6169 7365 2053 3342         raise S3B
-000134b0: 7563 6b65 744e 6f74 466f 756e 6445 7272  ucketNotFoundErr
-000134c0: 6f72 2827 456d 7074 7920 6275 636b 6574  or('Empty bucket
-000134d0: 206e 616d 653a 2025 7227 2025 2073 656c   name: %r' % sel
-000134e0: 662e 7061 7468 290a 2020 2020 2020 2020  f.path).        
-000134f0: 6966 206e 6f74 2064 7374 5f62 7563 6b65  if not dst_bucke
-00013500: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-00013510: 6169 7365 2053 3342 7563 6b65 744e 6f74  aise S3BucketNot
-00013520: 466f 756e 6445 7272 6f72 2827 456d 7074  FoundError('Empt
-00013530: 7920 6275 636b 6574 206e 616d 653a 2025  y bucket name: %
-00013540: 7227 2025 2064 7374 5f70 6174 6829 0a20  r' % dst_path). 
-00013550: 2020 2020 2020 2069 6620 6e6f 7420 6473         if not ds
-00013560: 745f 6b65 7920 6f72 2064 7374 5f6b 6579  t_key or dst_key
-00013570: 2e65 6e64 7377 6974 6828 272f 2729 3a0a  .endswith('/'):.
-00013580: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00013590: 6520 5333 4973 4144 6972 6563 746f 7279  e S3IsADirectory
-000135a0: 4572 726f 7228 2749 7320 6120 6469 7265  Error('Is a dire
-000135b0: 6374 6f72 793a 2025 7227 2025 2064 7374  ctory: %r' % dst
-000135c0: 5f70 6174 6829 0a0a 2020 2020 2020 2020  _path)..        
-000135d0: 7372 635f 7061 7468 203d 2073 656c 662e  src_path = self.
-000135e0: 5f73 335f 7061 7468 0a20 2020 2020 2020  _s3_path.       
-000135f0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00013600: 2020 7372 635f 7061 7468 203d 2073 656c    src_path = sel
-00013610: 662e 7265 6164 6c69 6e6b 2829 2e5f 7333  f.readlink()._s3
-00013620: 5f70 6174 680a 2020 2020 2020 2020 6578  _path.        ex
-00013630: 6365 7074 2053 334e 6f74 414c 696e 6b45  cept S3NotALinkE
-00013640: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-00013650: 2020 7061 7373 0a20 2020 2020 2020 2077    pass.        w
-00013660: 6974 6820 7261 6973 655f 7333 5f65 7272  ith raise_s3_err
-00013670: 6f72 2864 7374 5f70 6174 6829 3a0a 2020  or(dst_path):.  
-00013680: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00013690: 636c 6965 6e74 2e70 7574 5f6f 626a 6563  client.put_objec
-000136a0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-000136b0: 2020 2042 7563 6b65 743d 6473 745f 6275     Bucket=dst_bu
-000136c0: 636b 6574 2c0a 2020 2020 2020 2020 2020  cket,.          
-000136d0: 2020 2020 2020 4b65 793d 6473 745f 6b65        Key=dst_ke
-000136e0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-000136f0: 2020 204d 6574 6164 6174 613d 7b22 7379     Metadata={"sy
-00013700: 6d6c 696e 6b5f 746f 223a 2073 7263 5f70  mlink_to": src_p
-00013710: 6174 687d 290a 0a20 2020 2064 6566 2072  ath})..    def r
-00013720: 6561 646c 696e 6b28 7365 6c66 2920 2d3e  eadlink(self) ->
-00013730: 2027 5333 5061 7468 273a 0a20 2020 2020   'S3Path':.     
-00013740: 2020 2027 2727 0a20 2020 2020 2020 2052     '''.        R
-00013750: 6574 7572 6e20 6120 5333 5061 7468 2069  eturn a S3Path i
-00013760: 6e73 7461 6e63 6520 7265 7072 6573 656e  nstance represen
-00013770: 7469 6e67 2074 6865 2070 6174 6820 746f  ting the path to
-00013780: 2077 6869 6368 2074 6865 2073 796d 626f   which the symbo
-00013790: 6c69 6320 6c69 6e6b 2070 6f69 6e74 732e  lic link points.
-000137a0: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-000137b0: 6e73 3a20 5265 7475 726e 2061 2053 3350  ns: Return a S3P
-000137c0: 6174 6820 696e 7374 616e 6365 2072 6570  ath instance rep
-000137d0: 7265 7365 6e74 696e 6720 7468 6520 7061  resenting the pa
-000137e0: 7468 2074 6f20 7768 6963 6820 7468 6520  th to which the 
-000137f0: 7379 6d62 6f6c 6963 206c 696e 6b20 706f  symbolic link po
-00013800: 696e 7473 2e0a 2020 2020 2020 2020 3a72  ints..        :r
-00013810: 6169 7365 733a 2053 334e 616d 6554 6f6f  aises: S3NameToo
-00013820: 4c6f 6e67 4572 726f 722c 2053 3342 7563  LongError, S3Buc
-00013830: 6b65 744e 6f74 466f 756e 6445 7272 6f72  ketNotFoundError
-00013840: 2c20 5333 4973 4144 6972 6563 746f 7279  , S3IsADirectory
-00013850: 4572 726f 722c 2053 334e 6f74 414c 696e  Error, S3NotALin
-00013860: 6b45 7272 6f72 0a20 2020 2020 2020 2027  kError.        '
-00013870: 2727 0a20 2020 2020 2020 2062 7563 6b65  ''.        bucke
-00013880: 742c 206b 6579 203d 2070 6172 7365 5f73  t, key = parse_s
-00013890: 335f 7572 6c28 7365 6c66 2e70 6174 685f  3_url(self.path_
-000138a0: 7769 7468 5f70 726f 746f 636f 6c29 0a20  with_protocol). 
-000138b0: 2020 2020 2020 2069 6620 6e6f 7420 6275         if not bu
-000138c0: 636b 6574 3a0a 2020 2020 2020 2020 2020  cket:.          
-000138d0: 2020 7261 6973 6520 5333 4275 636b 6574    raise S3Bucket
-000138e0: 4e6f 7446 6f75 6e64 4572 726f 7228 0a20  NotFoundError(. 
-000138f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00013900: 456d 7074 7920 6275 636b 6574 206e 616d  Empty bucket nam
-00013910: 653a 2025 7227 2025 2073 656c 662e 7061  e: %r' % self.pa
-00013920: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
-00013930: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-00013940: 206b 6579 206f 7220 6b65 792e 656e 6473   key or key.ends
-00013950: 7769 7468 2827 2f27 293a 0a20 2020 2020  with('/'):.     
-00013960: 2020 2020 2020 2072 6169 7365 2053 3349         raise S3I
-00013970: 7341 4469 7265 6374 6f72 7945 7272 6f72  sADirectoryError
-00013980: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00013990: 2020 2749 7320 6120 6469 7265 6374 6f72    'Is a director
-000139a0: 793a 2025 7227 2025 2073 656c 662e 7061  y: %r' % self.pa
-000139b0: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
-000139c0: 290a 2020 2020 2020 2020 6d65 7461 6461  ).        metada
-000139d0: 7461 203d 2073 656c 662e 5f73 335f 6765  ta = self._s3_ge
-000139e0: 745f 6d65 7461 6461 7461 2829 0a0a 2020  t_metadata()..  
-000139f0: 2020 2020 2020 6966 206e 6f74 2027 7379        if not 'sy
-00013a00: 6d6c 696e 6b5f 746f 2720 696e 206d 6574  mlink_to' in met
-00013a10: 6164 6174 613a 0a20 2020 2020 2020 2020  adata:.         
-00013a20: 2020 2072 6169 7365 2053 334e 6f74 414c     raise S3NotAL
-00013a30: 696e 6b45 7272 6f72 2827 4e6f 7420 6120  inkError('Not a 
-00013a40: 6c69 6e6b 3a20 2572 2720 2520 7365 6c66  link: %r' % self
-00013a50: 2e70 6174 685f 7769 7468 5f70 726f 746f  .path_with_proto
-00013a60: 636f 6c29 0a20 2020 2020 2020 2065 6c73  col).        els
-00013a70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00013a80: 6574 7572 6e20 7365 6c66 2e66 726f 6d5f  eturn self.from_
-00013a90: 7061 7468 286d 6574 6164 6174 615b 2773  path(metadata['s
-00013aa0: 796d 6c69 6e6b 5f74 6f27 5d29 0a0a 2020  ymlink_to'])..  
-00013ab0: 2020 6465 6620 6973 5f73 796d 6c69 6e6b    def is_symlink
-00013ac0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-00013ad0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00013ae0: 2020 2020 5465 7374 2077 6865 7468 6572      Test whether
-00013af0: 2061 2070 6174 6820 6973 206c 696e 6b0a   a path is link.
-00013b00: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00013b10: 733a 2054 7275 6520 6966 2061 2070 6174  s: True if a pat
-00013b20: 6820 6973 206c 696e 6b2c 2065 6c73 6520  h is link, else 
-00013b30: 4661 6c73 650a 2020 2020 2020 2020 3a72  False.        :r
-00013b40: 6169 7365 733a 2053 334e 6f74 414c 696e  aises: S3NotALin
-00013b50: 6b45 7272 6f72 0a20 2020 2020 2020 2027  kError.        '
-00013b60: 2727 0a20 2020 2020 2020 2062 7563 6b65  ''.        bucke
-00013b70: 742c 206b 6579 203d 2070 6172 7365 5f73  t, key = parse_s
-00013b80: 335f 7572 6c28 7365 6c66 2e70 6174 685f  3_url(self.path_
-00013b90: 7769 7468 5f70 726f 746f 636f 6c29 0a20  with_protocol). 
-00013ba0: 2020 2020 2020 2069 6620 6e6f 7420 6275         if not bu
-00013bb0: 636b 6574 3a0a 2020 2020 2020 2020 2020  cket:.          
-00013bc0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-00013bd0: 2020 2020 2020 2069 6620 6e6f 7420 6b65         if not ke
-00013be0: 7920 6f72 206b 6579 2e65 6e64 7377 6974  y or key.endswit
-00013bf0: 6828 272f 2729 3a0a 2020 2020 2020 2020  h('/'):.        
-00013c00: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00013c10: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-00013c20: 6120 3d20 7365 6c66 2e5f 7333 5f67 6574  a = self._s3_get
-00013c30: 5f6d 6574 6164 6174 6128 290a 2020 2020  _metadata().    
-00013c40: 2020 2020 7265 7475 726e 2027 7379 6d6c      return 'syml
-00013c50: 696e 6b5f 746f 2720 696e 206d 6574 6164  ink_to' in metad
-00013c60: 6174 610a 0a20 2020 2064 6566 2073 6176  ata..    def sav
-00013c70: 6528 7365 6c66 2c20 6669 6c65 5f6f 626a  e(self, file_obj
-00013c80: 6563 743a 2042 696e 6172 7949 4f29 3a0a  ect: BinaryIO):.
-00013c90: 2020 2020 2020 2020 2727 2757 7269 7465          '''Write
-00013ca0: 2074 6865 206f 7065 6e65 6420 6269 6e61   the opened bina
-00013cb0: 7279 2073 7472 6561 6d20 746f 2073 7065  ry stream to spe
-00013cc0: 6369 6669 6564 2070 6174 682c 2062 7574  cified path, but
-00013cd0: 2074 6865 2073 7472 6561 6d20 776f 6e27   the stream won'
-00013ce0: 7420 6265 2063 6c6f 7365 640a 0a20 2020  t be closed..   
-00013cf0: 2020 2020 203a 7061 7261 6d20 6669 6c65       :param file
-00013d00: 5f6f 626a 6563 743a 2053 7472 6561 6d20  _object: Stream 
-00013d10: 746f 2062 6520 7265 6164 0a20 2020 2020  to be read.     
-00013d20: 2020 2027 2727 0a20 2020 2020 2020 2062     '''.        b
-00013d30: 7563 6b65 742c 206b 6579 203d 2070 6172  ucket, key = par
-00013d40: 7365 5f73 335f 7572 6c28 7365 6c66 2e70  se_s3_url(self.p
-00013d50: 6174 685f 7769 7468 5f70 726f 746f 636f  ath_with_protoco
-00013d60: 6c29 0a20 2020 2020 2020 2069 6620 6e6f  l).        if no
-00013d70: 7420 6275 636b 6574 3a0a 2020 2020 2020  t bucket:.      
-00013d80: 2020 2020 2020 7261 6973 6520 5333 4275        raise S3Bu
-00013d90: 636b 6574 4e6f 7446 6f75 6e64 4572 726f  cketNotFoundErro
-00013da0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00013db0: 2020 2027 456d 7074 7920 6275 636b 6574     'Empty bucket
-00013dc0: 206e 616d 653a 2025 7227 2025 2073 656c   name: %r' % sel
-00013dd0: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
-00013de0: 6f63 6f6c 290a 2020 2020 2020 2020 6966  ocol).        if
-00013df0: 206e 6f74 206b 6579 206f 7220 6b65 792e   not key or key.
-00013e00: 656e 6473 7769 7468 2827 2f27 293a 0a20  endswith('/'):. 
-00013e10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00013e20: 2053 3349 7341 4469 7265 6374 6f72 7945   S3IsADirectoryE
-00013e30: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00013e40: 2020 2020 2020 2749 7320 6120 6469 7265        'Is a dire
-00013e50: 6374 6f72 793a 2025 7227 2025 2073 656c  ctory: %r' % sel
-00013e60: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
-00013e70: 6f63 6f6c 290a 0a20 2020 2020 2020 2077  ocol)..        w
-00013e80: 6974 6820 7261 6973 655f 7333 5f65 7272  ith raise_s3_err
-00013e90: 6f72 2873 656c 662e 7061 7468 5f77 6974  or(self.path_wit
-00013ea0: 685f 7072 6f74 6f63 6f6c 293a 0a20 2020  h_protocol):.   
-00013eb0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00013ec0: 6c69 656e 742e 7570 6c6f 6164 5f66 696c  lient.upload_fil
-00013ed0: 656f 626a 2866 696c 655f 6f62 6a65 6374  eobj(file_object
-00013ee0: 2c20 4275 636b 6574 3d62 7563 6b65 742c  , Bucket=bucket,
-00013ef0: 204b 6579 3d6b 6579 290a 0a20 2020 2064   Key=key)..    d
-00013f00: 6566 206f 7065 6e28 0a20 2020 2020 2020  ef open(.       
-00013f10: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00013f20: 2020 2020 2020 206d 6f64 653a 2073 7472         mode: str
-00013f30: 203d 2027 7227 2c0a 2020 2020 2020 2020   = 'r',.        
-00013f40: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
-00013f50: 2020 2073 335f 6f70 656e 5f66 756e 633a     s3_open_func:
-00013f60: 2043 616c 6c61 626c 655b 5b73 7472 2c20   Callable[[str, 
-00013f70: 7374 725d 2c20 4269 6e61 7279 494f 5d20  str], BinaryIO] 
-00013f80: 3d20 7333 5f6f 7065 6e2c 0a20 2020 2020  = s3_open,.     
-00013f90: 2020 2020 2020 202a 2a6b 7761 7267 7329         **kwargs)
-00013fa0: 202d 3e20 494f 5b41 6e79 5374 725d 3a20   -> IO[AnyStr]: 
-00013fb0: 2023 2070 7974 7970 653a 2064 6973 6162   # pytype: disab
-00013fc0: 6c65 3d73 6967 6e61 7475 7265 2d6d 6973  le=signature-mis
-00013fd0: 6d61 7463 680a 2020 2020 2020 2020 7265  match.        re
-00013fe0: 7475 726e 2073 335f 6f70 656e 5f66 756e  turn s3_open_fun
-00013ff0: 6328 0a20 2020 2020 2020 2020 2020 2073  c(.            s
-00014000: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
-00014010: 6f74 6f63 6f6c 2c20 6d6f 6465 2c0a 2020  otocol, mode,.  
-00014020: 2020 2020 2020 2020 2020 2a2a 6e65 6365            **nece
-00014030: 7373 6172 795f 7061 7261 6d73 2873 335f  ssary_params(s3_
-00014040: 6f70 656e 5f66 756e 632c 202a 2a6b 7761  open_func, **kwa
-00014050: 7267 7329 290a 0a20 2020 2064 6566 2061  rgs))..    def a
-00014060: 6273 6f6c 7574 6528 7365 6c66 2920 2d3e  bsolute(self) ->
-00014070: 2027 5333 5061 7468 273a 0a20 2020 2020   'S3Path':.     
-00014080: 2020 2027 2727 0a20 2020 2020 2020 204d     '''.        M
-00014090: 616b 6520 7468 6520 7061 7468 2061 6273  ake the path abs
-000140a0: 6f6c 7574 652c 2077 6974 686f 7574 206e  olute, without n
-000140b0: 6f72 6d61 6c69 7a61 7469 6f6e 206f 7220  ormalization or 
-000140c0: 7265 736f 6c76 696e 6720 7379 6d6c 696e  resolving symlin
-000140d0: 6b73 2e20 5265 7475 726e 7320 6120 6e65  ks. Returns a ne
-000140e0: 7720 7061 7468 206f 626a 6563 740a 2020  w path object.  
-000140f0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00014100: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
-00014110: 2020 2064 6566 2063 7764 2873 656c 6629     def cwd(self)
-00014120: 202d 3e20 2753 3350 6174 6827 3a0a 2020   -> 'S3Path':.  
-00014130: 2020 2020 2020 2727 2752 6574 7572 6e20        '''Return 
-00014140: 6375 7272 656e 7420 776f 726b 696e 6720  current working 
-00014150: 6469 7265 6374 6f72 790a 0a20 2020 2020  directory..     
-00014160: 2020 2072 6574 7572 6e73 3a20 4375 7272     returns: Curr
-00014170: 656e 7420 776f 726b 696e 6720 6469 7265  ent working dire
-00014180: 6374 6f72 790a 2020 2020 2020 2020 2727  ctory.        ''
-00014190: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
-000141a0: 2073 656c 662e 6672 6f6d 5f70 6174 6828   self.from_path(
-000141b0: 7365 6c66 2e70 6174 685f 7769 7468 5f70  self.path_with_p
-000141c0: 726f 746f 636f 6c29 0a0a 0a63 6c61 7373  rotocol)...class
-000141d0: 204d 756c 7469 5061 7274 5772 6974 6572   MultiPartWriter
-000141e0: 3a0a 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-000141f0: 745f 5f28 7365 6c66 2c20 636c 6965 6e74  t__(self, client
-00014200: 2c20 7061 7468 3a20 5061 7468 4c69 6b65  , path: PathLike
-00014210: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00014220: 2020 2073 656c 662e 5f63 6c69 656e 7420     self._client 
-00014230: 3d20 636c 6965 6e74 0a20 2020 2020 2020  = client.       
-00014240: 2073 656c 662e 5f6d 756c 7469 7061 7274   self._multipart
-00014250: 5f75 706c 6f61 645f 696e 666f 203d 205b  _upload_info = [
-00014260: 5d0a 0a20 2020 2020 2020 2062 7563 6b65  ]..        bucke
-00014270: 742c 206b 6579 203d 2070 6172 7365 5f73  t, key = parse_s
-00014280: 335f 7572 6c28 7061 7468 290a 2020 2020  3_url(path).    
-00014290: 2020 2020 7365 6c66 2e5f 6275 636b 6574      self._bucket
-000142a0: 203d 2062 7563 6b65 740a 2020 2020 2020   = bucket.      
-000142b0: 2020 7365 6c66 2e5f 6b65 7920 3d20 6b65    self._key = ke
-000142c0: 790a 2020 2020 2020 2020 7365 6c66 2e5f  y.        self._
-000142d0: 7570 6c6f 6164 5f69 6420 3d20 7365 6c66  upload_id = self
-000142e0: 2e5f 636c 6965 6e74 2e63 7265 6174 655f  ._client.create_
-000142f0: 6d75 6c74 6970 6172 745f 7570 6c6f 6164  multipart_upload
-00014300: 280a 2020 2020 2020 2020 2020 2020 4275  (.            Bu
-00014310: 636b 6574 3d73 656c 662e 5f62 7563 6b65  cket=self._bucke
-00014320: 742c 204b 6579 3d73 656c 662e 5f6b 6579  t, Key=self._key
-00014330: 295b 2755 706c 6f61 6449 6427 5d0a 0a20  )['UploadId'].. 
-00014340: 2020 2064 6566 2075 706c 6f61 645f 7061     def upload_pa
-00014350: 7274 2873 656c 662c 2070 6172 745f 6e75  rt(self, part_nu
-00014360: 6d3a 2069 6e74 2c20 6669 6c65 5f6f 626a  m: int, file_obj
-00014370: 3a20 696f 2e42 7974 6573 494f 2920 2d3e  : io.BytesIO) ->
-00014380: 204e 6f6e 653a 0a20 2020 2020 2020 2072   None:.        r
-00014390: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-000143a0: 636c 6965 6e74 2e75 706c 6f61 645f 7061  client.upload_pa
-000143b0: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-000143c0: 426f 6479 3d66 696c 655f 6f62 6a2c 0a20  Body=file_obj,. 
-000143d0: 2020 2020 2020 2020 2020 2055 706c 6f61             Uploa
-000143e0: 6449 643d 7365 6c66 2e5f 7570 6c6f 6164  dId=self._upload
-000143f0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00014400: 2050 6172 744e 756d 6265 723d 7061 7274   PartNumber=part
-00014410: 5f6e 756d 2c0a 2020 2020 2020 2020 2020  _num,.          
-00014420: 2020 4275 636b 6574 3d73 656c 662e 5f62    Bucket=self._b
-00014430: 7563 6b65 742c 0a20 2020 2020 2020 2020  ucket,.         
-00014440: 2020 204b 6579 3d73 656c 662e 5f6b 6579     Key=self._key
-00014450: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00014460: 2020 2020 7365 6c66 2e5f 6d75 6c74 6970      self._multip
-00014470: 6172 745f 7570 6c6f 6164 5f69 6e66 6f2e  art_upload_info.
-00014480: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-00014490: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000144a0: 2020 2020 2020 2750 6172 744e 756d 6265        'PartNumbe
-000144b0: 7227 3a20 7061 7274 5f6e 756d 2c0a 2020  r': part_num,.  
-000144c0: 2020 2020 2020 2020 2020 2020 2020 2745                'E
-000144d0: 5461 6727 3a20 7265 7370 6f6e 7365 5b27  Tag': response['
-000144e0: 4554 6167 275d 0a20 2020 2020 2020 2020  ETag'].         
-000144f0: 2020 207d 290a 0a20 2020 2064 6566 2075     })..    def u
-00014500: 706c 6f61 645f 7061 7274 5f62 795f 7061  pload_part_by_pa
-00014510: 7468 7328 0a20 2020 2020 2020 2020 2020  ths(.           
-00014520: 2073 656c 662c 2070 6172 745f 6e75 6d3a   self, part_num:
-00014530: 2069 6e74 2c20 7061 7468 733a 204c 6973   int, paths: Lis
-00014540: 745b 5475 706c 655b 5061 7468 4c69 6b65  t[Tuple[PathLike
-00014550: 2c20 7374 725d 5d29 202d 3e20 4e6f 6e65  , str]]) -> None
-00014560: 3a0a 2020 2020 2020 2020 6669 6c65 5f6f  :.        file_o
-00014570: 626a 203d 2069 6f2e 4279 7465 7349 4f28  bj = io.BytesIO(
-00014580: 290a 2020 2020 2020 2020 666f 7220 7061  ).        for pa
-00014590: 7468 2c20 6279 7465 735f 7261 6e67 6520  th, bytes_range 
-000145a0: 696e 2070 6174 6873 3a0a 2020 2020 2020  in paths:.      
-000145b0: 2020 2020 2020 6275 636b 6574 2c20 6b65        bucket, ke
-000145c0: 7920 3d20 7061 7273 655f 7333 5f75 726c  y = parse_s3_url
-000145d0: 2870 6174 6829 0a20 2020 2020 2020 2020  (path).         
-000145e0: 2020 2069 6620 6279 7465 735f 7261 6e67     if bytes_rang
-000145f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00014600: 2020 2066 696c 655f 6f62 6a2e 7772 6974     file_obj.writ
-00014610: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00014620: 2020 2020 2020 2073 656c 662e 5f63 6c69         self._cli
-00014630: 656e 742e 6765 745f 6f62 6a65 6374 280a  ent.get_object(.
-00014640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014650: 2020 2020 2020 2020 4275 636b 6574 3d62          Bucket=b
-00014660: 7563 6b65 742c 204b 6579 3d6b 6579 2c0a  ucket, Key=key,.
-00014670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014680: 2020 2020 2020 2020 5261 6e67 653d 6279          Range=by
-00014690: 7465 735f 7261 6e67 6529 5b27 426f 6479  tes_range)['Body
-000146a0: 275d 2e72 6561 6428 2929 0a20 2020 2020  '].read()).     
-000146b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000146c0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000146d0: 655f 6f62 6a2e 7772 6974 6528 0a20 2020  e_obj.write(.   
-000146e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146f0: 2073 656c 662e 5f63 6c69 656e 742e 6765   self._client.ge
-00014700: 745f 6f62 6a65 6374 2842 7563 6b65 743d  t_object(Bucket=
-00014710: 6275 636b 6574 2c0a 2020 2020 2020 2020  bucket,.        
-00014720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014740: 2020 2020 4b65 793d 6b65 7929 5b27 426f      Key=key)['Bo
-00014750: 6479 275d 2e72 6561 6428 2929 0a20 2020  dy'].read()).   
-00014760: 2020 2020 2066 696c 655f 6f62 6a2e 7365       file_obj.se
-00014770: 656b 2830 2c20 6f73 2e53 4545 4b5f 5345  ek(0, os.SEEK_SE
-00014780: 5429 0a20 2020 2020 2020 2073 656c 662e  T).        self.
-00014790: 7570 6c6f 6164 5f70 6172 7428 7061 7274  upload_part(part
-000147a0: 5f6e 756d 2c20 6669 6c65 5f6f 626a 290a  _num, file_obj).
-000147b0: 0a20 2020 2064 6566 2075 706c 6f61 645f  .    def upload_
-000147c0: 7061 7274 5f63 6f70 7928 0a20 2020 2020  part_copy(.     
-000147d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000147e0: 2020 2020 2020 2020 2070 6172 745f 6e75           part_nu
-000147f0: 6d3a 2069 6e74 2c0a 2020 2020 2020 2020  m: int,.        
-00014800: 2020 2020 7061 7468 3a20 5061 7468 4c69      path: PathLi
-00014810: 6b65 2c0a 2020 2020 2020 2020 2020 2020  ke,.            
-00014820: 636f 7079 5f73 6f75 7263 655f 7261 6e67  copy_source_rang
-00014830: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-00014840: 203d 204e 6f6e 6529 202d 3e20 4e6f 6e65   = None) -> None
-00014850: 3a0a 2020 2020 2020 2020 6275 636b 6574  :.        bucket
-00014860: 2c20 6b65 7920 3d20 7061 7273 655f 7333  , key = parse_s3
-00014870: 5f75 726c 2870 6174 6829 0a20 2020 2020  _url(path).     
-00014880: 2020 2070 6172 616d 7320 3d20 6469 6374     params = dict
-00014890: 280a 2020 2020 2020 2020 2020 2020 5570  (.            Up
-000148a0: 6c6f 6164 4964 3d73 656c 662e 5f75 706c  loadId=self._upl
-000148b0: 6f61 645f 6964 2c0a 2020 2020 2020 2020  oad_id,.        
-000148c0: 2020 2020 5061 7274 4e75 6d62 6572 3d70      PartNumber=p
-000148d0: 6172 745f 6e75 6d2c 0a20 2020 2020 2020  art_num,.       
-000148e0: 2020 2020 2043 6f70 7953 6f75 7263 653d       CopySource=
-000148f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00014900: 2020 2742 7563 6b65 7427 3a20 6275 636b    'Bucket': buck
-00014910: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
-00014920: 2020 2020 274b 6579 273a 206b 6579 0a20      'Key': key. 
-00014930: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00014940: 2020 2020 2020 2020 2020 4275 636b 6574            Bucket
-00014950: 3d73 656c 662e 5f62 7563 6b65 742c 0a20  =self._bucket,. 
-00014960: 2020 2020 2020 2020 2020 204b 6579 3d73             Key=s
-00014970: 656c 662e 5f6b 6579 2c0a 2020 2020 2020  elf._key,.      
-00014980: 2020 290a 2020 2020 2020 2020 6966 2063    ).        if c
-00014990: 6f70 795f 736f 7572 6365 5f72 616e 6765  opy_source_range
-000149a0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-000149b0: 7261 6d73 5b27 436f 7079 536f 7572 6365  rams['CopySource
-000149c0: 5261 6e67 6527 5d20 3d20 636f 7079 5f73  Range'] = copy_s
-000149d0: 6f75 7263 655f 7261 6e67 650a 2020 2020  ource_range.    
-000149e0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-000149f0: 656c 662e 5f63 6c69 656e 742e 7570 6c6f  elf._client.uplo
-00014a00: 6164 5f70 6172 745f 636f 7079 282a 2a70  ad_part_copy(**p
-00014a10: 6172 616d 7329 0a20 2020 2020 2020 2073  arams).        s
-00014a20: 656c 662e 5f6d 756c 7469 7061 7274 5f75  elf._multipart_u
-00014a30: 706c 6f61 645f 696e 666f 2e61 7070 656e  pload_info.appen
-00014a40: 6428 0a20 2020 2020 2020 2020 2020 207b  d(.            {
-00014a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014a60: 2027 5061 7274 4e75 6d62 6572 273a 2070   'PartNumber': p
-00014a70: 6172 745f 6e75 6d2c 0a20 2020 2020 2020  art_num,.       
-00014a80: 2020 2020 2020 2020 2027 4554 6167 273a           'ETag':
-00014a90: 2072 6573 706f 6e73 655b 2743 6f70 7950   response['CopyP
-00014aa0: 6172 7452 6573 756c 7427 5d5b 2745 5461  artResult']['ETa
-00014ab0: 6727 5d0a 2020 2020 2020 2020 2020 2020  g'].            
-00014ac0: 7d29 0a0a 2020 2020 6465 6620 636c 6f73  })..    def clos
-00014ad0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00014ae0: 2073 656c 662e 5f6d 756c 7469 7061 7274   self._multipart
-00014af0: 5f75 706c 6f61 645f 696e 666f 2e73 6f72  _upload_info.sor
-00014b00: 7428 6b65 793d 6c61 6d62 6461 2074 3a20  t(key=lambda t: 
-00014b10: 745b 2750 6172 744e 756d 6265 7227 5d29  t['PartNumber'])
-00014b20: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00014b30: 6c69 656e 742e 636f 6d70 6c65 7465 5f6d  lient.complete_m
-00014b40: 756c 7469 7061 7274 5f75 706c 6f61 6428  ultipart_upload(
-00014b50: 0a20 2020 2020 2020 2020 2020 2055 706c  .            Upl
-00014b60: 6f61 6449 643d 7365 6c66 2e5f 7570 6c6f  oadId=self._uplo
-00014b70: 6164 5f69 642c 0a20 2020 2020 2020 2020  ad_id,.         
-00014b80: 2020 2042 7563 6b65 743d 7365 6c66 2e5f     Bucket=self._
-00014b90: 6275 636b 6574 2c0a 2020 2020 2020 2020  bucket,.        
-00014ba0: 2020 2020 4b65 793d 7365 6c66 2e5f 6b65      Key=self._ke
-00014bb0: 792c 0a20 2020 2020 2020 2020 2020 204d  y,.            M
-00014bc0: 756c 7469 7061 7274 5570 6c6f 6164 3d7b  ultipartUpload={
-00014bd0: 2750 6172 7473 273a 2073 656c 662e 5f6d  'Parts': self._m
-00014be0: 756c 7469 7061 7274 5f75 706c 6f61 645f  ultipart_upload_
-00014bf0: 696e 666f 7d29 0a0a 2020 2020 6465 6620  info})..    def 
-00014c00: 5f5f 656e 7465 725f 5f28 7365 6c66 293a  __enter__(self):
-00014c10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014c20: 7365 6c66 0a0a 2020 2020 6465 6620 5f5f  self..    def __
-00014c30: 6578 6974 5f5f 2873 656c 662c 2065 7863  exit__(self, exc
-00014c40: 5f74 7970 652c 2065 7863 5f76 616c 2c20  _type, exc_val, 
-00014c50: 6578 635f 7462 293a 0a20 2020 2020 2020  exc_tb):.       
-00014c60: 2073 656c 662e 636c 6f73 6528 290a        self.close().
+00010670: 2020 2020 2066 6f72 2063 6f6e 7465 6e74       for content
+00010680: 2069 6e20 7265 7370 2e67 6574 2827 436f   in resp.get('Co
+00010690: 6e74 656e 7473 272c 205b 5d29 3a0a 2020  ntents', []):.  
+000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106b0: 2020 2020 2020 7372 635f 7572 6c20 3d20        src_url = 
+000106c0: 6765 6e65 7261 7465 5f73 335f 7061 7468  generate_s3_path
+000106d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000106e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000106f0: 6c66 2e5f 7072 6f74 6f63 6f6c 5f77 6974  lf._protocol_wit
+00010700: 685f 7072 6f66 696c 652c 2062 7563 6b65  h_profile, bucke
+00010710: 742c 2063 6f6e 7465 6e74 5b27 4b65 7927  t, content['Key'
+00010720: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+00010730: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00010740: 6f6c 6c6f 776c 696e 6b73 2061 6e64 2053  ollowlinks and S
+00010750: 3350 6174 6828 7372 635f 7572 6c29 2e69  3Path(src_url).i
+00010760: 735f 7379 6d6c 696e 6b28 293a 0a20 2020  s_symlink():.   
+00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010780: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+00010790: 5b27 6973 6c6e 6b27 5d20 3d20 5472 7565  ['islnk'] = True
+000107a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000107b0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+000107c0: 4669 6c65 456e 7472 7928 0a20 2020 2020  FileEntry(.     
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107e0: 2020 2020 2020 2063 6f6e 7465 6e74 5b27         content['
+000107f0: 4b65 7927 5d5b 6c65 6e28 7072 6566 6978  Key'][len(prefix
+00010800: 293a 5d2c 2073 7263 5f75 726c 2c0a 2020  ):], src_url,.  
+00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010820: 2020 2020 2020 2020 2020 5f6d 616b 655f            _make_
+00010830: 7374 6174 2863 6f6e 7465 6e74 2929 0a0a  stat(content))..
+00010840: 2020 2020 2020 2020 7265 7475 726e 2043          return C
+00010850: 6f6e 7465 7874 4974 6572 6174 6f72 2863  ontextIterator(c
+00010860: 7265 6174 655f 6765 6e65 7261 746f 7228  reate_generator(
+00010870: 2929 0a0a 2020 2020 6465 6620 5f67 6574  ))..    def _get
+00010880: 6469 7273 7461 7428 7365 6c66 2920 2d3e  dirstat(self) ->
+00010890: 2053 7461 7452 6573 756c 743a 0a20 2020   StatResult:.   
+000108a0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+000108b0: 2052 6574 7572 6e20 5374 6174 5265 7375   Return StatResu
+000108c0: 6c74 206f 6620 6769 7665 6e20 7333 5f75  lt of given s3_u
+000108d0: 726c 2064 6972 6563 746f 7279 2c20 696e  rl directory, in
+000108e0: 636c 7564 696e 673a 200a 0a20 2020 2020  cluding: ..     
+000108f0: 2020 2031 2e20 4469 7265 6374 6f72 7920     1. Directory 
+00010900: 7369 7a65 3a20 7468 6520 7375 6d20 6f66  size: the sum of
+00010910: 2061 6c6c 2066 696c 6520 7369 7a65 2069   all file size i
+00010920: 6e20 6974 2c20 696e 636c 7564 696e 6720  n it, including 
+00010930: 6669 6c65 2069 6e20 7375 6264 6972 6563  file in subdirec
+00010940: 746f 7269 6573 2028 6966 2065 7869 7374  tories (if exist
+00010950: 292e 0a20 2020 2020 2020 2054 6865 2072  )..        The r
+00010960: 6573 756c 7420 6578 636c 7564 6573 2074  esult excludes t
+00010970: 6865 2073 697a 6520 6f66 2064 6972 6563  he size of direc
+00010980: 746f 7279 2069 7473 656c 662e 2049 6e20  tory itself. In 
+00010990: 6f74 6865 7220 776f 7264 732c 2072 6574  other words, ret
+000109a0: 7572 6e20 3020 4279 7465 206f 6e20 616e  urn 0 Byte on an
+000109b0: 2065 6d70 7479 2064 6972 6563 746f 7279   empty directory
+000109c0: 2070 6174 680a 2020 2020 2020 2020 322e   path.        2.
+000109d0: 204c 6173 742d 6d6f 6469 6669 6564 2074   Last-modified t
+000109e0: 696d 6520 6f66 2064 6972 6563 746f 7279  ime of directory
+000109f0: 3a20 7265 7475 726e 2074 6865 206c 6174  : return the lat
+00010a00: 6573 7420 6d6f 6469 6669 6564 2074 696d  est modified tim
+00010a10: 6520 6f66 2061 6c6c 2066 696c 6520 696e  e of all file in
+00010a20: 2069 742e 2054 6865 206d 7469 6d65 206f   it. The mtime o
+00010a30: 6620 656d 7074 7920 6469 7265 6374 6f72  f empty director
+00010a40: 7920 6973 2031 3937 302d 3031 2d30 3120  y is 1970-01-01 
+00010a50: 3030 3a30 303a 3030 0a0a 2020 2020 2020  00:00:00..      
+00010a60: 2020 3a72 6574 7572 6e73 3a20 416e 2069    :returns: An i
+00010a70: 6e74 2069 6e64 6963 6174 6573 2073 697a  nt indicates siz
+00010a80: 6520 696e 2042 7974 6573 0a20 2020 2020  e in Bytes.     
+00010a90: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+00010aa0: 6620 6e6f 7420 7365 6c66 2e69 735f 6469  f not self.is_di
+00010ab0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
+00010ac0: 2072 6169 7365 2053 3346 696c 654e 6f74   raise S3FileNot
+00010ad0: 466f 756e 6445 7272 6f72 280a 2020 2020  FoundError(.    
+00010ae0: 2020 2020 2020 2020 2020 2020 274e 6f20              'No 
+00010af0: 7375 6368 2066 696c 6520 6f72 2064 6972  such file or dir
+00010b00: 6563 746f 7279 3a20 2572 2720 2520 7365  ectory: %r' % se
+00010b10: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
+00010b20: 746f 636f 6c29 0a0a 2020 2020 2020 2020  tocol)..        
+00010b30: 6275 636b 6574 2c20 6b65 7920 3d20 7061  bucket, key = pa
+00010b40: 7273 655f 7333 5f75 726c 2873 656c 662e  rse_s3_url(self.
+00010b50: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
+00010b60: 6f6c 290a 2020 2020 2020 2020 7072 6566  ol).        pref
+00010b70: 6978 203d 205f 6265 636f 6d65 5f70 7265  ix = _become_pre
+00010b80: 6669 7828 6b65 7929 0a20 2020 2020 2020  fix(key).       
+00010b90: 2063 6c69 656e 7420 3d20 7365 6c66 2e5f   client = self._
+00010ba0: 636c 6965 6e74 0a20 2020 2020 2020 2073  client.        s
+00010bb0: 697a 6520 3d20 300a 2020 2020 2020 2020  ize = 0.        
+00010bc0: 6d74 696d 6520 3d20 302e 300a 2020 2020  mtime = 0.0.    
+00010bd0: 2020 2020 7769 7468 2072 6169 7365 5f73      with raise_s
+00010be0: 335f 6572 726f 7228 7365 6c66 2e70 6174  3_error(self.pat
+00010bf0: 685f 7769 7468 5f70 726f 746f 636f 6c29  h_with_protocol)
+00010c00: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00010c10: 7220 7265 7370 2069 6e20 5f6c 6973 745f  r resp in _list_
+00010c20: 6f62 6a65 6374 735f 7265 6375 7273 6976  objects_recursiv
+00010c30: 6528 636c 6965 6e74 2c20 6275 636b 6574  e(client, bucket
+00010c40: 2c20 7072 6566 6978 293a 0a20 2020 2020  , prefix):.     
+00010c50: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00010c60: 6f6e 7465 6e74 2069 6e20 7265 7370 2e67  ontent in resp.g
+00010c70: 6574 2827 436f 6e74 656e 7473 272c 205b  et('Contents', [
+00010c80: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00010c90: 2020 2020 2020 2020 7369 7a65 202b 3d20          size += 
+00010ca0: 636f 6e74 656e 745b 2753 697a 6527 5d0a  content['Size'].
+00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cc0: 2020 2020 6c61 7374 5f6d 6f64 6966 6965      last_modifie
+00010cd0: 6420 3d20 636f 6e74 656e 745b 274c 6173  d = content['Las
+00010ce0: 744d 6f64 6966 6965 6427 5d2e 7469 6d65  tModified'].time
+00010cf0: 7374 616d 7028 290a 2020 2020 2020 2020  stamp().        
+00010d00: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00010d10: 7469 6d65 203c 206c 6173 745f 6d6f 6469  time < last_modi
+00010d20: 6669 6564 3a0a 2020 2020 2020 2020 2020  fied:.          
+00010d30: 2020 2020 2020 2020 2020 2020 2020 6d74                mt
+00010d40: 696d 6520 3d20 6c61 7374 5f6d 6f64 6966  ime = last_modif
+00010d50: 6965 640a 0a20 2020 2020 2020 2072 6574  ied..        ret
+00010d60: 7572 6e20 5374 6174 5265 7375 6c74 2873  urn StatResult(s
+00010d70: 697a 653d 7369 7a65 2c20 6d74 696d 653d  ize=size, mtime=
+00010d80: 6d74 696d 652c 2069 7364 6972 3d54 7275  mtime, isdir=Tru
+00010d90: 6529 0a0a 2020 2020 6465 6620 7374 6174  e)..    def stat
+00010da0: 2873 656c 662c 2066 6f6c 6c6f 775f 7379  (self, follow_sy
+00010db0: 6d6c 696e 6b73 3d54 7275 6529 202d 3e20  mlinks=True) -> 
+00010dc0: 5374 6174 5265 7375 6c74 3a0a 2020 2020  StatResult:.    
+00010dd0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00010de0: 4765 7420 5374 6174 5265 7375 6c74 206f  Get StatResult o
+00010df0: 6620 7333 5f75 726c 2066 696c 652c 2069  f s3_url file, i
+00010e00: 6e63 6c75 6469 6e67 2066 696c 6520 7369  ncluding file si
+00010e10: 7a65 2061 6e64 206d 7469 6d65 2c20 7265  ze and mtime, re
+00010e20: 6665 7272 696e 6720 746f 2073 335f 6765  ferring to s3_ge
+00010e30: 7473 697a 6520 616e 6420 7333 5f67 6574  tsize and s3_get
+00010e40: 6d74 696d 650a 0a20 2020 2020 2020 2049  mtime..        I
+00010e50: 6620 7333 5f75 726c 2069 7320 6e6f 7420  f s3_url is not 
+00010e60: 616e 2065 7869 7374 656e 7420 7061 7468  an existent path
+00010e70: 2c20 7768 6963 6820 6d65 616e 7320 7333  , which means s3
+00010e80: 5f65 7869 7374 2873 335f 7572 6c29 2072  _exist(s3_url) r
+00010e90: 6574 7572 6e73 2046 616c 7365 2c20 7468  eturns False, th
+00010ea0: 656e 2072 6169 7365 2053 3346 696c 654e  en raise S3FileN
+00010eb0: 6f74 466f 756e 6445 7272 6f72 0a20 2020  otFoundError.   
+00010ec0: 2020 2020 2049 6620 6174 7465 6d70 7420       If attempt 
+00010ed0: 746f 2067 6574 2053 7461 7452 6573 756c  to get StatResul
+00010ee0: 7420 6f66 2063 6f6d 706c 6574 6520 7333  t of complete s3
+00010ef0: 2c20 7375 6368 2061 7320 7333 5f64 6972  , such as s3_dir
+00010f00: 5f75 726c 203d 3d20 2773 333a 2f2f 272c  _url == 's3://',
+00010f10: 2072 6169 7365 2053 3342 7563 6b65 744e   raise S3BucketN
+00010f20: 6f74 466f 756e 6445 7272 6f72 0a0a 2020  otFoundError..  
+00010f30: 2020 2020 2020 3a72 6574 7572 6e73 3a20        :returns: 
+00010f40: 5374 6174 5265 7375 6c74 0a20 2020 2020  StatResult.     
+00010f50: 2020 203a 7261 6973 6573 3a20 5333 4669     :raises: S3Fi
+00010f60: 6c65 4e6f 7446 6f75 6e64 4572 726f 722c  leNotFoundError,
+00010f70: 2053 3342 7563 6b65 744e 6f74 466f 756e   S3BucketNotFoun
+00010f80: 6445 7272 6f72 0a20 2020 2020 2020 2027  dError.        '
+00010f90: 2727 0a20 2020 2020 2020 2069 736c 6e6b  ''.        islnk
+00010fa0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00010fb0: 2062 7563 6b65 742c 206b 6579 203d 2070   bucket, key = p
+00010fc0: 6172 7365 5f73 335f 7572 6c28 7365 6c66  arse_s3_url(self
+00010fd0: 2e70 6174 685f 7769 7468 5f70 726f 746f  .path_with_proto
+00010fe0: 636f 6c29 0a20 2020 2020 2020 2069 6620  col).        if 
+00010ff0: 6e6f 7420 6275 636b 6574 3a0a 2020 2020  not bucket:.    
+00011000: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
+00011010: 4275 636b 6574 4e6f 7446 6f75 6e64 4572  BucketNotFoundEr
+00011020: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00011030: 2020 2020 2027 456d 7074 7920 6275 636b       'Empty buck
+00011040: 6574 206e 616d 653a 2025 7227 2025 2073  et name: %r' % s
+00011050: 656c 662e 7061 7468 5f77 6974 685f 7072  elf.path_with_pr
+00011060: 6f74 6f63 6f6c 290a 0a20 2020 2020 2020  otocol)..       
+00011070: 2069 6620 6e6f 7420 7365 6c66 2e69 735f   if not self.is_
+00011080: 6669 6c65 2829 3a0a 2020 2020 2020 2020  file():.        
+00011090: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000110a0: 5f67 6574 6469 7273 7461 7428 290a 0a20  _getdirstat().. 
+000110b0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+000110c0: 7365 6c66 2e5f 636c 6965 6e74 0a20 2020  self._client.   
+000110d0: 2020 2020 2077 6974 6820 7261 6973 655f       with raise_
+000110e0: 7333 5f65 7272 6f72 2873 656c 662e 7061  s3_error(self.pa
+000110f0: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
+00011100: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00011110: 6f6e 7465 6e74 203d 2063 6c69 656e 742e  ontent = client.
+00011120: 6865 6164 5f6f 626a 6563 7428 4275 636b  head_object(Buck
+00011130: 6574 3d62 7563 6b65 742c 204b 6579 3d6b  et=bucket, Key=k
+00011140: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
+00011150: 6966 2027 4d65 7461 6461 7461 2720 696e  if 'Metadata' in
+00011160: 2063 6f6e 7465 6e74 3a0a 2020 2020 2020   content:.      
+00011170: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00011180: 7461 203d 2064 6963 7428 0a20 2020 2020  ta = dict(.     
+00011190: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+000111a0: 6b65 792e 6c6f 7765 7228 292c 2076 616c  key.lower(), val
+000111b0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+000111c0: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
+000111d0: 2076 616c 7565 2069 6e20 636f 6e74 656e   value in conten
+000111e0: 745b 274d 6574 6164 6174 6127 5d2e 6974  t['Metadata'].it
+000111f0: 656d 7328 2929 0a20 2020 2020 2020 2020  ems()).         
+00011200: 2020 2020 2020 2069 6620 6d65 7461 6461         if metada
+00011210: 7461 2061 6e64 2027 7379 6d6c 696e 6b5f  ta and 'symlink_
+00011220: 746f 2720 696e 206d 6574 6164 6174 613a  to' in metadata:
+00011230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011240: 2020 2020 2069 736c 6e6b 203d 2054 7275       islnk = Tru
+00011250: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00011260: 2020 2020 2020 6966 2069 736c 6e6b 2061        if islnk a
+00011270: 6e64 2066 6f6c 6c6f 775f 7379 6d6c 696e  nd follow_symlin
+00011280: 6b73 3a0a 2020 2020 2020 2020 2020 2020  ks:.            
+00011290: 2020 2020 2020 2020 2020 2020 7333 5f75              s3_u
+000112a0: 726c 203d 206d 6574 6164 6174 615b 2773  rl = metadata['s
+000112b0: 796d 6c69 6e6b 5f74 6f27 5d0a 2020 2020  ymlink_to'].    
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112d0: 2020 2020 6275 636b 6574 2c20 6b65 7920      bucket, key 
+000112e0: 3d20 7061 7273 655f 7333 5f75 726c 2873  = parse_s3_url(s
+000112f0: 335f 7572 6c29 0a20 2020 2020 2020 2020  3_url).         
+00011300: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011310: 6f6e 7465 6e74 203d 2063 6c69 656e 742e  ontent = client.
+00011320: 6865 6164 5f6f 626a 6563 7428 4275 636b  head_object(Buck
+00011330: 6574 3d62 7563 6b65 742c 204b 6579 3d6b  et=bucket, Key=k
+00011340: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
+00011350: 7374 6174 5f72 6563 6f72 6420 3d20 5374  stat_record = St
+00011360: 6174 5265 7375 6c74 280a 2020 2020 2020  atResult(.      
+00011370: 2020 2020 2020 2020 2020 6973 6c6e 6b3d            islnk=
+00011380: 6973 6c6e 6b2c 0a20 2020 2020 2020 2020  islnk,.         
+00011390: 2020 2020 2020 2073 697a 653d 636f 6e74         size=cont
+000113a0: 656e 745b 2743 6f6e 7465 6e74 4c65 6e67  ent['ContentLeng
+000113b0: 7468 275d 2c0a 2020 2020 2020 2020 2020  th'],.          
+000113c0: 2020 2020 2020 6d74 696d 653d 636f 6e74        mtime=cont
+000113d0: 656e 745b 274c 6173 744d 6f64 6966 6965  ent['LastModifie
+000113e0: 6427 5d2e 7469 6d65 7374 616d 7028 292c  d'].timestamp(),
+000113f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011400: 2065 7874 7261 3d63 6f6e 7465 6e74 290a   extra=content).
+00011410: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011420: 7461 745f 7265 636f 7264 0a0a 2020 2020  tat_record..    
+00011430: 6465 6620 6c73 7461 7428 7365 6c66 2920  def lstat(self) 
+00011440: 2d3e 2053 7461 7452 6573 756c 743a 0a20  -> StatResult:. 
+00011450: 2020 2020 2020 2027 2727 4c69 6b65 2050         '''Like P
+00011460: 6174 682e 7374 6174 2829 2062 7574 2c20  ath.stat() but, 
+00011470: 6966 2074 6865 2070 6174 6820 706f 696e  if the path poin
+00011480: 7473 2074 6f20 6120 7379 6d62 6f6c 6963  ts to a symbolic
+00011490: 206c 696e 6b2c 2072 6574 7572 6e20 7468   link, return th
+000114a0: 6520 7379 6d62 6f6c 6963 206c 696e 6be2  e symbolic link.
+000114b0: 8099 7320 696e 666f 726d 6174 696f 6e20  ..s information 
+000114c0: 7261 7468 6572 2074 6861 6e20 6974 7320  rather than its 
+000114d0: 7461 7267 6574 e280 9973 2e27 2727 0a20  target...s.'''. 
+000114e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000114f0: 6c66 2e73 7461 7428 666f 6c6c 6f77 5f73  lf.stat(follow_s
+00011500: 796d 6c69 6e6b 733d 4661 6c73 6529 0a0a  ymlinks=False)..
+00011510: 2020 2020 6465 6620 756e 6c69 6e6b 2873      def unlink(s
+00011520: 656c 662c 206d 6973 7369 6e67 5f6f 6b3a  elf, missing_ok:
+00011530: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
+00011540: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00011550: 2727 270a 2020 2020 2020 2020 5265 6d6f  '''.        Remo
+00011560: 7665 2074 6865 2066 696c 6520 6f6e 2073  ve the file on s
+00011570: 330a 0a20 2020 2020 2020 203a 7061 7261  3..        :para
+00011580: 6d20 6d69 7373 696e 675f 6f6b 3a20 6966  m missing_ok: if
+00011590: 2046 616c 7365 2061 6e64 2074 6172 6765   False and targe
+000115a0: 7420 6669 6c65 206e 6f74 2065 7869 7374  t file not exist
+000115b0: 732c 2072 6169 7365 2053 3346 696c 654e  s, raise S3FileN
+000115c0: 6f74 466f 756e 6445 7272 6f72 0a20 2020  otFoundError.   
+000115d0: 2020 2020 203a 7261 6973 6573 3a20 5333       :raises: S3
+000115e0: 5065 726d 6973 7369 6f6e 4572 726f 722c  PermissionError,
+000115f0: 2053 3346 696c 654e 6f74 466f 756e 6445   S3FileNotFoundE
+00011600: 7272 6f72 2c20 5333 4973 4144 6972 6563  rror, S3IsADirec
+00011610: 746f 7279 4572 726f 720a 2020 2020 2020  toryError.      
+00011620: 2020 2727 270a 2020 2020 2020 2020 6275    '''.        bu
+00011630: 636b 6574 2c20 6b65 7920 3d20 7061 7273  cket, key = pars
+00011640: 655f 7333 5f75 726c 2873 656c 662e 7061  e_s3_url(self.pa
+00011650: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
+00011660: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00011670: 2062 7563 6b65 7420 6f72 206e 6f74 206b   bucket or not k
+00011680: 6579 206f 7220 6b65 792e 656e 6473 7769  ey or key.endswi
+00011690: 7468 2827 2f27 293a 0a20 2020 2020 2020  th('/'):.       
+000116a0: 2020 2020 2072 6169 7365 2053 3349 7341       raise S3IsA
+000116b0: 4469 7265 6374 6f72 7945 7272 6f72 280a  DirectoryError(.
+000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116d0: 2749 7320 6120 6469 7265 6374 6f72 793a  'Is a directory:
+000116e0: 2025 7227 2025 2073 656c 662e 7061 7468   %r' % self.path
+000116f0: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
+00011700: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00011710: 656c 662e 6973 5f66 696c 6528 293a 0a20  elf.is_file():. 
+00011720: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
+00011730: 7373 696e 675f 6f6b 3a0a 2020 2020 2020  ssing_ok:.      
+00011740: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011750: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00011760: 7365 2053 3346 696c 654e 6f74 466f 756e  se S3FileNotFoun
+00011770: 6445 7272 6f72 280a 2020 2020 2020 2020  dError(.        
+00011780: 2020 2020 2020 2020 274e 6f20 7375 6368          'No such
+00011790: 2066 696c 653a 2025 7227 2025 2073 656c   file: %r' % sel
+000117a0: 662e 7061 7468 5f77 6974 685f 7072 6f74  f.path_with_prot
+000117b0: 6f63 6f6c 290a 0a20 2020 2020 2020 2077  ocol)..        w
+000117c0: 6974 6820 7261 6973 655f 7333 5f65 7272  ith raise_s3_err
+000117d0: 6f72 2873 656c 662e 7061 7468 5f77 6974  or(self.path_wit
+000117e0: 685f 7072 6f74 6f63 6f6c 293a 0a20 2020  h_protocol):.   
+000117f0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00011800: 6c69 656e 742e 6465 6c65 7465 5f6f 626a  lient.delete_obj
+00011810: 6563 7428 4275 636b 6574 3d62 7563 6b65  ect(Bucket=bucke
+00011820: 742c 204b 6579 3d6b 6579 290a 0a20 2020  t, Key=key)..   
+00011830: 2064 6566 2077 616c 6b28 7365 6c66 2c20   def walk(self, 
+00011840: 666f 6c6c 6f77 6c69 6e6b 733a 2062 6f6f  followlinks: boo
+00011850: 6c20 3d20 4661 6c73 650a 2020 2020 2020  l = False.      
+00011860: 2020 2020 2020 2920 2d3e 2049 7465 7261        ) -> Itera
+00011870: 746f 725b 5475 706c 655b 7374 722c 204c  tor[Tuple[str, L
+00011880: 6973 745b 7374 725d 2c20 4c69 7374 5b73  ist[str], List[s
+00011890: 7472 5d5d 5d3a 0a20 2020 2020 2020 2027  tr]]]:.        '
+000118a0: 2727 0a20 2020 2020 2020 2049 7465 7261  ''.        Itera
+000118b0: 7469 7665 6c79 2074 7261 7665 7273 6520  tively traverse 
+000118c0: 7468 6520 6769 7665 6e20 7333 2064 6972  the given s3 dir
+000118d0: 6563 746f 7279 2c20 696e 2074 6f70 2d62  ectory, in top-b
+000118e0: 6f74 746f 6d20 6f72 6465 722e 2049 6e20  ottom order. In 
+000118f0: 6f74 6865 7220 776f 7264 732c 2066 6972  other words, fir
+00011900: 7374 6c79 2074 7261 7665 7273 6520 7061  stly traverse pa
+00011910: 7265 6e74 2064 6972 6563 746f 7279 2c20  rent directory, 
+00011920: 6966 2073 7562 6469 7265 6374 6f72 6965  if subdirectorie
+00011930: 7320 6578 6973 742c 2074 7261 7665 7273  s exist, travers
+00011940: 6520 7468 6520 7375 6264 6972 6563 746f  e the subdirecto
+00011950: 7269 6573 2069 6e20 616c 7068 6162 6574  ries in alphabet
+00011960: 6963 616c 206f 7264 6572 2e0a 2020 2020  ical order..    
+00011970: 2020 2020 4576 6572 7920 6974 6572 6174      Every iterat
+00011980: 696f 6e20 6f6e 2067 656e 6572 6174 6f72  ion on generator
+00011990: 2079 6965 6c64 7320 6120 332d 7475 706c   yields a 3-tupl
+000119a0: 653a 2028 726f 6f74 2c20 6469 7273 2c20  e: (root, dirs, 
+000119b0: 6669 6c65 7329 0a0a 2020 2020 2020 2020  files)..        
+000119c0: 2d20 726f 6f74 3a20 4375 7272 656e 7420  - root: Current 
+000119d0: 7333 2070 6174 683b 0a20 2020 2020 2020  s3 path;.       
+000119e0: 202d 2064 6972 733a 204e 616d 6520 6c69   - dirs: Name li
+000119f0: 7374 206f 6620 7375 6264 6972 6563 746f  st of subdirecto
+00011a00: 7269 6573 2069 6e20 6375 7272 656e 7420  ries in current 
+00011a10: 6469 7265 6374 6f72 792e 2054 6865 206c  directory. The l
+00011a20: 6973 7420 6973 2073 6f72 7465 6420 6279  ist is sorted by
+00011a30: 206e 616d 6520 696e 2061 7363 656e 6469   name in ascendi
+00011a40: 6e67 2061 6c70 6861 6265 7469 6361 6c20  ng alphabetical 
+00011a50: 6f72 6465 723b 0a20 2020 2020 2020 202d  order;.        -
+00011a60: 2066 696c 6573 3a20 4e61 6d65 206c 6973   files: Name lis
+00011a70: 7420 6f66 2066 696c 6573 2069 6e20 6375  t of files in cu
+00011a80: 7272 656e 7420 6469 7265 6374 6f72 792e  rrent directory.
+00011a90: 2054 6865 206c 6973 7420 6973 2073 6f72   The list is sor
+00011aa0: 7465 6420 6279 206e 616d 6520 696e 2061  ted by name in a
+00011ab0: 7363 656e 6469 6e67 2061 6c70 6861 6265  scending alphabe
+00011ac0: 7469 6361 6c20 6f72 6465 723b 0a0a 2020  tical order;..  
+00011ad0: 2020 2020 2020 4966 2073 335f 7572 6c20        If s3_url 
+00011ae0: 6973 2061 2066 696c 6520 7061 7468 2c20  is a file path, 
+00011af0: 7265 7475 726e 2061 6e20 656d 7074 7920  return an empty 
+00011b00: 6765 6e65 7261 746f 720a 2020 2020 2020  generator.      
+00011b10: 2020 4966 2073 335f 7572 6c20 6973 2061    If s3_url is a
+00011b20: 206e 6f6e 2d65 7869 7374 656e 7420 7061   non-existent pa
+00011b30: 7468 2c20 7265 7475 726e 2061 6e20 656d  th, return an em
+00011b40: 7074 7920 6765 6e65 7261 746f 720a 2020  pty generator.  
+00011b50: 2020 2020 2020 4966 2073 335f 7572 6c20        If s3_url 
+00011b60: 6973 2061 2062 7563 6b65 7420 7061 7468  is a bucket path
+00011b70: 2c20 6275 636b 6574 2077 696c 6c20 6265  , bucket will be
+00011b80: 2074 6865 2074 6f70 2064 6972 6563 746f   the top directo
+00011b90: 7279 2c20 616e 6420 7769 6c6c 2062 6520  ry, and will be 
+00011ba0: 7265 7475 726e 6564 2061 7420 6669 7273  returned at firs
+00011bb0: 7420 6974 6572 6174 696f 6e20 6f66 2067  t iteration of g
+00011bc0: 656e 6572 6174 6f72 0a20 2020 2020 2020  enerator.       
+00011bd0: 2049 6620 7333 5f75 726c 2069 7320 616e   If s3_url is an
+00011be0: 2065 6d70 7479 2062 7563 6b65 742c 206f   empty bucket, o
+00011bf0: 6e6c 7920 7969 656c 6420 6f6e 6520 332d  nly yield one 3-
+00011c00: 7475 706c 6520 286e 6f74 6573 3a20 7333  tuple (notes: s3
+00011c10: 2064 6f65 736e 2774 2068 6176 6520 656d   doesn't have em
+00011c20: 7074 7920 6469 7265 6374 6f72 7929 0a20  pty directory). 
+00011c30: 2020 2020 2020 2049 6620 7333 5f75 726c         If s3_url
+00011c40: 2064 6f65 736e 2774 2063 6f6e 7461 696e   doesn't contain
+00011c50: 2061 6e79 2062 7563 6b65 742c 2077 6869   any bucket, whi
+00011c60: 6368 2069 7320 7333 5f75 726c 203d 3d20  ch is s3_url == 
+00011c70: 2773 333a 2f2f 272c 2072 6169 7365 2055  's3://', raise U
+00011c80: 6e73 7570 706f 7274 6564 4572 726f 722e  nsupportedError.
+00011c90: 2077 616c 6b28 2920 6f6e 2063 6f6d 706c   walk() on compl
+00011ca0: 6574 6520 7333 2069 7320 6e6f 7420 7375  ete s3 is not su
+00011cb0: 7070 6f72 7465 6420 696e 206d 6567 6669  pported in megfi
+00011cc0: 6c65 0a0a 2020 2020 2020 2020 3a70 6172  le..        :par
+00011cd0: 616d 2066 6f6c 6c6f 776c 696e 6b73 3a20  am followlinks: 
+00011ce0: 7768 6574 6865 7220 666f 6c6c 6f77 6c69  whether followli
+00011cf0: 6e6b 7320 6973 2054 7275 6520 6f72 2046  nks is True or F
+00011d00: 616c 7365 2c20 7265 7375 6c74 2069 7320  alse, result is 
+00011d10: 7468 6520 7361 6d65 2e20 4265 6361 7573  the same. Becaus
+00011d20: 6520 7333 2073 796d 6c69 6e6b 206e 6f74  e s3 symlink not
+00011d30: 2073 7570 706f 7274 2064 6972 2e0a 2020   support dir..  
+00011d40: 2020 2020 2020 3a72 6169 7365 733a 2055        :raises: U
+00011d50: 6e73 7570 706f 7274 6564 4572 726f 720a  nsupportedError.
+00011d60: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+00011d70: 3a20 4120 332d 7475 706c 6520 6765 6e65  : A 3-tuple gene
+00011d80: 7261 746f 720a 2020 2020 2020 2020 2727  rator.        ''
+00011d90: 270a 2020 2020 2020 2020 6275 636b 6574  '.        bucket
+00011da0: 2c20 6b65 7920 3d20 7061 7273 655f 7333  , key = parse_s3
+00011db0: 5f75 726c 2873 656c 662e 7061 7468 5f77  _url(self.path_w
+00011dc0: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
+00011dd0: 2020 2020 2020 6966 206e 6f74 2062 7563        if not buc
+00011de0: 6b65 743a 0a20 2020 2020 2020 2020 2020  ket:.           
+00011df0: 2072 6169 7365 2055 6e73 7570 706f 7274   raise Unsupport
+00011e00: 6564 4572 726f 7228 2757 616c 6b20 7768  edError('Walk wh
+00011e10: 6f6c 6520 7333 272c 2073 656c 662e 7061  ole s3', self.pa
+00011e20: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
+00011e30: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+00011e40: 7420 7365 6c66 2e69 735f 6469 7228 293a  t self.is_dir():
+00011e50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011e60: 7572 6e0a 0a20 2020 2020 2020 2073 7461  urn..        sta
+00011e70: 636b 203d 205b 6b65 795d 0a20 2020 2020  ck = [key].     
+00011e80: 2020 2063 6c69 656e 7420 3d20 7365 6c66     client = self
+00011e90: 2e5f 636c 6965 6e74 0a20 2020 2020 2020  ._client.       
+00011ea0: 2077 6869 6c65 206c 656e 2873 7461 636b   while len(stack
+00011eb0: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
+00011ec0: 2020 2063 7572 7265 6e74 203d 205f 6265     current = _be
+00011ed0: 636f 6d65 5f70 7265 6669 7828 7374 6163  come_prefix(stac
+00011ee0: 6b2e 706f 7028 2929 0a20 2020 2020 2020  k.pop()).       
+00011ef0: 2020 2020 2064 6972 732c 2066 696c 6573       dirs, files
+00011f00: 203d 205b 5d2c 205b 5d0a 2020 2020 2020   = [], [].      
+00011f10: 2020 2020 2020 666f 7220 7265 7370 2069        for resp i
+00011f20: 6e20 5f6c 6973 745f 6f62 6a65 6374 735f  n _list_objects_
+00011f30: 7265 6375 7273 6976 6528 636c 6965 6e74  recursive(client
+00011f40: 2c20 6275 636b 6574 2c20 6375 7272 656e  , bucket, curren
+00011f50: 742c 2027 2f27 293a 0a20 2020 2020 2020  t, '/'):.       
+00011f60: 2020 2020 2020 2020 2066 6f72 2063 6f6d           for com
+00011f70: 6d6f 6e5f 7072 6566 6978 2069 6e20 7265  mon_prefix in re
+00011f80: 7370 2e67 6574 2827 436f 6d6d 6f6e 5072  sp.get('CommonPr
+00011f90: 6566 6978 6573 272c 205b 5d29 3a0a 2020  efixes', []):.  
+00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fb0: 2020 6469 7273 2e61 7070 656e 6428 636f    dirs.append(co
+00011fc0: 6d6d 6f6e 5f70 7265 6669 785b 2750 7265  mmon_prefix['Pre
+00011fd0: 6669 7827 5d5b 3a2d 315d 290a 2020 2020  fix'][:-1]).    
+00011fe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011ff0: 636f 6e74 656e 7420 696e 2072 6573 702e  content in resp.
+00012000: 6765 7428 2743 6f6e 7465 6e74 7327 2c20  get('Contents', 
+00012010: 5b5d 293a 0a20 2020 2020 2020 2020 2020  []):.           
+00012020: 2020 2020 2020 2020 2066 696c 6573 2e61           files.a
+00012030: 7070 656e 6428 636f 6e74 656e 745b 274b  ppend(content['K
+00012040: 6579 275d 290a 0a20 2020 2020 2020 2020  ey'])..         
+00012050: 2020 2064 6972 7320 3d20 736f 7274 6564     dirs = sorted
+00012060: 2864 6972 7329 0a20 2020 2020 2020 2020  (dirs).         
+00012070: 2020 2073 7461 636b 2e65 7874 656e 6428     stack.extend(
+00012080: 7265 7665 7273 6564 2864 6972 7329 290a  reversed(dirs)).
+00012090: 0a20 2020 2020 2020 2020 2020 2072 6f6f  .            roo
+000120a0: 7420 3d20 7333 5f70 6174 685f 6a6f 696e  t = s3_path_join
+000120b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000120c0: 2020 6627 7b73 656c 662e 5f70 726f 746f    f'{self._proto
+000120d0: 636f 6c5f 7769 7468 5f70 726f 6669 6c65  col_with_profile
+000120e0: 7d3a 2f2f 272c 2062 7563 6b65 742c 2063  }://', bucket, c
+000120f0: 7572 7265 6e74 295b 3a2d 315d 0a20 2020  urrent)[:-1].   
+00012100: 2020 2020 2020 2020 2064 6972 7320 3d20           dirs = 
+00012110: 5b70 6174 685b 6c65 6e28 6375 7272 656e  [path[len(curren
+00012120: 7429 3a5d 2066 6f72 2070 6174 6820 696e  t):] for path in
+00012130: 2064 6972 735d 0a20 2020 2020 2020 2020   dirs].         
+00012140: 2020 2066 696c 6573 203d 2073 6f72 7465     files = sorte
+00012150: 6428 7061 7468 5b6c 656e 2863 7572 7265  d(path[len(curre
+00012160: 6e74 293a 5d20 666f 7220 7061 7468 2069  nt):] for path i
+00012170: 6e20 6669 6c65 7329 0a20 2020 2020 2020  n files).       
+00012180: 2020 2020 2079 6965 6c64 2072 6f6f 742c       yield root,
+00012190: 2064 6972 732c 2066 696c 6573 0a0a 2020   dirs, files..  
+000121a0: 2020 6465 6620 6d64 3528 7365 6c66 2c20    def md5(self, 
+000121b0: 7265 6361 6c63 756c 6174 653a 2062 6f6f  recalculate: boo
+000121c0: 6c20 3d20 4661 6c73 652c 2066 6f6c 6c6f  l = False, follo
+000121d0: 776c 696e 6b73 3a20 626f 6f6c 203d 2046  wlinks: bool = F
+000121e0: 616c 7365 2920 2d3e 2073 7472 3a0a 2020  alse) -> str:.  
+000121f0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00012200: 2020 4765 7420 6d64 3520 6d65 7461 2069    Get md5 meta i
+00012210: 6e66 6f20 696e 2066 696c 6573 2074 6861  nfo in files tha
+00012220: 7420 7570 6c6f 6164 6564 2f63 6f70 6965  t uploaded/copie
+00012230: 6420 7669 6120 6d65 6766 696c 650a 0a20  d via megfile.. 
+00012240: 2020 2020 2020 2049 6620 6d65 7461 2069         If meta i
+00012250: 6e66 6f20 6973 206c 6f73 7420 6f72 206e  nfo is lost or n
+00012260: 6f6e 2d65 7869 7374 656e 742c 2072 6574  on-existent, ret
+00012270: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00012280: 2020 3a70 6172 616d 2072 6563 616c 6375    :param recalcu
+00012290: 6c61 7465 3a20 6361 6c63 756c 6174 6520  late: calculate 
+000122a0: 6d64 3520 696e 2072 6561 6c2d 7469 6d65  md5 in real-time
+000122b0: 206f 7220 7265 7475 726e 2073 3320 6574   or return s3 et
+000122c0: 6167 0a20 2020 2020 2020 203a 7061 7261  ag.        :para
+000122d0: 6d20 666f 6c6c 6f77 6c69 6e6b 733a 2049  m followlinks: I
+000122e0: 6620 6973 2054 7275 652c 2063 616c 6375  f is True, calcu
+000122f0: 6c61 7465 206d 6435 2066 6f72 2072 6561  late md5 for rea
+00012300: 6c20 6669 6c65 0a20 2020 2020 2020 203a  l file.        :
+00012310: 7265 7475 726e 733a 206d 6435 206d 6574  returns: md5 met
+00012320: 6120 696e 666f 0a20 2020 2020 2020 2027  a info.        '
+00012330: 2727 0a20 2020 2020 2020 2062 7563 6b65  ''.        bucke
+00012340: 742c 205f 203d 2070 6172 7365 5f73 335f  t, _ = parse_s3_
+00012350: 7572 6c28 7365 6c66 2e70 6174 685f 7769  url(self.path_wi
+00012360: 7468 5f70 726f 746f 636f 6c29 0a20 2020  th_protocol).   
+00012370: 2020 2020 2069 6620 6e6f 7420 6275 636b       if not buck
+00012380: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+00012390: 7261 6973 6520 5333 4275 636b 6574 4e6f  raise S3BucketNo
+000123a0: 7446 6f75 6e64 4572 726f 7228 0a20 2020  tFoundError(.   
+000123b0: 2020 2020 2020 2020 2020 2020 2027 456d               'Em
+000123c0: 7074 7920 6275 636b 6574 206e 616d 653a  pty bucket name:
+000123d0: 2025 7227 2025 2073 656c 662e 7061 7468   %r' % self.path
+000123e0: 5f77 6974 685f 7072 6f74 6f63 6f6c 290a  _with_protocol).
+000123f0: 2020 2020 2020 2020 7374 6174 203d 2073          stat = s
+00012400: 656c 662e 7374 6174 2866 6f6c 6c6f 775f  elf.stat(follow_
+00012410: 7379 6d6c 696e 6b73 3d66 6f6c 6c6f 776c  symlinks=followl
+00012420: 696e 6b73 290a 2020 2020 2020 2020 6966  inks).        if
+00012430: 2073 7461 742e 6973 6469 723a 0a20 2020   stat.isdir:.   
+00012440: 2020 2020 2020 2020 2068 6173 685f 6d64           hash_md
+00012450: 3520 3d20 6861 7368 6c69 622e 6d64 3528  5 = hashlib.md5(
+00012460: 2920 2023 206e 6f73 6563 0a20 2020 2020  )  # nosec.     
+00012470: 2020 2020 2020 2066 6f72 2066 696c 655f         for file_
+00012480: 6e61 6d65 2069 6e20 7365 6c66 2e6c 6973  name in self.lis
+00012490: 7464 6972 2829 3a0a 2020 2020 2020 2020  tdir():.        
+000124a0: 2020 2020 2020 2020 6368 756e 6b20 3d20          chunk = 
+000124b0: 5333 5061 7468 280a 2020 2020 2020 2020  S3Path(.        
+000124c0: 2020 2020 2020 2020 2020 2020 7333 5f70              s3_p
+000124d0: 6174 685f 6a6f 696e 280a 2020 2020 2020  ath_join(.      
+000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124f0: 2020 7365 6c66 2e70 6174 685f 7769 7468    self.path_with
+00012500: 5f70 726f 746f 636f 6c2c 0a20 2020 2020  _protocol,.     
+00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012520: 2020 2066 696c 655f 6e61 6d65 2929 2e6d     file_name)).m
+00012530: 6435 2872 6563 616c 6375 6c61 7465 3d72  d5(recalculate=r
+00012540: 6563 616c 6375 6c61 7465 292e 656e 636f  ecalculate).enco
+00012550: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00012560: 2020 2020 2068 6173 685f 6d64 352e 7570       hash_md5.up
+00012570: 6461 7465 2863 6875 6e6b 290a 2020 2020  date(chunk).    
+00012580: 2020 2020 2020 2020 7265 7475 726e 2068          return h
+00012590: 6173 685f 6d64 352e 6865 7864 6967 6573  ash_md5.hexdiges
+000125a0: 7428 290a 2020 2020 2020 2020 6966 2072  t().        if r
+000125b0: 6563 616c 6375 6c61 7465 3a0a 2020 2020  ecalculate:.    
+000125c0: 2020 2020 2020 2020 7061 7468 5f69 6e73          path_ins
+000125d0: 7461 6e63 6520 3d20 7365 6c66 0a20 2020  tance = self.   
+000125e0: 2020 2020 2020 2020 2069 6620 666f 6c6c           if foll
+000125f0: 6f77 6c69 6e6b 733a 0a20 2020 2020 2020  owlinks:.       
+00012600: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012620: 2020 7061 7468 5f69 6e73 7461 6e63 6520    path_instance 
+00012630: 3d20 7365 6c66 2e72 6561 646c 696e 6b28  = self.readlink(
+00012640: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012650: 2020 6578 6365 7074 2053 334e 6f74 414c    except S3NotAL
+00012660: 696e 6b45 7272 6f72 3a0a 2020 2020 2020  inkError:.      
+00012670: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00012680: 7373 0a20 2020 2020 2020 2020 2020 2077  ss.            w
+00012690: 6974 6820 7061 7468 5f69 6e73 7461 6e63  ith path_instanc
+000126a0: 652e 6f70 656e 2827 7262 2729 2061 7320  e.open('rb') as 
+000126b0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+000126c0: 2020 2072 6574 7572 6e20 6361 6c63 756c     return calcul
+000126d0: 6174 655f 6d64 3528 6629 0a20 2020 2020  ate_md5(f).     
+000126e0: 2020 2072 6574 7572 6e20 7374 6174 2e65     return stat.e
+000126f0: 7874 7261 2e67 6574 2827 4554 6167 272c  xtra.get('ETag',
+00012700: 2027 2729 5b31 3a2d 315d 0a0a 2020 2020   '')[1:-1]..    
+00012710: 6465 6620 636f 7079 280a 2020 2020 2020  def copy(.      
+00012720: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00012730: 2020 2020 2020 2020 6473 745f 7572 6c3a          dst_url:
+00012740: 2050 6174 684c 696b 652c 0a20 2020 2020   PathLike,.     
+00012750: 2020 2020 2020 2066 6f6c 6c6f 776c 696e         followlin
+00012760: 6b73 3a20 626f 6f6c 203d 2046 616c 7365  ks: bool = False
+00012770: 2c0a 2020 2020 2020 2020 2020 2020 6361  ,.            ca
+00012780: 6c6c 6261 636b 3a20 4f70 7469 6f6e 616c  llback: Optional
+00012790: 5b43 616c 6c61 626c 655b 5b69 6e74 5d2c  [Callable[[int],
+000127a0: 204e 6f6e 655d 5d20 3d20 4e6f 6e65 2920   None]] = None) 
+000127b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000127c0: 2027 2727 2046 696c 6520 636f 7079 206f   ''' File copy o
+000127d0: 6e20 5333 0a20 2020 2020 2020 2043 6f70  n S3.        Cop
+000127e0: 7920 636f 6e74 656e 7420 6f66 2066 696c  y content of fil
+000127f0: 6520 6f6e 2060 7372 635f 7061 7468 6020  e on `src_path` 
+00012800: 746f 2060 6473 745f 7061 7468 602e 0a20  to `dst_path`.. 
+00012810: 2020 2020 2020 2049 7427 7320 6361 6c6c         It's call
+00012820: 6572 2773 2072 6573 706f 6e73 6562 696c  er's responsebil
+00012830: 6974 7920 746f 2065 6e73 7572 6520 7468  ity to ensure th
+00012840: 6520 7333 5f69 7366 696c 6528 7372 635f  e s3_isfile(src_
+00012850: 7572 6c29 203d 3d20 5472 7565 0a0a 2020  url) == True..  
+00012860: 2020 2020 2020 3a70 6172 616d 2064 7374        :param dst
+00012870: 5f70 6174 683a 2054 6172 6765 7420 6669  _path: Target fi
+00012880: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
+00012890: 3a70 6172 616d 2063 616c 6c62 6163 6b3a  :param callback:
+000128a0: 2043 616c 6c65 6420 7065 7269 6f64 6963   Called periodic
+000128b0: 616c 6c79 2064 7572 696e 6720 636f 7079  ally during copy
+000128c0: 2c20 616e 6420 7468 6520 696e 7075 7420  , and the input 
+000128d0: 7061 7261 6d65 7465 7220 6973 2074 6865  parameter is the
+000128e0: 2064 6174 6120 7369 7a65 2028 696e 2062   data size (in b
+000128f0: 7974 6573 2920 6f66 2063 6f70 7920 7369  ytes) of copy si
+00012900: 6e63 6520 7468 6520 6c61 7374 2063 616c  nce the last cal
+00012910: 6c0a 2020 2020 2020 2020 2727 270a 2020  l.        '''.  
+00012920: 2020 2020 2020 7372 635f 7572 6c20 3d20        src_url = 
+00012930: 7365 6c66 2e70 6174 685f 7769 7468 5f70  self.path_with_p
+00012940: 726f 746f 636f 6c0a 2020 2020 2020 2020  rotocol.        
+00012950: 7372 635f 6275 636b 6574 2c20 7372 635f  src_bucket, src_
+00012960: 6b65 7920 3d20 7061 7273 655f 7333 5f75  key = parse_s3_u
+00012970: 726c 2873 7263 5f75 726c 290a 2020 2020  rl(src_url).    
+00012980: 2020 2020 6473 745f 6275 636b 6574 2c20      dst_bucket, 
+00012990: 6473 745f 6b65 7920 3d20 7061 7273 655f  dst_key = parse_
+000129a0: 7333 5f75 726c 2864 7374 5f75 726c 290a  s3_url(dst_url).
+000129b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000129c0: 7372 635f 6275 636b 6574 3a0a 2020 2020  src_bucket:.    
+000129d0: 2020 2020 2020 2020 7261 6973 6520 5333          raise S3
+000129e0: 4275 636b 6574 4e6f 7446 6f75 6e64 4572  BucketNotFoundEr
+000129f0: 726f 7228 2745 6d70 7479 2062 7563 6b65  ror('Empty bucke
+00012a00: 7420 6e61 6d65 3a20 2572 2720 2520 7372  t name: %r' % sr
+00012a10: 635f 7572 6c29 0a20 2020 2020 2020 2069  c_url).        i
+00012a20: 6620 7365 6c66 2e69 735f 6469 7228 293a  f self.is_dir():
+00012a30: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00012a40: 7365 2053 3349 7341 4469 7265 6374 6f72  se S3IsADirector
+00012a50: 7945 7272 6f72 2827 4973 2061 2064 6972  yError('Is a dir
+00012a60: 6563 746f 7279 3a20 2572 2720 2520 7372  ectory: %r' % sr
+00012a70: 635f 7572 6c29 0a0a 2020 2020 2020 2020  c_url)..        
+00012a80: 6966 206e 6f74 2064 7374 5f62 7563 6b65  if not dst_bucke
+00012a90: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00012aa0: 6169 7365 2053 3342 7563 6b65 744e 6f74  aise S3BucketNot
+00012ab0: 466f 756e 6445 7272 6f72 2827 456d 7074  FoundError('Empt
+00012ac0: 7920 6275 636b 6574 206e 616d 653a 2025  y bucket name: %
+00012ad0: 7227 2025 2064 7374 5f75 726c 290a 2020  r' % dst_url).  
+00012ae0: 2020 2020 2020 6966 206e 6f74 2064 7374        if not dst
+00012af0: 5f6b 6579 206f 7220 6473 745f 6b65 792e  _key or dst_key.
+00012b00: 656e 6473 7769 7468 2827 2f27 293a 0a20  endswith('/'):. 
+00012b10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00012b20: 2053 3349 7341 4469 7265 6374 6f72 7945   S3IsADirectoryE
+00012b30: 7272 6f72 2827 4973 2061 2064 6972 6563  rror('Is a direc
+00012b40: 746f 7279 3a20 2572 2720 2520 6473 745f  tory: %r' % dst_
+00012b50: 7572 6c29 0a0a 2020 2020 2020 2020 6966  url)..        if
+00012b60: 2066 6f6c 6c6f 776c 696e 6b73 3a0a 2020   followlinks:.  
+00012b70: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012b90: 335f 7572 6c20 3d20 7365 6c66 2e72 6561  3_url = self.rea
+00012ba0: 646c 696e 6b28 292e 7061 7468 0a20 2020  dlink().path.   
+00012bb0: 2020 2020 2020 2020 2020 2020 2073 7263               src
+00012bc0: 5f62 7563 6b65 742c 2073 7263 5f6b 6579  _bucket, src_key
+00012bd0: 203d 2070 6172 7365 5f73 335f 7572 6c28   = parse_s3_url(
+00012be0: 7333 5f75 726c 290a 2020 2020 2020 2020  s3_url).        
+00012bf0: 2020 2020 6578 6365 7074 2053 334e 6f74      except S3Not
+00012c00: 414c 696e 6b45 7272 6f72 3a0a 2020 2020  ALinkError:.    
+00012c10: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00012c20: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
+00012c30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012c40: 5f63 6c69 656e 742e 636f 7079 280a 2020  _client.copy(.  
+00012c50: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c70: 2020 2020 2742 7563 6b65 7427 3a20 7372      'Bucket': sr
+00012c80: 635f 6275 636b 6574 2c0a 2020 2020 2020  c_bucket,.      
+00012c90: 2020 2020 2020 2020 2020 2020 2020 274b                'K
+00012ca0: 6579 273a 2073 7263 5f6b 6579 2c0a 2020  ey': src_key,.  
+00012cb0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00012cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012cd0: 2042 7563 6b65 743d 6473 745f 6275 636b   Bucket=dst_buck
+00012ce0: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+00012cf0: 2020 2020 4b65 793d 6473 745f 6b65 792c      Key=dst_key,
+00012d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d10: 2043 616c 6c62 6163 6b3d 6361 6c6c 6261   Callback=callba
+00012d20: 636b 290a 2020 2020 2020 2020 6578 6365  ck).        exce
+00012d30: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00012d40: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
+00012d50: 2020 2065 7272 6f72 203d 2074 7261 6e73     error = trans
+00012d60: 6c61 7465 5f73 335f 6572 726f 7228 6572  late_s3_error(er
+00012d70: 726f 722c 2064 7374 5f75 726c 290a 2020  ror, dst_url).  
+00012d80: 2020 2020 2020 2020 2020 2320 4572 726f            # Erro
+00012d90: 7220 6361 6e27 7420 6865 6c70 2074 656c  r can't help tel
+00012da0: 6c20 7768 6963 6820 6973 2070 726f 626c  l which is probl
+00012db0: 656d 6174 6963 0a20 2020 2020 2020 2020  ematic.         
+00012dc0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00012dd0: 2865 7272 6f72 2c20 5333 4275 636b 6574  (error, S3Bucket
+00012de0: 4e6f 7446 6f75 6e64 4572 726f 7229 3a0a  NotFoundError):.
+00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e00: 6966 206e 6f74 2073 656c 662e 6861 7362  if not self.hasb
+00012e10: 7563 6b65 7428 293a 0a20 2020 2020 2020  ucket():.       
+00012e20: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00012e30: 7365 2053 3342 7563 6b65 744e 6f74 466f  se S3BucketNotFo
+00012e40: 756e 6445 7272 6f72 2827 4e6f 2073 7563  undError('No suc
+00012e50: 6820 6275 636b 6574 3a20 2572 2720 2520  h bucket: %r' % 
+00012e60: 7372 635f 7572 6c29 0a20 2020 2020 2020  src_url).       
+00012e70: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00012e80: 616e 6365 2865 7272 6f72 2c20 5333 4669  ance(error, S3Fi
+00012e90: 6c65 4e6f 7446 6f75 6e64 4572 726f 7229  leNotFoundError)
+00012ea0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012eb0: 2020 6966 206e 6f74 2073 656c 662e 6973    if not self.is
+00012ec0: 5f66 696c 6528 293a 0a20 2020 2020 2020  _file():.       
+00012ed0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00012ee0: 7365 2053 3346 696c 654e 6f74 466f 756e  se S3FileNotFoun
+00012ef0: 6445 7272 6f72 2827 4e6f 2073 7563 6820  dError('No such 
+00012f00: 6669 6c65 3a20 2572 2720 2520 7372 635f  file: %r' % src_
+00012f10: 7572 6c29 0a20 2020 2020 2020 2020 2020  url).           
+00012f20: 2072 6169 7365 2065 7272 6f72 0a0a 2020   raise error..  
+00012f30: 2020 6465 6620 7379 6e63 2873 656c 662c    def sync(self,
+00012f40: 2064 7374 5f75 726c 3a20 5061 7468 4c69   dst_url: PathLi
+00012f50: 6b65 2c20 666f 6c6c 6f77 6c69 6e6b 733a  ke, followlinks:
+00012f60: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
+00012f70: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00012f80: 2727 270a 2020 2020 2020 2020 436f 7079  '''.        Copy
+00012f90: 2066 696c 652f 6469 7265 6374 6f72 7920   file/directory 
+00012fa0: 6f6e 2073 7263 5f75 726c 2074 6f20 6473  on src_url to ds
+00012fb0: 745f 7572 6c0a 0a20 2020 2020 2020 203a  t_url..        :
+00012fc0: 7061 7261 6d20 6473 745f 7572 6c3a 2047  param dst_url: G
+00012fd0: 6976 656e 2064 6573 7469 6e61 7469 6f6e  iven destination
+00012fe0: 2070 6174 680a 2020 2020 2020 2020 2727   path.        ''
+00012ff0: 270a 2020 2020 2020 2020 666f 7220 7372  '.        for sr
+00013000: 635f 6669 6c65 5f70 6174 682c 2064 7374  c_file_path, dst
+00013010: 5f66 696c 655f 7061 7468 2069 6e20 5f73  _file_path in _s
+00013020: 335f 7363 616e 5f70 6169 7273 280a 2020  3_scan_pairs(.  
+00013030: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013040: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
+00013050: 746f 636f 6c2c 2064 7374 5f75 726c 293a  tocol, dst_url):
+00013060: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
+00013070: 5f66 696c 655f 7061 7468 203d 2073 656c  _file_path = sel
+00013080: 662e 6672 6f6d 5f70 6174 6828 7372 635f  f.from_path(src_
+00013090: 6669 6c65 5f70 6174 6829 0a20 2020 2020  file_path).     
+000130a0: 2020 2020 2020 2064 7374 5f66 696c 655f         dst_file_
+000130b0: 7061 7468 203d 2073 656c 662e 6672 6f6d  path = self.from
+000130c0: 5f70 6174 6828 6473 745f 6669 6c65 5f70  _path(dst_file_p
+000130d0: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+000130e0: 2069 6620 6473 745f 6669 6c65 5f70 6174   if dst_file_pat
+000130f0: 682e 6578 6973 7473 2829 2061 6e64 2069  h.exists() and i
+00013100: 735f 7361 6d65 5f66 696c 6528 0a20 2020  s_same_file(.   
+00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013120: 2073 7263 5f66 696c 655f 7061 7468 2e73   src_file_path.s
+00013130: 7461 7428 292c 2064 7374 5f66 696c 655f  tat(), dst_file_
+00013140: 7061 7468 2e73 7461 7428 292c 2027 636f  path.stat(), 'co
+00013150: 7079 2729 3a0a 2020 2020 2020 2020 2020  py'):.          
+00013160: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00013170: 2020 2020 2020 2020 2020 2073 7263 5f66             src_f
+00013180: 696c 655f 7061 7468 2e63 6f70 7928 6473  ile_path.copy(ds
+00013190: 745f 6669 6c65 5f70 6174 682c 2066 6f6c  t_file_path, fol
+000131a0: 6c6f 776c 696e 6b73 3d66 6f6c 6c6f 776c  lowlinks=followl
+000131b0: 696e 6b73 290a 0a20 2020 2064 6566 2073  inks)..    def s
+000131c0: 796d 6c69 6e6b 2873 656c 662c 2064 7374  ymlink(self, dst
+000131d0: 5f70 6174 683a 2050 6174 684c 696b 6529  _path: PathLike)
+000131e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000131f0: 2020 2727 270a 2020 2020 2020 2020 4372    '''.        Cr
+00013200: 6561 7465 2061 2073 796d 626f 6c69 6320  eate a symbolic 
+00013210: 6c69 6e6b 2070 6f69 6e74 696e 6720 746f  link pointing to
+00013220: 2073 7263 5f70 6174 6820 6e61 6d65 6420   src_path named 
+00013230: 6473 745f 7061 7468 2e0a 0a20 2020 2020  dst_path...     
+00013240: 2020 203a 7061 7261 6d20 6473 745f 7061     :param dst_pa
+00013250: 7468 3a20 4465 7369 6e61 7469 6f6e 2070  th: Desination p
+00013260: 6174 680a 2020 2020 2020 2020 3a72 6169  ath.        :rai
+00013270: 7365 733a 2053 334e 616d 6554 6f6f 4c6f  ses: S3NameTooLo
+00013280: 6e67 4572 726f 722c 2053 3342 7563 6b65  ngError, S3Bucke
+00013290: 744e 6f74 466f 756e 6445 7272 6f72 2c20  tNotFoundError, 
+000132a0: 5333 4973 4144 6972 6563 746f 7279 4572  S3IsADirectoryEr
+000132b0: 726f 720a 2020 2020 2020 2020 2727 270a  ror.        '''.
+000132c0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+000132d0: 7472 2873 656c 662e 5f73 335f 7061 7468  tr(self._s3_path
+000132e0: 292e 656e 636f 6465 2829 2920 3e20 3130  ).encode()) > 10
+000132f0: 3234 3a0a 2020 2020 2020 2020 2020 2020  24:.            
+00013300: 7261 6973 6520 5333 4e61 6d65 546f 6f4c  raise S3NameTooL
+00013310: 6f6e 6745 7272 6f72 2827 4669 6c65 206e  ongError('File n
+00013320: 616d 6520 746f 6f20 6c6f 6e67 3a20 2572  ame too long: %r
+00013330: 2720 2520 6473 745f 7061 7468 290a 2020  ' % dst_path).  
+00013340: 2020 2020 2020 7372 635f 6275 636b 6574        src_bucket
+00013350: 2c20 7372 635f 6b65 7920 3d20 7061 7273  , src_key = pars
+00013360: 655f 7333 5f75 726c 2873 656c 662e 7061  e_s3_url(self.pa
+00013370: 7468 5f77 6974 685f 7072 6f74 6f63 6f6c  th_with_protocol
+00013380: 290a 2020 2020 2020 2020 6473 745f 6275  ).        dst_bu
+00013390: 636b 6574 2c20 6473 745f 6b65 7920 3d20  cket, dst_key = 
+000133a0: 7061 7273 655f 7333 5f75 726c 2864 7374  parse_s3_url(dst
+000133b0: 5f70 6174 6829 0a0a 2020 2020 2020 2020  _path)..        
+000133c0: 6966 206e 6f74 2073 7263 5f62 7563 6b65  if not src_bucke
+000133d0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+000133e0: 6169 7365 2053 3342 7563 6b65 744e 6f74  aise S3BucketNot
+000133f0: 466f 756e 6445 7272 6f72 2827 456d 7074  FoundError('Empt
+00013400: 7920 6275 636b 6574 206e 616d 653a 2025  y bucket name: %
+00013410: 7227 2025 2073 656c 662e 7061 7468 290a  r' % self.path).
+00013420: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+00013430: 7374 5f62 7563 6b65 743a 0a20 2020 2020  st_bucket:.     
+00013440: 2020 2020 2020 2072 6169 7365 2053 3342         raise S3B
+00013450: 7563 6b65 744e 6f74 466f 756e 6445 7272  ucketNotFoundErr
+00013460: 6f72 2827 456d 7074 7920 6275 636b 6574  or('Empty bucket
+00013470: 206e 616d 653a 2025 7227 2025 2064 7374   name: %r' % dst
+00013480: 5f70 6174 6829 0a20 2020 2020 2020 2069  _path).        i
+00013490: 6620 6e6f 7420 6473 745f 6b65 7920 6f72  f not dst_key or
+000134a0: 2064 7374 5f6b 6579 2e65 6e64 7377 6974   dst_key.endswit
+000134b0: 6828 272f 2729 3a0a 2020 2020 2020 2020  h('/'):.        
+000134c0: 2020 2020 7261 6973 6520 5333 4973 4144      raise S3IsAD
+000134d0: 6972 6563 746f 7279 4572 726f 7228 2749  irectoryError('I
+000134e0: 7320 6120 6469 7265 6374 6f72 793a 2025  s a directory: %
+000134f0: 7227 2025 2064 7374 5f70 6174 6829 0a0a  r' % dst_path)..
+00013500: 2020 2020 2020 2020 7372 635f 7061 7468          src_path
+00013510: 203d 2073 656c 662e 5f73 335f 7061 7468   = self._s3_path
+00013520: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00013530: 2020 2020 2020 2020 2020 7372 635f 7061            src_pa
+00013540: 7468 203d 2073 656c 662e 7265 6164 6c69  th = self.readli
+00013550: 6e6b 2829 2e5f 7333 5f70 6174 680a 2020  nk()._s3_path.  
+00013560: 2020 2020 2020 6578 6365 7074 2053 334e        except S3N
+00013570: 6f74 414c 696e 6b45 7272 6f72 3a0a 2020  otALinkError:.  
+00013580: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00013590: 2020 2020 2020 2077 6974 6820 7261 6973         with rais
+000135a0: 655f 7333 5f65 7272 6f72 2864 7374 5f70  e_s3_error(dst_p
+000135b0: 6174 6829 3a0a 2020 2020 2020 2020 2020  ath):.          
+000135c0: 2020 7365 6c66 2e5f 636c 6965 6e74 2e70    self._client.p
+000135d0: 7574 5f6f 626a 6563 7428 0a20 2020 2020  ut_object(.     
+000135e0: 2020 2020 2020 2020 2020 2042 7563 6b65             Bucke
+000135f0: 743d 6473 745f 6275 636b 6574 2c0a 2020  t=dst_bucket,.  
+00013600: 2020 2020 2020 2020 2020 2020 2020 4b65                Ke
+00013610: 793d 6473 745f 6b65 792c 0a20 2020 2020  y=dst_key,.     
+00013620: 2020 2020 2020 2020 2020 204d 6574 6164             Metad
+00013630: 6174 613d 7b22 7379 6d6c 696e 6b5f 746f  ata={"symlink_to
+00013640: 223a 2073 7263 5f70 6174 687d 290a 0a20  ": src_path}).. 
+00013650: 2020 2064 6566 2072 6561 646c 696e 6b28     def readlink(
+00013660: 7365 6c66 2920 2d3e 2027 5333 5061 7468  self) -> 'S3Path
+00013670: 273a 0a20 2020 2020 2020 2027 2727 0a20  ':.        '''. 
+00013680: 2020 2020 2020 2052 6574 7572 6e20 6120         Return a 
+00013690: 5333 5061 7468 2069 6e73 7461 6e63 6520  S3Path instance 
+000136a0: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
+000136b0: 2070 6174 6820 746f 2077 6869 6368 2074   path to which t
+000136c0: 6865 2073 796d 626f 6c69 6320 6c69 6e6b  he symbolic link
+000136d0: 2070 6f69 6e74 732e 0a0a 2020 2020 2020   points...      
+000136e0: 2020 3a72 6574 7572 6e73 3a20 5265 7475    :returns: Retu
+000136f0: 726e 2061 2053 3350 6174 6820 696e 7374  rn a S3Path inst
+00013700: 616e 6365 2072 6570 7265 7365 6e74 696e  ance representin
+00013710: 6720 7468 6520 7061 7468 2074 6f20 7768  g the path to wh
+00013720: 6963 6820 7468 6520 7379 6d62 6f6c 6963  ich the symbolic
+00013730: 206c 696e 6b20 706f 696e 7473 2e0a 2020   link points..  
+00013740: 2020 2020 2020 3a72 6169 7365 733a 2053        :raises: S
+00013750: 334e 616d 6554 6f6f 4c6f 6e67 4572 726f  3NameTooLongErro
+00013760: 722c 2053 3342 7563 6b65 744e 6f74 466f  r, S3BucketNotFo
+00013770: 756e 6445 7272 6f72 2c20 5333 4973 4144  undError, S3IsAD
+00013780: 6972 6563 746f 7279 4572 726f 722c 2053  irectoryError, S
+00013790: 334e 6f74 414c 696e 6b45 7272 6f72 0a20  3NotALinkError. 
+000137a0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+000137b0: 2020 2062 7563 6b65 742c 206b 6579 203d     bucket, key =
+000137c0: 2070 6172 7365 5f73 335f 7572 6c28 7365   parse_s3_url(se
+000137d0: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
+000137e0: 746f 636f 6c29 0a20 2020 2020 2020 2069  tocol).        i
+000137f0: 6620 6e6f 7420 6275 636b 6574 3a0a 2020  f not bucket:.  
+00013800: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00013810: 5333 4275 636b 6574 4e6f 7446 6f75 6e64  S3BucketNotFound
+00013820: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00013830: 2020 2020 2020 2027 456d 7074 7920 6275         'Empty bu
+00013840: 636b 6574 206e 616d 653a 2025 7227 2025  cket name: %r' %
+00013850: 2073 656c 662e 7061 7468 5f77 6974 685f   self.path_with_
+00013860: 7072 6f74 6f63 6f6c 290a 2020 2020 2020  protocol).      
+00013870: 2020 6966 206e 6f74 206b 6579 206f 7220    if not key or 
+00013880: 6b65 792e 656e 6473 7769 7468 2827 2f27  key.endswith('/'
+00013890: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000138a0: 6169 7365 2053 3349 7341 4469 7265 6374  aise S3IsADirect
+000138b0: 6f72 7945 7272 6f72 280a 2020 2020 2020  oryError(.      
+000138c0: 2020 2020 2020 2020 2020 2749 7320 6120            'Is a 
+000138d0: 6469 7265 6374 6f72 793a 2025 7227 2025  directory: %r' %
+000138e0: 2073 656c 662e 7061 7468 5f77 6974 685f   self.path_with_
+000138f0: 7072 6f74 6f63 6f6c 290a 2020 2020 2020  protocol).      
+00013900: 2020 6d65 7461 6461 7461 203d 2073 656c    metadata = sel
+00013910: 662e 5f73 335f 6765 745f 6d65 7461 6461  f._s3_get_metada
+00013920: 7461 2829 0a0a 2020 2020 2020 2020 6966  ta()..        if
+00013930: 206e 6f74 2027 7379 6d6c 696e 6b5f 746f   not 'symlink_to
+00013940: 2720 696e 206d 6574 6164 6174 613a 0a20  ' in metadata:. 
+00013950: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00013960: 2053 334e 6f74 414c 696e 6b45 7272 6f72   S3NotALinkError
+00013970: 2827 4e6f 7420 6120 6c69 6e6b 3a20 2572  ('Not a link: %r
+00013980: 2720 2520 7365 6c66 2e70 6174 685f 7769  ' % self.path_wi
+00013990: 7468 5f70 726f 746f 636f 6c29 0a20 2020  th_protocol).   
+000139a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000139b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000139c0: 6c66 2e66 726f 6d5f 7061 7468 286d 6574  lf.from_path(met
+000139d0: 6164 6174 615b 2773 796d 6c69 6e6b 5f74  adata['symlink_t
+000139e0: 6f27 5d29 0a0a 2020 2020 6465 6620 6973  o'])..    def is
+000139f0: 5f73 796d 6c69 6e6b 2873 656c 6629 202d  _symlink(self) -
+00013a00: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00013a10: 2727 270a 2020 2020 2020 2020 5465 7374  '''.        Test
+00013a20: 2077 6865 7468 6572 2061 2070 6174 6820   whether a path 
+00013a30: 6973 206c 696e 6b0a 0a20 2020 2020 2020  is link..       
+00013a40: 203a 7265 7475 726e 733a 2054 7275 6520   :returns: True 
+00013a50: 6966 2061 2070 6174 6820 6973 206c 696e  if a path is lin
+00013a60: 6b2c 2065 6c73 6520 4661 6c73 650a 2020  k, else False.  
+00013a70: 2020 2020 2020 3a72 6169 7365 733a 2053        :raises: S
+00013a80: 334e 6f74 414c 696e 6b45 7272 6f72 0a20  3NotALinkError. 
+00013a90: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00013aa0: 2020 2062 7563 6b65 742c 206b 6579 203d     bucket, key =
+00013ab0: 2070 6172 7365 5f73 335f 7572 6c28 7365   parse_s3_url(se
+00013ac0: 6c66 2e70 6174 685f 7769 7468 5f70 726f  lf.path_with_pro
+00013ad0: 746f 636f 6c29 0a20 2020 2020 2020 2069  tocol).        i
+00013ae0: 6620 6e6f 7420 6275 636b 6574 3a0a 2020  f not bucket:.  
+00013af0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00013b00: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
+00013b10: 6620 6e6f 7420 6b65 7920 6f72 206b 6579  f not key or key
+00013b20: 2e65 6e64 7377 6974 6828 272f 2729 3a0a  .endswith('/'):.
+00013b30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013b40: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00013b50: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
+00013b60: 2e5f 7333 5f67 6574 5f6d 6574 6164 6174  ._s3_get_metadat
+00013b70: 6128 290a 2020 2020 2020 2020 7265 7475  a().        retu
+00013b80: 726e 2027 7379 6d6c 696e 6b5f 746f 2720  rn 'symlink_to' 
+00013b90: 696e 206d 6574 6164 6174 610a 0a20 2020  in metadata..   
+00013ba0: 2064 6566 2073 6176 6528 7365 6c66 2c20   def save(self, 
+00013bb0: 6669 6c65 5f6f 626a 6563 743a 2042 696e  file_object: Bin
+00013bc0: 6172 7949 4f29 3a0a 2020 2020 2020 2020  aryIO):.        
+00013bd0: 2727 2757 7269 7465 2074 6865 206f 7065  '''Write the ope
+00013be0: 6e65 6420 6269 6e61 7279 2073 7472 6561  ned binary strea
+00013bf0: 6d20 746f 2073 7065 6369 6669 6564 2070  m to specified p
+00013c00: 6174 682c 2062 7574 2074 6865 2073 7472  ath, but the str
+00013c10: 6561 6d20 776f 6e27 7420 6265 2063 6c6f  eam won't be clo
+00013c20: 7365 640a 0a20 2020 2020 2020 203a 7061  sed..        :pa
+00013c30: 7261 6d20 6669 6c65 5f6f 626a 6563 743a  ram file_object:
+00013c40: 2053 7472 6561 6d20 746f 2062 6520 7265   Stream to be re
+00013c50: 6164 0a20 2020 2020 2020 2027 2727 0a20  ad.        '''. 
+00013c60: 2020 2020 2020 2062 7563 6b65 742c 206b         bucket, k
+00013c70: 6579 203d 2070 6172 7365 5f73 335f 7572  ey = parse_s3_ur
+00013c80: 6c28 7365 6c66 2e70 6174 685f 7769 7468  l(self.path_with
+00013c90: 5f70 726f 746f 636f 6c29 0a20 2020 2020  _protocol).     
+00013ca0: 2020 2069 6620 6e6f 7420 6275 636b 6574     if not bucket
+00013cb0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00013cc0: 6973 6520 5333 4275 636b 6574 4e6f 7446  ise S3BucketNotF
+00013cd0: 6f75 6e64 4572 726f 7228 0a20 2020 2020  oundError(.     
+00013ce0: 2020 2020 2020 2020 2020 2027 456d 7074             'Empt
+00013cf0: 7920 6275 636b 6574 206e 616d 653a 2025  y bucket name: %
+00013d00: 7227 2025 2073 656c 662e 7061 7468 5f77  r' % self.path_w
+00013d10: 6974 685f 7072 6f74 6f63 6f6c 290a 2020  ith_protocol).  
+00013d20: 2020 2020 2020 6966 206e 6f74 206b 6579        if not key
+00013d30: 206f 7220 6b65 792e 656e 6473 7769 7468   or key.endswith
+00013d40: 2827 2f27 293a 0a20 2020 2020 2020 2020  ('/'):.         
+00013d50: 2020 2072 6169 7365 2053 3349 7341 4469     raise S3IsADi
+00013d60: 7265 6374 6f72 7945 7272 6f72 280a 2020  rectoryError(.  
+00013d70: 2020 2020 2020 2020 2020 2020 2020 2749                'I
+00013d80: 7320 6120 6469 7265 6374 6f72 793a 2025  s a directory: %
+00013d90: 7227 2025 2073 656c 662e 7061 7468 5f77  r' % self.path_w
+00013da0: 6974 685f 7072 6f74 6f63 6f6c 290a 0a20  ith_protocol).. 
+00013db0: 2020 2020 2020 2077 6974 6820 7261 6973         with rais
+00013dc0: 655f 7333 5f65 7272 6f72 2873 656c 662e  e_s3_error(self.
+00013dd0: 7061 7468 5f77 6974 685f 7072 6f74 6f63  path_with_protoc
+00013de0: 6f6c 293a 0a20 2020 2020 2020 2020 2020  ol):.           
+00013df0: 2073 656c 662e 5f63 6c69 656e 742e 7570   self._client.up
+00013e00: 6c6f 6164 5f66 696c 656f 626a 2866 696c  load_fileobj(fil
+00013e10: 655f 6f62 6a65 6374 2c20 4275 636b 6574  e_object, Bucket
+00013e20: 3d62 7563 6b65 742c 204b 6579 3d6b 6579  =bucket, Key=key
+00013e30: 290a 0a20 2020 2064 6566 206f 7065 6e28  )..    def open(
+00013e40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013e50: 662c 0a20 2020 2020 2020 2020 2020 206d  f,.            m
+00013e60: 6f64 653a 2073 7472 203d 2027 7227 2c0a  ode: str = 'r',.
+00013e70: 2020 2020 2020 2020 2020 2020 2a2c 0a20              *,. 
+00013e80: 2020 2020 2020 2020 2020 2073 335f 6f70             s3_op
+00013e90: 656e 5f66 756e 633a 2043 616c 6c61 626c  en_func: Callabl
+00013ea0: 655b 5b73 7472 2c20 7374 725d 2c20 4269  e[[str, str], Bi
+00013eb0: 6e61 7279 494f 5d20 3d20 7333 5f6f 7065  naryIO] = s3_ope
+00013ec0: 6e2c 0a20 2020 2020 2020 2020 2020 202a  n,.            *
+00013ed0: 2a6b 7761 7267 7329 202d 3e20 494f 5b41  *kwargs) -> IO[A
+00013ee0: 6e79 5374 725d 3a20 2023 2070 7974 7970  nyStr]:  # pytyp
+00013ef0: 653a 2064 6973 6162 6c65 3d73 6967 6e61  e: disable=signa
+00013f00: 7475 7265 2d6d 6973 6d61 7463 680a 2020  ture-mismatch.  
+00013f10: 2020 2020 2020 7265 7475 726e 2073 335f        return s3_
+00013f20: 6f70 656e 5f66 756e 6328 0a20 2020 2020  open_func(.     
+00013f30: 2020 2020 2020 2073 656c 662e 7061 7468         self.path
+00013f40: 5f77 6974 685f 7072 6f74 6f63 6f6c 2c20  _with_protocol, 
+00013f50: 6d6f 6465 2c0a 2020 2020 2020 2020 2020  mode,.          
+00013f60: 2020 2a2a 6e65 6365 7373 6172 795f 7061    **necessary_pa
+00013f70: 7261 6d73 2873 335f 6f70 656e 5f66 756e  rams(s3_open_fun
+00013f80: 632c 202a 2a6b 7761 7267 7329 290a 0a20  c, **kwargs)).. 
+00013f90: 2020 2064 6566 2061 6273 6f6c 7574 6528     def absolute(
+00013fa0: 7365 6c66 2920 2d3e 2027 5333 5061 7468  self) -> 'S3Path
+00013fb0: 273a 0a20 2020 2020 2020 2027 2727 0a20  ':.        '''. 
+00013fc0: 2020 2020 2020 204d 616b 6520 7468 6520         Make the 
+00013fd0: 7061 7468 2061 6273 6f6c 7574 652c 2077  path absolute, w
+00013fe0: 6974 686f 7574 206e 6f72 6d61 6c69 7a61  ithout normaliza
+00013ff0: 7469 6f6e 206f 7220 7265 736f 6c76 696e  tion or resolvin
+00014000: 6720 7379 6d6c 696e 6b73 2e20 5265 7475  g symlinks. Retu
+00014010: 726e 7320 6120 6e65 7720 7061 7468 206f  rns a new path o
+00014020: 626a 6563 740a 2020 2020 2020 2020 2727  bject.        ''
+00014030: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
+00014040: 2073 656c 660a 0a20 2020 2064 6566 2063   self..    def c
+00014050: 7764 2873 656c 6629 202d 3e20 2753 3350  wd(self) -> 'S3P
+00014060: 6174 6827 3a0a 2020 2020 2020 2020 2727  ath':.        ''
+00014070: 2752 6574 7572 6e20 6375 7272 656e 7420  'Return current 
+00014080: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
+00014090: 790a 0a20 2020 2020 2020 2072 6574 7572  y..        retur
+000140a0: 6e73 3a20 4375 7272 656e 7420 776f 726b  ns: Current work
+000140b0: 696e 6720 6469 7265 6374 6f72 790a 2020  ing directory.  
+000140c0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000140d0: 2020 7265 7475 726e 2073 656c 662e 6672    return self.fr
+000140e0: 6f6d 5f70 6174 6828 7365 6c66 2e70 6174  om_path(self.pat
+000140f0: 685f 7769 7468 5f70 726f 746f 636f 6c29  h_with_protocol)
+00014100: 0a0a 0a63 6c61 7373 204d 756c 7469 5061  ...class MultiPa
+00014110: 7274 5772 6974 6572 3a0a 0a20 2020 2064  rtWriter:..    d
+00014120: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00014130: 2c20 636c 6965 6e74 2c20 7061 7468 3a20  , client, path: 
+00014140: 5061 7468 4c69 6b65 2920 2d3e 204e 6f6e  PathLike) -> Non
+00014150: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
+00014160: 5f63 6c69 656e 7420 3d20 636c 6965 6e74  _client = client
+00014170: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+00014180: 756c 7469 7061 7274 5f75 706c 6f61 645f  ultipart_upload_
+00014190: 696e 666f 203d 205b 5d0a 0a20 2020 2020  info = []..     
+000141a0: 2020 2062 7563 6b65 742c 206b 6579 203d     bucket, key =
+000141b0: 2070 6172 7365 5f73 335f 7572 6c28 7061   parse_s3_url(pa
+000141c0: 7468 290a 2020 2020 2020 2020 7365 6c66  th).        self
+000141d0: 2e5f 6275 636b 6574 203d 2062 7563 6b65  ._bucket = bucke
+000141e0: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
+000141f0: 6b65 7920 3d20 6b65 790a 2020 2020 2020  key = key.      
+00014200: 2020 7365 6c66 2e5f 7570 6c6f 6164 5f69    self._upload_i
+00014210: 6420 3d20 7365 6c66 2e5f 636c 6965 6e74  d = self._client
+00014220: 2e63 7265 6174 655f 6d75 6c74 6970 6172  .create_multipar
+00014230: 745f 7570 6c6f 6164 280a 2020 2020 2020  t_upload(.      
+00014240: 2020 2020 2020 4275 636b 6574 3d73 656c        Bucket=sel
+00014250: 662e 5f62 7563 6b65 742c 204b 6579 3d73  f._bucket, Key=s
+00014260: 656c 662e 5f6b 6579 295b 2755 706c 6f61  elf._key)['Uploa
+00014270: 6449 6427 5d0a 0a20 2020 2064 6566 2075  dId']..    def u
+00014280: 706c 6f61 645f 7061 7274 2873 656c 662c  pload_part(self,
+00014290: 2070 6172 745f 6e75 6d3a 2069 6e74 2c20   part_num: int, 
+000142a0: 6669 6c65 5f6f 626a 3a20 696f 2e42 7974  file_obj: io.Byt
+000142b0: 6573 494f 2920 2d3e 204e 6f6e 653a 0a20  esIO) -> None:. 
+000142c0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000142d0: 3d20 7365 6c66 2e5f 636c 6965 6e74 2e75  = self._client.u
+000142e0: 706c 6f61 645f 7061 7274 280a 2020 2020  pload_part(.    
+000142f0: 2020 2020 2020 2020 426f 6479 3d66 696c          Body=fil
+00014300: 655f 6f62 6a2c 0a20 2020 2020 2020 2020  e_obj,.         
+00014310: 2020 2055 706c 6f61 6449 643d 7365 6c66     UploadId=self
+00014320: 2e5f 7570 6c6f 6164 5f69 642c 0a20 2020  ._upload_id,.   
+00014330: 2020 2020 2020 2020 2050 6172 744e 756d           PartNum
+00014340: 6265 723d 7061 7274 5f6e 756d 2c0a 2020  ber=part_num,.  
+00014350: 2020 2020 2020 2020 2020 4275 636b 6574            Bucket
+00014360: 3d73 656c 662e 5f62 7563 6b65 742c 0a20  =self._bucket,. 
+00014370: 2020 2020 2020 2020 2020 204b 6579 3d73             Key=s
+00014380: 656c 662e 5f6b 6579 2c0a 2020 2020 2020  elf._key,.      
+00014390: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+000143a0: 2e5f 6d75 6c74 6970 6172 745f 7570 6c6f  ._multipart_uplo
+000143b0: 6164 5f69 6e66 6f2e 6170 7065 6e64 280a  ad_info.append(.
+000143c0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+000143d0: 2020 2020 2020 2020 2020 2020 2020 2750                'P
+000143e0: 6172 744e 756d 6265 7227 3a20 7061 7274  artNumber': part
+000143f0: 5f6e 756d 2c0a 2020 2020 2020 2020 2020  _num,.          
+00014400: 2020 2020 2020 2745 5461 6727 3a20 7265        'ETag': re
+00014410: 7370 6f6e 7365 5b27 4554 6167 275d 0a20  sponse['ETag']. 
+00014420: 2020 2020 2020 2020 2020 207d 290a 0a20             }).. 
+00014430: 2020 2064 6566 2075 706c 6f61 645f 7061     def upload_pa
+00014440: 7274 5f62 795f 7061 7468 7328 0a20 2020  rt_by_paths(.   
+00014450: 2020 2020 2020 2020 2073 656c 662c 2070           self, p
+00014460: 6172 745f 6e75 6d3a 2069 6e74 2c20 7061  art_num: int, pa
+00014470: 7468 733a 204c 6973 745b 5475 706c 655b  ths: List[Tuple[
+00014480: 5061 7468 4c69 6b65 2c20 7374 725d 5d29  PathLike, str]])
+00014490: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000144a0: 2020 6669 6c65 5f6f 626a 203d 2069 6f2e    file_obj = io.
+000144b0: 4279 7465 7349 4f28 290a 2020 2020 2020  BytesIO().      
+000144c0: 2020 666f 7220 7061 7468 2c20 6279 7465    for path, byte
+000144d0: 735f 7261 6e67 6520 696e 2070 6174 6873  s_range in paths
+000144e0: 3a0a 2020 2020 2020 2020 2020 2020 6275  :.            bu
+000144f0: 636b 6574 2c20 6b65 7920 3d20 7061 7273  cket, key = pars
+00014500: 655f 7333 5f75 726c 2870 6174 6829 0a20  e_s3_url(path). 
+00014510: 2020 2020 2020 2020 2020 2069 6620 6279             if by
+00014520: 7465 735f 7261 6e67 653a 0a20 2020 2020  tes_range:.     
+00014530: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+00014540: 6f62 6a2e 7772 6974 6528 0a20 2020 2020  obj.write(.     
+00014550: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014560: 656c 662e 5f63 6c69 656e 742e 6765 745f  elf._client.get_
+00014570: 6f62 6a65 6374 280a 2020 2020 2020 2020  object(.        
+00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014590: 4275 636b 6574 3d62 7563 6b65 742c 204b  Bucket=bucket, K
+000145a0: 6579 3d6b 6579 2c0a 2020 2020 2020 2020  ey=key,.        
+000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145c0: 5261 6e67 653d 6279 7465 735f 7261 6e67  Range=bytes_rang
+000145d0: 6529 5b27 426f 6479 275d 2e72 6561 6428  e)['Body'].read(
+000145e0: 2929 0a20 2020 2020 2020 2020 2020 2065  )).            e
+000145f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014600: 2020 2020 2066 696c 655f 6f62 6a2e 7772       file_obj.wr
+00014610: 6974 6528 0a20 2020 2020 2020 2020 2020  ite(.           
+00014620: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00014630: 6c69 656e 742e 6765 745f 6f62 6a65 6374  lient.get_object
+00014640: 2842 7563 6b65 743d 6275 636b 6574 2c0a  (Bucket=bucket,.
+00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014670: 2020 2020 2020 2020 2020 2020 4b65 793d              Key=
+00014680: 6b65 7929 5b27 426f 6479 275d 2e72 6561  key)['Body'].rea
+00014690: 6428 2929 0a20 2020 2020 2020 2066 696c  d()).        fil
+000146a0: 655f 6f62 6a2e 7365 656b 2830 2c20 6f73  e_obj.seek(0, os
+000146b0: 2e53 4545 4b5f 5345 5429 0a20 2020 2020  .SEEK_SET).     
+000146c0: 2020 2073 656c 662e 7570 6c6f 6164 5f70     self.upload_p
+000146d0: 6172 7428 7061 7274 5f6e 756d 2c20 6669  art(part_num, fi
+000146e0: 6c65 5f6f 626a 290a 0a20 2020 2064 6566  le_obj)..    def
+000146f0: 2075 706c 6f61 645f 7061 7274 5f63 6f70   upload_part_cop
+00014700: 7928 0a20 2020 2020 2020 2020 2020 2073  y(.            s
+00014710: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00014720: 2070 6172 745f 6e75 6d3a 2069 6e74 2c0a   part_num: int,.
+00014730: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00014740: 3a20 5061 7468 4c69 6b65 2c0a 2020 2020  : PathLike,.    
+00014750: 2020 2020 2020 2020 636f 7079 5f73 6f75          copy_sou
+00014760: 7263 655f 7261 6e67 653a 204f 7074 696f  rce_range: Optio
+00014770: 6e61 6c5b 7374 725d 203d 204e 6f6e 6529  nal[str] = None)
+00014780: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00014790: 2020 6275 636b 6574 2c20 6b65 7920 3d20    bucket, key = 
+000147a0: 7061 7273 655f 7333 5f75 726c 2870 6174  parse_s3_url(pat
+000147b0: 6829 0a20 2020 2020 2020 2070 6172 616d  h).        param
+000147c0: 7320 3d20 6469 6374 280a 2020 2020 2020  s = dict(.      
+000147d0: 2020 2020 2020 5570 6c6f 6164 4964 3d73        UploadId=s
+000147e0: 656c 662e 5f75 706c 6f61 645f 6964 2c0a  elf._upload_id,.
+000147f0: 2020 2020 2020 2020 2020 2020 5061 7274              Part
+00014800: 4e75 6d62 6572 3d70 6172 745f 6e75 6d2c  Number=part_num,
+00014810: 0a20 2020 2020 2020 2020 2020 2043 6f70  .            Cop
+00014820: 7953 6f75 7263 653d 7b0a 2020 2020 2020  ySource={.      
+00014830: 2020 2020 2020 2020 2020 2742 7563 6b65            'Bucke
+00014840: 7427 3a20 6275 636b 6574 2c0a 2020 2020  t': bucket,.    
+00014850: 2020 2020 2020 2020 2020 2020 274b 6579              'Key
+00014860: 273a 206b 6579 0a20 2020 2020 2020 2020  ': key.         
+00014870: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00014880: 2020 4275 636b 6574 3d73 656c 662e 5f62    Bucket=self._b
+00014890: 7563 6b65 742c 0a20 2020 2020 2020 2020  ucket,.         
+000148a0: 2020 204b 6579 3d73 656c 662e 5f6b 6579     Key=self._key
+000148b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000148c0: 2020 2020 6966 2063 6f70 795f 736f 7572      if copy_sour
+000148d0: 6365 5f72 616e 6765 3a0a 2020 2020 2020  ce_range:.      
+000148e0: 2020 2020 2020 7061 7261 6d73 5b27 436f        params['Co
+000148f0: 7079 536f 7572 6365 5261 6e67 6527 5d20  pySourceRange'] 
+00014900: 3d20 636f 7079 5f73 6f75 7263 655f 7261  = copy_source_ra
+00014910: 6e67 650a 2020 2020 2020 2020 7265 7370  nge.        resp
+00014920: 6f6e 7365 203d 2073 656c 662e 5f63 6c69  onse = self._cli
+00014930: 656e 742e 7570 6c6f 6164 5f70 6172 745f  ent.upload_part_
+00014940: 636f 7079 282a 2a70 6172 616d 7329 0a20  copy(**params). 
+00014950: 2020 2020 2020 2073 656c 662e 5f6d 756c         self._mul
+00014960: 7469 7061 7274 5f75 706c 6f61 645f 696e  tipart_upload_in
+00014970: 666f 2e61 7070 656e 6428 0a20 2020 2020  fo.append(.     
+00014980: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00014990: 2020 2020 2020 2020 2027 5061 7274 4e75           'PartNu
+000149a0: 6d62 6572 273a 2070 6172 745f 6e75 6d2c  mber': part_num,
+000149b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000149c0: 2027 4554 6167 273a 2072 6573 706f 6e73   'ETag': respons
+000149d0: 655b 2743 6f70 7950 6172 7452 6573 756c  e['CopyPartResul
+000149e0: 7427 5d5b 2745 5461 6727 5d0a 2020 2020  t']['ETag'].    
+000149f0: 2020 2020 2020 2020 7d29 0a0a 2020 2020          })..    
+00014a00: 6465 6620 636c 6f73 6528 7365 6c66 293a  def close(self):
+00014a10: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+00014a20: 756c 7469 7061 7274 5f75 706c 6f61 645f  ultipart_upload_
+00014a30: 696e 666f 2e73 6f72 7428 6b65 793d 6c61  info.sort(key=la
+00014a40: 6d62 6461 2074 3a20 745b 2750 6172 744e  mbda t: t['PartN
+00014a50: 756d 6265 7227 5d29 0a20 2020 2020 2020  umber']).       
+00014a60: 2073 656c 662e 5f63 6c69 656e 742e 636f   self._client.co
+00014a70: 6d70 6c65 7465 5f6d 756c 7469 7061 7274  mplete_multipart
+00014a80: 5f75 706c 6f61 6428 0a20 2020 2020 2020  _upload(.       
+00014a90: 2020 2020 2055 706c 6f61 6449 643d 7365       UploadId=se
+00014aa0: 6c66 2e5f 7570 6c6f 6164 5f69 642c 0a20  lf._upload_id,. 
+00014ab0: 2020 2020 2020 2020 2020 2042 7563 6b65             Bucke
+00014ac0: 743d 7365 6c66 2e5f 6275 636b 6574 2c0a  t=self._bucket,.
+00014ad0: 2020 2020 2020 2020 2020 2020 4b65 793d              Key=
+00014ae0: 7365 6c66 2e5f 6b65 792c 0a20 2020 2020  self._key,.     
+00014af0: 2020 2020 2020 204d 756c 7469 7061 7274         Multipart
+00014b00: 5570 6c6f 6164 3d7b 2750 6172 7473 273a  Upload={'Parts':
+00014b10: 2073 656c 662e 5f6d 756c 7469 7061 7274   self._multipart
+00014b20: 5f75 706c 6f61 645f 696e 666f 7d29 0a0a  _upload_info})..
+00014b30: 2020 2020 6465 6620 5f5f 656e 7465 725f      def __enter_
+00014b40: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00014b50: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+00014b60: 2020 6465 6620 5f5f 6578 6974 5f5f 2873    def __exit__(s
+00014b70: 656c 662c 2065 7863 5f74 7970 652c 2065  elf, exc_type, e
+00014b80: 7863 5f76 616c 2c20 6578 635f 7462 293a  xc_val, exc_tb):
+00014b90: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+00014ba0: 6f73 6528 290a                           ose().
```

## megfile/sftp_path.py

```diff
@@ -89,15 +89,18 @@
     if not password:
         password = os.getenv(SFTP_PASSWORD)
     private_key = get_private_key()
     return hostname, port, username, password, private_key
 
 
 def sftp_should_retry(error: Exception) -> bool:
-    if isinstance(error, paramiko.ssh_exception.SSHException):
+    if type(error) is EOFError:
+        return False
+    elif isinstance(error,
+                    (paramiko.ssh_exception.SSHException, ConnectionError)):
         return True
     elif isinstance(error, OSError) and str(error) == 'Socket is closed':
         return True
     return False
 
 
 def _patch_sftp_client_request(
```

## megfile/version.py

```diff
@@ -1 +1 @@
-VERSION = "2.0.6.post1"
+VERSION = "2.0.7"
```

## Comparing `megfile-2.0.6.post1.dist-info/LICENSE` & `megfile-2.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `megfile-2.0.6.post1.dist-info/LICENSE.pyre` & `megfile-2.0.7.dist-info/LICENSE.pyre`

 * *Files identical despite different names*

## Comparing `megfile-2.0.6.post1.dist-info/METADATA` & `megfile-2.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megfile
-Version: 2.0.6.post1
+Version: 2.0.7
 Summary: Megvii file operation library
 Home-page: https://github.com/megvii-research/megfile
 Author: megvii
 Author-email: megfile@megvii.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

## Comparing `megfile-2.0.6.post1.dist-info/RECORD` & `megfile-2.0.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 megfile/__init__.py,sha256=wlijLJS6F8Vdm1xjpsjd9fKBeDGpgIMrVsXYSeOQ4Xw,5434
 megfile/cli.py,sha256=t299Wo9lA0EbZlS5k3tCxW19liCqY7-i7zbu8oHOwHo,10033
-megfile/errors.py,sha256=oYmKXD-nguj491hzaRlHfOsE_ENKIGEgSHjECwUHjY4,11686
+megfile/errors.py,sha256=H5wCiVBvOtQo5cu3JLhAUCpQJsCkPNm1KNw9o8y4Las,11349
 megfile/fs.py,sha256=sjkm_LsvNCw8hj9Ee-1HSNzvg7bRHTPem8KTDDBQlCw,11621
 megfile/fs_path.py,sha256=xadMpuqRCdr3CLFmRMg6lTlZfSvnPbc_Dql23NO24SU,38552
 megfile/http.py,sha256=EtyFazgenIhEvkwMpX6ga32POKUG21969Y2cRQbFn58,1852
 megfile/http_path.py,sha256=nmmKLRM5I3SozEfX0m9BcHhSaq8LE4SLTTkBjvQnVEc,4487
 megfile/interfaces.py,sha256=h3tWE8hVt5S-HopaMAX6lunPJ97vzhv6jH_2HubcDNc,6219
 megfile/pathlike.py,sha256=52e6POtMfUCC3Hb9XNwBLXM3Gkz3aGP8H8AagGKlDSg,29307
 megfile/s3.py,sha256=hlXqQvZuXuDJbLjsrK23LD25cblThO9f-r78eWFsYZ8,12456
-megfile/s3_path.py,sha256=C_0xCeuUIj7eMj-Fl-Kt-aM2YTDRAlT87daS8ZwYjvU,85102
+megfile/s3_path.py,sha256=QoVHvOAO-ewYHXYIyKiJXzXNsmnITZg8u1c1dSxvOvE,84902
 megfile/sftp.py,sha256=qzfgI-MGzNsr7adUQaiVKS7zRHGuK-Hs6o45wNIAcww,11943
-megfile/sftp_path.py,sha256=rO7HnJ91Jv849Ns3A4KX3IQTPOPUznL-p2Ycg0SiYnw,44039
+megfile/sftp_path.py,sha256=Wkm4RKt8Se2ZAjhvEo3R5Rs1gR3IlGpC4TFxTGdiI5o,44133
 megfile/smart.py,sha256=l4orTpsYzwuNkg0mdS-gBy2_iZ8asL8UUhqMzztN2xQ,31952
 megfile/smart_path.py,sha256=Rwb1McXsshi9-F6miTRqE6j8FO2j1edjmSxZF32YZ6E,6708
 megfile/stdio.py,sha256=qmi1c7VTll6Y6ya9MCd-dSKffocX2GafA-YUncZRU1Y,559
 megfile/stdio_path.py,sha256=ULMzGOj7SBMn3c7fYVSDepT_1nEUiVetc-xRt2pR5o4,2682
-megfile/version.py,sha256=_qcZEiLLfeioNA5CCIzOkmDuezgK12ue_3nyZYvL9qw,25
+megfile/version.py,sha256=8Oo_AEGb0CBuw8BvcSpsyaxwT_YvFqxMhgZBsUGMyxM,19
 megfile/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 megfile/lib/combine_reader.py,sha256=TkjvYvM5ZBVCh3tA7cOmTe8dYZc_eI7XbpPhnzqaNvU,4580
 megfile/lib/compare.py,sha256=yG2fZve_gMg32rQVCdwixBdqgYRsjn-24TqhALQaOrA,2233
 megfile/lib/compat.py,sha256=QYIO6RkvfJ2ewdn9bP_17H_fhIlfnL9g-4RQnSt18zM,3053
 megfile/lib/fnmatch.py,sha256=HgdlnEWBsdFUOZqnW_v1kj1jeH_9lMcCqW85pyMu4vM,4054
 megfile/lib/glob.py,sha256=OEa3_3sWP_nwgESj5m4XCdNWV44RQKwdB0im6A6haNI,9514
 megfile/lib/joinpath.py,sha256=D4Px6-lnDDpYs1LMUHkTIGqMPJQ0oCBGfTzREs373iU,929
@@ -32,14 +32,14 @@
 megfile/lib/s3_prefetch_reader.py,sha256=zSd_gmpDtQCDA-Rrh7Nxh2WOb0Z8Q1QZZg1g7WO6JNg,15053
 megfile/lib/s3_share_cache_reader.py,sha256=q3MVEDUgOvalO7js6S_LWQ-eJS4xFHiio8ZoJZt40e4,3791
 megfile/lib/shadow_handler.py,sha256=IbFyTw107t-yWH0cGrDjAJX-CS3xeEr77_PTGsnSgk4,2683
 megfile/lib/stdio_handler.py,sha256=QDWtcZxz-hzi-rqQUiSlR3NrihX1fjK_Rj9T2mdTFEg,2044
 megfile/lib/url.py,sha256=VbQLjo0s4AaV0iSk66BcjI68aUTcN9zBZ5x6-cM4Qvs,103
 megfile/utils/__init__.py,sha256=gWplPIHzpSqV9AiQiRvUrBCkD737caNYyudsgwQBbKk,9025
 megfile/utils/mutex.py,sha256=BE16gbmZxr0RgU0ULaAFVDTZGwiOA-Jven-fDeG3ltQ,2461
-megfile-2.0.6.post1.dist-info/LICENSE,sha256=WNHhf_5RCaeuKWyq_K39vmp9F28LxKsB4SpomwSZ2L0,11357
-megfile-2.0.6.post1.dist-info/LICENSE.pyre,sha256=9lf5nT-5ZH25JijpYAequ0bl8E8z5JmZB1qrjiUMp84,1080
-megfile-2.0.6.post1.dist-info/METADATA,sha256=y-7SUwxYATEnq348lFyV7TiHg354HVZABw-AHRgIxoU,10160
-megfile-2.0.6.post1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-megfile-2.0.6.post1.dist-info/entry_points.txt,sha256=M6ZWSSv5_5_QtIpZafy3vq7WuOJ_5dSGQQnEZbByt2Q,49
-megfile-2.0.6.post1.dist-info/top_level.txt,sha256=i3rMgdU1ZAJekAceojhA-bkm3749PzshtRmLTbeLUPQ,8
-megfile-2.0.6.post1.dist-info/RECORD,,
+megfile-2.0.7.dist-info/LICENSE,sha256=WNHhf_5RCaeuKWyq_K39vmp9F28LxKsB4SpomwSZ2L0,11357
+megfile-2.0.7.dist-info/LICENSE.pyre,sha256=9lf5nT-5ZH25JijpYAequ0bl8E8z5JmZB1qrjiUMp84,1080
+megfile-2.0.7.dist-info/METADATA,sha256=eh8bixA1xh4-8rHSzoV-WFzbz71PXcnocLNCOWOMEvI,10154
+megfile-2.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+megfile-2.0.7.dist-info/entry_points.txt,sha256=M6ZWSSv5_5_QtIpZafy3vq7WuOJ_5dSGQQnEZbByt2Q,49
+megfile-2.0.7.dist-info/top_level.txt,sha256=i3rMgdU1ZAJekAceojhA-bkm3749PzshtRmLTbeLUPQ,8
+megfile-2.0.7.dist-info/RECORD,,
```

