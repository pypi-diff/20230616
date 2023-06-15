# Comparing `tmp/gseapy-1.0.4.tar.gz` & `tmp/gseapy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gseapy-1.0.4.tar", last modified: Wed Feb  8 00:03:06 2023, max compression
+gzip compressed data, was "dist/gseapy-1.0.5.tar", last modified: Thu Jun 15 23:00:24 2023, max compression
```

## Comparing `gseapy-1.0.4.tar` & `gseapy-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 00:03:06.000000 gseapy-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-08 00:02:54.000000 gseapy-1.0.4/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-08 00:02:54.000000 gseapy-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-08 00:02:54.000000 gseapy-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-02-08 00:03:06.000000 gseapy-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-02-08 00:02:54.000000 gseapy-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy/
--rw-r--r--   0 runner    (1001) docker     (123)    25556 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24344 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27980 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25707 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/biomart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy/data/
--rw-r--r--   0 runner    (1001) docker     (123)    23465 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/data/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)    19620 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/enrichr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30264 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/gsea.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    45295 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/scipalette.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-02-08 00:02:54.000000 gseapy-1.0.4/gseapy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-08 00:03:06.000000 gseapy-1.0.4/gseapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-08 00:02:54.000000 gseapy-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-08 00:02:54.000000 gseapy-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 00:03:06.000000 gseapy-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-02-08 00:02:54.000000 gseapy-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 00:03:06.000000 gseapy-1.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-02-08 00:02:54.000000 gseapy-1.0.4/src/algorithm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-02-08 00:02:54.000000 gseapy-1.0.4/src/help.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-02-08 00:02:54.000000 gseapy-1.0.4/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    42893 2023-02-08 00:02:54.000000 gseapy-1.0.4/src/stats.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-02-08 00:02:54.000000 gseapy-1.0.4/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 00:03:06.000000 gseapy-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-02-08 00:02:54.000000 gseapy-1.0.4/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:24.000000 gseapy-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 23:00:14.000000 gseapy-1.0.5/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-15 23:00:14.000000 gseapy-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 23:00:14.000000 gseapy-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-06-15 23:00:24.000000 gseapy-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-06-15 23:00:14.000000 gseapy-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26045 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24685 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27980 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28339 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/biomart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    23465 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/data/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/enrichr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30264 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/gsea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55789 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/scipalette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-15 23:00:14.000000 gseapy-1.0.5/gseapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 23:00:24.000000 gseapy-1.0.5/gseapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 23:00:14.000000 gseapy-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 23:00:14.000000 gseapy-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 23:00:24.000000 gseapy-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-15 23:00:14.000000 gseapy-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:24.000000 gseapy-1.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-06-15 23:00:14.000000 gseapy-1.0.5/src/algorithm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-06-15 23:00:14.000000 gseapy-1.0.5/src/help.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-15 23:00:14.000000 gseapy-1.0.5/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-06-15 23:00:14.000000 gseapy-1.0.5/src/stats.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-06-15 23:00:14.000000 gseapy-1.0.5/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:24.000000 gseapy-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 23:00:15.000000 gseapy-1.0.5/tests/test_commands.py
```

### Comparing `gseapy-1.0.4/Cargo.toml` & `gseapy-1.0.5/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/LICENSE` & `gseapy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/PKG-INFO` & `gseapy-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gseapy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Gene Set Enrichment Analysis in Python
 Home-page: https://github.com/zqfang/gseapy
 Download-URL: https://github.com/zqfang/gseapy
 Author: Zhuoqing Fang
 Author-email: fzq518@gmail.com
 License: MIT
 Project-URL: Documentation, https://gseapy.readthedocs.io/en/latest/
```

### Comparing `gseapy-1.0.4/README.rst` & `gseapy-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/gseapy/__init__.py` & `gseapy-1.0.5/gseapy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 import pandas as pd
 
 from .__main__ import __version__
 from .biomart import Biomart
 from .enrichr import Enrichr
 from .gsea import GSEA, Prerank, Replot, SingleSampleGSEA
 from .parser import get_library, get_library_name, read_gmt
