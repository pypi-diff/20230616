# Comparing `tmp/Augusta-1.0.3.tar.gz` & `tmp/Augusta-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Augusta-1.0.3.tar", last modified: Sun Sep 11 16:21:50 2022, max compression
+gzip compressed data, was "Augusta-1.0.4.tar", last modified: Fri Jun 16 18:47:48 2023, max compression
```

## Comparing `Augusta-1.0.3.tar` & `Augusta-1.0.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.975619 Augusta-1.0.3/
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.880913 Augusta-1.0.3/Augusta/
--rw-rw-rw-   0        0        0     4688 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/Augusta.py
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.882969 Augusta-1.0.3/Augusta/DBs/
--rw-rw-rw-   0        0        0     3934 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/DBs/CC_search_filter.py
--rw-rw-rw-   0        0        0     4413 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/DBs/DBs_filter.py
--rw-rw-rw-   0        0        0    10087 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/DBs/DBs_search.py
--rw-rw-rw-   0        0        0       15 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/DBs/__init__.py
--rw-rw-rw-   0        0        0     2212 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/DBs/get_synonyms.py
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.882969 Augusta-1.0.3/Augusta/GRN_MI/
--rw-rw-rw-   0        0        0     1966 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/GRN_MI/GRNmi_infer.py
--rw-rw-rw-   0        0        0       15 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/GRN_MI/__init__.py
--rw-rw-rw-   0        0        0     2454 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/GRN_MI/preprocessing.py
--rw-rw-rw-   0        0        0      902 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/RNASeq_normalization.py
--rw-rw-rw-   0        0        0     7299 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/SBML_generation.py
--rw-rw-rw-   0        0        0       82 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.882969 Augusta-1.0.3/Augusta/cno/
--rw-rw-rw-   0        0        0     1308 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/LICENSE
--rw-rw-rw-   0        0        0     2261 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/README.rst
--rw-rw-rw-   0        0        0     1280 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.925816 Augusta-1.0.3/Augusta/cno/io/
--rw-rw-rw-   0        0        0      522 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/__init__.py
--rw-rw-rw-   0        0        0     4014 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/adj2sif.py
--rw-rw-rw-   0        0        0     8070 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/cna.py
--rw-rw-rw-   0        0        0   121261 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/cnograph.py
--rw-rw-rw-   0        0        0     4337 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/eda.py
--rw-rw-rw-   0        0        0     7291 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/mapback.py
--rw-rw-rw-   0        0        0    13821 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/measurements.py
--rw-rw-rw-   0        0        0     5786 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/metabolites.py
--rw-rw-rw-   0        0        0   101619 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/midas.py
--rw-rw-rw-   0        0        0    19232 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/midas_normalisation.py
--rw-rw-rw-   0        0        0     4423 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/multigraph.py
--rw-rw-rw-   0        0        0     5306 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/multimidas.py
--rw-rw-rw-   0        0        0     5481 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/net.py
--rw-rw-rw-   0        0        0     2935 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/obs.py
--rw-rw-rw-   0        0        0     4819 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/randomisation.py
--rw-rw-rw-   0        0        0    19140 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/reactions.py
--rw-rw-rw-   0        0        0     9581 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/sbml.py
--rw-rw-rw-   0        0        0    20880 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/sbmlqual.py
--rw-rw-rw-   0        0        0    15471 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/sif.py
--rw-rw-rw-   0        0        0     2280 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/sif2asp.py
--rw-rw-rw-   0        0        0     8339 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/sop2sif.py
--rw-rw-rw-   0        0        0     1462 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/validation.py
--rw-rw-rw-   0        0        0    15507 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/xcnograph.py
--rw-rw-rw-   0        0        0     2657 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/io/xmlmidas.py
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.928876 Augusta-1.0.3/Augusta/cno/misc/
--rw-rw-rw-   0        0        0       85 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/misc/__init__.py
--rw-rw-rw-   0        0        0     6682 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/misc/classifier.py
--rw-rw-rw-   0        0        0     1836 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/misc/dependencies.py
--rw-rw-rw-   0        0        0     9450 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/misc/matfun.py
--rw-rw-rw-   0        0        0       32 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/misc/profiler.py
--rw-rw-rw-   0        0        0      229 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/misc/tools.py
--rw-rw-rw-   0        0        0     2393 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/cno/misc/truthtable.py
--rw-rw-rw-   0        0        0     4426 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/core.py
--rw-rw-rw-   0        0        0      793 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/data_export.py
--rw-rw-rw-   0        0        0     6344 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/data_import.py
--rw-rw-rw-   0        0        0     5487 2022-09-11 16:21:20.000000 Augusta-1.0.3/Augusta/motif_discovery.py
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.882969 Augusta-1.0.3/Augusta.egg-info/
--rw-rw-rw-   0        0        0     2135 2022-09-11 16:21:50.000000 Augusta-1.0.3/Augusta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1945 2022-09-11 16:21:50.000000 Augusta-1.0.3/Augusta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-11 16:21:50.000000 Augusta-1.0.3/Augusta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2022-09-11 16:21:50.000000 Augusta-1.0.3/Augusta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-11 16:21:50.000000 Augusta-1.0.3/Augusta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1119 2022-09-11 16:21:20.000000 Augusta-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2135 2022-09-11 16:21:50.975619 Augusta-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2022-09-11 16:21:20.000000 Augusta-1.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.962969 Augusta-1.0.3/data/
--rw-rw-rw-   0        0        0   266984 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/Cbeijerinckii.csv
--rw-rw-rw-   0        0        0 13094427 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/Cbeijerinckii.gb
--rw-rw-rw-   0        0        0 11707807 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/Ecoli.gb
--rw-rw-rw-   0        0        0    22219 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/Ecoli_DREAM4.csv
--rw-rw-rw-   0        0        0    24959 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/GRN_example.csv
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.971966 Augusta-1.0.3/data/output/
--rw-rw-rw-   0        0        0  5860646 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/output/Ecoli_BN.sbml
--rw-rw-rw-   0        0        0    24492 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/output/Ecoli_GRN.csv
--rw-rw-rw-   0        0        0    20798 2022-09-11 16:21:20.000000 Augusta-1.0.3/data/output/Ecoli_discovered_motifs.sto
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.975619 Augusta-1.0.3/docs/
--rw-rw-rw-   0        0        0     7348 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/Examples.rst
--rw-rw-rw-   0        0        0     1688 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/Installation.rst
--rw-rw-rw-   0        0        0      654 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/Makefile
--rw-rw-rw-   0        0        0     5033 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/User guide.rst
-drwxrwxrwx   0        0        0        0 2022-09-11 16:21:50.975619 Augusta-1.0.3/docs/_static/
--rw-rw-rw-   0        0        0   306980 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/_static/Augusta_logo.png
--rw-rw-rw-   0        0        0   350471 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/_static/Ecoli_BN.png
--rw-rw-rw-   0        0        0   777470 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/_static/Ecoli_GRN.png
--rw-rw-rw-   0        0        0    40464 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/_static/pipeline.png
--rw-rw-rw-   0        0        0     2478 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/conf.py
--rw-rw-rw-   0        0        0     1102 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/index.rst
--rwxrwxrwx   0        0        0      800 2022-09-11 16:21:20.000000 Augusta-1.0.3/docs/make.bat
--rw-rw-rw-   0        0        0      197 2022-09-11 16:21:20.000000 Augusta-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-09-11 16:21:50.975619 Augusta-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1197 2022-09-11 16:21:20.000000 Augusta-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.276903 Augusta-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.152058 Augusta-1.0.4/Augusta/
+-rw-rw-rw-   0        0        0     3900 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/Augusta.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.183218 Augusta-1.0.4/Augusta/DBs/
+-rw-rw-rw-   0        0        0     3953 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/DBs/CC_search_filter.py
+-rw-rw-rw-   0        0        0     4432 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/DBs/DBs_filter.py
+-rw-rw-rw-   0        0        0    10087 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/DBs/DBs_search.py
+-rw-rw-rw-   0        0        0       15 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/DBs/__init__.py
+-rw-rw-rw-   0        0        0     2287 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/DBs/get_synonyms.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.183218 Augusta-1.0.4/Augusta/GRN_MI/
+-rw-rw-rw-   0        0        0     2069 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/GRN_MI/GRNmi_infer.py
+-rw-rw-rw-   0        0        0       15 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/GRN_MI/__init__.py
+-rw-rw-rw-   0        0        0     2438 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/GRN_MI/preprocessing.py
+-rw-rw-rw-   0        0        0      902 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/RNASeq_normalization.py
+-rw-rw-rw-   0        0        0     8422 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/SBML_generation.py
+-rw-rw-rw-   0        0        0       82 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.183218 Augusta-1.0.4/Augusta/cno/
+-rw-rw-rw-   0        0        0     1308 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/LICENSE
+-rw-rw-rw-   0        0        0     2261 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/README.rst
+-rw-rw-rw-   0        0        0     1280 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.214381 Augusta-1.0.4/Augusta/cno/io/
+-rw-rw-rw-   0        0        0      522 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/__init__.py
+-rw-rw-rw-   0        0        0     4014 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/adj2sif.py
+-rw-rw-rw-   0        0        0     8070 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/cna.py
+-rw-rw-rw-   0        0        0   121261 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/cnograph.py
+-rw-rw-rw-   0        0        0     4337 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/eda.py
+-rw-rw-rw-   0        0        0     7291 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/mapback.py
+-rw-rw-rw-   0        0        0    13821 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/measurements.py
+-rw-rw-rw-   0        0        0     5786 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/metabolites.py
+-rw-rw-rw-   0        0        0   101619 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/midas.py
+-rw-rw-rw-   0        0        0    19232 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/midas_normalisation.py
+-rw-rw-rw-   0        0        0     4423 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/multigraph.py
+-rw-rw-rw-   0        0        0     5306 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/multimidas.py
+-rw-rw-rw-   0        0        0     5481 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/net.py
+-rw-rw-rw-   0        0        0     2935 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/obs.py
+-rw-rw-rw-   0        0        0     4819 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/randomisation.py
+-rw-rw-rw-   0        0        0    19140 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/reactions.py
+-rw-rw-rw-   0        0        0     9581 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/sbml.py
+-rw-rw-rw-   0        0        0    20880 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/sbmlqual.py
+-rw-rw-rw-   0        0        0    15471 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/sif.py
+-rw-rw-rw-   0        0        0     2280 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/sif2asp.py
+-rw-rw-rw-   0        0        0     8339 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/sop2sif.py
+-rw-rw-rw-   0        0        0     1462 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/validation.py
+-rw-rw-rw-   0        0        0    15507 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/xcnograph.py
+-rw-rw-rw-   0        0        0     2657 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/io/xmlmidas.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.230030 Augusta-1.0.4/Augusta/cno/misc/
+-rw-rw-rw-   0        0        0       85 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/misc/__init__.py
+-rw-rw-rw-   0        0        0     6682 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/misc/classifier.py
+-rw-rw-rw-   0        0        0     1836 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/misc/dependencies.py
+-rw-rw-rw-   0        0        0     9450 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/misc/matfun.py
+-rw-rw-rw-   0        0        0       32 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/misc/profiler.py
+-rw-rw-rw-   0        0        0      229 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/misc/tools.py
+-rw-rw-rw-   0        0        0     2393 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/cno/misc/truthtable.py
+-rw-rw-rw-   0        0        0     4343 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/core.py
+-rw-rw-rw-   0        0        0      793 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/data_export.py
+-rw-rw-rw-   0        0        0     6337 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/data_import.py
+-rw-rw-rw-   0        0        0     5950 2023-06-16 18:47:34.000000 Augusta-1.0.4/Augusta/motif_discovery.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.183218 Augusta-1.0.4/Augusta.egg-info/
+-rw-rw-rw-   0        0        0     2190 2023-06-16 18:47:47.000000 Augusta-1.0.4/Augusta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1945 2023-06-16 18:47:48.000000 Augusta-1.0.4/Augusta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:47:47.000000 Augusta-1.0.4/Augusta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-06-16 18:47:47.000000 Augusta-1.0.4/Augusta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 18:47:47.000000 Augusta-1.0.4/Augusta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1119 2023-06-16 18:47:34.000000 Augusta-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2190 2023-06-16 18:47:48.276903 Augusta-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2023-06-16 18:47:34.000000 Augusta-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.261276 Augusta-1.0.4/data/
+-rw-rw-rw-   0        0        0   451983 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/Cbeijerinckii.csv
+-rw-rw-rw-   0        0        0 13094427 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/Cbeijerinckii.gb
+-rw-rw-rw-   0        0        0 11707807 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/Ecoli.gb
+-rw-rw-rw-   0        0        0    22219 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/Ecoli_DREAM4.csv
+-rw-rw-rw-   0        0        0    22984 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/example_GRN.csv
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.261276 Augusta-1.0.4/data/output/
+-rw-rw-rw-   0        0        0   628339 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/output/Ecoli_BN.sbml
+-rw-rw-rw-   0        0        0    22984 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/output/Ecoli_GRN.csv
+-rw-rw-rw-   0        0        0     6489 2023-06-16 18:47:34.000000 Augusta-1.0.4/data/output/Ecoli_discovered_motifs.sto
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.276903 Augusta-1.0.4/docs/
+-rw-rw-rw-   0        0        0     7121 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/Examples.rst
+-rw-rw-rw-   0        0        0     1688 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/Installation.rst
+-rw-rw-rw-   0        0        0      654 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/Makefile
+-rw-rw-rw-   0        0        0     6029 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/User guide.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 18:47:48.276903 Augusta-1.0.4/docs/_static/
+-rw-rw-rw-   0        0        0   306980 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/_static/Augusta_logo.png
+-rw-rw-rw-   0        0        0   350471 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/_static/Ecoli_BN.png
+-rw-rw-rw-   0        0        0   777470 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/_static/Ecoli_GRN.png
+-rw-rw-rw-   0        0        0    40464 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/_static/pipeline.png
+-rw-rw-rw-   0        0        0     2478 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/conf.py
+-rw-rw-rw-   0        0        0     1102 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2023-06-16 18:47:34.000000 Augusta-1.0.4/docs/make.bat
+-rw-rw-rw-   0        0        0      197 2023-06-16 18:47:34.000000 Augusta-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:47:48.276903 Augusta-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-06-16 18:47:34.000000 Augusta-1.0.4/setup.py
```

### Comparing `Augusta-1.0.3/Augusta/Augusta.py` & `Augusta-1.0.4/Augusta/Augusta.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-from .core import *
+from .core import RNASeq_to_GRNmi, GRNmi_to_GRNmotifs, get_DBs_data, get_CC_data
+from .data_import import import_CountTable, genbank_process, import_GRN
+from .RNASeq_normalization import normalize_CountTable
+from .SBML_generation import GRN_to_SBML
+from .data_export import export_GRN
+from os import makedirs, path, getcwd
+from gc import collect
 
