# Comparing `tmp/scutls-0.2.5.tar.gz` & `tmp/scutls-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.2.5.tar", max compression
+gzip compressed data, was "scutls-0.2.6.tar", max compression
```

## Comparing `scutls-0.2.5.tar` & `scutls-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      583 2023-06-07 03:49:29.237022 scutls-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-07 03:49:41.441593 scutls-0.2.5/scutls/__init__.py
--rw-r--r--   0        0        0     6256 2023-05-10 15:48:41.694697 scutls-0.2.5/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.5/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.5/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.5/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.5/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     5001 2023-06-07 00:17:17.566877 scutls-0.2.5/scutls/barcode.py
--rw-r--r--   0        0        0     1074 2023-05-10 15:45:19.722039 scutls-0.2.5/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.5/scutls/download.py
--rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.5/scutls/fastq.py
--rw-r--r--   0        0        0     9253 2023-06-07 03:48:53.820816 scutls-0.2.5/scutls/util.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.5/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-06-16 21:11:31.148249 scutls-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-16 21:11:42.503322 scutls-0.2.6/scutls/__init__.py
+-rw-r--r--   0        0        0     6447 2023-06-16 20:58:58.224143 scutls-0.2.6/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.6/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.6/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.6/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.6/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     5324 2023-06-16 20:48:21.500529 scutls-0.2.6/scutls/barcode.py
+-rw-r--r--   0        0        0     1114 2023-06-16 20:42:39.857306 scutls-0.2.6/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.6/scutls/download.py
+-rw-r--r--   0        0        0     3845 2023-06-02 19:44:04.605614 scutls-0.2.6/scutls/fastq.py
+-rw-r--r--   0        0        0     9373 2023-06-16 21:10:25.736248 scutls-0.2.6/scutls/util.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.6/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.6/PKG-INFO
```

### Comparing `scutls-0.2.5/pyproject.toml` & `scutls-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.2.5"
+version = "0.2.6"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.2.5/scutls/arguments.py` & `scutls-0.2.6/scutls/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,19 +157,25 @@
 
 parser_barcode.add_argument(
     "-e", "--error",
     help = "allowed mismatchs (including INDELs) when searching for barcode string",
     required = False, type = int, default = 1
 )
 parser_barcode.add_argument(
+    "-m", "--mismatch_only",
+    help = "exclude INDELs when searching for barcode string",
+    required = False, default = False, 
+    action = 'store_true'
+)
+parser_barcode.add_argument(
     "-rcb", "--rc_barcode", 
     help = "reverse complement the barcode before searching",
     required = False,
     default = False,
-    action='store_true' # quick hack to skip requred input: https://stackoverflow.com/questions/59363298/argparse-expected-one-argument
+    action = 'store_true' # quick hack to skip requred input: https://stackoverflow.com/questions/59363298/argparse-expected-one-argument
 )
 parser_barcode.add_argument(
     "-nproc", "--num_processor",
     help = "number of parallel jobs",
     required = False, type = int, default = 1
 )
 ## set default values
```

### Comparing `scutls-0.2.5/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.2.6/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.5/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.2.6/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.2.5/scutls/assets/genome_ucsc.json` & `scutls-0.2.6/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.5/scutls/barcode.py` & `scutls-0.2.6/scutls/barcode.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,35 +3,37 @@
 from multiprocessing import Pool
 from Bio import SeqIO, bgzf
 from Bio.Seq import Seq
 from .util import fastq_chunk_interval, fastq_contain_barcode, get_search_pattern, fastq_locate_barcode
 import os
 import regex
 
-def barcode(input = None, output = None, output2 = None, contain = None, locate = None, pos = 0, error = 1, rc_barcode = False, nproc = 1):
+def barcode(input = None, output = None, output2 = None, contain = None, locate = None, pos = 0, error = 1, mismatch_only = False, rc_barcode = False, nproc = 1):
     """barcode subcommand
     Paramters
     ---------
 
     input : str
         input file name, auto detects .gz
     output : str
         output file name, auto detects .gz, contains fastq that contains specified barcode via contain
     contain: str
         barcode to detect, if multiple barcode, separate with comma: "AATTCCC,AGGGCCC,CCGGCG"
         # optional for "contain" sub-command:
         error: int
-            allowed nucleotide mismatches (can be INDELs) when aligning, default to 1
+            allowed nucleotide mismatches (can be INDELs) when searching regex pattern, default to 1
+        mismatch_only: bool
+            if true, only mismatches (INDELs excluded) are allowed when searching regex pattern, default to False
         nproc: int
             number of parallel jobs, default to 1
         rc_barcode: bool
             take reverse complement of the barcode when aligning, default to False
     locate: str
         barcode to detect its location in reads
-        # shared arguments with "contain": error, nproc, rc_barcode
+        # shared arguments with "contain": error, mismatch_only, nproc, rc_barcode
         pos: int
             which matched position to return, default to 0 meaning the first, use -1 to indicate the last.
         
     """
 
     args = list(locals().keys())
 