-from .plot import barplot, dotplot, enrichment_map, gseaplot, heatmap, ringplot
+from .plot import (
+    barplot,
+    dotplot,
+    enrichment_map,
+    gseaplot,
+    gseaplot2,
+    heatmap,
+    ringplot,
+)
 
 
 def gsea(
     data: Union[pd.DataFrame, str],
     gene_sets: Union[List[str], str, Dict[str, str]],
     cls: Union[List[str], str],
     outdir: Optional[str] = None,
@@ -251,16 +259,34 @@
                  |  matched genes: genes matched to the data,
                  | }
 
 
     """
     if "processes" in kwargs:
         warnings.warn("processes is deprecated; use threads", DeprecationWarning, 2)
-        kwargs["threads"] = kwargs["processes"]
-    ss = SingleSampleGSEA(data=data, gene_sets=gene_sets, **kwargs)
+        threads = kwargs["processes"]
+    ss = SingleSampleGSEA(
+        data=data,
+        gene_sets=gene_sets,
+        outdir=outdir,
+        sample_norm_method=sample_norm_method,
+        correl_norm_type=correl_norm_type,
+        min_size=min_size,
+        max_size=max_size,
+        permutation_num=permutation_num,
+        weight=weighted_score_type,
+        ascending=ascending,
+        threads=threads,
+        figsize=figsize,
+        format=format,
+        graph_num=graph_num,
+        no_plot=no_plot,
+        seed=seed,
+        verbose=verbose,
+    )
     ss.run()
     return ss
 
 
 def prerank(
     rnk: Union[pd.DataFrame, pd.Series, str],
     gene_sets: Union[List[str], str, Dict[str, str]],
@@ -401,15 +427,15 @@
 
 
 def enrichr(
     gene_list: Iterable[str],
     gene_sets: Union[List[str], str, Dict[str, str]],
     organism: str = "human",
     outdir: Optional[str] = None,
-    background: Union[List[str], int, str] = "hsapiens_gene_ensembl",
+    background: Union[List[str], int, str] = None,
     cutoff: float = 0.05,
     format: str = "pdf",
     figsize: Tuple[float, float] = (6.5, 6),
     top_term: int = 10,
     no_plot: bool = False,
     verbose: bool = False,
 ) -> Enrichr:
@@ -613,14 +639,15 @@
 __all__ = [
     "dotplot",
     "barplot",
     "enrichment_map",
     "ringplot",
     "heatmap",
     "gseaplot",
+    "gseaplot2",
     "replot",
     "prerank",
     "gsea",
     "ssgsea",
     "enrichr",
     "enrich",
     "Replot",
```

### Comparing `gseapy-1.0.4/gseapy/__main__.py` & `gseapy-1.0.5/gseapy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Main function
 # ------------------------------------
 
 # there is a bug in add_argument(required=True), for hacking, don't set metavar='' when required=True,
 # or args = argparser.parse_args() will throw bugs!!!
 
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 
 def main():
     """The Main function/pipeline for GSEApy."""
 
     # Parse options...
     argparser = prepare_argparser()
@@ -755,17 +755,21 @@
         help="Adjust-Pval cutoff, used for generating plots. Default: 0.05.",
     )
     enrichr_opt.add_argument(
         "--bg",
         "--background",
         action="store",
         dest="bg",
-        default="hsapiens_gene_ensembl",
-        metavar="BGNUM",
-        help="BioMart Dataset name or Background total genes number. Default: None",
+        default=None,
+        metavar="BG",
+        help="Choose background from one of the following. \n"
+        + "(1) A BioMart Dataset name, e.g. 'hsapiens_gene_ensembl' . \n"
+        + "(2) A total gene number, e.g. 20000. Only works for GMT file input. \n"
+        + "(3) A text file contains the background gene list (one gene per row). Gene identifier should be the same to your input (-i). \n"
+        + "(4) Default: None. It means all genes in the (-g) input as the background.",
     )
     enrichr_opt.add_argument(
         "-t",
         "--top-term",
         dest="term",
         action="store",
         type=int,
```

### Comparing `gseapy-1.0.4/gseapy/algorithm.py` & `gseapy-1.0.5/gseapy/algorithm.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/gseapy/base.py` & `gseapy-1.0.5/gseapy/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #! python
 # -*- coding: utf-8 -*-
 
 import json
 import logging
 import os
-from tempfile import TemporaryDirectory
-from typing import Dict, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-import requests
 
-from gseapy.plot import gseaplot, heatmap
+from gseapy.plot import GSEAPlot, TracePlot, gseaplot, heatmap
 from gseapy.utils import DEFAULT_CACHE_PATH, log_init, mkdirs, retry
 
 
 class GSEAbase(object):
     """base class of GSEA."""
 
     def __init__(
@@ -27,15 +25,14 @@
         enrichr_url: str = "http://maayanlab.cloud",
         verbose: bool = False,
     ):
         self.outdir = outdir
         self.gene_sets = gene_sets
         self.fdr = 0.05
         self.module = module
-        self.results = None
         self.res2d = None
         self.ranking = None
         self.ascending = False
         self.verbose = verbose
         self._threads = threads
         self.ENRICHR_URL = enrichr_url
         self.pheno_pos = ""
@@ -341,25 +338,29 @@
         # Plotting
         for i, idx in enumerate(indices):
             record = self.res2d.iloc[idx]
             if self.module != "ssgsea" and record["FDR q-val"] > 0.25:
                 continue
             if i >= self.graph_num:  # already sorted by abs(NES) in descending order
                 break
-            if self.res2d["Name"].nunique() > 1 and hasattr(
-                self, "_metric_dict"
-            ):  # self.module != "ssgsea":
-                key = record["Name"]
-                rank_metric = metric[key]
-                hit = self.results[key][record["Term"]]["hits"]
-                RES = self.results[key][record["Term"]]["RES"]
-            else:
-                rank_metric = metric[self.module]
-                hit = self.results[record["Term"]]["hits"]
-                RES = self.results[record["Term"]]["RES"]
+            # if self.res2d["Name"].nunique() > 1 and hasattr(
+            #     self, "_metric_dict"
+            # ):  # self.module != "ssgsea":
+            #     key = record["Name"]
+            #     rank_metric = metric[key]
+            #     hit = self._results[key][record["Term"]]["hits"]
+            #     RES = self._results[key][record["Term"]]["RES"]
+            # else:
+            #     rank_metric = metric[self.module]
+            #     hit = self._results[record["Term"]]["hits"]
+            #     RES = self._results[record["Term"]]["RES"]
+            key = record["Name"]
+            rank_metric = metric[key]
+            hit = self._results[key][record["Term"]]["hits"]
+            RES = self._results[key][record["Term"]]["RES"]
 
             outdir = os.path.join(self.outdir, record["Name"])
             mkdirs(outdir)
             term = record["Term"].replace("/", "-").replace(":", "_")
             outfile = os.path.join(outdir, "{0}.{1}".format(term, self.format))
             if self.module == "gsea":
                 outfile2 = "{0}/{1}.heatmap.{2}".format(outdir, term, self.format)
@@ -375,21 +376,21 @@
                     xticklabels=True,
                     yticklabels=True,
                 )
 
             if self.permutation_num > 0:
                 # skip plotting when nperm=0
                 gseaplot(
-                    rank_metric=rank_metric,
                     term=record["Term"].split("__")[-1],
                     hits=hit,
                     nes=record["NES"],
                     pval=record["NOM p-val"],
                     fdr=record["FDR q-val"],
                     RES=RES,
+                    rank_metric=rank_metric,
                     pheno_pos=self.pheno_pos,
                     pheno_neg=self.pheno_neg,
                     figsize=self.figsize,
                     ofname=outfile,
                 )
 
     def _to_df(
@@ -495,21 +496,23 @@
                 for i, n in enumerate(rank_metric.columns)  # indices is a 2d list
             }
         else:
             metric = {self.module: rank_metric}
             self._metric_dict = {self.module: self.module}
 
         res_df = self._to_df(gsea_summary, gmt, metric)
-        self.results = {}
+        self._results = {}
         # save dict
-        if res_df["name"].nunique() >= 2:
-            for name, dd in res_df.groupby(["name"]):
-                self.results[name] = dd.set_index("term").to_dict(orient="index")
-        else:
-            self.results = res_df.set_index("term").to_dict(orient="index")
+        # if res_df["name"].nunique() >= 2:
+        #     for name, dd in res_df.groupby(["name"]):
+        #         self._results[name] = dd.set_index("term").to_dict(orient="index")
+        # else:
+        #     self._results = res_df.set_index("term").to_dict(orient="index")
+        for name, dd in res_df.groupby("name"):
+            self._results[name] = dd.set_index("term").to_dict(orient="index")
         # trim
         res_df.rename(
             columns={
                 "name": "Name",
                 "term": "Term",
                 "es": "ES",
                 "nes": "NES",
@@ -559,14 +562,24 @@
                     gg = "\t".join(genes)
                     gout.write(f"{term}\t{collection}\t{gg}\n")
         # generate gseaplots
         if not self._noplot:
             self._plotting(metric)
         return
 
+    @property
+    def results(self):
+        """
+        compatible to old style
+        """
+        keys = list(self._results.keys())
+        if len(keys) == 1:
+            return self._results[keys[0]]
+        return self._results
+
     def enrichment_score(
         self,
         gene_list: Iterable[str],
         correl_vector: Iterable[float],
         gene_set: Dict[str, List[str]],
         weight: float = 1.0,
         nperm: int = 1000,
@@ -651,7 +664,68 @@
         else:
             max_ES, min_ES = RES.max(axis=axis), RES.min(axis=axis)
             es_vec = np.where(np.abs(max_ES) > np.abs(min_ES), max_ES, min_ES)
         # extract values
         es, esnull, RES = es_vec[-1], es_vec[:-1], RES[-1, :]
 
         return es, esnull, hit_ind, RES
+
+    def plot(
+        self,
+        terms: Union[str, List[str]],
+        colors: Optional[Union[str, List[str]]] = None,
+        legend_kws: Optional[Dict[str, Any]] = None,
+        figsize: Tuple[float, float] = (4, 5),
+        show_ranking: bool = True,
+        ofname: Optional[str] = None,
+    ):
+        """
+        terms: str, list.  terms/pathways to show
+        colors: str, list. list of colors for each term/pathway
+        legend_kws: kwargs to pass to ax.legend. e.g. `loc`, `bbox_to_achor`.
+        ofname: savefig
+        """
+        # if hasattr(self, "results"):
+        if self.module == "ssgsea":
+            raise NotImplementedError("not for ssgsea")
+        keys = list(self._results.keys())
+        if len(keys) > 1:
+            raise NotImplementedError("Multiple Dataset input No supported yet!")
+
+        ranking = self.ranking if show_ranking else None
+        if isinstance(terms, str):
+            gsdict = self.results[terms]
+            g = GSEAPlot(
+                term=terms,
+                tag=gsdict["hits"],
+                rank_metric=ranking,
+                runes=gsdict["RES"],
+                nes=gsdict["nes"],
+                pval=gsdict["pval"],
+                fdr=gsdict["fdr"],
+                ofname=ofname,
+                pheno_pos=self.pheno_pos,
+                pheno_neg=self.pheno_neg,
+                color=colors,
+                figsize=figsize,
+            )
+            g.add_axes()
+            g.savefig()
+            return g.fig
+
+        elif hasattr(terms, "__len__"):  # means iterable
+            terms = list(terms)
+            tags = [self.results[t]["hits"] for t in terms]
+            runes = [self.results[t]["RES"] for t in terms]
+            t = TracePlot(
+                terms=terms,
+                tags=tags,
+                runes=runes,
+                rank_metric=ranking,
+                colors=colors,
+                legend_kws=legend_kws,
+            )
+            t.add_axes()
+            t.savefig(ofname)
+            return t.fig
+        else:
+            print("not supported input: terms")
```

### Comparing `gseapy-1.0.4/gseapy/biomart.py` & `gseapy-1.0.5/gseapy/biomart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 from collections.abc import Iterable
 from io import StringIO
 from typing import Any, AnyStr, Dict, Iterable, List, Optional, Set, Tuple, Union
 from xml.etree import cElementTree as ET
 
 import pandas as pd
 import requests
@@ -267,14 +268,15 @@
 
         if "entrezgene_id" in df.columns:
             df["entrezgene_id"] = df["entrezgene_id"].astype(pd.Int32Dtype())
 
         self.results = df
         # save file to cache path.
         if filename is not None:
+            mkdirs(os.path.dirname(filename))
             df.to_csv(filename, sep="\t", index=False)
 
         return df
 
     def query_simple(
         self,
         dataset: str = "hsapiens_gene_ensembl",
```

### Comparing `gseapy-1.0.4/gseapy/data/palette.json` & `gseapy-1.0.5/gseapy/data/palette.json`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/gseapy/enrichr.py` & `gseapy-1.0.5/gseapy/enrichr.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 from collections import OrderedDict
 from io import StringIO
 from typing import Any, AnyStr, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 import pandas as pd
 import requests
-from numpy import isscalar
+from numpy import isscalar, log
 
 from gseapy.biomart import Biomart
 from gseapy.plot import barplot
 from gseapy.stats import calc_pvalues, multiple_testing_correction
 from gseapy.utils import DEFAULT_CACHE_PATH, log_init, mkdirs, retry
 
 
@@ -49,14 +49,15 @@
         self.module = "enrichr"
         self.res2d = None
         self.background = background
         self._bg = None
         self.organism = organism
         self._organism = None
         self.ENRICHR_URL = "http://maayanlab.cloud"
+        self.ENRICHR_URL_SPEED = "https://maayanlab.cloud/speedrichr"
         # init logger
         self.prepare_outdir()
 
     def __del__(self):
         handlers = self._logger.handlers[:]
         for handler in handlers:
             handler.close()  # close file
@@ -189,28 +190,45 @@
         if self._isezid:
             self._gls = set(map(int, genes))
         else:
             self._gls = genes
 
         return "\n".join(genes)
 
-    def send_genes(self, gene_list, url) -> AnyStr:
+    def send_genes(self, payload, url) -> Dict:
         """send gene list to enrichr server"""
-        payload = {"list": (None, gene_list), "description": (None, self.descriptions)}
+        # payload = {"list": (None, gene_list), "description": (None, self.descriptions)}
         # response
         s = retry(num=5)
         response = s.post(url, files=payload, verify=True)
         if not response.ok:
             self._logger.debug(url)
             self._logger.debug(payload)
             raise Exception("Error sending gene list, try again later")
         job_id = json.loads(response.text)
-
+        # response.text
+        # {
+        # 	"userListId": 667152768,
+        # 	"shortId": "27c3f180"
+        # }
         return job_id
 
+    def send_background(self, payload, url) -> Dict:
+        s = retry(num=5)
+        res = s.post(url, data=payload)
+        if not res.ok:
+            self._logger.debug(url)
+            self._logger.debug(payload)
+            raise Exception("Error sending background list, try again later")
+        background_response = res.json()
+        # {
+        #     "backgroundid": "3ff7ef9d"
+        # }
+        return background_response
+
     def check_genes(self, gene_list: List[str], usr_list_id: str):
         """
         Compare the genes sent and received to get successfully recognized genes
         """
         response = requests.get(
             "%s/%s/view?userListId=%s"
             % (self.ENRICHR_URL, self._organism, usr_list_id),
@@ -220,18 +238,72 @@
             raise Exception("Error getting gene list back")
         returnedL = json.loads(response.text)["genes"]
         returnedN = sum([1 for gene in gene_list if gene in returnedL])
         self._logger.info(
             "{} genes successfully recognized by Enrichr".format(returnedN)
         )
 
+    def get_results_with_background(
+        self, gene_list: List[str], background: List[str]
+    ) -> Tuple[AnyStr, pd.DataFrame]:
+        ## add gene list
+        ADDLIST_URL = "%s/api/addList" % (self.ENRICHR_URL_SPEED)
+        payload = {"list": (None, gene_list), "description": (None, self.descriptions)}
+        job_id = self.send_genes(payload, ADDLIST_URL)
+        ## add background list
+        ADDBG_URL = "%s/api/addbackground" % (self.ENRICHR_URL_SPEED)
+        payload = dict(background="\n".join(background))
+        bg_id = self.send_background(payload, ADDBG_URL)
+
+        # now get background enrich result
+        BGENR_URL = "%s/api/backgroundenrich" % (self.ENRICHR_URL_SPEED)
+        payload = dict(
+            userListId=job_id["userListId"],
+            backgroundid=bg_id["backgroundid"],
+            backgroundType=self._gs,
+        )
+        s = retry(num=5)
+        response = s.post(BGENR_URL, data=payload)
+        if not response.ok:
+            self._logger.error("Error fetching enrichment results: %s" % self._gs)
+
+        data = response.json()
+        # Note: missig Overlap column
+        colnames = [
+            "Rank",
+            "Term",
+            "P-value",
+            "Odds Ratio",  # Z-Score
+            "Combined Score",
+            "Genes",
+            "Adjusted P-value",
+            "Old P-value",
+            "Old adjusted P-value",
+        ]
+        res = pd.DataFrame(data[self._gs], columns=colnames)
+        # res.drop(columns=["Rank"], inplace=True)
+        res["Genes"] = res["Genes"].apply(";".join)
+        colord = [
+            "Term",
+            "P-value",
+            "Adjusted P-value",
+            "Old P-value",
+            "Old adjusted P-value",
+            "Odds Ratio",  # Z-Score
+            "Combined Score",
+            "Genes",
+        ]
+        res = res.loc[:, colord]
+        return (job_id["shortId"], res)
+
     def get_results(self, gene_list: List[str]) -> Tuple[AnyStr, pd.DataFrame]:
         """Enrichr API"""
         ADDLIST_URL = "%s/%s/addList" % (self.ENRICHR_URL, self._organism)
-        job_id = self.send_genes(gene_list, ADDLIST_URL)
+        payload = {"list": (None, gene_list), "description": (None, self.descriptions)}
+        job_id = self.send_genes(payload, ADDLIST_URL)
         user_list_id = job_id["userListId"]
 
         RESULTS_URL = "%s/%s/export" % (self.ENRICHR_URL, self._organism)
         query_string = "?userListId=%s&filename=%s&backgroundType=%s"
         # set max retries num =5
         s = retry(num=5)
         filename = "%s.%s.reports" % (self._gs, self.descriptions)
@@ -251,25 +323,37 @@
             if not response.ok:
                 self._logger.error("Error fetching enrichment results: %s" % self._gs)
             data = json.loads(response.text)
             colnames = [
                 "Rank",
                 "Term",
                 "P-value",
-                "Z-score",
+                "Odds Ratio",  # 'oddsratio'
                 "Combined Score",
                 "Genes",
                 "Adjusted P-value",
                 "Old P-value",
                 "Old adjusted P-value",
             ]
             res = pd.DataFrame(data[self._gs], columns=colnames)
+            # res.drop(columns=["Rank"], inplace=True)
             res["Genes"] = res["Genes"].apply(";".join)
+            colord = [
+                "Term",
+                "P-value",
+                "Adjusted P-value",
+                "Old P-value",
+                "Old adjusted P-value",
+                "Odds Ratio",  # Z-Score
+                "Combined Score",
+                "Genes",
+            ]
+            res = res.loc[:, colord]
 
-        return [job_id["shortId"], res]
+        return (job_id["shortId"], res)
 
     def _is_entrez_id(self, idx: Union[int, str]) -> bool:
         try:
             int(idx)
             return True
         except:
             return False
@@ -317,19 +401,20 @@
                     DEFAULT_CACHE_PATH,
                     "{}.background.genes.txt".format(self.background),
                 ),
             )
         self._logger.info(
             "Using all annotated genes with GO_ID as background: %s" % self.background
         )
-        df.dropna(subset=["entrezgene_id"], inplace=True)
         # input id type: entrez or gene_name
         if self._isezid:
+            df.dropna(subset=["entrezgene_id"], inplace=True)
             bg = df["entrezgene_id"].astype(int)
         else:
+            df.dropna(subset=["external_gene_name"], inplace=True)
             bg = df["external_gene_name"]
 
         return set(bg)
 
     def set_organism(self):
         """Select Enrichr organism from below:
 