-def RNASeq_to_GRN(count_table_input, promoter_length = 1000, genbank_file_input = None, normalization_type = None):
+def RNASeq_to_GRN(count_table_input, promoter_length = 1000, genbank_file_input = None, normalization_type = None, motifs_max_time = 180):
    count_table = import_CountTable(count_table_input)  # data import
    gene_names = count_table.index
-   output_directory = os.path.join(os.getcwd(), r'output')  # data export
-   if not os.path.exists(output_directory):
-      os.makedirs(output_directory)
+   output_directory = path.join(getcwd(), r'output')  # data export
+   if not path.exists(output_directory):
+      makedirs(output_directory)
    if genbank_file_input:
       gene_lengths, gene_promoters, organism, taxon, genes_IDs = genbank_process(genbank_file_input, gene_names, promoter_length)
       if normalization_type:  # count table normalization
          normalized_count_table = normalize_CountTable(count_table, gene_lengths, normalization_type)
       else:
          normalized_count_table = count_table
       GRNmi, count_table_differences = RNASeq_to_GRNmi(normalized_count_table)  # GRN inference using MI
-      GRNmotifs = GRNmi_to_GRNmotifs(GRNmi, gene_promoters, count_table_differences)  # GRN verification using motif search
+      GRNmotifs = GRNmi_to_GRNmotifs(GRNmi, gene_promoters, count_table_differences, motifs_max_time)  # GRN verification using motif search
       GRNdb, genes_IDs_all = get_DBs_data(organism, genes_IDs, taxon, GRNmotifs)  # GRN verification using databases
       if GRNdb is None:
          print('No databases interaction data available; GRN verification skipped.')
          GRNdb = GRNmotifs.copy()
       export_GRN(GRNdb)
-      return GRNdb
+      return GRNdb, genes_IDs_all
    elif genbank_file_input is None:
       if normalization_type:
          print('Count table normalization not available - GenBank missing; skipped.')
       GRNmi, count_table_differences = RNASeq_to_GRNmi(count_table)
       export_GRN(GRNmi)
-      return GRNmi
-
+      genes_IDs_all = None
+      return GRNmi, genes_IDs_all
 
 def GRN_to_BN(GRN_input, promoter_length = 1000, genbank_file_input = None, add_dbs_info = None):
    try:
-      GRN_imported = import_GRN(GRN_input) # GRN input from file
+      GRN_imported = import_GRN(GRN_input).astype(dtype='int8') # GRN input from file
    except TypeError:
       GRN_imported = GRN_input.copy() # GRN input from variable
-
-   output_directory = os.path.join(os.getcwd(), r'output') # data export
-   if not os.path.exists(output_directory):
-      os.makedirs(output_directory)
-
+   output_directory = path.join(getcwd(), r'output') # data export
+   if not path.exists(output_directory):
+      makedirs(output_directory)
    if (add_dbs_info == 'yes' or add_dbs_info == 'Yes' or add_dbs_info == 1):
       if genbank_file_input:
          gene_names = GRN_imported.index
          gene_lengths, gene_promoters, organism, taxon, genes_IDs = genbank_process(genbank_file_input, gene_names, promoter_length)
          GRNdb, genes_IDs_all = get_DBs_data(organism, genes_IDs, taxon, GRN_imported)
          if GRNdb is None:
             print('No databases interaction data available; GRN verification skipped.')
@@ -51,36 +55,16 @@
          GRN_to_SBML(GRNcc, CC_conditions) # GRN to BN
       else:
          print('Databases info add not available - GenBank missing; skipped.')
          GRN_to_SBML(GRN_imported) # GRN to BN
    else:
       GRN_to_SBML(GRN_imported) # GRN to BN
 
-
-def RNASeq_to_SBML(count_table_input, promoter_length=1000, genbank_file_input=None, normalization_type=None):
-   count_table = import_CountTable(count_table_input)  # data import
-   gene_names = count_table.index
-   output_directory = os.path.join(os.getcwd(), r'output')  # data export
-   if not os.path.exists(output_directory):
-      os.makedirs(output_directory)
-   if genbank_file_input:
-      gene_lengths, gene_promoters, organism, taxon, genes_IDs = genbank_process(genbank_file_input, gene_names, promoter_length)
-      if normalization_type:  # count table normalization
-         normalized_count_table = normalize_CountTable(count_table, gene_lengths, normalization_type)
-      else:
-         normalized_count_table = count_table
-      GRNmi, count_table_differences = RNASeq_to_GRNmi(normalized_count_table)  # GRN inference using MI
-      GRNmotifs = GRNmi_to_GRNmotifs(GRNmi, gene_promoters, count_table_differences)  # GRN verification using motif search
-      GRNdb, genes_IDs_all = get_DBs_data(organism, genes_IDs, taxon, GRNmotifs)  # GRN verification using databases
-      if GRNdb is None:
-         print('No databases interaction data available; GRN verification skipped.')
-         GRNdb = GRNmotifs.copy()
-      export_GRN(GRNdb)
-      GRNcc, CC_conditions = get_CC_data(genes_IDs_all, GRNdb)  # GRN verification using Cell Colective db
+def RNASeq_to_BN(count_table_input, promoter_length=1000, genbank_file_input=None, normalization_type=None, motifs_max_time = 180):
+   GRN, genes_IDs_all = RNASeq_to_GRN(count_table_input, promoter_length, genbank_file_input, normalization_type, motifs_max_time)
+   if genes_IDs_all:
+      GRNcc, CC_conditions = get_CC_data(genes_IDs_all, GRN)  # GRN verification using Cell Colective db
+      del genes_IDs_all, GRN
+      collect()
       GRN_to_SBML(GRNcc, CC_conditions)  # GRN to BN
-
-   elif genbank_file_input is None:
-      if normalization_type:
-         print('Count table normalization and databases info add not available - GenBank missing; skipped.')
-      GRNmi, count_table_differences = RNASeq_to_GRNmi(count_table)
-      export_GRN(GRNmi)
-      GRN_to_SBML(GRN_mi) # GRN to BN
+   else:
+      GRN_to_SBML(GRN)  # GRN to BN
```

### Comparing `Augusta-1.0.3/Augusta/DBs/CC_search_filter.py` & `Augusta-1.0.4/Augusta/DBs/CC_search_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import ccapi
+from ccapi import Client
 import logging
 
 ### get interactions and logical rules from Cell Collective (CC) database
 def CC_search(organism_all_names):
     models = []
     try:
         logging.disable(logging.INFO) # disable print log info messages
         logging.disable(logging.WARNING)
-        client = ccapi.Client()
+        client = Client()
         fetch_models = client.get('model', size = 1000, filters = {'modelTypes': ['boolean']})
         logging.disable(logging.NOTSET)
     except:
         print('Cell Collective database not available; skipped.')
         return models
 