@@ -40,15 +42,15 @@
         print("scutls fastq: warning: use 'scutls contain -h' for usage")
     # use True since args can be either None or False
     # arguments.py defines requirments of each argument
 
     # check if input fastq contains specified barcode:
     if contain:
         # prepare search pattern
-        barcode_pattern = get_search_pattern(pattern = contain, error = error, rc_barcode = rc_barcode)
+        barcode_pattern = get_search_pattern(pattern = contain, error = error, mismatch_only = mismatch_only, rc_barcode = rc_barcode)
         
         # print("barcode_pattern: ", barcode_pattern)
 
         # multiprocessing
         if not output == None:
             print("Saving to " + output + " ...")
         else:
@@ -90,15 +92,15 @@
                 SeqIO.write(fastq_non_hit, output2, "fastq")
         
         print("Done!")
 
     # check if input fastq contains specified barcode
     if locate:
         # prepare search pattern
-        barcode_pattern = get_search_pattern(pattern = locate, error = error, rc_barcode = rc_barcode)
+        barcode_pattern = get_search_pattern(pattern = locate, error = error, mismatch_only = mismatch_only, rc_barcode = rc_barcode)
 
         # multiprocessing
         intervals = fastq_chunk_interval(input, nproc = nproc)
         p = Pool(nproc)
         res_list = p.map_async(
             functools.partial(
                 fastq_locate_barcode,
@@ -117,12 +119,13 @@
     parser.add_argument('--output', '-o', type   = str)
     parser.add_argument('--output2', '-o2', type = str)
     parser.add_argument('--contain', '-c', type = str)
     parser.add_argument('--locate', '-l', type = str)
     parser.add_argument('--position', '-p', type = int)
     
     parser.add_argument('--error',   '-e', type   = int)
+    parser.add_argument('--mismatch_only', '-m', default = False)
     parser.add_argument('--rc_barcode', '-rcb', default = False)
     parser.add_argument('--num_processor', '-nproc', default = 1)
     
 if __name__ == "__main__":
     main()
```

### Comparing `scutls-0.2.5/scutls/cli.py` & `scutls-0.2.6/scutls/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,10 +29,11 @@
     input  = args.input,
     output = args.output,
     output2 = args.output2,
     contain = args.contain,
     locate = args.locate,
     pos = args.position,
     error   = args.error,
+    mismatch_only = args.mismatch_only,
     rc_barcode = args.rc_barcode,
     nproc = args.num_processor # must use full name
     )
```

### Comparing `scutls-0.2.5/scutls/download.py` & `scutls-0.2.6/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.5/scutls/fastq.py` & `scutls-0.2.6/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.5/scutls/util.py` & `scutls-0.2.6/scutls/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,48 +194,53 @@
                 if regex.search(barcode_pattern, str(record.seq)):
                     fastq_hit.append(record)
                 else:
                     fastq_non_hit.append(record)
     return([fastq_hit, fastq_non_hit])
 
 # obtain search pattern given string pattern and allowed mismatches (error)
-def get_search_pattern(pattern, error, rc_barcode):
+def get_search_pattern(pattern, error, mismatch_only, rc_barcode):
+    if mismatch_only:
+        error_pattern = "){s<="
+    else:
+        error_pattern = "){e<="
+    
     if not "," in pattern:
         if rc_barcode:
             pattern = str(Seq(pattern).reverse_complement())
-        barcode_pattern = "(" + pattern + "){e<=" + str(error) + "}"
+        barcode_pattern = "(" + pattern + error_pattern + str(error) + "}"
     else:
         barcode_pattern = ""
         barcodes = pattern.split(",")
         if rc_barcode:
             barcodes = barcodes[::-1]
             
         for barcode in barcodes:
             if rc_barcode:
                 pattern = str(Seq(barcode).reverse_complement())
             else:
                 pattern = barcode
-            barcode_pattern += "(" + pattern + "){e<=" + str(error) + "}(.*?)"
+            barcode_pattern += "(" + pattern + error_pattern + str(error) + "}(.*?)"
     return(barcode_pattern)
 
 # obtain fastq coordinates for specified barcode
 def fastq_locate_barcode(interval, fastq, barcode_pattern, pos = 0):
     """
     pos: which match to return: use 0 for the first match, use -1 for the last match.
     The return value will be: record.id match_location_0_based len(record.seq)s
     
     """
     res = []
+
     with _open(fastq) as f:
         for i, record in enumerate(SeqIO.parse(f, "fastq")):
             if i in interval:
                 matches = regex.finditer(barcode_pattern, str(record.seq))
                 # tem = [match for match in matches]
                 pos_start = [match.start() for match in matches]
-        
                 if not len(pos_start) == 0:
                     res.append([record.id, pos_start[pos], len(record.seq)])
                 else:
                     res.append([record.id, "NA", len(record.seq)])
     return(res)
 
 if __name__ == "__main__":
```

### Comparing `scutls-0.2.5/setup.py` & `scutls-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.2.5/PKG-INFO` & `scutls-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.2.5
+Version: 0.2.6
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