@@ -397,40 +482,33 @@
         for term, genes in gmt.items():
             # If value satisfies the condition, then store it in new_dict
             newgenes = [g for g in genes if g in background]
             if len(newgenes) > 0:
                 gmt2[term] = newgenes
         return gmt2
 
-    def enrich(self, gmt: Dict[str, List[str]]):
-        """use local mode
-
-        p = p-value computed using the Fisher exact test (Hypergeometric test)
-
-        Not implemented here:
-
-            combine score = log(p)·z
-
-        see here: http://amp.pharm.mssm.edu/Enrichr/help#background&q=4
-
-        columns contain:
-
-            Term Overlap P-value Adjusted_P-value Genes
-
+    def parse_background(self, gmt: Dict[str, List[str]] = None):
         """
+        set background genes
+        """
+        if hasattr(self, "_bg") and self._bg:
+            return self._bg
+
+        self._bg = set()
         if self.background is None:
             # use all genes in the dict input as background if background is None
-            bg = set()
-            for term, genes in gmt.items():
-                bg = bg.union(set(genes))
-            self._logger.info(
-                "Background is not set! Use all %s genes in %s." % (len(bg), self._gs)
-            )
-            self._bg = bg
-
+            if gmt:
+                bg = set()
+                for term, genes in gmt.items():
+                    bg = bg.union(set(genes))
+                self._logger.info(
+                    "Background is not set! Use all %s genes in %s."
+                    % (len(bg), self._gs)
+                )
+                self._bg = bg
         elif isscalar(self.background):
             if isinstance(self.background, int) or self.background.isdigit():
                 self._bg = int(self.background)
             elif isinstance(self.background, str):
                 # self.background = set(reduce(lambda x,y: x+y, gmt.values(),[]))
                 self._bg = self.get_background()
                 self._logger.info("Background: found %s genes" % (len(self._bg)))
@@ -439,28 +517,47 @@
         else:
             # handle array object: nd.array, list, tuple, set, Series
             try:
                 it = iter(self.background)
                 self._bg = set(self.background)
             except TypeError:
                 self._logger.error("Unsupported background data type")
+
+        return self._bg
+
+    def enrich(self, gmt: Dict[str, List[str]]):
+        """use local mode
+
+        p = p-value computed using the Fisher exact test (Hypergeometric test)
+        z = z-score (Odds Ratio)
+        combine score = - log(p)·z
+
+        see here: http://amp.pharm.mssm.edu/Enrichr/help#background&q=4
+
+        columns contain:
+
+            Term Overlap P-value Odds Ratio Combinde Score Adjusted_P-value Genes
+
+        """
+        bg = self.parse_background(gmt)
         # statistical testing
-        hgtest = list(calc_pvalues(query=self._gls, gene_sets=gmt, background=self._bg))
+        hgtest = list(calc_pvalues(query=self._gls, gene_sets=gmt, background=bg))
         if len(hgtest) > 0:
             terms, pvals, oddr, olsz, gsetsz, genes = hgtest
             fdrs, rej = multiple_testing_correction(
                 ps=pvals, alpha=self.cutoff, method="benjamini-hochberg"
             )
             # save to a dataframe
             odict = OrderedDict()
             odict["Term"] = terms
             odict["Overlap"] = list(map(lambda h, g: "%s/%s" % (h, g), olsz, gsetsz))
             odict["P-value"] = pvals
             odict["Adjusted P-value"] = fdrs
             odict["Odds Ratio"] = oddr
+            odict["Combined Score"] = -1 * log(pvals) * oddr
             # odict['Reject (FDR< %s)'%self.cutoff ] = rej
             odict["Genes"] = [";".join(g) for g in genes]
             res = pd.DataFrame(odict)
             return res
         return
 
     def run(self):
@@ -497,19 +594,27 @@
                     self._logger.info(
                         "No hits return, for gene set: Custom%s" % shortID
                     )
                     continue
             else:
                 ## online mode
                 self._gs = name
-                self._logger.debug("Enrichr service using library: %s" % (self._gs))
+                self._logger.debug("Enrichr service using library: %s" % (name))
                 # self._logger.info("Enrichr Library: %s"% self._gs)
-                shortID, res = self.get_results(genes_list)
-                # Remember gene set library used
-            res.insert(0, "Gene_set", self._gs)
+                bg = self.parse_background()
+                # whether user input background
+                if isinstance(bg, set) and len(bg) > 0:
+                    shortID, res = self.get_results_with_background(
+                        genes_list, self._bg
+                    )
+                else:
+                    shortID, res = self.get_results(genes_list)
+
+            # Remember gene set library used
+            res.insert(0, "Gene_set", name)
             # Append to master dataframe
             self.results.append(res)
             self.res2d = res
             if self._outdir is None:
                 continue
             outfile = "%s/%s.%s.%s.reports.txt" % (
                 self.outdir,
```

### Comparing `gseapy-1.0.4/gseapy/gsea.py` & `gseapy-1.0.5/gseapy/gsea.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/gseapy/parser.py` & `gseapy-1.0.5/gseapy/parser.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/gseapy/plot.py` & `gseapy-1.0.5/gseapy/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import operator
 import sys
 import warnings
-from typing import Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import matplotlib.pyplot as plt
 import matplotlib.transforms as transforms
 import numpy as np
 import pandas as pd
 import scipy.cluster.hierarchy as sch
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
@@ -206,43 +206,64 @@
     # canvas.print_figure(ofname, bbox_inches='tight', dpi=300)
     ht.fig.savefig(ofname, bbox_inches="tight", dpi=300)
 
 
 class GSEAPlot(object):
     def __init__(
         self,
-        rank_metric: Iterable[float],
         term: str,
-        hits: Iterable[int],
+        tag: Sequence[int],
+        runes: Sequence[float],
         nes: float,
         pval: float,
         fdr: float,
-        RES: Iterable[float],
+        rank_metric: Optional[Sequence[float]] = None,
         pheno_pos: str = "",
         pheno_neg: str = "",
+        color: Optional[str] = None,
         figsize: Tuple[float, float] = (6, 5.5),
         cmap: str = "seismic",
         ofname: Optional[str] = None,
+        ax: Optional[plt.Axes] = None,
         **kwargs,
     ):
+        """
+        :param term: gene_set name
+        :param tag: hit indices of rank_metric.index presented in gene set S.
+        :param runes: running enrichment scores.
+        :param nes: Normalized enrichment scores.
+        :param pval: nominal p-value.
+        :param fdr: false discovery rate.
+        :param rank_metric: pd.Series for rankings, rank_metric.values.
+        :param pheno_pos: phenotype label, positive correlated.
+        :param pheno_neg: phenotype label, negative correlated.
+        :param figsize: matplotlib figsize.
+        :param ofname: output file name. If None, don't save figure
+        """
         # dataFrame of ranked matrix scores
-        self._x = np.arange(len(rank_metric))
-        self.rankings = np.asarray(rank_metric)
-        self.RES = np.asarray(RES)
+        self.color = "#88C544" if color is None else color
+        self._x = np.arange(len(runes))
+        self.rankings = None
+        self._zero_score_ind = None
+        self._z_score_label = None
+        if rank_metric is not None:
+            self.rankings = np.asarray(rank_metric)
+            self._zero_score_ind = np.abs(self.rankings).argmin()
+            self._z_score_label = "Zero score at " + str(self._zero_score_ind)
+
+        self.RES = np.asarray(runes)
 
         self.figsize = figsize
         self.term = term
         self.cmap = cmap
         self.ofname = ofname
 
         self._pos_label = pheno_pos
         self._neg_label = pheno_neg
-        self._zero_score_ind = np.abs(self.rankings).argmin()
-        self._z_score_label = "Zero score at " + str(self._zero_score_ind)
-        self._hit_indices = hits
+        self._hit_indices = tag
         self.module = "tmp" if ofname is None else ofname.split(".")[-2]
         if self.module == "ssgsea":
             self._nes_label = "ES: " + "{:.3f}".format(float(nes))
             self._pval_label = "Pval: invliad for ssgsea"
             self._fdr_label = "FDR: invalid for ssgsea"
         else:
             self._nes_label = "NES: " + "{:.3f}".format(float(nes))
@@ -251,38 +272,41 @@
 
         # output truetype
         plt.rcParams.update({"pdf.fonttype": 42, "ps.fonttype": 42})
         # in most case, we will have many plots, so do not display plots
         # It's also usefull to run this script on command line.
 
         # GSEA Plots
-        if hasattr(sys, "ps1") and (self.ofname is None):
-            # working inside python console, show figure
-            self.fig = plt.figure(figsize=self.figsize)
+        if ax is None:
+            if hasattr(sys, "ps1") and (self.ofname is None):
+                # working inside python console, show figure
+                self.fig = plt.figure(figsize=self.figsize, facecolor="white")
+            else:
+                # If working on command line, don't show figure
+                self.fig = Figure(figsize=self.figsize, facecolor="white")
+                self._canvas = FigureCanvas(self.fig)
         else:
-            # If working on command line, don't show figure
-            self.fig = Figure(figsize=self.figsize)
-            self._canvas = FigureCanvas(self.fig)
+            self.fig = ax.figure
 
         self.fig.suptitle(self.term, fontsize=16, wrap=True, fontweight="bold")
 
     def axes_rank(self, rect):
         """
         rect : sequence of float
                The dimensions [left, bottom, width, height] of the new axes. All
                quantities are in fractions of figure width and height.
         """
         # Ranked Metric Scores Plot
-        ax1 = self.fig.add_axes(rect, sharex=self.ax)
+        ax1 = self.fig.add_axes(rect)
         if self.module == "ssgsea":
             ax1.fill_between(self._x, y1=np.log(self.rankings), y2=0, color="#C9D3DB")
             ax1.set_ylabel("log ranked metric", fontsize=16, fontweight="bold")
         else:
             ax1.fill_between(self._x, y1=self.rankings, y2=0, color="#C9D3DB")
-            ax1.set_ylabel("Ranked list metric", fontsize=16, fontweight="bold")
+            ax1.set_ylabel("Ranked metric", fontsize=16, fontweight="bold")
 
         ax1.text(
             0.05,
             0.9,
             self._pos_label,
             color="red",
             horizontalalignment="left",
@@ -322,61 +346,68 @@
             0.5,
             self._z_score_label,
             horizontalalignment=ha,
             verticalalignment="center",
             transform=ax1.transAxes,
             fontsize=14,
         )
-        ax1.set_xlabel("Rank in Ordered Dataset", fontsize=16, fontweight="bold")
+        ax1.set_xlabel("Gene Rank", fontsize=16, fontweight="bold")
         ax1.spines["top"].set_visible(False)
         ax1.tick_params(
             axis="both", which="both", top=False, right=False, left=False, labelsize=14
         )
         ax1.locator_params(axis="y", nbins=5)
         ax1.yaxis.set_major_formatter(
             plt.FuncFormatter(lambda tick_loc, tick_num: "{:.1f}".format(tick_loc))
         )
 
-    def axes_hits(self, rect):
+    def axes_hits(self, rect, bottom: bool = False):
         """
         rect : sequence of float
                The dimensions [left, bottom, width, height] of the new axes. All
                quantities are in fractions of figure width and height.
         """
         # gene hits
-        ax2 = self.fig.add_axes(rect, sharex=self.ax)
+        ax2 = self.fig.add_axes(rect)
         # the x coords of this transformation are data, and the y coord are axes
         trans2 = transforms.blended_transform_factory(ax2.transData, ax2.transAxes)
-        ax2.vlines(self._hit_indices, 0, 1, linewidth=0.5, transform=trans2)
-        ax2.spines["bottom"].set_visible(False)
+        ax2.vlines(
+            self._hit_indices, 0, 1, linewidth=0.5, transform=trans2, color=self.color
+        )
         ax2.tick_params(
             axis="both",
             which="both",
-            bottom=False,
+            bottom=bottom,
             top=False,
             right=False,
             left=False,
-            labelbottom=False,
+            labelbottom=bottom,
             labelleft=False,
         )
+        if bottom:
+            ax2.set_xlabel("Gene Rank", fontsize=16, fontweight="bold")
+            ax2.spines["bottom"].set_visible(True)
 
     def axes_cmap(self, rect):
         """
         rect : sequence of float
                The dimensions [left, bottom, width, height] of the new axes. All
                quantities are in fractions of figure width and height.
         """
         # center color map at midpoint = 0
-        vmin = np.percentile(self.rankings.min(), 2)
-        vmax = np.percentile(self.rankings.max(), 98)
+        mat = self.rankings
+        if self.rankings is None:
+            mat = self.RES
+        vmin = np.percentile(mat.min(), 2)
+        vmax = np.percentile(mat.max(), 98)
         midnorm = MidpointNormalize(vmin=vmin, vcenter=0, vmax=vmax)
         # colormap
-        ax3 = self.fig.add_axes(rect, sharex=self.ax)
+        ax3 = self.fig.add_axes(rect)
         ax3.pcolormesh(
-            self.rankings[np.newaxis, :],
+            mat[np.newaxis, :],
             rasterized=True,
             norm=midnorm,
             cmap=self.cmap,
         )  # cm.coolwarm
         ax3.spines["bottom"].set_visible(False)
         ax3.tick_params(
             axis="both",
@@ -394,15 +425,15 @@
         rect : sequence of float
                The dimensions [left, bottom, width, height] of the new axes. All
                quantities are in fractions of figure width and height.
         """
         # Enrichment score plot
 
         ax4 = self.fig.add_axes(rect)