-    # filter CC data based on input organism
+    # filter CC models based on input organism
     pos = 0
     while pos < len(fetch_models):
         one_model = fetch_models[pos]
         for name in organism_all_names:
             if (one_model.name and (name in one_model.name)) or (one_model.description and (name in one_model.description)):
                 models.append(one_model.default_version)
                 pos += 1
                 break
             elif name == organism_all_names[-1]:
                 pos += 1
     print('Cell Collective database search done.')
     return models
 
-### filter CC data based on input organism
+### filter CC data based on input organism´s genes
 def CC_filter(genes_IDs_all, GRN, models):
     GRN_CC = GRN.copy()
     global genes_IDs_all_values
     genes_IDs_all_values = sum(genes_IDs_all.values(), [])
     CC_conditions = {}
     for model in models:
         for component in model.internal_components: # check if component and regulator genes are present in the input data
@@ -76,8 +76,8 @@
             names.append(name)
         else:
             should_continue = False
             break
     if should_continue:
         names.append(cComp.name)
         values = [names, condition.type, condition.relation, condition.state]
-    return values
+    return values
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Augusta-1.0.3/Augusta/DBs/DBs_filter.py` & `Augusta-1.0.4/Augusta/DBs/DBs_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,11 +52,11 @@
         c = int(np.where(names == DBs_interactions_GRNGeneMatches.loc[i, 'target_GeneID'])[0])
         GRN_filled.iloc[r, c] = DBs_interactions_GRNGeneMatches.loc[i, 'interaction_type']
     return GRN_filled
 
 ### infer GRN from databases intractions
 def DBsInteractions_to_GRN(DBs_interactions_GRNGeneMatches):
     DB_GRN_names = np.unique(DBs_interactions_GRNGeneMatches[['source_GeneID', 'target_GeneID']].values)
-    DBsGRN_np = np.zeros((len(DB_GRN_names), len(DB_GRN_names)), dtype=int)
-    DBsGRN = pd.DataFrame(DBsGRN_np, columns=DB_GRN_names, index=DB_GRN_names)
+    DBsGRN_np = np.zeros((len(DB_GRN_names), len(DB_GRN_names)), dtype='int8')
+    DBsGRN = pd.DataFrame(DBsGRN_np, columns=DB_GRN_names, index=DB_GRN_names, dtype='int8')
     DBsGRN_filled = fill_GRN(DBsGRN, DB_GRN_names, DBs_interactions_GRNGeneMatches)
-    return DBsGRN_filled
+    return DBsGRN_filled
```

### Comparing `Augusta-1.0.3/Augusta/DBs/DBs_search.py` & `Augusta-1.0.4/Augusta/DBs/DBs_search.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/DBs/get_synonyms.py` & `Augusta-1.0.4/Augusta/DBs/get_synonyms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from EcoNameTranslator import to_common, synonyms
-import numpy as np
-import mygene
+from numpy import unique
+from mygene import MyGeneInfo
 
 ### translate scientific organism name into common name
 def organism_synonyms(organism):
     if len(organism.split()) > 2: # remove strain from organism name and save as list
         organism = [' '.join(organism.split()[0:2])]
     else:
         organism = [organism]
@@ -18,22 +18,25 @@
 
     organism_all_names = organism + common_names + synonym_names
     return organism_all_names
 
 ### get gene name synonyms
 def gene_synonyms(genes_IDs_input, taxon):
     genes_IDs = genes_IDs_input.copy()
-    mg = mygene.MyGeneInfo()
+    mg = MyGeneInfo()
     for gene_key in genes_IDs_input:
         if genes_IDs_input[gene_key]:
             genes = [gene_key] + genes_IDs_input[gene_key]
         else:
             genes = [gene_key]
         all_IDs = genes
-        new_IDs = mg.querymany(genes, scopes='symbol, locus_tag, homologene, alias, accession', fields='symbol, alias', as_dataframe=True, species=taxon)
+        try:
+            new_IDs = mg.querymany(genes, scopes='symbol, locus_tag, homologene, alias, accession', fields='symbol, alias', as_dataframe=True, species=taxon)
+        except:
+            new_IDs = None
         if new_IDs is not None:
             if 'notfound' in new_IDs:
                 new_IDs = new_IDs[new_IDs['notfound'] != True]  # filter searched names
                 new_IDs = new_IDs.drop('notfound', axis=1)
             if not new_IDs.empty:
                 if '_score' in new_IDs:
                     new_IDs = new_IDs.drop('_score', axis=1)
@@ -41,10 +44,10 @@
                 new_IDs_extracted = []  # unlist listed values
                 for value in new_IDs_list:
                     if isinstance(value, list):
                         new_IDs_extracted = value + new_IDs_extracted
                     elif isinstance(value, str):
                         new_IDs_extracted = [value] + new_IDs_extracted
                 all_IDs += new_IDs_extracted
-        all_IDs_unique = np.unique(all_IDs).tolist()
+        all_IDs_unique = unique(all_IDs).tolist()
         genes_IDs[gene_key] = all_IDs_unique
     return genes_IDs
```

### Comparing `Augusta-1.0.3/Augusta/GRN_MI/GRNmi_infer.py` & `Augusta-1.0.4/Augusta/GRN_MI/GRNmi_infer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-import math
-from .preprocessing import *
+from math import floor, sqrt
+from pandas import DataFrame
+from numpy import histogram2d, zeros, shape, arange, delete
+from .preprocessing import expression_differences, select_expression
 from sklearn.metrics import mutual_info_score
 
-
 # preprocess count table for MI computation
 def preprocess(count_table):
     gene_names = count_table.index
     difference_matrix = expression_differences(count_table, gene_names)
     highest_expression = select_expression(difference_matrix, gene_names)
     return difference_matrix, highest_expression
 
 # compute MI
 def MI_value(x, y, bins):
-    bin_xy = np.histogram2d(x, y, bins)[0]
+    bin_xy = histogram2d(x, y, bins)[0]
     MI = mutual_info_score(None, None, contingency=bin_xy)
     return MI
 
 # create matrix of MIs
 def calc_MI(input_matrix, highest_expression):
     gene_names = input_matrix.index
-    MI_matrix_np = np.zeros((np.shape(input_matrix)[0], np.shape(input_matrix)[0]))
-    MI_matrix = pd.DataFrame(MI_matrix_np, columns=gene_names, index=gene_names)
+    MI_matrix_np = zeros((shape(input_matrix)[0], shape(input_matrix)[0]))
+    MI_matrix = DataFrame(MI_matrix_np, columns=gene_names, index=gene_names)
 
     # set number of bins to discretize normalized RNA-seq
-    bins = math.floor(math.sqrt(np.shape(input_matrix)[0]/5))
+    bins = floor(sqrt(shape(input_matrix)[0]/5))
     if bins > 10:
         bins = 10
 
     # compute MI
-    vector_cols = np.arange(1, np.shape(input_matrix)[0])
-    for i in range(0, np.shape(input_matrix)[0]):
-        #print(f'MI for gene: {i+1} / {np.shape(input_matrix)[0]}')
+    vector_cols = arange(1, shape(input_matrix)[0])
+    for i in range(0, shape(input_matrix)[0]):
+        #print(f'MI for gene: {i+1} / {shape(input_matrix)[0]}')
         for j in vector_cols:
             if highest_expression.iloc[i, 1] != highest_expression.iloc[j, 1]: # compute MI only if highest expression is in different time points
                 if highest_expression.iloc[i, 1] < highest_expression.iloc[j, 1]: # set direction of edges
                     MI_matrix.iloc[i, j] = MI_value(input_matrix.iloc[i, :], input_matrix.iloc[j, :], bins)
                 else:
                     MI_matrix.iloc[j, i] = MI_value(input_matrix.iloc[i, :], input_matrix.iloc[j, :], bins)
         if len(vector_cols) > 0:
-            vector_cols = np.delete(vector_cols, 0) # delete first item in vector in order to fill only triangle in MI_matrix
+            vector_cols = delete(vector_cols, 0) # delete first item in vector in order to fill only triangle in MI_matrix
     print('Mutual information computation done.')
     return MI_matrix
```

### Comparing `Augusta-1.0.3/Augusta/GRN_MI/preprocessing.py` & `Augusta-1.0.4/Augusta/GRN_MI/preprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import numpy as np
-import pandas as pd
+from numpy import zeros, shape
+from pandas import DataFrame
 
 ### compute times differences from count table data
 def expression_differences(input_matrix, gene_names):
-    dif_matrix_np = np.zeros((np.shape(input_matrix)[0], np.shape(input_matrix)[1] - 1))
-    column_names = list(range(1, np.shape(dif_matrix_np)[1] + 1))
-    difference_matrix = pd.DataFrame(dif_matrix_np, columns=column_names, index=gene_names)
+    dif_matrix_np = zeros((shape(input_matrix)[0], shape(input_matrix)[1] - 1))
+    column_names = list(range(1, shape(dif_matrix_np)[1] + 1))
+    difference_matrix = DataFrame(dif_matrix_np, columns=column_names, index=gene_names)
 
-    for i in range(0, np.shape(difference_matrix)[0]):
-        for j in range(0, np.shape(difference_matrix)[1]):
+    for i in range(0, shape(difference_matrix)[0]):
+        for j in range(0, shape(difference_matrix)[1]):
             difference_matrix.iloc[i, j] = (input_matrix.iloc[i, j+1] - input_matrix.iloc[i, j])
     return difference_matrix
 
 
 ### select highest difference in times differences
 def select_expression(difference_matrix, gene_names):
-    highest_expr_np = np.zeros((np.shape(difference_matrix)[0], 2))
+    highest_expr_np = zeros((shape(difference_matrix)[0], 2))
     column_names = ['highest expr value', 'n of diff']
-    highest_expression = pd.DataFrame(highest_expr_np, columns = column_names, index=gene_names)
+    highest_expression = DataFrame(highest_expr_np, columns = column_names, index=gene_names)
 
     position = difference_matrix.abs().values.argmax(axis=1)
     highest_expression['n of diff'] = position  # column name in dif_matrix where the highest difference occures (i.e. 1 = first difference, column 0)
     highest_expression['highest expr value'] = ([difference_matrix.values[i][position[i]] for i in range(len(difference_matrix.values))])
     return highest_expression
 
 ### get type of interactions (positive or negative)
 def find_interaction_type(coexpression_matrix, dif_matrix):
-    dif_matrix.columns = list(range(0,np.shape(dif_matrix)[1]))
+    dif_matrix.columns = list(range(0,shape(dif_matrix)[1]))
     gene_names = coexpression_matrix.index
     GRN_matrix = coexpression_matrix.copy()
     max_expr_pos = dif_matrix.abs().values.argmax(axis=1)
 
-    for col in range(0, np.shape(GRN_matrix)[1]):
+    for col in range(0, shape(GRN_matrix)[1]):
         pos_target = max_expr_pos[col]
         if pos_target == 0: # max expression change in zero time - target couldn´t be regulated
             GRN_matrix[gene_names[col]] = GRN_matrix[gene_names[col]].replace(1, 0)
             continue
 
         expr_value_target = dif_matrix.loc[gene_names[col], pos_target]
-        for row in range(0, np.shape(GRN_matrix)[0]):
+        for row in range(0, shape(GRN_matrix)[0]):
             if GRN_matrix.iloc[row, col] == 1:
                 expr_value_source = dif_matrix.loc[gene_names[row], pos_target-1]
                 if ((expr_value_source > 0 and expr_value_target < 0) or (expr_value_source < 0 and expr_value_target > 0)):
                     GRN_matrix.iloc[row, col] = -1
-    return GRN_matrix
+    return GRN_matrix
```

### Comparing `Augusta-1.0.3/Augusta/RNASeq_normalization.py` & `Augusta-1.0.4/Augusta/RNASeq_normalization.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/SBML_generation.py` & `Augusta-1.0.4/Augusta/SBML_generation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,99 @@
 from .cno.io import cnograph
-import numpy as np
+from numpy import all
+from os import remove
+from gc import collect
 
-### convert GRN to Boolean netwok in SBML-qual file format
+### convert GRN to BN in SBML-qual file format
 def GRN_to_SBML(GRN, CC_conditions = {}):
-    c = cnograph.CNOGraph()
+    lonely_nodes = GRN_to_BNequations(GRN, CC_conditions)
+    try:
+        c_sbml = BNequations_to_SBML('output/BN.txt')
+    except MemoryError:
+        print('Low memory for exporting BN to SBML-qual. BN is saved in a form of logical equations as "BN.txt".')
+        return
+    else:
+        SBML_to_file(c_sbml, lonely_nodes)
+        remove('output/BN.txt')
+
+### convert GRN to Boolean netwok in logical equations
+def GRN_to_BNequations(GRN, CC_conditions):
     lonely_nodes = []
-    for source in GRN.columns: # get column name
-        values = GRN[source] # get column values
-        neg_values = values.index[values < 0].tolist()
-        pos_values = values.index[values > 0].tolist()
-        react = str()
-        if len(CC_conditions) > 0: # get conditions if exist for the source and target nodes
-            if (source + '_0') in CC_conditions:
+    with open('output/BN.txt', 'w') as BN_file:  # motif sequences in Stockholm format
+        for source in GRN.columns: # get column name
+            neg_values = GRN[source].index[GRN[source] < 0].tolist() # extract negative regulators
+            pos_values = GRN[source].index[GRN[source] > 0].tolist() # extract positive regulators
+            react = str()
+            if (len(CC_conditions) > 0) and ((source + '_0') in CC_conditions): # get conditions if exist for the source and target nodes
                 source_conditions = get_conditions(source, CC_conditions)
-        try:source_conditions
-        except NameError: source_conditions = []
-
-        if (len(neg_values) > 0) and (len(pos_values) > 0):
-            for pos_regulator in pos_values:
-                pos_regulator_number = 0
-                more_pos_regulator_conditions = True
-                while more_pos_regulator_conditions == True:
-                    add_pos_regulator, more_pos_regulator_conditions, pos_regulator_number = search_condition(pos_regulator, pos_regulator_number, source_conditions)
-                    if len(react) > 0:
-                        react = react + '+'
-                    react = react + add_pos_regulator
-                    for neg_regulator in neg_values:
-                        neg_regulator_number = 0
-                        more_neg_regulator_conditions = True
-                        while more_neg_regulator_conditions == True:
-                            add_neg_regulator, more_neg_regulator_conditions, neg_regulator_number = search_condition(neg_regulator, neg_regulator_number, source_conditions)
-                            react = react + '^!' + add_neg_regulator
-
-        elif (len(neg_values) > 0) and (len(pos_values) == 0):
-            for neg_regulator in neg_values:
-                neg_regulator_number = 0
-                more_neg_regulator_conditions = True
-                while more_neg_regulator_conditions == True:
-                    add_neg_regulator, more_neg_regulator_conditions, neg_regulator_number = search_condition(neg_regulator, neg_regulator_number, source_conditions)
-                    if len(react) > 0:
-                        react = react + '^'
-                    react = react + '!' + add_neg_regulator
-
-        elif (len(neg_values) == 0) and (len(pos_values) > 0):
-            for pos_regulator in pos_values:
-                pos_regulator_number = 0
-                more_pos_regulator_conditions = True
-                while more_pos_regulator_conditions == True:
-                    add_pos_regulator, more_pos_regulator_conditions, pos_regulator_number = search_condition(pos_regulator, pos_regulator_number, source_conditions)
-                    if len(react) > 0:
-                        react = react + '+'
-                    react = react + add_pos_regulator
-
-        if len(react) > 0:
-            react = react + '=' + source
-            c.add_reaction(react)
+            else: source_conditions = []
 
-        elif np.all((GRN.loc[source]) == 0): # check for nodes without edges
-            lonely_nodes.append(source)
+            if (len(neg_values) > 0) and (len(pos_values) > 0):
+                for pos_regulator in pos_values:
+                    pos_regulator_number = 0
+                    more_pos_regulator_conditions = True
+                    while more_pos_regulator_conditions == True:
+                        add_pos_regulator, more_pos_regulator_conditions, pos_regulator_number = search_condition(pos_regulator, pos_regulator_number, source_conditions)
+                        if len(react) > 0:
+                            react = react + '+'
+                        react = react + add_pos_regulator
+                        for neg_regulator in neg_values:
+                            neg_regulator_number = 0
+                            more_neg_regulator_conditions = True
+                            while more_neg_regulator_conditions == True:
+                                add_neg_regulator, more_neg_regulator_conditions, neg_regulator_number = search_condition(neg_regulator, neg_regulator_number, source_conditions)
+                                react = react + '^!' + add_neg_regulator
+
+            elif (len(neg_values) > 0) and (len(pos_values) == 0):
+                for neg_regulator in neg_values:
+                    neg_regulator_number = 0
+                    more_neg_regulator_conditions = True
+                    while more_neg_regulator_conditions == True:
+                        add_neg_regulator, more_neg_regulator_conditions, neg_regulator_number = search_condition(neg_regulator, neg_regulator_number, source_conditions)
+                        if len(react) > 0:
+                            react = react + '^'
+                        react = react + '!' + add_neg_regulator
+
+            elif (len(neg_values) == 0) and (len(pos_values) > 0):
+                for pos_regulator in pos_values:
+                    pos_regulator_number = 0
+                    more_pos_regulator_conditions = True
+                    while more_pos_regulator_conditions == True:
+                        add_pos_regulator, more_pos_regulator_conditions, pos_regulator_number = search_condition(pos_regulator, pos_regulator_number, source_conditions)
+                        if len(react) > 0:
+                            react = react + '+'
+                        react = react + add_pos_regulator
+
+            if len(react) > 0:
+                react = react + '=' + source
+                BN_file.write(react + '\n')
+            elif all((GRN.loc[source]) == 0): # check for nodes without edges
+                lonely_nodes.append(source)
+            collect()
+    return lonely_nodes
+
+### convert Boolean netwok in logical equations into BN is SBML-qual file format
+def BNequations_to_SBML(filename):
+    c = cnograph.CNOGraph() # generate SBML-qual object
+    with open(filename) as file:
+        for line in file:
+            c.add_reaction(line)
     c_sbml = c.to_sbmlqual()
+    return c_sbml
 
-    # write sbml file; add nodes without edges
+### write SBML-qual file; add nodes without edges (lonely nodes)
+def SBML_to_file(c_sbml, lonely_nodes):
     with open('output/BN.sbml','w') as f_out:
         for line_no, line in enumerate(c_sbml.split("\n")):
             f_out.write(line + "\n")
             if "<qual:listOfQualitativeSpecies" in line:
                 for lonely_node in lonely_nodes:
                     f_out.write("""<qual:qualitativeSpecies qual:constant="false" qual:compartment="main" qual:id="{0}"/>\n""".format(lonely_node))
     print('Boolean network stored as "BN.sbml".')
 
-
 # add reaction´s equation in case conditions are available
 def get_conditions(source, CC_conditions):
     source_conditions = {}
     condition_number = 0  # helper variable for getting condition in case one component has more conditions
     regulator_number = 0 # helper variable for getting condition in case one regulator has more conditions
     more_conditions = True
     while more_conditions == True:
@@ -108,17 +128,16 @@
 def get_conditions_parameters(condition_value, condition_react, condition):
     if (condition_value[1] == 'if' and condition_value[3] == 'on') or (condition_value[1] == 'unless' and condition_value[3] == 'off'):
         condition_react = condition_react + '^' + condition
     elif (condition_value[1] == 'if' and condition_value[3] == 'off') or (condition_value[1] == 'unless' and condition_value[3] == 'on'):
         condition_react = condition_react + '^!' + condition
     return condition_react
 
-
 def search_condition(regulator, regulator_number, source_conditions):
-    if (regulator + '_' + str(regulator_number)) in source_conditions:  # add conditions
+    if (str(regulator) + '_' + str(regulator_number)) in source_conditions:  # add conditions
         add_regulator = source_conditions[regulator + '_' + str(regulator_number)]
         regulator_number += 1
         more_regulator_conditions = True
     else:
         add_regulator = regulator
         more_regulator_conditions = False
     return add_regulator, more_regulator_conditions, regulator_number