-        ax4.plot(self._x, self.RES, linewidth=4, color="#88C544")
+        ax4.plot(self._x, self.RES, linewidth=4, color=self.color)
         ax4.text(0.1, 0.1, self._fdr_label, transform=ax4.transAxes, fontsize=14)
         ax4.text(0.1, 0.2, self._pval_label, transform=ax4.transAxes, fontsize=14)
         ax4.text(0.1, 0.3, self._nes_label, transform=ax4.transAxes, fontsize=14)
 
         # the y coords of this transformation are data, and the x coord are axes
         trans4 = transforms.blended_transform_factory(ax4.transAxes, ax4.transData)
         ax4.hlines(0, 0, 1, linewidth=1, transform=trans4, color="grey")
@@ -434,18 +465,50 @@
         just used:
 
             self.axes_stat([0.1,0.2,0.8,0.8]) # axes_stat should be called first
             self.axes_cmap([0.1,0.1,0.8,0.1])
             self.axes_hits([0.1,0.1,0.8,0.1])
 
         """
-        self.axes_stat([0.1, 0.5, 0.8, 0.4])
-        self.axes_hits([0.1, 0.45, 0.8, 0.05])
-        self.axes_cmap([0.1, 0.40, 0.8, 0.05])
-        self.axes_rank([0.1, 0.1, 0.8, 0.3])
+
+        left = 0.1
+        width = 0.8
+        bottom = 0.1
+        height = 0
+
+        stat_height_ratio = 0.4
+        hits_height_ratio = 0.05
+        cmap_height_ratio = 0.05
+        rank_height_ratio = 0.3
+        ## make stat /hits height ratio const
+        if self.rankings is None:
+            rank_height_ratio = 0
+            cmap_height_ratio = 0
+        base = 0.8 / (
+            stat_height_ratio
+            + hits_height_ratio
+            + cmap_height_ratio
+            + rank_height_ratio
+        )
+        # for i, hit in enumerate(self.hits):
+        #     height = hits_height_ratio * base
+        if self.rankings is not None:
+            height = rank_height_ratio * base
+            self.axes_rank([left, bottom, width, height])
+            bottom += height
+            height = cmap_height_ratio * base
+            self.axes_cmap([left, bottom, width, height])
+            bottom += height
+        height = hits_height_ratio * base
+        self.axes_hits(
+            [left, bottom, width, height], bottom=False if bottom > 0.1 else True
+        )
+        bottom += height
+        height = stat_height_ratio * base
+        self.axes_stat([left, bottom, width, height])
         # self.fig.subplots_adjust(hspace=0)
         # self.fig.tight_layout()
 
     def savefig(self, bbox_inches="tight", dpi=300):
         # if self.ofname is not None:
         if hasattr(sys, "ps1") and (self.ofname is not None):
             self.fig.savefig(self.ofname, bbox_inches=bbox_inches, dpi=dpi)
@@ -453,58 +516,64 @@
             return
         else:
             self._canvas.print_figure(self.ofname, bbox_inches=bbox_inches, dpi=300)
         return
 
 
 def gseaplot(
-    rank_metric: Iterable[float],
     term: str,
-    hits: Iterable[int],
+    hits: Sequence[int],
     nes: float,
     pval: float,
     fdr: float,
-    RES: Iterable[float],
+    RES: Sequence[float],
+    rank_metric: Optional[Sequence[float]] = None,
     pheno_pos: str = "",
     pheno_neg: str = "",
+    color: str = "#88C544",
     figsize: Tuple[float, float] = (6, 5.5),
     cmap: str = "seismic",
     ofname: Optional[str] = None,
     **kwargs,
-):
-    """This is the main function for reproducing the gsea plot.
+) -> Optional[List[plt.Axes]]:
+    """This is the main function for generating the gsea plot.
 
-    :param rank_metric: pd.Series for rankings, rank_metric.values.
     :param term: gene_set name
     :param hits: hits indices of rank_metric.index presented in gene set S.
     :param nes: Normalized enrichment scores.
     :param pval: nominal p-value.
     :param fdr: false discovery rate.
     :param RES: running enrichment scores.
+    :param rank_metric: pd.Series for rankings, rank_metric.values.
     :param pheno_pos: phenotype label, positive correlated.
     :param pheno_neg: phenotype label, negative correlated.
+    :param color: color for RES and hits.
     :param figsize: matplotlib figsize.
     :param ofname: output file name. If None, don't save figure
 
+    return matplotlib.Figure.
     """
     g = GSEAPlot(
-        rank_metric,
         term,
         hits,
+        RES,
         nes,
         pval,
         fdr,
-        RES,
+        rank_metric,
         pheno_pos,
         pheno_neg,
+        color,
         figsize,
         cmap,
         ofname,
     )
     g.add_axes()