```

### Comparing `Augusta-1.0.3/Augusta/cno/LICENSE` & `Augusta-1.0.4/Augusta/cno/LICENSE`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/README.rst` & `Augusta-1.0.4/Augusta/cno/README.rst`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/__init__.py` & `Augusta-1.0.4/Augusta/cno/__init__.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/__init__.py` & `Augusta-1.0.4/Augusta/cno/io/__init__.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/adj2sif.py` & `Augusta-1.0.4/Augusta/cno/io/adj2sif.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/cna.py` & `Augusta-1.0.4/Augusta/cno/io/cna.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/cnograph.py` & `Augusta-1.0.4/Augusta/cno/io/cnograph.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/eda.py` & `Augusta-1.0.4/Augusta/cno/io/eda.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/mapback.py` & `Augusta-1.0.4/Augusta/cno/io/mapback.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/measurements.py` & `Augusta-1.0.4/Augusta/cno/io/measurements.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/metabolites.py` & `Augusta-1.0.4/Augusta/cno/io/metabolites.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/midas.py` & `Augusta-1.0.4/Augusta/cno/io/midas.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/midas_normalisation.py` & `Augusta-1.0.4/Augusta/cno/io/midas_normalisation.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/multigraph.py` & `Augusta-1.0.4/Augusta/cno/io/multigraph.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/multimidas.py` & `Augusta-1.0.4/Augusta/cno/io/multimidas.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/net.py` & `Augusta-1.0.4/Augusta/cno/io/net.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/obs.py` & `Augusta-1.0.4/Augusta/cno/io/obs.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/randomisation.py` & `Augusta-1.0.4/Augusta/cno/io/randomisation.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/reactions.py` & `Augusta-1.0.4/Augusta/cno/io/reactions.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/sbml.py` & `Augusta-1.0.4/Augusta/cno/io/sbml.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/sbmlqual.py` & `Augusta-1.0.4/Augusta/cno/io/sbmlqual.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/sif.py` & `Augusta-1.0.4/Augusta/cno/io/sif.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/sif2asp.py` & `Augusta-1.0.4/Augusta/cno/io/sif2asp.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/sop2sif.py` & `Augusta-1.0.4/Augusta/cno/io/sop2sif.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/validation.py` & `Augusta-1.0.4/Augusta/cno/io/validation.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/xcnograph.py` & `Augusta-1.0.4/Augusta/cno/io/xcnograph.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/io/xmlmidas.py` & `Augusta-1.0.4/Augusta/cno/io/xmlmidas.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/misc/classifier.py` & `Augusta-1.0.4/Augusta/cno/misc/classifier.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/misc/dependencies.py` & `Augusta-1.0.4/Augusta/cno/misc/dependencies.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/misc/matfun.py` & `Augusta-1.0.4/Augusta/cno/misc/matfun.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/cno/misc/truthtable.py` & `Augusta-1.0.4/Augusta/cno/misc/truthtable.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/Augusta/core.py` & `Augusta-1.0.4/Augusta/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-import pandas as pd
-import numpy as np
-import sys, os
+from pandas import DataFrame, concat
+from numpy import where, sum
+import sys
+from os import path, remove, devnull
 
-from .data_import import import_CountTable, genbank_process, import_GRN
 from .GRN_MI import GRNmi_infer, preprocessing
-from .RNASeq_normalization import normalize_CountTable
 from .motif_discovery import find_motifs
 from .DBs import DBs_search, DBs_filter, CC_search_filter, get_synonyms
-from .SBML_generation import GRN_to_SBML
 from .data_export import export_interactions, export_GRN
 
 
 # infer GRN from count table using mutual information
 def RNASeq_to_GRNmi(count_table):
     print('Mutual information computation...')
     gene_names = count_table.index
     count_table_differences, highest_difference = GRNmi_infer.preprocess(count_table)
     MI_matrix = GRNmi_infer.calc_MI(count_table, highest_difference)
-    CoeN_np = np.where(MI_matrix > 0, 1, MI_matrix).astype(int)
-    CoeN = pd.DataFrame(CoeN_np, columns=gene_names, index=gene_names)
+    CoeN_np = where(MI_matrix > 0, 1, MI_matrix).astype(dtype='int8')
+    CoeN = DataFrame(CoeN_np, columns=gene_names, index=gene_names, dtype='int8')
     GRNmi = preprocessing.find_interaction_type(CoeN, count_table_differences)
     return GRNmi, count_table_differences
 
 # verify GRN using motif search
-def GRNmi_to_GRNmotifs(GRNmi, gene_promoters, count_table_differences):
-    n_of_reg_genes = np.sum(GRNmi > 0)
-    if np.sum(n_of_reg_genes >= 5) == 0:  # if no TF regulates at least 5 genes, motif search is not possible
+def GRNmi_to_GRNmotifs(GRNmi, gene_promoters, count_table_differences, motifs_max_time):
+    n_of_reg_genes = sum(GRNmi > 0)
+    if sum(n_of_reg_genes >= 5) == 0:  # if no TF regulates at least 5 genes, motif search is not possible
         print('Motif search not available; skipped.')
         return GRNmi
     else:
-        CoeNmotifs = find_motifs(GRNmi, gene_promoters)
-        if os.path.exists('temporary_coreg_seq.fasta'):
-            os.remove('temporary_coreg_seq.fasta')
-        if os.path.getsize('output/discovered_motifs.sto') == 0:
-            os.remove('output/discovered_motifs.sto')
+        CoeNmotifs = find_motifs(GRNmi, gene_promoters, motifs_max_time)
+        if path.exists('temporary_coreg_seq.fasta'):
+            remove('temporary_coreg_seq.fasta')
+        if path.getsize('output/discovered_motifs.sto') == 0:
+            remove('output/discovered_motifs.sto')
             print('No motif found; skipped.')
             return GRNmi
         elif sum(CoeNmotifs.sum(axis=1)) == 0:
             print('No motifs reversely searched in genome. Discovered motifs have been saved as "discovered_motifs.sto".')
             return GRNmi
         else:
             GRNmotifs = preprocessing.find_interaction_type(CoeNmotifs, count_table_differences)
@@ -45,26 +43,26 @@
 
 # search genes interactions in databases
 def get_DBs_data(organism, genes_IDs_gb, taxon, GRN = None):
     global organism_all_names
     print('Synonym organism names search...')
     organism_all_names = get_synonyms.organism_synonyms(organism)
     print('Synonym genes names search...')
-    sys.stdout = open(os.devnull, 'w')  # block print
+    sys.stdout = open(devnull, 'w')  # block print
     genes_IDs_all = get_synonyms.gene_synonyms(genes_IDs_gb, taxon)
     sys.stdout = sys.__stdout__  # enable print
     print('Synonym names search done.')
 
     # search interaction databases
     op_interactions = DBs_search.search_OmniPath(taxon)
     signor_interactions = DBs_search.search_Signor(taxon)
     sl_interactions = DBs_search.search_SignaLink(taxon)
     trrust_interactions = DBs_search.search_TRRUST(organism_all_names)
     try:
-        allDBs_interactions = pd.concat([signor_interactions, op_interactions, sl_interactions, trrust_interactions])
+        allDBs_interactions = concat([signor_interactions, op_interactions, sl_interactions, trrust_interactions])
     except ValueError:
         print('No data searched in interaction databases.')
         return GRN, genes_IDs_all
     else:
         interactions_all, interactions_uncertain, interactions_filtered = DBs_filter.filter_interactions(allDBs_interactions, genes_IDs_all)
         export_interactions(interactions_all, interactions_uncertain)
         if len(interactions_filtered) > 0:
```

### Comparing `Augusta-1.0.3/Augusta/data_export.py` & `Augusta-1.0.4/Augusta/data_export.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import pandas as pd
+from pandas import DataFrame
 
 ### export interactions found in databases
 def export_interactions(interactions_all, interactions_uncertain):
     if len(interactions_all) > 0:
-        pd.DataFrame(interactions_all).to_csv('output/DBs_interactions_list.csv', index=False)
+        DataFrame(interactions_all).to_csv('output/DBs_interactions_list.csv', index=False)
         print('All interactions searched across databases stored as "DBs_interactions_list.csv".')
     if len(interactions_uncertain) > 0:
-        pd.DataFrame(interactions_uncertain).to_csv('output/DBs_interactions_uncertain.csv', index=False)
+        DataFrame(interactions_uncertain).to_csv('output/DBs_interactions_uncertain.csv', index=False)
         print('Uncertain interactions stored as "DBs_interactions_uncertain.csv". The more prevaled interaction type was used for the GRN inference.')
 
 ### export GRN
 def export_GRN(GRN):
-    pd.DataFrame(GRN).to_csv('output/GRN.csv')
+    DataFrame(GRN).to_csv('output/GRN.csv')
     print('GRN stored as "GRN.csv".')
```

### Comparing `Augusta-1.0.3/Augusta/data_import.py` & `Augusta-1.0.4/Augusta/data_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import pandas as pd
-import numpy as np
+from pandas import read_table
+from numpy import shape
 from Bio import SeqIO
 
 ### import count table (RNA-Seq) data: matrix MxN (M = gene locus tag / name; N = time)
 def import_CountTable(count_table):
-    input_matrix = pd.read_table(count_table, index_col=[0], sep = None, engine = 'python')
-    if (np.shape(input_matrix)[1]) < 3:
+    input_matrix = read_table(count_table, index_col=[0], sep = None, engine = 'python')
+    if (shape(input_matrix)[1]) < 3:
         print('Expression data error: Not enough time points included. Provide at least 3 time points.')
         return
-    elif (np.shape(input_matrix)[0]) < 2:
+    elif (shape(input_matrix)[0]) < 2:
         print ('Expression data error: Not enough genes included. Provide at least 2 genes.')
         return
-    elif (len(input_matrix.columns) != np.shape(input_matrix)[1]) or (len(input_matrix.index) != np.shape(input_matrix)[0]):
+    elif (len(input_matrix.columns) != shape(input_matrix)[1]) or (len(input_matrix.index) != shape(input_matrix)[0]):
         print('Expression data error: Provide names of rows and columns.')
         return
     else:
         print('Count table uploaded.')
         return input_matrix
 
 
 ### import GenBank file
 def genbank_process(gb_file, gene_names, promoter_length):
-    gene_lengths = [0] * np.shape(gene_names)[0]
+    gene_lengths = [0] * shape(gene_names)[0]
     gene_promoters = []
     qualifier = find_qualifier(gb_file, gene_names)
 
     for record in SeqIO.parse(gb_file, 'genbank'):
         sequence = record.seq
         indexes = index_genbank_features(record, 'gene', qualifier)
         genes_IDs = dict.fromkeys(gene_names)
-        for i in range(0, np.shape(gene_names)[0]):
+        for i in range(0, shape(gene_names)[0]):
             # get gene promoter
             try:
                 feature = record.features[indexes[gene_names[i]]]
                 gene_start = feature.location._start.position + 1 # (exact gene start - python marks gene start at position - 1)
                 gene_end = feature.location._end.position
             except:
                 raise Exception('Gene name ', gene_names[i], ' does not correspond to Genbank IDs. Needed gene names in count table: Locus tag or Gene name.')
@@ -121,10 +121,10 @@
                            % (value, feature_type, answer[value], index))
                     else:
                         answer[value] = index
     return answer
 
 ### import gene regulatory network
 def import_GRN(input_GRN):
-    GRN = pd.read_table(input_GRN, index_col=[0], sep=None, engine='python') # import table with unknown separator
+    GRN = read_table(input_GRN, index_col=[0], sep=None, engine='python') # import table with unknown separator
     print('GRN uploaded.')
-    return GRN
+    return GRN
```

### Comparing `Augusta-1.0.3/Augusta/motif_discovery.py` & `Augusta-1.0.4/Augusta/motif_discovery.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,104 @@
-import numpy as np
-import pandas as pd
-import os
-import shutil
-import docker
+from numpy import sum, zeros, shape, max
+from pandas import DataFrame
+from os import path, mkdir, chmod, getcwd, remove
+from shutil import rmtree
+from docker import from_env
 from Bio import motifs
-import time
+from time import sleep
+from gc import collect
 
 ### search for motifs in promoter sequences of coregulated genes; search for discovered motifs in all promoter sequences
-def find_motifs(initial_GRN, gene_promoters):
+def find_motifs(initial_GRN, gene_promoters, motifs_max_time):
     print('Motifs search...')
     genes = initial_GRN.index
-    n_of_reg_genes = np.sum(initial_GRN != 0)
-    verified_GRN_np = np.zeros((np.shape(initial_GRN)[0], np.shape(initial_GRN)[1]), dtype = int)
-    verified_GRN = pd.DataFrame(verified_GRN_np, columns=genes, index=genes)
-    client = docker.from_env()
+    n_of_reg_genes = sum(initial_GRN != 0)
+    verified_GRN_np = zeros((shape(initial_GRN)[0], shape(initial_GRN)[1]), dtype='int8')
+    verified_GRN = DataFrame(verified_GRN_np, columns=genes, index=genes, dtype='int8')
+    client = from_env()
     client.images.pull('memesuite/memesuite:latest')
     sto_file = open('output/discovered_motifs.sto', 'w') # motif sequences in Stockholm format
 
-    for r in range (0, np.shape(initial_GRN)[0]):
+    for r in range (0, shape(initial_GRN)[0]):
         if n_of_reg_genes[r] >= 5: # motif search only if TFs regulates at least 5 genes
-            #print(f'Motif: {r+1} / {np.shape(initial_GRN)[0]}')
-            ofile = open('temporary_coreg_seq.fasta', 'w') # promoter sequences
-            prom_no = 1
-            coreg_seqs = 0
-            for c in range(0, np.shape(initial_GRN)[1]): # write individual promoters into temporary_coreg_seq.fasta, filter out promoters shorter than 5
-                if initial_GRN.iloc[r, c] > 0 and len(gene_promoters[c]) >= 5:
-                    ofile.write('>' + str(genes[r]) + '_' + str(prom_no) + '\n' + str(gene_promoters[c]) + '\n')
-                    coreg_seqs += 1
-                    prom_no += 1
-            ofile.close()
+            gene_name = genes[r]
+            #print(f'Motif: {r+1} / {shape(initial_GRN)[0]}')
+            with open('temporary_coreg_seq.fasta', 'w') as ofile: # promoter sequences
+                prom_no = 1
+                coreg_seqs = 0
+                for c in range(0, shape(initial_GRN)[1]): # write individual promoters into temporary_coreg_seq.fasta, filter out promoters shorter than 5
+                    if initial_GRN.iloc[r, c] > 0 and len(gene_promoters[c]) >= 5:
+                        ofile.write('>' + str(gene_name) + '_' + str(prom_no) + '\n' + str(gene_promoters[c]) + '\n')
+                        coreg_seqs += 1
+                        prom_no += 1
+
             # motif discovery using MEME Suite Docker if promoters were exported to the fasta file
-            if (os.path.getsize('temporary_coreg_seq.fasta') > 0) & (coreg_seqs > 1): # number of sequences must be 2 at least
-                if not os.path.exists('meme_out'):
-                    os.mkdir('meme_out')
-                os.chmod('meme_out', 0o777)
-                os.chmod('temporary_coreg_seq.fasta', 0o777)
-                client.containers.run('memesuite/memesuite:latest',
+            if (path.getsize('temporary_coreg_seq.fasta') > 0) & (coreg_seqs > 1): # number of sequences must be 2 at least
+                if not path.exists('meme_out'):
+                    mkdir('meme_out')
+                chmod('meme_out', 0o777)
+                chmod('temporary_coreg_seq.fasta', 0o777)
+                container = client.containers.run('memesuite/memesuite:latest',
                                                   'meme -mod zoops -minw 5  -dna temporary_coreg_seq.fasta',
-                                                  volumes={os.getcwd(): {'bind': '/home/meme', 'mode': 'rw'}}, detach=True, remove=True)
-                sleep = 0
-                while not os.path.exists('meme_out/meme.xml'):
-                    time.sleep(2)
-                    sleep += 1
-                    if sleep > 30: # skip current motif search as meme suite has not returned results in a long time
+                                                  volumes={getcwd(): {'bind': '/home/meme', 'mode': 'rw'}},
+                                                  detach=True, name=str(gene_name), remove=True)
+
+                sleep_count = 0
+                while client.containers.list(filters={'name':str(gene_name)}): # check if MEME Suite is still running
+                    if sleep_count > motifs_max_time:  # skip current motif search as meme suite container has not finished in a long time
+                        print("Motif search terminated for TF: ", str(gene_name), " (time limit exceeded).")
+                        try:
+                            container.stop(timeout=5)
+                        except: # container already finished or removal already in progress
+                            pass
                         break
+                    else:
+                        sleep(5)
+                        sleep_count += 5
+                del container
+
                 try:
-                    handle = open('meme_out/meme.xml')
-                    record = motifs.parse(handle, 'meme')
-                    handle.close()
+                    with open('meme_out/meme.xml') as handle:
+                        record = motifs.parse(handle, 'meme')
                 except:
                     continue
 
                 for m in range(0, len(record)):  # search each discovered motif
                     motif = record[m]
                     motif.pseudocounts = 0.5
                     pssm = motif.pssm # Position-Specific Scoring Matrix
                     distribution = pssm.distribution()
-                    threshold = distribution.threshold_fpr(0.01)
+                    threshold = round(distribution.threshold_balanced(1000),2) # distribution.threshold_fpr(0.01) - puvodne, pak balanced(10000) ###smazat KOMENTAR
+                    threshold_int = int(threshold*100)
 
                     for n in range(0, len(gene_promoters)): # search motif in each promoter
                         if len(gene_promoters[n]) >= motif.instances[0].length:
                             score = pssm.calculate(gene_promoters[n])
-                            try:
-                                score_max = max(score)
-                            except TypeError: # score has only 1 value
-                                score_max = score
-                            except ValueError: # score has 0 values
-                                score_max = threshold - 10
-                            rpssm = pssm.reverse_complement()
+                            score_max = round(max(score, initial=threshold),2)
+                            score_max_int = int(score_max*100)
+                            rpssm = pssm.reverse_complement() # reverse complement
                             score_rev = rpssm.calculate(gene_promoters[n])
-                            try:
-                                score_rev_max = max(score_rev)
-                            except TypeError:
-                                score_rev_max = score_rev
-                            except ValueError:
-                                score_rev_max = threshold - 10
-                            if score_max >= threshold or score_rev_max >= threshold:
+                            score_rev_max = round(max(score_rev, initial=threshold),2)
+                            score_rev_max_int = int(score_rev_max*100)
+                            if (score_max_int > threshold_int) or (score_rev_max_int > threshold_int):
                                 verified_GRN.iloc[r, n] = 1 # assign found motif in the promoter to the TF
 
-                # MEME Suite output into Stockholm file format
-                motifs_stockholm(genes, r, record, sto_file)
+                    # MEME Suite output into Stockholm file format
+                    motifs_stockholm(gene_name, m, motif.consensus, sto_file)
                 try:
-                    shutil.rmtree('meme_out')
+                    rmtree('meme_out')
                 except PermissionError:
                     pass
-            os.remove('temporary_coreg_seq.fasta')
+        collect()
+    remove('temporary_coreg_seq.fasta')
     sto_file.close()
     print('Motifs search done.')
     return(verified_GRN)
 
 ### MEME Suite output into Stockholm file format
-def motifs_stockholm(genes, r, record, sto_file):
-    for i in range(0, len(record)):  # save each discovered motif into Stockholm file
-        motifs_discovered = record[i]
-        sto_file.write('# STOCKHOLM 1.0' + '\n')
-        sto_file.write('#=GF ID   ' + str(genes[r]) + '\n')
-
-        for z in range(0,motifs_discovered.num_occurrences): # save each sequence containing discovered motif into Stockholm file
-            sto_file.write(
-                str(motifs_discovered.instances[z].sequence_name) + '	' + str(motifs_discovered.instances[z]) + '\n')
-        sto_file.write('//' + '\n')
+def motifs_stockholm(gene_name, count, consensus, sto_file): # save each discovered motif into Stockholm file
+    sto_file.write('# STOCKHOLM 1.0' + '\n')                # header
+    sto_file.write('#=GF ID   ' + str(gene_name) + '\n')    # header
+    sto_file.write(                                         # sequence name, consensus motif
+                str(gene_name) + '_' + str(count) +
+                '	' + str(consensus) + '\n')
+    sto_file.write('//' + '\n')                             # tail
```

### Comparing `Augusta-1.0.3/Augusta.egg-info/PKG-INFO` & `Augusta-1.0.4/Augusta.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augusta
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for inference of the gene regulatory network and the boolean network using RNA-Seq data.
 Home-page: https://github.com/JanaMus/Augusta
 Author: Jana Musilova, Zdenek Vafek, Karel Sedlar
 Author-email: musilovajana@vut.cz
 License: MIT
 Keywords: Computational biology,Bioinformatics,RNA-Seq,mutual information,database,Boolean network,Gene Regulatory network,SBML
 Classifier: Programming Language :: Python :: 3
@@ -40,38 +40,38 @@
    
 
 .. code-block::
 
    $ pip install Augusta
 
 
-**Usage:**
+**Usage:** 
 
 See `Inputs <https://augusta.readthedocs.io/en/latest/User%20guide.html>`_ for details about input files and variables.
 
 .. code-block:: 
 
    $ python
    >>> import Augusta
    
 GRN and BN inference using RNA-Seq:
 
 .. code-block:: 
 