+    if ofname is None:
+        return g.fig.axes
     g.savefig()
 
 
 class DotPlot(object):
     def __init__(
         self,
         df: pd.DataFrame,
@@ -613,19 +682,22 @@
                 df.groupby(self.x)
                 .apply(lambda _x: _x.sort_values(by=self.colname).tail(self.n_terms))
                 .reset_index(drop=True)
             )
         else:
             df = df.sort_values(by=self.colname).tail(self.n_terms)  # acending
         # get scatter area
-        ol = df.columns[df.columns.isin(["Overlap", "Tag %"])]
-        temp = (
-            df[ol].squeeze(axis=1).str.split("/", expand=True).astype(int)
-        )  # axis=1, in case you have only 1 row
-        df = df.assign(Hits_ratio=temp.iloc[:, 0] / temp.iloc[:, 1])
+        if df.columns.isin(["Overlap", "Tag %"]).any():
+            ol = df.columns[df.columns.isin(["Overlap", "Tag %"])]
+            temp = (
+                df[ol].squeeze(axis=1).str.split("/", expand=True).astype(int)
+            )  # axis=1, in case you have only 1 row
+            df = df.assign(Hits_ratio=temp.iloc[:, 0] / temp.iloc[:, 1])
+        else:
+            df = df.assign(Hits_ratio=1.0)  # if Overlap column missing
         return df
 
     def _hierarchical_clustering(self, mat, method, metric) -> List[int]:
         # mat.shape -> [n_sample, m_features]
         Y0 = sch.linkage(mat, method=method, metric=metric)
         Z0 = sch.dendrogram(
             Y0,
@@ -640,15 +712,15 @@
     def get_x_order(
         self, method: str = "single", metric: str = "euclidean"
     ) -> List[str]:
         """See scipy.cluster.hierarchy.linkage()
         Perform hierarchical/agglomerative clustering.
         Return categorical order.
         """
-        if isinstance(self.x_order, Iterable):
+        if hasattr(self.x_order, "__len__"):
             return self.x_order
         mat = self.data.pivot(
             index=self.y,
             columns=self.x,
             values=self.colname,  # [self.colname, "Hits_ratio"],
         ).fillna(0)
         idx = self._hierarchical_clustering(mat.T, method, metric)
@@ -657,15 +729,15 @@
     def get_y_order(
         self, method: str = "single", metric: str = "euclidean"
     ) -> List[str]:
         """See scipy.cluster.hierarchy.linkage()
         Perform hierarchical/agglomerative clustering.
         Return categorical order.
         """
-        if isinstance(self.y_order, Iterable):
+        if hasattr(self.y_order, "__len__"):
             return self.y_order
         mat = self.data.pivot(
             index=self.y,
             columns=self.x,
             values=self.colname,  # [self.colname, "Hits_ratio"],
         ).fillna(0)
         idx = self._hierarchical_clustering(mat, method, metric)
@@ -863,15 +935,15 @@
             xlabel = self.hue
         bar.set_xlabel(xlabel, fontsize=16, fontweight="bold")
         bar.set_ylabel("")
         bar.set_title(self.title, fontsize=24, fontweight="bold")
         bar.xaxis.set_major_locator(MaxNLocator(nbins=5, integer=True))
 
         # get default color cycle
-        if (not isinstance(color, str)) and isinstance(color, Iterable):
+        if (not isinstance(color, str)) and hasattr(color, "__len__"):
             _colors = list(color)
         else:
             prop_cycle = plt.rcParams["axes.prop_cycle"]
             _colors = prop_cycle.by_key()["color"]
         colors = _colors
         # remove old legend first
         bar.legend_.remove()
@@ -1157,67 +1229,273 @@
     ax = dot.barh(color=color, group=group)
 
     if ofname is None:
         return ax
     dot.fig.savefig(ofname, bbox_inches="tight", dpi=300)
 
 
-def traceplot(
-    obj,
-    terms: Optional[Union[str, List[str]]] = None,
-    pheno_pos: str = "",
-    pheno_neg: str = "",
+class TracePlot(object):
+    def __init__(
+        self,
+        terms: List[str],
+        tags: List[Sequence[int]],
+        runes: List[Sequence[float]],
+        rank_metric: Optional[Sequence[float]] = None,
+        figsize: Tuple[float, float] = (6, 5.5),
+        colors: Union[str, List[str], None] = None,
+        legend_kws: Optional[Dict[str, Any]] = None,
+        ofname: Optional[str] = None,
+        ax: Optional[plt.Axes] = None,
+        **kwargs,
+    ):
+        """
+        terms: list of terms/pathways to show
+        tags: list of hit indices for each term
+        runes: list runing enrichment score for each term
+        hits: list of ranks of the overlap genes in pathway/term.
+        rank_metric: ranking metric in descending order.
+        colors: list of colors for each term/pathway
+        legend_kws: kwargs to pass to ax.legend. e.g. `loc`, `bbox_to_achor`.
+        ofname: savefig
+        ax: matplotlib's Axes.
+        """
+        # dataFrame of ranked matrix scores
+        self.rankings = rank_metric
+        self.terms = terms
+        self.runes = runes
+        self.hits = tags
+        self.figsize = figsize
+        if isinstance(colors, str):
+            colors = [colors]
+        self.colors = colors
+        self.ofname = ofname
+        self.legend_kws = legend_kws
+
+        # self._pos_label = pheno_pos
+        # self._neg_label = pheno_neg
+        # output truetype
+        plt.rcParams.update({"pdf.fonttype": 42, "ps.fonttype": 42})
+        # in most case, we will have many plots, so do not display plots
+        # It's also usefull to run this script on command line.
+        if ax is None:
+            # GSEA Plots
+            if hasattr(sys, "ps1") and (self.ofname is None):
+                # working inside python console, show figure
+                self.fig = plt.figure(figsize=self.figsize, facecolor="white")
+            else:
+                # If working on command line, don't show figure
+                self.fig = Figure(figsize=self.figsize, facecolor="white")
+                self._canvas = FigureCanvas(self.fig)
+        else:
+            self.fig = ax.figure
+        # self.fig.suptitle(self.term, fontsize=16, wrap=True, fontweight="bold")
+
+    def axes_hits(
+        self, tags: Sequence[int], rect: List[float], color="#0033FF", bottom=False
+    ):
+        """
+        hits: 1d array of this
+        rect : sequence of float
+               The dimensions [left, bottom, width, height] of the new axes. All
+               quantities are in fractions of figure width and height.
+        """
+        # gene hits
+        ax2 = self.fig.add_axes(rect)
+        # the x coords of this transformation are data, and the y coord are axes
+        trans2 = transforms.blended_transform_factory(ax2.transData, ax2.transAxes)
+        ax2.vlines(tags, 0, 1, linewidth=0.5, transform=trans2, color=color)
+        ax2.spines["bottom"].set_visible(True)
+        ax2.tick_params(
+            axis="both",
+            which="both",
+            bottom=bottom,
+            top=False,
+            right=False,
+            left=False,
+            labelbottom=bottom,
+            labelleft=False,
+            labelsize=14,
+        )
+        if bottom:
+            ax2.set_xlabel("Gene Rank", fontsize=16, fontweight="bold")
+
+    def axes_stat(self, rect: List[float]):
+        """
+        rect : sequence of float
+               The dimensions [left, bottom, width, height] of the new axes. All
+               quantities are in fractions of figure width and height.
+        """
+        # Enrichment score plot
+
+        ax4 = self.fig.add_axes(rect)
+        if self.rankings is not None:
+            ax44 = ax4.twinx()  # instantiate a second axes that shares the same x-axis
+            ax44.fill_between(
+                range(len(self.rankings)),
+                y1=self.rankings,
+                y2=0,
+                color="#C9D3DB",
+                zorder=1,
+                alpha=0.5,
+            )
+            ax44.tick_params(axis="y", labelcolor="#808080")
+            ax44.set_ylabel(
+                "Ranked metric", fontsize=16, fontweight="bold", color="#808080"
+            )
+        if self.colors is None:
+            cycle = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+        else:
+            cycle = self.colors
+        for i, r, term in zip(range(len(self.terms)), self.runes, self.terms):
+            ax4.plot(
+                range(len(r)),
+                r,
+                linewidth=2,
+                label=term,
+                color=cycle[i % len(cycle)],
+                zorder=2 + i,
+            )  # color=color)
+
+        # the y coords of this transformation are data, and the x coord are axes
+        trans4 = transforms.blended_transform_factory(ax4.transAxes, ax4.transData)
+        ax4.hlines(0, 0, 1, linewidth=1, transform=trans4, color="grey")
+        ax4.set_ylabel("Enrichment Score", fontsize=16, fontweight="bold")
+        # ax4.set_xlim(min(self._x), max(self._x))
+        ax4.tick_params(
+            axis="both",
+            which="both",
+            bottom=False,
+            top=False,
+            right=False,
+            labelbottom=False,
+            labelsize=14,
+        )
+        ax4.locator_params(axis="y", nbins=5)
+        # FuncFormatter need two argument, I don't know why. this lambda function used to format yaxis tick labels.
+        ax4.yaxis.set_major_formatter(
+            plt.FuncFormatter(lambda tick_loc, tick_num: "{:.1f}".format(tick_loc))
+        )
+        if isinstance(self.legend_kws, dict):
+            ax4.legend(**self.legend_kws)
+        else:
+            ax4.legend(loc=(0, 1.02))
+
+        if self.rankings is not None:
+            self.align_yaxis(ax4, ax44)
+
+    def add_axes(self):
+        """
+        Please check matplotlib docs about how to `add_axes` to figure.
+        """
+        left = 0.1
+        width = 0.8
+        bottom = 0.1
+        # height = 0
+
+        stat_height_ratio = 4
+        hits_height_ratio = 0.5
+        ## make stat /hits height ratio const
+        # 0.8 = base*(4 + len(terms)*0.05)
+        base = 0.8 / (stat_height_ratio + len(self.terms) * hits_height_ratio)
+        # add each hit track
+        if self.colors is None:
+            cycle = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+        else:
+            cycle = self.colors
+
+        for i, hit in enumerate(self.hits):
+            height = hits_height_ratio * base
+            self.axes_hits(
+                tags=hit,
+                rect=[left, bottom, width, height],
+                color=cycle[i % len(cycle)],
+                bottom=False if bottom > 0.1 else True,
+            )
+            bottom += height
+        height = stat_height_ratio * base
+        # add mountain curve
+        self.axes_stat([left, bottom, width, height])
+        # self.fig.subplots_adjust(hspace=0)
+        # self.fig.tight_layout()
+
+    def savefig(self, ofname: str, bbox_inches: str = "tight", dpi: float = 300):
+        # if self.ofname is not None:
+        if hasattr(sys, "ps1") and (ofname is not None):
+            self.fig.savefig(self.ofname, bbox_inches=bbox_inches, dpi=dpi)
+        elif self.ofname is None:
+            return
+        else:
+            self._canvas.print_figure(ofname, bbox_inches=bbox_inches, dpi=300)
+        return
+
+    def align_yaxis(self, ax1, ax2):
+        """Align zeros of the two axes, zooming them out by same ratio"""
+        axes = np.array([ax1, ax2])
+        extrema = np.array([ax.get_ylim() for ax in axes])
+        tops = extrema[:, 1] / (extrema[:, 1] - extrema[:, 0])
+        # Ensure that plots (intervals) are ordered bottom to top:
+        if tops[0] > tops[1]:
+            axes, extrema, tops = [a[::-1] for a in (axes, extrema, tops)]
+
+        # How much would the plot overflow if we kept current zoom levels?
+        tot_span = tops[1] + 1 - tops[0]
+
+        extrema[0, 1] = extrema[0, 0] + tot_span * (extrema[0, 1] - extrema[0, 0])
+        extrema[1, 0] = extrema[1, 1] + tot_span * (extrema[1, 0] - extrema[1, 1])
+        [axes[i].set_ylim(*extrema[i]) for i in range(2)]
+
+
+def gseaplot2(
+    terms: List[str],
+    hits: List[Sequence[int]],
+    RESs: List[Sequence[float]],
+    rank_metric: Optional[Sequence[float]] = None,
+    colors: Optional[Union[str, List[str]]] = None,
     figsize: Tuple[float, float] = (6, 4),
-    cmap: str = "seismic",
+    legend_kws: Optional[Dict[str, Any]] = None,
     ofname: Optional[str] = None,
     **kwargs,
-):
-    """Trace plot for terms
-
-    :param obj: GSEA or Prerank Object.
-    :param terms: terms to show in trace plot
+) -> Optional[List[plt.Axes]]:
+    """Trace plot for combining multiple terms/pathways into one plot
+    :param terms: list of terms to show in trace plot
+    :param hits: list of hits indices correspond to each term.
+    :param RESs: list of running enrichment scores correspond to each term.
+    :param rank_metric: Optional, rankings.
+    :param figsize: matplotlib figsize.
+    :legend_kws: Optional, contol the location of lengends
+    :param ofname: output file name. If None, don't save figure
 
+    return matplotlib.Figure.
     """
-    # create bar plot
-    if hasattr(sys, "ps1") and (ofname is None):
-        # working inside python console, show (True) figure
-        fig = plt.figure(figsize=figsize)
-    else:
-        # If working on commandline, don't show figure
-        fig = Figure(figsize=figsize)
-        canvas = FigureCanvas(fig)
-    ax = fig.add_subplot(111)
-
+    # in case you just input one pathway
     if isinstance(terms, str):
-        _terms = [terms]
-    elif isinstance(terms, list):
-        _terms = terms
-    else:
-        _terms = list(obj.keys())
-
-    for t in _terms:
-        if obj.res2d["Name"].nunique() > 1:
-            for name, results in obj.results.items():
-                if t in results:
-                    RES = results[t]["RES"]
-                    ax.plot(range(len(RES)), RES, label=name)
-        else:
-            results = obj.results
-            if t in results:
-                RES = results[t]["RES"]
-                ax.plot(range(len(RES)), RES)
-    ax.axhline(0, linewidth=1, linestyle="dashed", color="gray")
-    ax.legend()
-    ax.set_xlabel("Gene list ranking", fontsize=14, fontweight="bold")
-    ax.set_ylabel("Enrichment Score", fontsize=14, fontweight="bold")
-    if ofname is not None:
-        # canvas.print_figure(ofname, bbox_inches='tight', dpi=300)
-        fig.savefig(ofname, bbox_inches="tight", dpi=300)
-        return
-    return ax
+        terms = [terms]
+    # make the inputs are legal
+    assert (
+        hasattr(terms, "__len__")
+        and hasattr(hits, "__len__")
+        and hasattr(RESs, "__len__")
+    )
+    assert len(terms) == len(hits) == len(RESs)
+
+    trace = TracePlot(
+        terms=list(terms),
+        runes=list(RESs),
+        tags=list(hits),
+        rank_metric=rank_metric,
+        colors=colors,
+        figsize=figsize,
+        ofname=ofname,
+        legend_kws=legend_kws,
+        **kwargs,
+    )
+    trace.add_axes()
+    if ofname is None:
+        return trace.fig.axes
+    trace.savefig(ofname)
 
 
 def enrichment_map(
     df: pd.DataFrame,
     column: str = "Adjusted P-value",
     cutoff: float = 0.05,
     top_term: int = 10,
```

### Comparing `gseapy-1.0.4/gseapy/scipalette.py` & `gseapy-1.0.5/gseapy/scipalette.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,19 @@
         choose category from (c10, c20a, c20b, c20c)
         """
         if category in self._db[self.d3js.__name__]:
             return self._db[self.d3js.__name__][category]
 
     def igv(self):
         # Color palette inspired by IGV
-        self._db[self.igv.__name__]
+        return self._db[self.igv.__name__]
 
     def igv_alternating(self):
         # Color palette inspired by IGV
-        self._db[self.igv_alternating.__name__]
+        return self._db[self.igv_alternating.__name__]
 
     def locuszoom(self):
         # Color palette inspired by LocusZoom
         return self._db[self.locuszoom.__name__]
 
     def uchicago(self, category="default"):
         """
```

### Comparing `gseapy-1.0.4/gseapy/stats.py` & `gseapy-1.0.5/gseapy/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,25 @@
         k: the random variate represents the number of Type I objects in N drawn
            without replacement from the total population.
 
     Therefore, these two functions are the same when using parameters from 2*2 table:
     R:     >   phyper(x-1, m, n, k, lower.tail=FALSE)
     Scipy: >>> hypergeom.sf(x-1, m+n, m, k)
 
+    For Odds ratio in Enrichr (see https://maayanlab.cloud/Enrichr/help#background&q=4)
+
+        oddsRatio = (1.0 * x * d) / Math.max(1.0 * b * c, 1)
+
+    where:
+
+        x are the overlapping genes,
+        b (m-x) are the genes in the annotated set - overlapping genes,
+        c (k-x) are the genes in the input set - overlapping genes,
+        d (bg-m-k+x) are the 20,000 genes (or total genes in the background) - genes in the annotated set - genes in the input set + overlapping genes
+
     """
 
     query = set(query)
     vals = []
     # background should be all genes in annotated database
     # such as go, kegg et.al.
     if isinstance(background, set):
```

### Comparing `gseapy-1.0.4/gseapy/utils.py` & `gseapy-1.0.5/gseapy/utils.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/gseapy.egg-info/PKG-INFO` & `gseapy-1.0.5/gseapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gseapy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Gene Set Enrichment Analysis in Python
 Home-page: https://github.com/zqfang/gseapy
 Download-URL: https://github.com/zqfang/gseapy
 Author: Zhuoqing Fang
 Author-email: fzq518@gmail.com
 License: MIT
 Project-URL: Documentation, https://gseapy.readthedocs.io/en/latest/
```

### Comparing `gseapy-1.0.4/gseapy.egg-info/SOURCES.txt` & `gseapy-1.0.5/gseapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/setup.py` & `gseapy-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/src/algorithm.rs` & `gseapy-1.0.5/src/algorithm.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/src/help.rs` & `gseapy-1.0.5/src/help.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/src/lib.rs` & `gseapy-1.0.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `gseapy-1.0.4/src/stats.rs` & `gseapy-1.0.5/src/stats.rs`

 * *Files 4% similar despite different names*

```diff
@@ -778,15 +778,15 @@
             .into_par_iter()
             .map(|rank| {
                 let mut tmp = rank.as_slice().argsort(false);
                 if self.weight > 0.0 {
                     // https://github.com/broadinstitute/ssGSEA2.0/blob/f682082f62ae34185421545f25041bae2c78c89b/src/ssGSEA2.0.R#L396
                     match correl_type {
                         CorrelType::SymRank => {
-                            let idx = (tmp.1.len() + 2 -1) / 2;
+                            let idx = (tmp.1.len() + 2 - 1) / 2;
                             let mid = tmp.1.get(idx).unwrap().to_owned();
                             tmp.1.iter_mut().for_each(|x| {
                                 if *x > mid {
                                     *x
                                 } else {
                                     (*x) + (*x) - mid
                                 };
@@ -878,23 +878,27 @@
     use super::*;
     use std::time::Instant;
     // use fastrand;
     use crate::stats::GSEAResult;
     use crate::utils::FileReader;
     #[test]
     fn test_prerank() {
+        let cwd = std::env::current_dir().unwrap(); // prjoject root, directory to Cargo.toml
+        let rnk_path = cwd.join("tests/data/mds.2k.rnk");
+        let gmt_path = cwd.join("tests/data/hallmark.gmt");
+
         let start = Instant::now();
         rayon::ThreadPoolBuilder::new()
             .num_threads(1)
             .build_global()
             .unwrap();
         let mut rnk = FileReader::new();
-        let _ = rnk.read_csv("data/mds.2k.rnk", b'\t', false, Some(b'#'));
+        let _ = rnk.read_csv(rnk_path.to_str().unwrap(), b'\t', false, Some(b'#'));
         let mut gmt = FileReader::new();
-        let _ = gmt.read_table("data/hallmark.gmt", '\t', false);
+        let _ = gmt.read_table(gmt_path.to_str().unwrap(), '\t', false);
 
         // let gene: Vec<String> = vec!["A","B","C","D","E","F","G","H","J","K"].into_iter().map(|s| s.to_string()).collect();
         // let gene_set: Vec<String> = vec!["B","A","D","G"].into_iter().map(|s| s.to_string()).collect();
         // let gene_metric = vec![9.0,4.0,3.0,2.0,1.0,0.5,0.1,-0.1,-0.2,-0.5];
         let weight = 1.0;
         let mut gene: Vec<String> = Vec::new();
         // let mut gene_set: Vec<String> = Vec::new();
@@ -920,36 +924,40 @@
         let mut gsea = GSEAResult::new(weight, 500, 5, 10, 123);
         gsea.prerank(&gene, &metric, &gmt2);
         let end = Instant::now();
         println!("Overall run time: {:.2?}", end.duration_since(start));
         println!("This version 1");
         gsea.summaries.iter().for_each(|g| {
             println!(
-                "name: {:?}, term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
-                g.name, g.term, g.es, g.nes, g.pval, g.fdr
+                "term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
+                g.term, g.es, g.nes, g.pval, g.fdr
             );
         });
     }
     #[test]
     fn test_gsea() {
+        let cwd = std::env::current_dir().unwrap(); // prjoject root, directory to Cargo.toml
+        let gct_path = cwd.join("tests/extdata/Leukemia_hgu95av2.trim2.txt");
+        let gmt_path = cwd.join("tests/extdata/h.all.v7.0.symbols.gmt");
+        let cls_path = cwd.join("tests/extdata/Leukemia.cls");
         let start = Instant::now();
         // set number of threads of rayon at the main()
         // rayon::ThreadPoolBuilder::new()
         //     .num_threads(1)
         //     .build_global()
         //     .unwrap();
 
         let mut gct = FileReader::new();
-        let _ = gct.read_csv("data/P53.txt", b'\t', true, Some(b'#'));
+        let _ = gct.read_csv(gct_path.to_str().unwrap(), b'\t', true, Some(b'#'));
         let mut gmt = FileReader::new();
-        let _ = gmt.read_table("data/genes.gmt", '\t', false);
+        let _ = gmt.read_table(gmt_path.to_str().unwrap(), '\t', false);
         let mut cls = FileReader::new();
-        let _ = cls.read_table("data/P53.cls", ' ', false);
+        let _ = cls.read_table(cls_path.to_str().unwrap(), ' ', false);
         println!("{:?}", &cls.record[2]);
-        let gboo: Vec<bool> = cls.record[2].iter().map(|x| x != "WT").collect();
+        let gboo: Vec<bool> = cls.record[2].iter().map(|x| x != "AML").collect();
         println!("{:?}", &gboo);
         let weight = 1.0;
         let mut gene: Vec<String> = Vec::new();
         // let mut gene_set: Vec<String> = Vec::new();
         let mut gene_exp: Vec<Vec<f64>> = Vec::new();
         for r in gct.record.iter() {
             gene.push(r[0].to_string());
@@ -972,46 +980,31 @@
         println!("Overall run time: {:.2?}", end.duration_since(start));
         gsea.summaries.iter().for_each(|g| {
             println!(
                 "term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.5?}, fdr: {:.5?}",
                 g.term, g.es, g.nes, g.pval, g.fdr
             );
         });
-
-        // GSEASummary._fdr() results
-        // term: "YvX_UpIN_Y", es: -0.2461258, nes: -0.7333695, pval: 0.89189, fdr: 0.99250
-        // term: "DvA_UpIN_A", es: -0.1894728, nes: -0.8517915, pval: 0.80000, fdr: 0.97980
-        // term: "DvA_UpIN_D", es: 0.2168890, nes: 0.8320893, pval: 0.72727, fdr: 0.70918
-        // term: "YvX_UpIN_X", es: -0.6054005, nes: -1.2666132, pval: 0.24528, fdr: 0.73196
-        // term: "BvA_UpIN_A", es: -0.2498697, nes: -1.0470712, pval: 0.37143, fdr: 0.91667
-        // term: "CvA_UpIN_C", es: -0.3799417, nes: -0.6438662, pval: 0.85366, fdr: 0.92807
-        // term: "BvA_UpIN_B", es: 0.2250848, nes: 0.8380035, pval: 0.68657, fdr: 0.89362
-        // term: "CvA_UpIN_A", es: -0.2987804, nes: -0.6507148, pval: 0.91667, fdr: 0.98495
-
-        // GSEASummary.fdr() result
-        // term: "DvA_UpIN_A", es: -0.1894728, nes: -0.8517915, pval: 0.80000, fdr: 1.00000
-        // term: "YvX_UpIN_Y", es: -0.2461258, nes: -0.7333695, pval: 0.89189, fdr: 1.00000
-        // term: "DvA_UpIN_D", es: 0.2168890, nes: 0.8320893, pval: 0.72727, fdr: 0.71000
-        // term: "BvA_UpIN_A", es: -0.2498697, nes: -1.0470712, pval: 0.37143, fdr: 1.00000
-        // term: "YvX_UpIN_X", es: -0.6054005, nes: -1.2666132, pval: 0.24528, fdr: 1.00000
-        // term: "CvA_UpIN_A", es: -0.2987804, nes: -0.6507148, pval: 0.91667, fdr: 1.00000
-        // term: "CvA_UpIN_C", es: -0.3799417, nes: -0.6438662, pval: 0.85366, fdr: 0.93167
-        // term: "BvA_UpIN_B", es: 0.2250848, nes: 0.8380035, pval: 0.68657, fdr: 1.00000
     }
 
     #[test]
     fn test_ssgsea() {
+        let cwd = std::env::current_dir().unwrap(); // prjoject root, directory to Cargo.toml
+        let gct_path = cwd.join("tests/extdata/Leukemia_hgu95av2.trim2.txt");
+        let gmt_path = cwd.join("tests/extdata/h.all.v7.0.symbols.gmt");
+        let cls_path = cwd.join("tests/extdata/Leukemia.cls");
+
         let mut gct = FileReader::new();
-        let _ = gct.read_csv("data/P53.txt", b'\t', true, Some(b'#'));
+        let _ = gct.read_csv(gct_path.to_str().unwrap(), b'\t', true, Some(b'#'));
         let mut gmt = FileReader::new();
-        let _ = gmt.read_table("data/genes.gmt", '\t', false);
+        let _ = gmt.read_table(gmt_path.to_str().unwrap(), '\t', false);
         let mut cls = FileReader::new();
-        let _ = cls.read_table("data/P53.cls", ' ', false);
+        let _ = cls.read_table(cls_path.to_str().unwrap(), ' ', false);
         println!("{:?}", &cls.record[2]);
-        let gboo: Vec<bool> = cls.record[2].iter().map(|x| x != "WT").collect();
+        let gboo: Vec<bool> = cls.record[2].iter().map(|x| x != "AML").collect();
         println!("{:?}", &gboo);
         let weight = 1.0;
         let mut gene: Vec<String> = Vec::new();
         // let mut gene_set: Vec<String> = Vec::new();
         let mut gene_exp: Vec<Vec<f64>> = Vec::new();
         for r in gct.record.iter() {
             gene.push(r[0].to_string());
@@ -1028,40 +1021,40 @@
         gmt.record.iter().for_each(|r| {
             gmt2.insert(r[0].as_str(), &r[2..]);
         });
 
         let nperm = 10;
         let mut gsea = GSEAResult::new(weight, 500, 3, nperm, 123);
         if nperm > 0 {
-            gsea.ss_gsea_permuate(&gene, &sample_names, &gene_exp, &gmt2);
+            gsea.ss_gsea_permuate(&gene, &gene_exp, &gmt2, CorrelType::Rank);
         } else {
-            gsea.ss_gsea(&gene, &sample_names, &gene_exp, &gmt2);
+            gsea.ss_gsea(&gene, &gene_exp, &gmt2, CorrelType::Rank);
         }
 
         gsea.summaries.iter().for_each(|g| {
             println!(
-                "sample: {:?}, term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
-                g.name, g.term, g.es, g.nes, g.pval, g.fdr
+                "term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
+                g.term, g.es, g.nes, g.pval, g.fdr
             );
         });
 
         let _gx: Vec<f64> = gene_exp.iter().map(|g| g[0]).collect();
         let (_gx_idx, _gx2) = _gx.as_slice().argsort(false);
         let _ge: Vec<String> = _gx_idx.into_iter().map(|i| gene[i].to_owned()).collect();
         gsea.prerank(&_ge, &_gx2, &gmt2);
         println!("\n\n\nThis version prerank version 1");
         gsea.summaries.iter().for_each(|g| {
             println!(
-                "name: {:?}, term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
-                g.name, g.term, g.es, g.nes, g.pval, g.fdr
+                "term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
+                g.term, g.es, g.nes, g.pval, g.fdr
             );
         });
         println!("\n\n\nThis version prerank version 2");
         gsea.prerank2(&gene, &gene_exp, &gmt2);
         gsea.summaries.iter().for_each(|g| {
             println!(
-                "name: {:?}, term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
-                g.name, g.term, g.es, g.nes, g.pval, g.fdr
+                "term: {:?}, es: {:.7?}, nes: {:.7?}, pval: {:.2e}, fdr: {:.2e}",
+                g.term, g.es, g.nes, g.pval, g.fdr
             );
         });
     }
 }
```

### Comparing `gseapy-1.0.4/src/utils.rs` & `gseapy-1.0.5/src/utils.rs`

 * *Files 6% similar despite different names*

```diff
@@ -263,19 +263,23 @@
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     #[test]
     fn test_rdr() {
+        let cwd = std::env::current_dir().unwrap(); // prjoject root, directory to Cargo.toml
+        let rnk_path = cwd.join("tests/data/edb/gsea_data.gsea_data.rnk");
+        let gmt_path = cwd.join("tests/data/edb/gene_sets.gmt");
+        println!("{:?}", &rnk_path);
         let mut rnk = FileReader::new();
-        let _ = rnk.read_csv("data/edb/gsea_data.gsea_data.rnk", b'\t', false, Some(b'#'));
+        let _ = rnk.read_csv(rnk_path.to_str().unwrap(), b'\t', false, Some(b'#'));
         let mut gmt = FileReader::new();
-        let _ = gmt.read_csv("data/edb/gene_sets.gmt", b'\t', false, None);
-        let _wr = rnk.to_csv("data/example.output.txt", b'\t', true);
+        let _ = gmt.read_csv(gmt_path.to_str().unwrap(), b'\t', false, None);
+        let _wr = rnk.to_csv("example.output.txt", b'\t', true);
     }
     #[test]
     fn test_dynum() {
         //let dynum = DynamicEnum::new();
         let vec = vec!["A", "B", "C", "D"];
         let mut dynum = DynamicEnum::from(&vec);
         let x = dynum.add_if_new("E");
```

### Comparing `gseapy-1.0.4/tests/test_commands.py` & `gseapy-1.0.5/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,21 @@
     ssgsea(ssGCT, geneGMT, None, permutation_num=0, correl_norm_type="zscore")
 
 
 def test_enrichr(genelist, geneGMT):
     # Only tests of the command runs successfully,
     # doesnt't check the image
     tmpdir = TemporaryDirectory(dir="tests")
-    enrichr(genelist, gene_sets=["KEGG_2016", geneGMT], outdir=None, cutoff=0.5)
+    enrichr(
+        genelist,
+        gene_sets=["KEGG_2016", geneGMT],
+        background="hsapiens_gene_ensembl",
+        outdir=None,
+        cutoff=0.5,
+    )
     tmpdir.cleanup()
     tmpdir = TemporaryDirectory(dir="tests")
     enrich(genelist, gene_sets=geneGMT, background=None, outdir=tmpdir.name, cutoff=0.5)
     tmpdir.cleanup()
 
 
 def test_replot(edbDIR):
```