-   >>> Augusta.RNASeq_to_SBML(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string')
+   >>> Augusta.RNASeq_to_BN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string', motifs_max_time = My_seconds)
 
 GRN inference using RNA-Seq:
 
 .. code-block:: 
 
-   >>> GRN = Augusta.RNASeq_to_GRN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string')
+   >>> Augusta.RNASeq_to_GRN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string', motifs_max_time = My_seconds)
 
 
 BN inference using GRN:
 
 .. code-block:: 
 
-   >>> Augusta.GRNtoBN(GRN_input = 'MyGRN_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', add_dbs_info = 'My_string')
+   >>> Augusta.GRN_to_BN(GRN_input = 'MyGRN_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', add_dbs_info = 'My_string')
```

### Comparing `Augusta-1.0.3/Augusta.egg-info/SOURCES.txt` & `Augusta-1.0.4/Augusta.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 Augusta/cno/misc/profiler.py
 Augusta/cno/misc/tools.py
 Augusta/cno/misc/truthtable.py
 data/Cbeijerinckii.csv
 data/Cbeijerinckii.gb
 data/Ecoli.gb
 data/Ecoli_DREAM4.csv
-data/GRN_example.csv
+data/example_GRN.csv
 data/output/Ecoli_BN.sbml
 data/output/Ecoli_GRN.csv
 data/output/Ecoli_discovered_motifs.sto
 docs/Examples.rst
 docs/Installation.rst
 docs/Makefile
 docs/User guide.rst
```

### Comparing `Augusta-1.0.3/LICENSE` & `Augusta-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/PKG-INFO` & `Augusta-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augusta
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for inference of the gene regulatory network and the boolean network using RNA-Seq data.
 Home-page: https://github.com/JanaMus/Augusta
 Author: Jana Musilova, Zdenek Vafek, Karel Sedlar
 Author-email: musilovajana@vut.cz
 License: MIT
 Keywords: Computational biology,Bioinformatics,RNA-Seq,mutual information,database,Boolean network,Gene Regulatory network,SBML
 Classifier: Programming Language :: Python :: 3
@@ -40,38 +40,38 @@
    
 
 .. code-block::
 
    $ pip install Augusta
 
 
-**Usage:**
+**Usage:** 
 
 See `Inputs <https://augusta.readthedocs.io/en/latest/User%20guide.html>`_ for details about input files and variables.
 
 .. code-block:: 
 
    $ python
    >>> import Augusta
    
 GRN and BN inference using RNA-Seq:
 
 .. code-block:: 
 
-   >>> Augusta.RNASeq_to_SBML(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string')
+   >>> Augusta.RNASeq_to_BN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string', motifs_max_time = My_seconds)
 
 GRN inference using RNA-Seq:
 
 .. code-block:: 
 
-   >>> GRN = Augusta.RNASeq_to_GRN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string')
+   >>> Augusta.RNASeq_to_GRN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string', motifs_max_time = My_seconds)
 
 
 BN inference using GRN:
 
 .. code-block:: 
 
-   >>> Augusta.GRNtoBN(GRN_input = 'MyGRN_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', add_dbs_info = 'My_string')
+   >>> Augusta.GRN_to_BN(GRN_input = 'MyGRN_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', add_dbs_info = 'My_string')
```

### Comparing `Augusta-1.0.3/README.rst` & `Augusta-1.0.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -24,38 +24,38 @@
    
 
 .. code-block::
 
    $ pip install Augusta
 
 
-**Usage:**
+**Usage:** 
 
 See `Inputs <https://augusta.readthedocs.io/en/latest/User%20guide.html>`_ for details about input files and variables.
 
 .. code-block:: 
 
    $ python
    >>> import Augusta
    
 GRN and BN inference using RNA-Seq:
 
 .. code-block:: 
 
-   >>> Augusta.RNASeq_to_SBML(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string')
+   >>> Augusta.RNASeq_to_BN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string', motifs_max_time = My_seconds)
 
 GRN inference using RNA-Seq:
 
 .. code-block:: 
 
-   >>> GRN = Augusta.RNASeq_to_GRN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string')
+   >>> Augusta.RNASeq_to_GRN(count_table_input = 'MyCT_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', normalization_type = 'My_string', motifs_max_time = My_seconds)
 
 
 BN inference using GRN:
 
 .. code-block:: 
 
-   >>> Augusta.GRNtoBN(GRN_input = 'MyGRN_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', add_dbs_info = 'My_string')
+   >>> Augusta.GRN_to_BN(GRN_input = 'MyGRN_file.csv', promoter_length = My_number, genbank_file_input = 'MyGB_file.gb', add_dbs_info = 'My_string')
```

### Comparing `Augusta-1.0.3/data/Cbeijerinckii.gb` & `Augusta-1.0.4/data/Cbeijerinckii.gb`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/data/Ecoli.gb` & `Augusta-1.0.4/data/Ecoli.gb`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/data/Ecoli_DREAM4.csv` & `Augusta-1.0.4/data/Ecoli_DREAM4.csv`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/Examples.rst` & `Augusta-1.0.4/docs/Examples.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Examples
 ----------
-The example section is divided into two sections.
-In the first on we infer subnetworks using *in silico* dataset with the aim to get familiar with Augusta.
-In the second section we infer networks using real organism´s dataset.
+The example section is divided into two subsections.
+In the first one, we infer subnetworks using *in silico* dataset with the aim to get familiar with Augusta.
+In the second section, we infer networks using a whole-genome organism´s dataset.
 All input data are available on GitHub in the `"data" directory <https://github.com/JanaMus/Augusta/tree/master/data>`_.
-Furthermore, in each section is tutorial how to download the inputs.
+Furthermore, in each section is a tutorial on how to download the inputs.
 
 
 Test data
 ^^^^^^^^^^^^
 Test data are made by *in silico* dataset of bacterium´s *Escherichia coli* selected genes
 provided by the `DREAM4 challenge <https://www.synapse.org/#!Synapse:syn3049712/wiki/74628>`_.
 
@@ -16,36 +16,36 @@
 """""""""""""
 
 * **count table** file
 
 We will use the file "insilico_size100_1_timeseries.csv" from the
 `DREAM4 challenge. <https://www.synapse.org/#!Synapse:syn3049712/wiki/74628>`_.
 We modified the file for our needs by swapping the matrix so that the genes are in the first column and times in the first row.
-We also rewrote the gene names according to the official gene names of the organism in order to match particular genes with information available in GenBank file.
+We also rewrote the gene names according to the official gene names of the organism in order to match particular genes with information available in the GenBank file.
 The modified file is available on GitHub in the "data" directory as `"Ecoli_DREAM4.csv" <https://github.com/JanaMus/Augusta/blob/master/data/Ecoli_DREAM4.csv>`_.
 
 
 * **GenBank** file
 
-We will use *Escherichia coli* BW25113 available from NCBI Nucleotide database under the accession `CP009273 <https://www.ncbi.nlm.nih.gov/nuccore/CP009273.1/>`_.
+We will use *Escherichia coli* BW25113 available from the NCBI Nucleotide database under the accession `CP009273 <https://www.ncbi.nlm.nih.gov/nuccore/CP009273.1/>`_.
 The GenBank file can be downloaded in the GenBank full format. Otherwise,
 it is also available on GitHub in the "data" directory as `"Ecoli.gb" <https://github.com/JanaMus/Augusta/blob/master/data/Ecoli.gb>`_.
 
 
 Usage example
 """""""""""""
-Below is provided an example of the functions for generating GRN and for converting GRN to BN. See :ref:`Usage` for further available functions.
+Below is provided an example of the functions for generating GRN and converting GRN to BN. See :ref:`Usage` for further available functions.
 
-*Note: input files must be in the current directory or full path must be provided.*
+*Note: input files must be in the current directory or a full path must be provided.*
 
 Generate GRN:
 
 .. code-block:: python
 
-   >>> GRN = Augusta.RNASeq_to_GRN(count_table_input = 'Ecoli_DREAM4.csv', promoter_length = 1000, genbank_file_input = 'Ecoli.gb', normalization_type = 'TPM')
+   >>> GRN = Augusta.RNASeq_to_GRN(count_table_input = 'Ecoli_DREAM4.csv', promoter_length = 1000, genbank_file_input = 'Ecoli.gb', normalization_type = 'TPM', motifs_max_time=180)[0]
 
    Count table uploaded.
    GenBank uploaded.
    Count table normalization done.
    Mutual information computation...
    Mutual information computation done.
    Motifs search...
@@ -61,15 +61,14 @@
 
 Convert generated GRN to BN:
 
 .. code-block:: python
 
    >>> Augusta.GRN_to_BN(GRN_input = GRN, promoter_length = 1000, genbank_file_input = 'Ecoli.gb', add_dbs_info = 1)
 
-   GRN uploaded.
    GenBank uploaded.
    Synonym organism names search...
    Synonym genes names search...
    Synonym names search done.
    No data searched in interaction databases.
    GRN stored as "GRN.csv".
    Cell Collective database search done.
@@ -78,117 +77,104 @@
 
 The computation should be done in several minutes, depending on the specific machine.
 
 Output files
 """""""""""""
 The files are stored in the generated "output" directory.
 
-* transcription motifs
+* motifs
 
- * all motifs discovered in the genome assigned to their transcription factor
+ * all TFBM discovered in the genome assigned to their transcription factor
  * Stockholm file format
  * "discovered_motifs.sto"
  * available on GitHub in the "data/output" directory as `"Ecoli_discovered_motifs.sto" <https://github.com/JanaMus/Augusta/blob/master/data/output/Ecoli_discovered_motifs.sto>`_
 
-First transcription factor´s motifs in the file (transcription factor is BW25113_0564; discovered motifs are in the second column):
+First transcription factor´s motifs in the file (transcription factor is BW25113_0564; discovered motif sequence is in the second column):
 
 .. code-block:: python
 
    # STOCKHOLM 1.0
    #=GF ID   BW25113_0564
-   BW25113_0995_10	CCCGCCAGC
-   BW25113_0995_5	GCGGCACGC
-   BW25113_0995_9	CCCGCCATC
-   BW25113_0995_7	CCAGCCCTC
-   BW25113_0995_4	GCGGCAGGC
-   BW25113_0995_11	CCGGGGAGC
-   BW25113_0995_12	GGAGCACAC
-   BW25113_0995_13	CGGGTCCAC
-   BW25113_0995_3	TCCGTGCGC
-   BW25113_0995_2	GGAGTGCGC
-   BW25113_0995_6	TGGGCCAGG
-   BW25113_0995_1	TAAGCAAGC
-   BW25113_0995_8	GGCTGAAAC
+   BW25113_0564_0	TTCTCCCCATCCTCCCAGGCATTACGCAACGTGAAACTCCAGGGATTTG
    //
 
 
 * Gene Regulatory Network
 
- * adjancency matrix in CSV file format
+ * adjancency matrix in the CSV file format
  * "GRN.csv"
  * available on GitHub in the "data/output" directory as `"Ecoli_GRN.csv" <https://github.com/JanaMus/Augusta/blob/master/data/output/Ecoli_GRN.csv>`_.
 
 
 GRN visualized in `Cytoscape software: <https://cytoscape.org/>`_
 
 .. image:: _static/Ecoli_GRN.png
   :alt: Ecoli_GRN_visualized
 
 
 * Boolean Network
 
- * network in SBML-qual file format
+ * network in the SBML-qual file format
  * "BN.sbml"
  * available on GitHub in the "data/output" directory as `"Ecoli_BN.sbml" <https://github.com/JanaMus/Augusta/blob/master/data/output/Ecoli_BN.sbml>`_.
 
 
 BN (selected genes) visualized in `Cell Collective platform: <https://research.cellcollective.org/?dashboard=true#/>`_
 
 .. image:: _static/Ecoli_BN.png
   :alt: Ecoli_BN_visualized
 
 
 
-Real data
+Whole-genome data
 ^^^^^^^^^^^^
-Real data are made by dataset of *Clostridium beijerinckii* NRL B-598 bacterium whole genome.
+The dataset consists of *Clostridium beijerinckii* NRL B-598 bacterium whole genome.
 
 Input files
 """""""""""""
 
 * **count table** file
 
-We will use the file we processed from the RNA-Seq dataset (available from the NCBI Sequence Read Archive (SRA) under the accession `SRP033480 <https://trace.ncbi.nlm.nih.gov/Traces/index.html?view=study&acc=SRP033480>`_; replicates B1 - B6).
-The processed count table file is available on GitHub in the "data" directory as `"Cbeijerinckii.csv" <https://github.com/JanaMus/Augusta/blob/master/data/Cbeijerinckii.csv>`_.
+We will use the file we processed from the RNA-Seq dataset (available from the NCBI Sequence Read Archive (SRA) under the accession `SRP033480 <https://trace.ncbi.nlm.nih.gov/Traces/index.html?view=study&acc=SRP033480>`_; replicates B1 - B6). We generated and normalized the count table by R´s Rsubread and DESeq2 libraries.
+The processed count table is available on GitHub in the "data" directory as `"Cbeijerinckii.csv" <https://github.com/JanaMus/Augusta/blob/master/data/Cbeijerinckii.csv>`_.
 
 
 * **GenBank** file
 
 We will use *C. beijerinckii* NRL B-598 genome available from NCBI Nucleotide database under the accession `CP011966.3 <https://www.ncbi.nlm.nih.gov/nuccore/CP011966.3>`_.
 The GenBank file can be downloaded in the GenBank full format. Otherwise,
 it is also available on GitHub in the "data" directory as `"Cbeijerinckii.gb" <https://github.com/JanaMus/Augusta/blob/master/data/Cbeijerinckii.gb>`_.
 
 
 Usage example
 """""""""""""
 Below is provided an example of the main function for generating GRN and BN. See :ref:`Usage` for further available functions.
 
-*Note: input files must be in the current directory or full path must be provided.*
+*Note: input files must be in the current directory or a full path must be provided.*
 
 .. code-block:: python
 
-   >>> Augusta.RNASeq_to_SBML(count_table_input = 'Cbeijerinckii.csv', promoter_length = 1000, genbank_file_input = 'Cbeijerinckii.gb', normalization_type = 'TPM')
+   >>> Augusta.RNASeq_to_BN(count_table_input = 'Cbeijerinckii.csv', promoter_length = 1000, genbank_file_input = 'Cbeijerinckii.gb', normalization_type = None, motifs_max_time = 300)
 
    Count table uploaded.
    GenBank uploaded.
-   Count table normalization done.
    Mutual information computation...
    Mutual information computation done.
    Motifs search...
    Motifs search done.
    Synonym organism names search...
    Synonym genes names search...
    Synonym names search done.
    No data searched in interaction databases.
    GRN stored as "GRN.csv".
    Cell Collective database search done.
    Boolean network stored as "BN.sbml".
 
 
-The computation should be done in approximately two days, depending on the specific machine.
+The computation should be done in several days, depending on the specific machine.
 
 
 Output files
 """""""""""""
 The files are stored in the generated "output" directory.
 
 * transcription motifs as "discovered_motifs.sto"
```

### Comparing `Augusta-1.0.3/docs/Installation.rst` & `Augusta-1.0.4/docs/Installation.rst`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/Makefile` & `Augusta-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/User guide.rst` & `Augusta-1.0.4/docs/User guide.rst`

 * *Files 12% similar despite different names*

```diff
@@ -56,41 +56,49 @@
  * examples: `"data" directory <https://github.com/JanaMus/Augusta/tree/master/data>`_ on GitHub or :ref:`Examples`)
 
 
 * **promoter length** parameter
 
  * *promoter_length*
  * optional, default: 1000 bp
+ * The length of a sequence in which a TFBM (transcription factor binding motif) is searched. E.g. promoter_length=1000 means that the sequence 1000 bp upstream of a gene is taken.
+
+
+* **maximum time for a TFMB search** parameter
+
+ * *motifs_max_time*
+ * optional, default: 180 s
+ * Maximum time in seconds to search TFBM for individual TF using MEME Suite. The recommended time by MEME Suite is 180 seconds, but it may take longer for large genomes. If the search is terminated due to timeout, a message will be displayed and the parameter should be extended.
 
 * **Gene Regulatory Network** file
 
  * *GRN_input*
- * Adjacency matrix NxN; N = genes
+ * Adjacency matrix NxN; N = number of genes; TF = transcription factor (regulator); TG = target (regulated) gene
  * CSV file format
  * examples: Table 2 or `"data" directory <https://github.com/JanaMus/Augusta/tree/master/data>`_ on GitHub
 
 .. list-table:: Table 2: GRN example
    :widths: 20 20 20 20
    :header-rows: 1
    :stub-columns: 1
    :align: center
 
    * -
-     - Gene 1
-     - Gene 2
-     - Gene 3
-   * - Gene 1
+     - TF 1
+     - TF 2
+     - TF 3
+   * - TG 1
      - 0
      - 1
      - -1
-   * - Gene 2
+   * - TG 2
      - 1
      - 0
      - 0
-   * - Gene 3
+   * - TG 3
      - 1
      - -1
      - 0
 
 
 * **Add database information** parameter
 
@@ -109,74 +117,76 @@
 
    > python3
    >>> import Augusta
    
    
 GRN and BN inference using RNA-Seq
 """"""""""""""""""""""""""""""""""""""""""""""""""""""""
-`RNASeq_to_SBML` is the main function for inferring both networks using RNA-Seq dataset as an input.
+`RNASeq_to_BN` is the main function for inferring both networks (GRN and BN) using RNA-Seq dataset as an input.
 
 Usage:
 
 .. code-block:: python
 
-   >>> Augusta.RNASeq_to_SBML(count_table_input, promoter_length, genbank_file_input, normalization_type)
+   >>> Augusta.RNASeq_to_BN(count_table_input, promoter_length, genbank_file_input, normalization_type, motifs_max_time)
 
 
 *Note: count_table_input is the only indispensable input, the remaining ones are optional.*
-*Not providing GenBank file results in only inferring GRN by computing mutual information. Further steps such as verification and BN inference would be skipped.*
+*Not providing GenBank file results in only inferring GRN by computing mutual information. Further steps such as count table normalization, GRN validation (TFBM and DBs search), and Cell Collective DB search would be skipped.*
 
 
 GRN inference using RNA-Seq
 """"""""""""""""""""""""""""
 `RNASeq_to_GRN` is the function for inferring only the Gene Regulatory Network using RNA-Seq dataset as an input.
 
 Usage:
 
 .. code-block:: python
 
-   >>> GRN = Augusta.RNASeq_to_GRN(count_table_input, promoter_length, genbank_file_input, normalization_type)
+   >>> Augusta.RNASeq_to_GRN(count_table_input, promoter_length, genbank_file_input, normalization_type, motifs_max_time)
 
 *Note: count_table_input is the only indispensable input, the remaining ones are optional.*
-*Not providing GenBank file results in only inferring GRN by computing mutual information. Further steps such as verification and BN inference would be skipped.*
+*Not providing GenBank file results in only inferring GRN by computing mutual information. Further steps such as count table normalization, GRN validation (TFBM and DBs search) would be skipped.*
 
 
 BN inference using GRN
 """""""""""""""""""""""
-`GRN_toBN` is the function for inferring the Boolean Network (BN) using the Gene Regulatory Network (GRN) file as an input.
+`GRN_to_BN` is the function for inferring the Boolean Network (BN) using the Gene Regulatory Network (GRN) file as an input.
 
 Usage:
 
 .. code-block:: python
 
-   >>> Augusta.GRNtoBN(GRN_input, promoter_length, genbank_file_input, add_dbs_info)
+   >>> Augusta.GRN_to_BN(GRN_input, promoter_length, genbank_file_input, add_dbs_info)
 
 
-*Note: GRN_input is the only indispensable input, the remaining ones are optional. Not providing GenBank file and/or not setting add_dbs_info only results in a GRN to BN conversion. Cell Collective database would not be searched.*
+*Note: GRN_input is the only indispensable input, the remaining ones are optional. Not providing GenBank file and/or not setting add_dbs_info only results in a GRN to BN conversion. CC DB would not be searched.*
 
 
 
 Outputs
 ^^^^^^^^
 All output files are stored in generated "output" directory.
-During motif search is moreover generated temporary file "temporary_coreg_seq.fasta" which is deleted at the end of the verification process.
+During motif search, the temporary file "temporary_coreg_seq.fasta" is generated and deleted at the end of the verification process.
 
 * Gene Regulatory Network
 
  * adjancency matrix in CSV file format
+ * rows: TFs (trascription factors / regulators), cols: TGs (target / regulated genes)
  * "GRN.csv"
 
 * Boolean Network
 
  * SBML-qual file format
  * "BN.sbml"
+ * *Note: GRN is primarily converted to the temporary file "BN.txt". If memory is sufficient, the "BN.txt" is converted to "BN.sbml". Otherwise, "BN.txt" is the final output.*
 
-* transcription motifs
+* motifs
 
- * all motifs discovered in the genome assigned to their transcription factor
+ * all TFBM discovered in the genome assigned to their transcription factor
  * Stockholm file format
  * "discovered_motifs.sto"
 
 * genes interactions
 
  * all interactions searched across databases stored as "DBs_interactions_list.csv"
  * uncertain interactions stored as "DBs_interactions_uncertain.csv" (i.e. the same gene pair has different interaction type in different DBs)
```

### Comparing `Augusta-1.0.3/docs/_static/Augusta_logo.png` & `Augusta-1.0.4/docs/_static/Augusta_logo.png`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/_static/Ecoli_BN.png` & `Augusta-1.0.4/docs/_static/Ecoli_BN.png`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/_static/Ecoli_GRN.png` & `Augusta-1.0.4/docs/_static/Ecoli_GRN.png`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/_static/pipeline.png` & `Augusta-1.0.4/docs/_static/pipeline.png`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/conf.py` & `Augusta-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/index.rst` & `Augusta-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/docs/make.bat` & `Augusta-1.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Augusta-1.0.3/setup.py` & `Augusta-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read_requirements(fname):
     with open(fname, 'r', encoding='utf-8') as file:
         return [line.rstrip() for line in file]
 
 setup(
     name='Augusta',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     url='https://github.com/JanaMus/Augusta',
     license='MIT',
     author='Jana Musilova, Zdenek Vafek, Karel Sedlar',
     author_email='musilovajana@vut.cz',
     description='Python package for inference of the gene regulatory network and the boolean network using RNA-Seq data.',
     long_description=long_description,
```

