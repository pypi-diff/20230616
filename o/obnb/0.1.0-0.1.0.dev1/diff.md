# Comparing `tmp/obnb-0.1.0.tar.gz` & `tmp/obnb-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obnb-0.1.0.tar", last modified: Fri Jun 16 18:54:28 2023, max compression
+gzip compressed data, was "obnb-0.1.0.dev1.tar", last modified: Thu Jun  8 17:27:17 2023, max compression
```

## Comparing `obnb-0.1.0.tar` & `obnb-0.1.0.dev1.tar`

### file list

```diff
@@ -1,140 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.457131 obnb-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 18:54:15.000000 obnb-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-06-16 18:54:28.457131 obnb-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-16 18:54:15.000000 obnb-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-16 18:54:15.000000 obnb-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:54:28.457131 obnb-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:54:15.000000 obnb-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.441131 obnb-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.441131 obnb-0.1.0/src/obnb/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.445131 obnb-0.1.0/src/obnb/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/config/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.445131 obnb-0.1.0/src/obnb/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.445131 obnb-0.1.0/src/obnb/data/annotated_ontology/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotated_ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotated_ontology/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotated_ontology/diseases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotated_ontology/disgenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotated_ontology/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotated_ontology/hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.445131 obnb-0.1.0/src/obnb/data/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotation/diseases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotation/disgenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotation/gene_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/annotation/human_phenotype_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.445131 obnb-0.1.0/src/obnb/data/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/experimental/alevinfry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.449131 obnb-0.1.0/src/obnb/data/network/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/biogrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/bioplex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/comppi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/consensuspathdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/funcoup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/hippie.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/humanbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/humannet.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/humap.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/huri.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/omnipath.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/pcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/proteomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/signor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/network/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.449131 obnb-0.1.0/src/obnb/data/ontology/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/ontology/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/ontology/gene_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/data/ontology/mondo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.449131 obnb-0.1.0/src/obnb/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/dataset/dataset_dgl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/dataset/dataset_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.449131 obnb-0.1.0/src/obnb/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/ext/grape.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/ext/orbital_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/ext/pecanpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/ext/sknetwork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.449131 obnb-0.1.0/src/obnb/feature/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/feature/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/feature/multifeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/feature/singlefeat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.453131 obnb-0.1.0/src/obnb/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/graph/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    33817 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/graph/sparse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.453131 obnb-0.1.0/src/obnb/label/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25241 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.453131 obnb-0.1.0/src/obnb/label/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/existence_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/negative_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/nonred.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/pairwise_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/filters/value_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.453131 obnb-0.1.0/src/obnb/label/split/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/split/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/split/holdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/label/split/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.453131 obnb-0.1.0/src/obnb/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/metric/graphgym_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/metric/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.453131 obnb-0.1.0/src/obnb/model/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model/label_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.453131 obnb-0.1.0/src/obnb/model_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model_trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model_trainer/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model_trainer/graphgym.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model_trainer/label_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/model_trainer/supervised_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.457131 obnb-0.1.0/src/obnb/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7224 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/cx_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/download.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16899 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/idhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10688 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/registers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1717 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-16 18:54:15.000000 obnb-0.1.0/src/obnb/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.445131 obnb-0.1.0/src/obnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-06-16 18:54:28.000000 obnb-0.1.0/src/obnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-16 18:54:28.000000 obnb-0.1.0/src/obnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:54:28.000000 obnb-0.1.0/src/obnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:54:28.000000 obnb-0.1.0/src/obnb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-16 18:54:28.000000 obnb-0.1.0/src/obnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 18:54:28.000000 obnb-0.1.0/src/obnb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:54:28.457131 obnb-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-16 18:54:15.000000 obnb-0.1.0/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-16 18:54:15.000000 obnb-0.1.0/test/test_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43045 2023-06-16 18:54:15.000000 obnb-0.1.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-16 18:54:15.000000 obnb-0.1.0/test/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-16 18:54:15.000000 obnb-0.1.0/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-16 18:54:15.000000 obnb-0.1.0/test/test_wrapper.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.990226 obnb-0.1.0.dev1/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1065 2021-11-16 18:51:22.000000 obnb-0.1.0.dev1/LICENSE
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     8894 2023-06-08 17:27:17.989388 obnb-0.1.0.dev1/PKG-INFO
+-rw-------   0 liurenmi (790872) cmse      (2362)     7847 2023-06-08 16:23:42.000000 obnb-0.1.0.dev1/README.md
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2618 2023-06-08 16:12:13.000000 obnb-0.1.0.dev1/pyproject.toml
+-rw-rw----   0 liurenmi (790872) cmse      (2362)       38 2023-06-08 17:27:17.990546 obnb-0.1.0.dev1/setup.cfg
+-rw-rw----   0 liurenmi (790872) cmse      (2362)       38 2022-05-15 11:19:44.000000 obnb-0.1.0.dev1/setup.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.471724 obnb-0.1.0.dev1/src/
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.523658 obnb-0.1.0.dev1/src/obnb/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      439 2023-06-08 15:57:17.000000 obnb-0.1.0.dev1/src/obnb/__init__.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.545227 obnb-0.1.0.dev1/src/obnb/config/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1123 2023-06-08 16:03:17.000000 obnb-0.1.0.dev1/src/obnb/config/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1458 2023-06-08 15:59:06.000000 obnb-0.1.0.dev1/src/obnb/config/logger_config.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.548821 obnb-0.1.0.dev1/src/obnb/data/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2024 2023-06-08 15:56:40.000000 obnb-0.1.0.dev1/src/obnb/data/__init__.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.593517 obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1003 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     4077 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2749 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/diseases.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2513 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/disgenet.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2198 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/go.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1620 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/hpo.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.617129 obnb-0.1.0.dev1/src/obnb/data/annotation/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      452 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/annotation/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1556 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/annotation/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5234 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/annotation/diseases.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     6070 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/annotation/disgenet.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     4627 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/annotation/gene_ontology.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2605 2023-06-08 17:22:31.000000 obnb-0.1.0.dev1/src/obnb/data/annotation/human_phenotype_ontology.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)    14914 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/base.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.620863 obnb-0.1.0.dev1/src/obnb/data/experimental/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      351 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/experimental/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3311 2023-06-08 16:23:42.000000 obnb-0.1.0.dev1/src/obnb/data/experimental/alevinfry.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.723115 obnb-0.1.0.dev1/src/obnb/data/network/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1060 2023-06-08 15:55:51.000000 obnb-0.1.0.dev1/src/obnb/data/network/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     7144 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/network/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      924 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/biogrid.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      932 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/bioplex.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3782 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/network/comppi.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5202 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/network/consensuspathdb.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1198 2023-06-08 16:03:17.000000 obnb-0.1.0.dev1/src/obnb/data/network/funcoup.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1154 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/hippie.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      831 2023-06-08 16:03:17.000000 obnb-0.1.0.dev1/src/obnb/data/network/humanbase.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3345 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/humannet.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      853 2023-06-08 16:03:17.000000 obnb-0.1.0.dev1/src/obnb/data/network/humap.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      901 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/huri.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      870 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/intact.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     4034 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/data/network/omnipath.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      934 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/pcnet.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1030 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/network/proteomehd.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1514 2023-06-08 16:01:58.000000 obnb-0.1.0.dev1/src/obnb/data/network/signor.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1067 2023-06-08 16:03:17.000000 obnb-0.1.0.dev1/src/obnb/data/network/string.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.733012 obnb-0.1.0.dev1/src/obnb/data/ontology/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      189 2023-06-08 15:56:40.000000 obnb-0.1.0.dev1/src/obnb/data/ontology/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2062 2023-06-08 16:02:16.000000 obnb-0.1.0.dev1/src/obnb/data/ontology/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      408 2023-06-08 15:56:40.000000 obnb-0.1.0.dev1/src/obnb/data/ontology/gene_ontology.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      471 2023-06-08 16:01:57.000000 obnb-0.1.0.dev1/src/obnb/data/ontology/mondo.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)    10366 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/dataset.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2958 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/dataset_pyg.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      693 2022-10-02 23:19:04.000000 obnb-0.1.0.dev1/src/obnb/exception.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.742674 obnb-0.1.0.dev1/src/obnb/ext/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)       48 2023-06-08 16:05:19.000000 obnb-0.1.0.dev1/src/obnb/ext/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     4175 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/ext/grape.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     6938 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/ext/orbital_features.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3264 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/ext/pecanpy.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1779 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/ext/sknetwork.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.776611 obnb-0.1.0.dev1/src/obnb/feature/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      166 2023-06-08 15:56:40.000000 obnb-0.1.0.dev1/src/obnb/feature/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     9381 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/feature/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5919 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/feature/multifeat.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      747 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/feature/singlefeat.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.827188 obnb-0.1.0.dev1/src/obnb/graph/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      289 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/graph/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     7609 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/graph/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     7794 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/graph/dense.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)    14616 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/graph/ontology.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)    32280 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/graph/sparse.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.833074 obnb-0.1.0.dev1/src/obnb/label/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      211 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/label/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)    25241 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/collection.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.879999 obnb-0.1.0.dev1/src/obnb/label/filters/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      939 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/label/filters/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3780 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/filters/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3461 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/label/filters/existence_filter.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3389 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/filters/negative_generator.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     6943 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/label/filters/nonred.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     4358 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/filters/pairwise_filter.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5315 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/filters/range_filter.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      722 2023-06-08 15:56:40.000000 obnb-0.1.0.dev1/src/obnb/label/filters/value_filter.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.890541 obnb-0.1.0.dev1/src/obnb/label/split/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      482 2023-06-08 15:56:40.000000 obnb-0.1.0.dev1/src/obnb/label/split/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5109 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/split/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     4743 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/split/holdout.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5732 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/label/split/partition.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.899075 obnb-0.1.0.dev1/src/obnb/metric/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      197 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/metric/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1017 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/metric/graphgym_metric.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3200 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/metric/standard.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.904128 obnb-0.1.0.dev1/src/obnb/model/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)       53 2022-09-05 17:56:57.000000 obnb-0.1.0.dev1/src/obnb/model/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5382 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/model/label_propagation.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.924279 obnb-0.1.0.dev1/src/obnb/model_trainer/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      376 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/model_trainer/__init__.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     7097 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/model_trainer/base.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     7613 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/model_trainer/gnn.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     9225 2023-06-08 16:08:45.000000 obnb-0.1.0.dev1/src/obnb/model_trainer/graphgym.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      740 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/model_trainer/label_propagation.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3292 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/model_trainer/supervised_learning.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1515 2023-06-08 15:58:16.000000 obnb-0.1.0.dev1/src/obnb/typing.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.972683 obnb-0.1.0.dev1/src/obnb/util/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)        0 2022-09-05 17:56:57.000000 obnb-0.1.0.dev1/src/obnb/util/__init__.py
+-rwxrwx---   0 liurenmi (790872) cmse      (2362)     6799 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/src/obnb/util/checkers.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)    13122 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/src/obnb/util/converter.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5444 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/src/obnb/util/cx_explorer.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     4196 2023-06-08 15:56:11.000000 obnb-0.1.0.dev1/src/obnb/util/dataset_constructors.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      819 2023-04-11 01:48:32.000000 obnb-0.1.0.dev1/src/obnb/util/deprecated.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     6010 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/src/obnb/util/download.py
+-rwxrwx---   0 liurenmi (790872) cmse      (2362)    16899 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/src/obnb/util/idhandler.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3003 2023-06-08 15:58:45.000000 obnb-0.1.0.dev1/src/obnb/util/logger.py
+-rwxrwx---   0 liurenmi (790872) cmse      (2362)    10688 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/src/obnb/util/parallel.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      331 2022-09-05 17:56:57.000000 obnb-0.1.0.dev1/src/obnb/util/path.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1382 2023-06-08 15:55:51.000000 obnb-0.1.0.dev1/src/obnb/util/registers.py
+-rwxrwx---   0 liurenmi (790872) cmse      (2362)     1717 2023-06-08 15:55:51.000000 obnb-0.1.0.dev1/src/obnb/util/timer.py
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.541399 obnb-0.1.0.dev1/src/obnb.egg-info/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     8894 2023-06-08 17:27:16.000000 obnb-0.1.0.dev1/src/obnb.egg-info/PKG-INFO
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     3456 2023-06-08 17:27:17.530430 obnb-0.1.0.dev1/src/obnb.egg-info/SOURCES.txt
+-rw-rw----   0 liurenmi (790872) cmse      (2362)        1 2023-06-08 17:27:16.000000 obnb-0.1.0.dev1/src/obnb.egg-info/dependency_links.txt
+-rw-rw----   0 liurenmi (790872) cmse      (2362)        1 2023-06-08 17:24:54.000000 obnb-0.1.0.dev1/src/obnb.egg-info/not-zip-safe
+-rw-rw----   0 liurenmi (790872) cmse      (2362)      413 2023-06-08 17:27:16.000000 obnb-0.1.0.dev1/src/obnb.egg-info/requires.txt
+-rw-rw----   0 liurenmi (790872) cmse      (2362)        5 2023-06-08 17:27:16.000000 obnb-0.1.0.dev1/src/obnb.egg-info/top_level.txt
+drwxrwx---   0 liurenmi (790872) cmse      (2362)        0 2023-06-08 17:27:17.984679 obnb-0.1.0.dev1/test/
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     5722 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/test/test_data.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     8196 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/test/test_dataset.py
+-rwxrwx---   0 liurenmi (790872) cmse      (2362)    43045 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/test/test_graph.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     1840 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/test/test_metric.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2736 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/test/test_model.py
+-rw-rw----   0 liurenmi (790872) cmse      (2362)     2910 2023-06-08 16:07:55.000000 obnb-0.1.0.dev1/test/test_wrapper.py
```

### Comparing `obnb-0.1.0/LICENSE` & `obnb-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/PKG-INFO` & `obnb-0.1.0.dev1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: obnb
-Version: 0.1.0
+Version: 0.1.0.dev1
 Summary: A Python toolkit for biological network learning evaluation
 Author-email: Remy Liu <liurenmi@msu.edu>
 License: MIT
-Project-URL: home, https://github.com/krishnanlab/obnb
-Project-URL: bug-tracker, https://github.com/krishnanlab/obnb/issues
+Project-URL: home, https://github.com/krishnanlab/NetworkLearningEval
+Project-URL: bug-tracker, https://github.com/krishnanlab/NetworkLearningEval/issues
 Keywords: Data Processing,Gene Classification,Machine Learning,Network Biology,Network Repositories
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
@@ -20,141 +20,142 @@
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: pyroe
 Provides-Extra: ext
 Provides-Extra: full
 License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/obnb.svg)](https://badge.fury.io/py/obnb)
-[![Documentation Status](https://readthedocs.org/projects/obnb/badge/?version=latest)](https://obnb.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/nleval.svg)](https://badge.fury.io/py/nleval)
+[![Documentation Status](https://readthedocs.org/projects/networklearningeval/badge/?version=latest)](https://networklearningeval.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-[![Tests](https://github.com/krishnanlab/obnb/actions/workflows/tests.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/tests.yml)
-[![Test Examples](https://github.com/krishnanlab/obnb/actions/workflows/examples.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/examples.yml)
-[![Test Data](https://github.com/krishnanlab/obnb/actions/workflows/test_data.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/test_data.yml)
+[![Tests](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/tests.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/tests.yml)
+[![Test Examples](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/examples.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/examples.yml)
+[![Test Data](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/test_data.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/test_data.yml)
 
 # Open Biomedical Network Benchmark
 
-The Open Biomedical Network Benchmark (OBNB) is a comprehensive resource for setting up benchmarking graph datasets using _biomedical networks_ and _gene annotations_.
-Our goal is to accelerate the adoption of advanced graph machine learning techniques, such as graph neural networks and graph embeddings, in network biology for gaining novel insights into genes' function, trait, and disease associations using biological networks.
-To make this adoption convenient, OBNB also provides dataset objects compatible with popular graph deep learning frameworks, including [PyTorch Geometric (PyG)](https://github.com/pyg-team/pytorch_geometric) and [Deep Graph Library (DGL)](https://github.com/dmlc/dgl).
-
-A comprehensive benchmarking study with a wide-range of graph neural networks and graph embedding methods on OBNB datasets can be found in our benchmarking repository [`obnbench`](https://github.com/krishnanlab/obnbench).
+## Installation
 
-## Package usage
+Clone the repository first and then install via `pip`
 
-### Construct default datasets
+```bash
+git clone https://github.com/krishnanlab/NetworkLearningEval && cd NetworkLearningEval
+pip install -e .
+```
 
-We provide a high-level dataset constructor to help users easily set up benchmarking graph datasets
-for a combination of network and label. In particular, the dataset will be set up with study-bias
-holdout split (6/2/2), where 60% of the most well-studied genes according to the number of
-associated PubMed publications are used for training, 20% of the least studied genes are used for
-testing, and the rest of the 20% genes are used for validation. For more customizable data loading
-and processing options, see the [customized dataset construction](#customized-dataset-construction)
-section below.
+The `-e` option means 'editable', i.e. no need to reinstall the library if you make changes to the source code.
+Feel free to not use the `-e` option and simply do `pip install .` if you do not plan on modifying the source code.
 
-```python
-from obnb.dataset import OpenBiomedNetBench
-from obnb.util.version import get_available_data_versions
+### Optional Pytorch Geometric installation
 
-root = "datasets"  # save dataset and cache under the datasets/ directory
-version = "current"  # use the last archived version
-# Optionally, set version to the specific data version number
-# Or, set version to "latest" to download the latest data from source and process it from scratch
+User need to install [Pytorch Geomtric](https://github.com/pyg-team/pytorch_geometric) to enable some GNN related features.
+To install PyG, first need to install [PyTorch](https://pytorch.org).
+For full details about installation instructions, visit the links above.
+Assuming the system has Python3.8 or above installed, with CUDA10.2, use the following to install both PyTorch and PyG.
 
-# Download and process network/label data. Use the adjacency matrix as the ML feature
-dataset = OpenBiomedNetBench(root=root, graph_name="BioGRID", label_name="DisGeNET",
-                             version=version, graph_as_feature=True, use_dense_graph=True)
+```bash
+conda install pytorch=1.12.1 torchvision cudatoolkit=10.2 -c pytorch
+pip install torch-geometric==2.0.4 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cu102.html
+```
 
-# Check the specific archive data version used
-print(dataset.version)
+### Quick install using the installation script
 
-# Check all available stable archive data versions
-print(get_available_data_versions())
+```bash
+source install.sh cu102  # other options are [cpu,cu113]
 ```
 
-Users can also load the dataset objects into ones that are compatible with PyG or DGL (see below).
+## Quick Demonstration
 
-#### PyG dataset
+### Construct default datasets
 
-```python
-from obnb.dataset import OpenBiomedNetBenchPyG
-dataset = OpenBiomedNetBenchPyG(root, "BioGRID", "DisGeNET")
-```
+We provide a high-level dataset constructor to help user effortlessly set up a ML-ready dataset
+for a combination of network and label. In particular, the dataset will be set up with study-bias
+holdout split (6/2/2), where 60% of the most well studied genes according to the number of
+associated PubMed publications are used for training, 20% of the least studied genes are used for
+testing, and rest of the 20% genes are used for validation. For more customizable data loading
+and processing options, see the [customized dataset construction](#customized-dataset-construction)
+section below.
 
-**Note**: requires installing PyG first (see [installation instructions](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html))
+```python
+from obnb.util.dataset_constructors import default_constructor
 
-#### DGL dataset
+root = "datasets"  # save dataset and cache under the datasets/ directory
+version = "nledata-v0.1.0-dev3"  # archive data version, use 'latest' to pull latest data from source instead
 
-```python
-from obnb.dataset import OpenBiomedNetBenchDGL
-dataset = OpenBiomedNetBenchDGL(root, "BioGRID", "DisGeNET")
+# Download and process network/label data. Use the adjacency matrix as the ML feature
+dataset = default_constructor(root=root, version=version, graph_name="BioGRID", label_name="DisGeNET",
+                              graph_as_feature=True, use_dense_graph=True)
 ```
 
-**Note**: requires installing DGL first (see [installation instructions](https://www.dgl.ai/pages/start.html))
-
 ### Evaluating standard models
 
 Evaluation of simple machine learning methods such as logistic regression and label propagation
-can be done easily using the trainer objects.
+can be done easily using the trainer objects. The trainer objects take a dictionary of metrics
+as input for evaluating the models' performances, and can be set up as follows.
 
 ```python
+from obnb.metric import auroc
 from obnb.model_trainer import SupervisedLearningTrainer, LabelPropagationTrainer
 
-sl_trainer = SupervisedLearningTrainer()
-lp_trainer = LabelPropagationTrainer()
+metrics = {"auroc": auroc}  # use AUROC as our default evaluation metric
+sl_trainer = SupervisedLearningTrainer(metrics)
+lp_trainer = LabelPropagationTrainer(metrics)
 ```
 
-Then, use the `fit_and_eval` method of the trainer to evaluate a given ML model over all tasks
+Then, use the `eval_multi_ovr` method of the trainer to evaluate a given ML model over all tasks
 in a one-vs-rest setting.
 
 ```python
 from sklearn.linear_model import LogisticRegression
 from obnb.model.label_propagation import OneHopPropagation
 
 # Initialize models
 sl_mdl = LogisticRegression(penalty="l2", solver="lbfgs")
 lp_mdl = OneHopPropagation()
 
 # Evaluate the models over all tasks
-sl_results = sl_trainer.fit_and_eval(sl_mdl, dataset)
-lp_results = lp_trainer.fit_and_eval(lp_mdl, dataset)
+sl_results = sl_trainer.eval_multi_ovr(sl_mdl, dataset)
+lp_results = lp_trainer.eval_multi_ovr(lp_mdl, dataset)
 ```
 
 ### Evaluating GNN models
 
 Training and evaluation of Graph Neural Network (GNN) models can be done in a very similar fashion.
 
 ```python
 from torch_geometric.nn import GCN
 from obnb.model_trainer.gnn import SimpleGNNTrainer
 
-# Use 1-dimensional trivial node feature by default
-dataset = OpenBiomedNetBench(root=root, graph_name="BioGRID", label_name="DisGeNET", version=version)
+# Use 1-dimensional trivial node feature
+dataset = default_constructor(root=root, version=version, graph_name="BioGRID", label_name="DisGeNET")
 
 # Train and evaluate a GCN
 gcn_mdl = GCN(in_channels=1, hidden_channels=64, num_layers=5, out_channels=n_tasks)
-gcn_trainer = SimpleGNNTrainer(device="cuda", metric_best="apop")
+gcn_trainer = SimpleGNNTrainer(metrics, device="cuda", metric_best="auroc")
 gcn_results = gcn_trainer.train(gcn_mdl, dataset)
 ```
 
 ### Customized dataset construction
 
 #### Load network and labels
 
 ```python
 from obnb import data
 
+root = "datasets"  # save dataset and cache under the datasets/ directory
+
 # Load processed BioGRID data from archive.
-g = data.BioGRID(root, version=version)
+# Alternatively, set version="latest" to get and process the newest data from scratch.
+g = data.BioGRID(root, version="nledata-v0.1.0-dev3")
 
 # Load DisGeNET gene set collections.
-lsc = data.DisGeNET(root, version=version)
+lsc = data.DisGeNET(root, version="latest")
 ```
 
 #### Setting up data and splits
 
 ```python
 from obnb.util.converter import GenePropertyConverter
 from obnb.label.split import RatioHoldout
@@ -183,35 +184,30 @@
 #### Combine into dataset
 
 ```python
 from obnb import Dataset
 dataset = Dataset(graph=g, feature=g.to_dense_graph().to_feature(), label=lsc, splitter=splitter)
 ```
 
-## Installation
+## Data preparation and releasing notes
 
-OBNB can be installed easily via pip from [PyPI](https://pypi.org/project/obnb/):
+First, bump data version in `__init__.py` to the next data release version, e.g., `nledata-v0.1.0 -> nledata-v0.1.1-dev`.
+Then, download and process all latest data by running
 
 ```bash
-pip install obnb
+python script/release_data.py
 ```
 
-### Install with extension modules (optional)
+By default, the data ready to be uploaded (e.g., to [Zenodo](zenodo.org)) is saved under `data_release/archived`.
+After some necessary inspection and checking, if everything looks good, upload and publish the new archived data.
 
-OBNB provides interfaces with several other packages for network feature extractions, such as
-[PecanPy](https://github.com/krishnanlab/PecanPy) and [GraPE](https://github.com/AnacletoLAB/grape).
-To enable those extensions, install `obnb` with the `ext` extra option enabled:
+**Note:** `dev` data should be uploaded to the [sandbox](https://sandbox.zenodo.org/record/1097545#.YxYrqezMJzV) instead.
 
-```bash
-pip install obnb[ext]
-```
+Check items:
 
-### Install graph deep learning libraries (optional)
+- [ ] Update `__data_version__`
+- [ ] Run [`release_data.py`](script/release_data.py)
+- [ ] Upload archived data to Zenodo (be sure to edit the data version there also)
+- [ ] Update url dict in config (will improve in the future to get info from Zenodo directly)
+- [ ] Update network stats in data [test](test/test_data.py)
 
-Follow installation instructions for [PyG](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html) or [DGL](https://www.dgl.ai/pages/start.html) to set up the graph deep learning library of your choice.
-
-Alternatively, we also provide an [installation script](install.sh) that helps you installthe graph deep-learning dependencies in a new conda environment `obnb`:
-
-```bash
-git clone https://github.com/krishnanlab/obnb && cd obnb
-source install.sh cu117  # other options are [cpu,cu118]
-```
+Finally, commit and push the bumped version.
```

### Comparing `obnb-0.1.0/README.md` & `obnb-0.1.0.dev1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,134 +1,135 @@
-[![PyPI version](https://badge.fury.io/py/obnb.svg)](https://badge.fury.io/py/obnb)
-[![Documentation Status](https://readthedocs.org/projects/obnb/badge/?version=latest)](https://obnb.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/nleval.svg)](https://badge.fury.io/py/nleval)
+[![Documentation Status](https://readthedocs.org/projects/networklearningeval/badge/?version=latest)](https://networklearningeval.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-[![Tests](https://github.com/krishnanlab/obnb/actions/workflows/tests.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/tests.yml)
-[![Test Examples](https://github.com/krishnanlab/obnb/actions/workflows/examples.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/examples.yml)
-[![Test Data](https://github.com/krishnanlab/obnb/actions/workflows/test_data.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/test_data.yml)
+[![Tests](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/tests.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/tests.yml)
+[![Test Examples](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/examples.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/examples.yml)
+[![Test Data](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/test_data.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/test_data.yml)
 
 # Open Biomedical Network Benchmark
 
-The Open Biomedical Network Benchmark (OBNB) is a comprehensive resource for setting up benchmarking graph datasets using _biomedical networks_ and _gene annotations_.
-Our goal is to accelerate the adoption of advanced graph machine learning techniques, such as graph neural networks and graph embeddings, in network biology for gaining novel insights into genes' function, trait, and disease associations using biological networks.
-To make this adoption convenient, OBNB also provides dataset objects compatible with popular graph deep learning frameworks, including [PyTorch Geometric (PyG)](https://github.com/pyg-team/pytorch_geometric) and [Deep Graph Library (DGL)](https://github.com/dmlc/dgl).
-
-A comprehensive benchmarking study with a wide-range of graph neural networks and graph embedding methods on OBNB datasets can be found in our benchmarking repository [`obnbench`](https://github.com/krishnanlab/obnbench).
+## Installation
 
-## Package usage
+Clone the repository first and then install via `pip`
 
-### Construct default datasets
+```bash
+git clone https://github.com/krishnanlab/NetworkLearningEval && cd NetworkLearningEval
+pip install -e .
+```
 
-We provide a high-level dataset constructor to help users easily set up benchmarking graph datasets
-for a combination of network and label. In particular, the dataset will be set up with study-bias
-holdout split (6/2/2), where 60% of the most well-studied genes according to the number of
-associated PubMed publications are used for training, 20% of the least studied genes are used for
-testing, and the rest of the 20% genes are used for validation. For more customizable data loading
-and processing options, see the [customized dataset construction](#customized-dataset-construction)
-section below.
+The `-e` option means 'editable', i.e. no need to reinstall the library if you make changes to the source code.
+Feel free to not use the `-e` option and simply do `pip install .` if you do not plan on modifying the source code.
 
-```python
-from obnb.dataset import OpenBiomedNetBench
-from obnb.util.version import get_available_data_versions
+### Optional Pytorch Geometric installation
 
-root = "datasets"  # save dataset and cache under the datasets/ directory
-version = "current"  # use the last archived version
-# Optionally, set version to the specific data version number
-# Or, set version to "latest" to download the latest data from source and process it from scratch
+User need to install [Pytorch Geomtric](https://github.com/pyg-team/pytorch_geometric) to enable some GNN related features.
+To install PyG, first need to install [PyTorch](https://pytorch.org).
+For full details about installation instructions, visit the links above.
+Assuming the system has Python3.8 or above installed, with CUDA10.2, use the following to install both PyTorch and PyG.
 
-# Download and process network/label data. Use the adjacency matrix as the ML feature
-dataset = OpenBiomedNetBench(root=root, graph_name="BioGRID", label_name="DisGeNET",
-                             version=version, graph_as_feature=True, use_dense_graph=True)
+```bash
+conda install pytorch=1.12.1 torchvision cudatoolkit=10.2 -c pytorch
+pip install torch-geometric==2.0.4 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cu102.html
+```
 
-# Check the specific archive data version used
-print(dataset.version)
+### Quick install using the installation script
 
-# Check all available stable archive data versions
-print(get_available_data_versions())
+```bash
+source install.sh cu102  # other options are [cpu,cu113]
 ```
 
-Users can also load the dataset objects into ones that are compatible with PyG or DGL (see below).
+## Quick Demonstration
 
-#### PyG dataset
+### Construct default datasets
 
-```python
-from obnb.dataset import OpenBiomedNetBenchPyG
-dataset = OpenBiomedNetBenchPyG(root, "BioGRID", "DisGeNET")
-```
+We provide a high-level dataset constructor to help user effortlessly set up a ML-ready dataset
+for a combination of network and label. In particular, the dataset will be set up with study-bias
+holdout split (6/2/2), where 60% of the most well studied genes according to the number of
+associated PubMed publications are used for training, 20% of the least studied genes are used for
+testing, and rest of the 20% genes are used for validation. For more customizable data loading
+and processing options, see the [customized dataset construction](#customized-dataset-construction)
+section below.
 
-**Note**: requires installing PyG first (see [installation instructions](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html))
+```python
+from obnb.util.dataset_constructors import default_constructor
 
-#### DGL dataset
+root = "datasets"  # save dataset and cache under the datasets/ directory
+version = "nledata-v0.1.0-dev3"  # archive data version, use 'latest' to pull latest data from source instead
 
-```python
-from obnb.dataset import OpenBiomedNetBenchDGL
-dataset = OpenBiomedNetBenchDGL(root, "BioGRID", "DisGeNET")
+# Download and process network/label data. Use the adjacency matrix as the ML feature
+dataset = default_constructor(root=root, version=version, graph_name="BioGRID", label_name="DisGeNET",
+                              graph_as_feature=True, use_dense_graph=True)
 ```
 
-**Note**: requires installing DGL first (see [installation instructions](https://www.dgl.ai/pages/start.html))
-
 ### Evaluating standard models
 
 Evaluation of simple machine learning methods such as logistic regression and label propagation
-can be done easily using the trainer objects.
+can be done easily using the trainer objects. The trainer objects take a dictionary of metrics
+as input for evaluating the models' performances, and can be set up as follows.
 
 ```python
+from obnb.metric import auroc
 from obnb.model_trainer import SupervisedLearningTrainer, LabelPropagationTrainer
 
-sl_trainer = SupervisedLearningTrainer()
-lp_trainer = LabelPropagationTrainer()
+metrics = {"auroc": auroc}  # use AUROC as our default evaluation metric
+sl_trainer = SupervisedLearningTrainer(metrics)
+lp_trainer = LabelPropagationTrainer(metrics)
 ```
 
-Then, use the `fit_and_eval` method of the trainer to evaluate a given ML model over all tasks
+Then, use the `eval_multi_ovr` method of the trainer to evaluate a given ML model over all tasks
 in a one-vs-rest setting.
 
 ```python
 from sklearn.linear_model import LogisticRegression
 from obnb.model.label_propagation import OneHopPropagation
 
 # Initialize models
 sl_mdl = LogisticRegression(penalty="l2", solver="lbfgs")
 lp_mdl = OneHopPropagation()
 
 # Evaluate the models over all tasks
-sl_results = sl_trainer.fit_and_eval(sl_mdl, dataset)
-lp_results = lp_trainer.fit_and_eval(lp_mdl, dataset)
+sl_results = sl_trainer.eval_multi_ovr(sl_mdl, dataset)
+lp_results = lp_trainer.eval_multi_ovr(lp_mdl, dataset)
 ```
 
 ### Evaluating GNN models
 
 Training and evaluation of Graph Neural Network (GNN) models can be done in a very similar fashion.
 
 ```python
 from torch_geometric.nn import GCN
 from obnb.model_trainer.gnn import SimpleGNNTrainer
 
-# Use 1-dimensional trivial node feature by default
-dataset = OpenBiomedNetBench(root=root, graph_name="BioGRID", label_name="DisGeNET", version=version)
+# Use 1-dimensional trivial node feature
+dataset = default_constructor(root=root, version=version, graph_name="BioGRID", label_name="DisGeNET")
 
 # Train and evaluate a GCN
 gcn_mdl = GCN(in_channels=1, hidden_channels=64, num_layers=5, out_channels=n_tasks)
-gcn_trainer = SimpleGNNTrainer(device="cuda", metric_best="apop")
+gcn_trainer = SimpleGNNTrainer(metrics, device="cuda", metric_best="auroc")
 gcn_results = gcn_trainer.train(gcn_mdl, dataset)
 ```
 
 ### Customized dataset construction
 
 #### Load network and labels
 
 ```python
 from obnb import data
 
+root = "datasets"  # save dataset and cache under the datasets/ directory
+
 # Load processed BioGRID data from archive.
-g = data.BioGRID(root, version=version)
+# Alternatively, set version="latest" to get and process the newest data from scratch.
+g = data.BioGRID(root, version="nledata-v0.1.0-dev3")
 
 # Load DisGeNET gene set collections.
-lsc = data.DisGeNET(root, version=version)
+lsc = data.DisGeNET(root, version="latest")
 ```
 
 #### Setting up data and splits
 
 ```python
 from obnb.util.converter import GenePropertyConverter
 from obnb.label.split import RatioHoldout
@@ -157,35 +158,30 @@
 #### Combine into dataset
 
 ```python
 from obnb import Dataset
 dataset = Dataset(graph=g, feature=g.to_dense_graph().to_feature(), label=lsc, splitter=splitter)
 ```
 
-## Installation
+## Data preparation and releasing notes
 
-OBNB can be installed easily via pip from [PyPI](https://pypi.org/project/obnb/):
+First, bump data version in `__init__.py` to the next data release version, e.g., `nledata-v0.1.0 -> nledata-v0.1.1-dev`.
+Then, download and process all latest data by running
 
 ```bash
-pip install obnb
+python script/release_data.py
 ```
 
-### Install with extension modules (optional)
+By default, the data ready to be uploaded (e.g., to [Zenodo](zenodo.org)) is saved under `data_release/archived`.
+After some necessary inspection and checking, if everything looks good, upload and publish the new archived data.
 
-OBNB provides interfaces with several other packages for network feature extractions, such as
-[PecanPy](https://github.com/krishnanlab/PecanPy) and [GraPE](https://github.com/AnacletoLAB/grape).
-To enable those extensions, install `obnb` with the `ext` extra option enabled:
+**Note:** `dev` data should be uploaded to the [sandbox](https://sandbox.zenodo.org/record/1097545#.YxYrqezMJzV) instead.
 
-```bash
-pip install obnb[ext]
-```
+Check items:
 
-### Install graph deep learning libraries (optional)
+- [ ] Update `__data_version__`
+- [ ] Run [`release_data.py`](script/release_data.py)
+- [ ] Upload archived data to Zenodo (be sure to edit the data version there also)
+- [ ] Update url dict in config (will improve in the future to get info from Zenodo directly)
+- [ ] Update network stats in data [test](test/test_data.py)
 
-Follow installation instructions for [PyG](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html) or [DGL](https://www.dgl.ai/pages/start.html) to set up the graph deep learning library of your choice.
-
-Alternatively, we also provide an [installation script](install.sh) that helps you installthe graph deep-learning dependencies in a new conda environment `obnb`:
-
-```bash
-git clone https://github.com/krishnanlab/obnb && cd obnb
-source install.sh cu117  # other options are [cpu,cu118]
-```
+Finally, commit and push the bumped version.
```

### Comparing `obnb-0.1.0/pyproject.toml` & `obnb-0.1.0.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "obnb"
-version = "0.1.0"
+version = "0.1.0-dev1"
 description = "A Python toolkit for biological network learning evaluation"
 readme = "README.md"
 
 authors = [
     {name = "Remy Liu", email = "liurenmi@msu.edu"},
 ]
 license = {text = "MIT"}
@@ -35,24 +35,22 @@
 dependencies = [
     "matplotlib",
     "mygene",
     "ndex2",
     "numpy>=1.20.0",
     "pyOpenSSL>=23.1.1",
     "pyyaml",
-    "requests",
     "scikit-learn>=1.0.0",
     "scipy",
     "tqdm",
-    "outdated",
 ]
 
 [project.urls]
-home = "https://github.com/krishnanlab/obnb"
-bug-tracker = "https://github.com/krishnanlab/obnb/issues"
+home = "https://github.com/krishnanlab/NetworkLearningEval"
+bug-tracker = "https://github.com/krishnanlab/NetworkLearningEval/issues"
 
 [project.optional-dependencies]
 dev = [
     "bump2version",
     "click",
     "jinja2",
     "parameterized",
```

### Comparing `obnb-0.1.0/src/obnb/config/__init__.py` & `obnb-0.1.0.dev1/src/obnb/config/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 """Configurations used by obnb."""
 from obnb.typing import Dict
 
 __all__ = [
     "DEFAULT_RETRY_DELAY",
     "MAX_DOWNLOAD_RETRIES",
     "STREAM_BLOCK_SIZE",
-    "OBNB_DATA_URL_DICT",
-    "OBNB_DATA_URL_DICT_DEV",
-    "OBNB_DATA_URL_DICT_STABLE",
+    "NLEDATA_URL_DICT",
+    "NLEDATA_URL_DICT_DEV",
+    "NLEDATA_URL_DICT_STABLE",
 ]
 
 DEFAULT_RETRY_DELAY = 5
 MAX_DOWNLOAD_RETRIES = 10
 STREAM_BLOCK_SIZE = 1024
 
-OBNB_DATA_URL_DICT_STABLE: Dict[str, str] = {
-    "obnbdata-0.1.0": "https://zenodo.org/record/8045270/files/",
-}
-OBNB_DATA_URL_DICT_DEV: Dict[str, str] = {
-    "obnbdata-0.1.0-dev": "https://sandbox.zenodo.org/record/1212773/files/",
-    "nledata-v0.1.0-dev6": "https://sandbox.zenodo.org/record/1172122/files/",
-    "nledata-v0.1.0-dev5": "https://sandbox.zenodo.org/record/1164492/files/",
-    "nledata-v0.1.0-dev4": "https://sandbox.zenodo.org/record/1163507/files/",
-    "nledata-v0.1.0-dev3": "https://sandbox.zenodo.org/record/1127466/files/",
-    "nledata-v0.1.0-dev2": "https://sandbox.zenodo.org/record/1103542/files/",
-    "nledata-v0.1.0-dev1": "https://sandbox.zenodo.org/record/1099982/files/",
-    "nledata-v0.1.0-dev": "https://sandbox.zenodo.org/record/1097545/files/",
+NLEDATA_URL_DICT_STABLE: Dict[str, str] = {}
+NLEDATA_URL_DICT_DEV: Dict[str, str] = {
     "nledata-v1.0-test": "https://sandbox.zenodo.org/record/1096827/files/",
+    "nledata-v0.1.0-dev": "https://sandbox.zenodo.org/record/1097545/files/",
+    "nledata-v0.1.0-dev1": "https://sandbox.zenodo.org/record/1099982/files/",
+    "nledata-v0.1.0-dev2": "https://sandbox.zenodo.org/record/1103542/files/",
+    "nledata-v0.1.0-dev3": "https://sandbox.zenodo.org/record/1127466/files/",
+    "nledata-v0.1.0-dev4": "https://sandbox.zenodo.org/record/1163507/files/",
+    "nledata-v0.1.0-dev5": "https://sandbox.zenodo.org/record/1164492/files/",
+    "nledata-v0.1.0-dev6": "https://sandbox.zenodo.org/record/1172122/files/",
 }
-OBNB_DATA_URL_DICT: Dict[str, str] = {
-    **OBNB_DATA_URL_DICT_STABLE,
-    **OBNB_DATA_URL_DICT_DEV,
-}
+NLEDATA_URL_DICT: Dict[str, str] = {**NLEDATA_URL_DICT_STABLE, **NLEDATA_URL_DICT_DEV}
```

### Comparing `obnb-0.1.0/src/obnb/config/logger_config.py` & `obnb-0.1.0.dev1/src/obnb/config/logger_config.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/__init__.py` & `obnb-0.1.0.dev1/src/obnb/data/__init__.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotated_ontology/__init__.py` & `obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/__init__.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotated_ontology/base.py` & `obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotated_ontology/diseases.py` & `obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/diseases.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotated_ontology/disgenet.py` & `obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/disgenet.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotated_ontology/go.py` & `obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/go.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotated_ontology/hpo.py` & `obnb-0.1.0.dev1/src/obnb/data/annotated_ontology/hpo.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotation/base.py` & `obnb-0.1.0.dev1/src/obnb/data/annotation/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotation/diseases.py` & `obnb-0.1.0.dev1/src/obnb/data/annotation/diseases.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotation/disgenet.py` & `obnb-0.1.0.dev1/src/obnb/data/annotation/disgenet.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotation/gene_ontology.py` & `obnb-0.1.0.dev1/src/obnb/data/annotation/gene_ontology.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/annotation/human_phenotype_ontology.py` & `obnb-0.1.0.dev1/src/obnb/data/annotation/human_phenotype_ontology.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         **kwargs,
     ):
         """Initialize GeneOntology annotation data object."""
         self._data_sources = data_sources
         super().__init__(root, **kwargs)
 
     @property
-    def data_sources(self) -> Optional[List[str]]:
+    def data_sources(self) -> List[str]:
         return self._data_sources
 
     def load_processed_data(self):
         path = self.raw_file_path(0)
         self.plogger.info(f"Loading raw annotation from {path}")
 
         # Load hpo gene annotation data
@@ -63,15 +63,15 @@
                 "frequency",
                 "disease_id",
             ],
         )
         annot_df["gene_id"] = annot_df["gene_id"].astype(str)
 
         # Select specified channels
-        if self.data_sources:
+        if self.data_sources is not None:
             evidence_str = pprint.pformat(self.data_sources)
             self.plogger.info(f"Subsetting annotations to evidences:\n{evidence_str}")
 
             annot_df["source"] = annot_df["disease_id"].str.split(":", expand=True)[0]
             ind = annot_df["source"].isin(self.data_sources)
             self.plogger.info(
                 f"{ind.sum():,} (out of {ind.shape[0]:,}) entries selected",
```

### Comparing `obnb-0.1.0/src/obnb/data/base.py` & `obnb-0.1.0.dev1/src/obnb/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             The `pre_transform` option is only valid when `version` is set to
             'latest'.
 
         """
         super().__init__(**kwargs)
 
         self.root = root
-        self.version = obnb.__data_version__ if version == "current" else version
+        self.version = version
         self.log_level = log_level
         self.cache_transform = cache_transform
         self.download_cache = download_cache
         self.gene_id_converter = gene_id_converter
 
         self.pre_transform = pre_transform
         self._setup_redos(redownload, reprocess, retransform)
```

### Comparing `obnb-0.1.0/src/obnb/data/experimental/alevinfry.py` & `obnb-0.1.0.dev1/src/obnb/data/experimental/alevinfry.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/__init__.py` & `obnb-0.1.0.dev1/src/obnb/data/network/__init__.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/base.py` & `obnb-0.1.0.dev1/src/obnb/data/network/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/biogrid.py` & `obnb-0.1.0.dev1/src/obnb/data/network/biogrid.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/bioplex.py` & `obnb-0.1.0.dev1/src/obnb/data/network/bioplex.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/comppi.py` & `obnb-0.1.0.dev1/src/obnb/data/network/comppi.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/consensuspathdb.py` & `obnb-0.1.0.dev1/src/obnb/data/network/consensuspathdb.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/funcoup.py` & `obnb-0.1.0.dev1/src/obnb/data/network/funcoup.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/hippie.py` & `obnb-0.1.0.dev1/src/obnb/data/network/hippie.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/humanbase.py` & `obnb-0.1.0.dev1/src/obnb/data/network/humanbase.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/humannet.py` & `obnb-0.1.0.dev1/src/obnb/data/network/humannet.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/humap.py` & `obnb-0.1.0.dev1/src/obnb/data/network/humap.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/huri.py` & `obnb-0.1.0.dev1/src/obnb/data/network/huri.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/omnipath.py` & `obnb-0.1.0.dev1/src/obnb/data/network/omnipath.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/pcnet.py` & `obnb-0.1.0.dev1/src/obnb/data/network/pcnet.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/proteomehd.py` & `obnb-0.1.0.dev1/src/obnb/data/network/proteomehd.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/signor.py` & `obnb-0.1.0.dev1/src/obnb/data/network/signor.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/network/string.py` & `obnb-0.1.0.dev1/src/obnb/data/network/string.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/data/ontology/base.py` & `obnb-0.1.0.dev1/src/obnb/data/ontology/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/dataset/base.py` & `obnb-0.1.0.dev1/src/obnb/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,38 @@
 """Dataset object."""
 import numpy as np
-from sklearn.preprocessing import KBinsDiscretizer
 
-from obnb.feature import FeatureVec, MultiFeatureVec
+from obnb.feature import MultiFeatureVec
 from obnb.feature.base import BaseFeature
 from obnb.graph.base import BaseGraph
 from obnb.label.collection import LabelsetCollection
 from obnb.label.split.base import BaseSplit
 from obnb.typing import Iterable, Iterator, Literal, Optional, PyG_Data, Tuple, Union
 from obnb.util.checkers import checkLiteral, checkNumpyArrayShape, checkType
 from obnb.util.idhandler import IDmap
 
 
 class Dataset:
-    """Dataset object.
-
-    Args:
-        graph: Graph object.
-        feature: Feature object.
-        label: Label set collection object.
-        auto_generate_feature: Automatically generate features from the input
-            graph if it is graph is available. If specified as None, then do
-            not generate features from the graph automatically.
-        dual: If set to True, consider each feature dimension as a sample.
-        splitter: Splitter object that determins train/val/test split.
-        split_kwargs: Keyword arguments for calling the split function of the
-            splitter.
-
-    """
+    """Dataset object."""
 
     def __init__(
         self,
         *,
         graph: Optional[BaseGraph] = None,
         feature: Optional[BaseFeature] = None,
         label: Optional[LabelsetCollection] = None,
-        auto_generate_feature: Optional[str] = "OneHotLogDeg",
         dual: bool = False,
         splitter: Optional[BaseSplit] = None,
         **split_kwargs,
     ):
         """Initialize Dataset."""
         self.set_idmap(graph, feature)
         self.graph = graph
         self.feature = feature
 
-        if self.feature is None and auto_generate_feature:
-            self.generate_features(auto_generate_feature)
-
         self.label = label
         self.splitter = splitter
         if label is None:
             raise ValueError("Missing required kwarg 'label'")
         elif splitter is None:
             self.y = label.get_y(target_ids=tuple(self.idmap.lst))
             self.masks = None
@@ -262,53 +243,33 @@
     ) -> Iterator[Tuple[str, Tuple[np.ndarray, np.ndarray]]]:
         """Iterate over all masks and return the mask name along with split."""
         if self.masks is None:
             raise ValueError("Masks not set.")
         for mask_name in self.masks:
             yield mask_name, self.get_split(mask_name, split_idx)
 
-    def generate_features(self, name: str = "OneHotLogDeg", overwrite: bool = False):
-        if self.graph is None:
-            raise ValueError("Missing graph in the dataset object")
-
-        if self.feature is not None and not overwrite:
-            raise ValueError(
-                "Feature already exists. Set overwrite to True to force "
-                "overwrite the original feature in the dataset object.",
-            )
-
-        if name == "OneHotLogDeg":
-            deg = self.graph.degree(weighted=False)[:, None]
-            feat = KBinsDiscretizer(
-                n_bins=32,
-                encode="onehot-dense",
-                strategy="uniform",
-            ).fit_transform(np.log(deg))
-            self._feature = FeatureVec.from_mat(feat, list(self.graph.node_ids))
-        else:
-            raise NotImplementedError(f"{name} feature is not implemented yet.")
-
     def to_pyg_data(
         self,
         *,
         device: str = "cpu",
         mask_suffix: str = "_mask",
     ) -> PyG_Data:
         """Convert dataset into PyG data."""
         # TODO: dense option
         import torch
         from torch_geometric.data import Data
 
         device = torch.device(device)
         num_nodes = self.size
 
-        x = self.feature.mat
+        # Use trivial feature if feature not available
+        x = np.ones((num_nodes, 1)) if self.feature is None else self.feature.mat
         edge_index, edge_weight = self.graph.to_coo()  # TODO: empty graph?
 
-        x = torch.FloatTensor(self.feature.mat)
+        x = torch.FloatTensor(x)
         edge_index = torch.LongTensor(edge_index)
         edge_weight = None if edge_weight is None else torch.FloatTensor(edge_weight)
 
         data = Data(
             num_nodes=num_nodes,
             edge_index=edge_index,
             edge_weight=edge_weight,
@@ -335,57 +296,7 @@
             for mask_name, mask in self.masks.items():
                 data.masks.append(attrname := mask_name + mask_suffix)
                 setattr(data, attrname, torch.BoolTensor(mask))
 
         data.to(device)
 
         return data
-
-    def to_dgl_data(
-        self,
-        *,
-        device: str = "cpu",
-        mask_suffix: str = "_mask",
-    ):
-        """Convert dataset into a DGL graph."""
-        # TODO: dense option
-        import dgl
-        import torch
-
-        device = torch.device(device)
-        num_nodes = self.size
-
-        # Use trivial feature if feature not available
-        x = self.feature.mat
-        (edges_src, edges_dst), edge_weight = self.graph.to_coo()  # TODO: empty graph?
-
-        dglgraph = dgl.graph(
-            (torch.LongTensor(edges_src), torch.LongTensor(edges_dst)),
-            num_nodes=num_nodes,
-        )
-        dglgraph.ndata["feat"] = torch.FloatTensor(x)
-
-        if edge_weight is not None:
-            dglgraph.edata["weight"] = torch.FloatTensor(edge_weight)
-
-        if self.graph is not None:
-            dglgraph.node_ids = list(self.graph.node_ids)
-
-        if self.label is not None:
-            dglgraph.task_ids = list(self.label.label_ids)
-
-        # Label (true) matrix
-        if self.y is not None:
-            dglgraph.ndata["label"] = torch.FloatTensor(self.y)
-
-        # Label mask (negative selection) matrix
-        if self.y_mask is not None:
-            dglgraph.ndata["label_mask"] = torch.BoolTensor(self.y_mask)
-
-        # Split mask matrix
-        if self.masks is not None:
-            for mask_name, mask in self.masks.items():
-                dglgraph.ndata[mask_name + mask_suffix] = torch.BoolTensor(mask)
-
-        dglgraph = dglgraph.to(device)
-
-        return dglgraph
```

### Comparing `obnb-0.1.0/src/obnb/dataset/dataset_dgl.py` & `obnb-0.1.0.dev1/src/obnb/dataset_pyg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,84 @@
-"""DGL dataset object."""
+"""PyTorch Geometric dataset object."""
 import os.path as osp
 
-try:
-    import torch
-    from dgl import load_graphs, save_graphs
-    from dgl.data import DGLDataset
-    from dgl.data.utils import load_info, save_info
-except (ModuleNotFoundError, OSError):
-    DGLDataset = object
-
-from obnb.dataset import OpenBiomedNetBench
-from obnb.typing import Callable, LogLevel, Optional
-from obnb.util.logger import verbose
-from obnb.util.version import parse_data_version
+import torch
+from torch_geometric.data import InMemoryDataset
 
+from obnb import __data_version__
+from obnb.typing import Callable, List, LogLevel, Optional
+from obnb.util.dataset_constructors import default_constructor
 
-class OpenBiomedNetBenchDGL(DGLDataset):
-    """DGL default dataset construct.
+
+class OpenBiomedNetBench(InMemoryDataset):
+    """PyTorch Geometric default dataset construct.
 
     Args:
         root: Root directory of the dataset to be saved.
         network: Name of the network to use.
         label: Name of the gene annotation label to use.
-        version: Version of the OpenBiomedNetBench data to use. By default,
-            "current" means using current (archived) release. If specified as
+        selected_genes: An optional list of genes. When supplied, will be used
+            to filter out genes in the label in addition to the filtering based
+            on network genes.
+        data_version: Version of the OpenBiomedNetBench data to use. If not
+            specified, will use the current (archived) release. If specified as
             "latest", then download data from source and process them from
             scratch.
         log_level: Data downloading and processing verbosity.
-        transform: DGL transforms to be applied to the DGL graph.
+        transform: PyG transformation to be applied.
+        pre_transform: PyG transformation to be applied before saving.
 
     """
 
     def __init__(
         self,
         root: str,
         network: str,
         label: str,
         *,
-        version: str = "current",
+        selected_genes: Optional[List[str]] = None,
+        data_version: Optional[str] = None,
         log_level: LogLevel = "INFO",
         transform: Optional[Callable] = None,
+        pre_transform: Optional[Callable] = None,
     ):
-        if DGLDataset is object:
-            raise ImportError(
-                "OpenBiomedNetBenchDGL requires the DGL libary, which is currently "
-                "missing.\nPlease follow the installation instructions on "
-                "https://www.dgl.ai/pages/start.html to install the DGL library first",
-            )
-
-        self.root = root
         self.network = network
         self.label = label
-        self.version = parse_data_version(version)
+        self.name = f"{network}-{label}"
+        self.selected_genes = selected_genes
+        self.data_version = data_version or __data_version__
         self.log_level = log_level
-        super().__init__(
-            name=f"{network}-{label}",
-            save_dir=osp.join(root, self.__class__.__name__),
-            verbose=verbose(log_level),
-            transform=transform,
-        )
 
-    def process(self):
-        dataset = OpenBiomedNetBench(
-            root=self.root,
-            graph_name=self.network,
-            label_name=self.label,
-            version=self.version,
-            log_level=self.log_level,
-        )
-        self._graph = dataset.to_dgl_data()
+        super().__init__(root, transform, pre_transform)
+        self.data, self.slices = torch.load(self.processed_paths[0])
+
+    def __repr__(self) -> str:
+        """Return the representation containing data size and names."""
+        paramstr = f"{len(self):,}, network={self.network}, label={self.label}"
+        return f"{self.__class__.__name__}({paramstr})"
 
     @property
-    def processed_graph_path(self) -> str:
-        return osp.join(self.save_path, "dgl_graph.bin")
+    def processed_dir(self) -> str:
+        return osp.join(self.root, self.__class__.__name__, self.name, "processed")
 
     @property
-    def processed_info_path(self) -> str:
-        return osp.join(self.save_path, "info.pkl")
+    def processed_file_names(self) -> str:
+        return "data.pt"
 
-    def save(self):
-        save_graphs(self.processed_graph_path, self._graph)
-        save_info(
-            self.processed_info_path,
-            {"node_ids": self._graph.node_ids, "task_ids": self._graph.task_ids},
+    def get_raw_dataset(self, log_level: Optional[LogLevel] = None):
+        return default_constructor(
+            self.root,
+            version=self.data_version,
+            graph_name=self.network,
+            label_name=self.label,
+            selected_genes=self.selected_genes,
+            log_level=log_level or self.log_level,
         )
 
-    def load(self):
-        graphs, _ = load_graphs(self.processed_graph_path)
-        self._graph = graphs[0]
-        info = load_info(self.processed_info_path)
-        self._graph.node_ids = info["node_ids"]
-        self._graph.task_ids = info["task_ids"]
-
-        for key, val in self._graph.ndata.items():
-            if key.endswith("_mask"):
-                self._graph.ndata[key] = val.to(dtype=torch.bool)
-
-    def has_cache(self) -> bool:
-        has_graph = osp.exists(self.processed_graph_path)
-        has_info = osp.exists(self.processed_info_path)
-        return has_graph and has_info
+    def process(self):
+        dataset = self.get_raw_dataset()
+        data = dataset.to_pyg_data()
 
-    def __getitem__(self, idx: int = 0):  # noqa: D105
-        return self._graph
+        if self.pre_transform is not None:
+            data = self.pre_transform(data)
 
-    def __len__(self):  # noqa: D105
-        return 1
+        torch.save(self.collate([data]), self.processed_paths[0])
```

### Comparing `obnb-0.1.0/src/obnb/exception.py` & `obnb-0.1.0.dev1/src/obnb/exception.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/ext/grape.py` & `obnb-0.1.0.dev1/src/obnb/ext/grape.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/ext/orbital_features.py` & `obnb-0.1.0.dev1/src/obnb/ext/orbital_features.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/ext/pecanpy.py` & `obnb-0.1.0.dev1/src/obnb/ext/pecanpy.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/ext/sknetwork.py` & `obnb-0.1.0.dev1/src/obnb/ext/sknetwork.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/feature/base.py` & `obnb-0.1.0.dev1/src/obnb/feature/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/feature/multifeat.py` & `obnb-0.1.0.dev1/src/obnb/feature/multifeat.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/feature/singlefeat.py` & `obnb-0.1.0.dev1/src/obnb/feature/singlefeat.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/graph/base.py` & `obnb-0.1.0.dev1/src/obnb/graph/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/graph/dense.py` & `obnb-0.1.0.dev1/src/obnb/graph/dense.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,37 +96,14 @@
         if direction == "in":
             return sorted(in_nbrs_idxs)
         elif direction == "out":
             return sorted(out_nbrs_idxs)
         else:
             return sorted(in_nbrs_idxs | out_nbrs_idxs)
 
-    def degree(self, weighted: bool = False, direction: str = "out") -> np.ndarray:
-        """Return node degrees.
-
-        Args:
-            weighted: Whether or not consider edge weights.
-            direction: 'in' or 'out' degrees. This option is only relevant for
-                directed graphs.
-
-        """
-        adj = self.mat.copy()
-
-        if not weighted:
-            adj = adj != 0
-
-        if direction == "in":
-            axis = 0
-        elif direction == "out":
-            axis = 1
-        else:
-            raise ValueError(f"direction must be 'in' or 'out', got {direction!r}")
-
-        return adj.sum(axis)
-
     def propagate(self, seed: np.ndarray) -> np.ndarray:
         """Propagate label informmation.
 
         Args:
             seeds: 1-dimensinoal numpy array where each entry is the seed
                 information for a specific node.
```

### Comparing `obnb-0.1.0/src/obnb/graph/ontology.py` & `obnb-0.1.0.dev1/src/obnb/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/graph/sparse.py` & `obnb-0.1.0.dev1/src/obnb/graph/sparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,34 +90,14 @@
         return fvec
 
     def _get_nbr_idxs(self, node_idx: int, direction: EdgeDir) -> List[int]:
         if self.directed and direction != "out":
             raise NotImplementedError("Use DirectedSparseGraph instead.")
         return sorted(self.edge_data[node_idx])
 
-    def degree(self, weighted: bool = False, direction: str = "out") -> np.ndarray:
-        """Return node degrees.
-
-        Args:
-            weighted: Whether or not consider edge weights.
-            direction: 'in' or 'out' degrees. This option is only relevant for
-                directed graphs.
-
-        """
-        if (not weighted) and (direction == "out"):
-            deg = np.array([len(i) for i in self._edge_data])
-        elif weighted and (direction == "out"):
-            deg = np.array([sum(i.values()) for i in self._edge_data])
-        elif direction == "in":
-            deg = np.zeros(self.size)
-            for _, dst_data in enumerate(self._edge_data):
-                for dst, weight in dst_data.items():
-                    deg[dst] += weight if weighted else 1
-        return deg
-
     def induced_subgraph(self, node_ids: List[str]):
         """Return a subgraph induced by a subset of nodes.
 
         Args:
             node_ids (List[str]): List of nodes of interest.
 
         """
@@ -812,24 +792,22 @@
     in addition to the more natural "propagation downwards" operation.
 
     """
 
     def __init__(
         self,
         weighted: bool = True,
-        directed: bool = True,
         log_level: LogLevel = "WARNING",
         verbose: bool = False,
         logger: Optional[logging.Logger] = None,
     ):
         """Initialize the directed sparse graoh."""
-        assert directed, "DirectedSparseGraph must have directed=True"
         super().__init__(
             weighted=weighted,
-            directed=directed,
+            directed=True,
             log_level=log_level,
             verbose=verbose,
             logger=logger,
         )
         self._rev_edge_data: EdgeData = []
 
     @property
@@ -853,31 +831,14 @@
         if direction == "in":
             return sorted(in_nbrs_idxs)
         elif direction == "out":
             return sorted(out_nbrs_idxs)
         else:
             return sorted(in_nbrs_idxs | out_nbrs_idxs)
 
-    def degree(self, weighted: bool = False, direction: str = "out") -> np.ndarray:
-        """Return node degrees.
-
-        Args:
-            weighted: Whether or not consider edge weights.
-            direction: 'in' or 'out' degrees. This option is only relevant for
-                directed graphs.
-
-        """
-        if direction == "out":
-            deg = super().degree(weighted=weighted, direction=direction)
-        elif not weighted:
-            deg = np.array([len(i) for i in self._rev_edge_data])
-        else:
-            deg = np.array([sum(i.values()) for i in self._rev_edge_data])
-        return deg
-
     def _new_node_data(self):
         self._edge_data.append({})
         self._rev_edge_data.append({})
 
     def add_edge(
         self,
         node_id1: str,
```

### Comparing `obnb-0.1.0/src/obnb/label/collection.py` & `obnb-0.1.0.dev1/src/obnb/label/collection.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/__init__.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/base.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/existence_filter.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/existence_filter.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/negative_generator.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/negative_generator.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/nonred.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/nonred.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/pairwise_filter.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/pairwise_filter.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/range_filter.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/filters/value_filter.py` & `obnb-0.1.0.dev1/src/obnb/label/filters/value_filter.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/split/base.py` & `obnb-0.1.0.dev1/src/obnb/label/split/base.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/split/holdout.py` & `obnb-0.1.0.dev1/src/obnb/label/split/holdout.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/label/split/partition.py` & `obnb-0.1.0.dev1/src/obnb/label/split/partition.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/metric/graphgym_metric.py` & `obnb-0.1.0.dev1/src/obnb/metric/graphgym_metric.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/metric/standard.py` & `obnb-0.1.0.dev1/src/obnb/metric/standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,28 @@
 """Standard metric extending those available in sklearn."""
 from functools import wraps
 
-try:
-    import torch
-except (ModuleNotFoundError, OSError):
-    torch = None
 import numpy as np
 import sklearn.metrics
 
-from obnb.typing import Optional, Tensor, Union
-
-
-def cast_ndarray_type(x: Union[np.ndarray, Tensor]) -> np.ndarray:
-    """Cast numpy ndarray type."""
-    if isinstance(x, np.ndarray):
-        x = x
-    elif torch is None or not isinstance(x, torch.Tensor):
-        raise TypeError(f"Cannot to typecast {type(x)} to numpy array")
-    else:
-        x = x.detach().clone().to("cpu", non_blocking=True).numpy()
-    return x
+from obnb.typing import Optional
 
 
 def wrap_metric(metric_func):
     """Wrap metric function with common processing steps.
 
     - Skip computation if None
     - Perturn reduction when calculating metrics in a multi-class setting
 
     """
 
     @wraps(metric_func)
     def wrapped(
-        y_true: Union[np.ndarray, Tensor],
-        y_pred: Union[np.ndarray, Tensor],
+        y_true: np.ndarray,
+        y_pred: np.ndarray,
         reduce: str = "mean",
         y_mask: Optional[np.ndarray] = None,
     ):
         """Metric function with common processing steps.
 
         Args:
             y_true: True label.
@@ -49,17 +34,14 @@
                 either positives or negatives when calculating the metric. In
                 other words, we ignore the neutrals in the calculation.
 
         """
         if reduce not in ["none", "mean", "median"]:
             raise ValueError(f"Unknown reduce option {reduce!r}")
 
-        y_true = cast_ndarray_type(y_true)
-        y_pred = cast_ndarray_type(y_pred)
-
         if _skip(y_true, y_pred):
             return np.nan
 
         if y_mask is None:
             y_mask = np.ones_like(y_true, dtype=bool)
 
         if len(y_true.shape) == 1 or y_true.shape[1] == 1:
```

### Comparing `obnb-0.1.0/src/obnb/model/label_propagation.py` & `obnb-0.1.0.dev1/src/obnb/model/label_propagation.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/model_trainer/base.py` & `obnb-0.1.0.dev1/src/obnb/model_trainer/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 import time
 from copy import deepcopy
 
 import numpy as np
 
-import obnb.metric
 from obnb.typing import Any, Callable, Dict, LogLevel, Optional
 from obnb.util.logger import attach_file_handler, get_logger
 
 
 class BaseTrainer:
     """The BaseTrainer object.
 
     Abstract class for trainer objects, which serve as interfaces or shortcuts
     for training specific types of models.
 
     """
 
     def __init__(
         self,
-        metrics: Optional[Dict[str, Callable[[np.ndarray, np.ndarray], float]]] = None,
+        metrics: Dict[str, Callable[[np.ndarray, np.ndarray], float]],
         train_on: str = "train",
         log_level: LogLevel = "INFO",
         log_path: Optional[str] = None,
     ):
         """Initialize BaseTraining.
 
         Note: "dual" mode only works if the input features is MultiFeatureVec.
 
         Args:
-            metrics: Dictionary of metrics used to train/evaluate the model. If
-                not specified, will use the default selection of APOP and AUROC.
+            metrics: Dictionary of metrics used to train/evaluate the model.
             train_on: Which mask to use for training.
             log_level: Log level.
             log_path: Log file path. If not set, then do not log to file.
 
         """
         self._tic: Optional[float] = None
-
-        if not metrics:
-            metrics = {
-                "apop": obnb.metric.log2_auprc_prior,
-                "auroc": obnb.metric.auroc,
-            }
         self.metrics = metrics
-
         self.train_on = train_on
         self.logger = get_logger(
             self.__class__.__name__,
             log_level=log_level,
             base_logger="obnb_brief",
         )
 
@@ -114,23 +105,23 @@
 
         _, _, get_predictions, compute_results = self._setup(dataset, split_idx)
         get_predictions(model, x, y, dataset.masks)
         results = compute_results(dataset.masks)
 
         return results
 
-    def fit_and_eval(
+    def eval_multi_ovr(
         self,
         model: Any,
         dataset,
         split_idx: int = 0,
         consider_negative: bool = False,
         reduce: str = "none",
     ) -> Dict[str, float]:
-        """Fit model and evaluate.
+        """Evaluate the model in a multiclass setting.
 
         Note:
             The original model is not trained. For each task, a deep copy of
             the model is created and it is evaluated via one-vs-rest.
 
         """
         g = dataset.graph
```

### Comparing `obnb-0.1.0/src/obnb/model_trainer/gnn.py` & `obnb-0.1.0.dev1/src/obnb/model_trainer/gnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from copy import deepcopy
 
-import numpy as np
 import torch
 
 from obnb.model_trainer.base import BaseTrainer
-from obnb.typing import Any, Callable, Dict, List, LogLevel, Optional, Tuple
+from obnb.typing import Any, Dict, List, LogLevel, Optional, Tuple
 
 
 class GNNTrainer(BaseTrainer):
     """Trainner for GNN models."""
 
     def __init__(
         self,
-        metrics: Optional[Dict[str, Callable[[np.ndarray, np.ndarray], float]]] = None,
+        metrics,
         train_on="train",
         val_on: str = "val",
         mask_suffix: str = "_mask",
         device: str = "cpu",
         metric_best: Optional[str] = None,
         lr: float = 0.01,
         epochs: int = 100,
@@ -26,15 +25,17 @@
         log_path: Optional[str] = None,
     ):
         """Initialize GNNTrainer.
 
         Args:
             val_on (str): Validation mask name (default: :obj:`"train"`).
             device (str): Training device (default: :obj:`"cpu"`).
-            metric_best (str): Metric used for determining the best epoch.
+            metric_best (str): Metric used for determining the best model
+                (default: :obj:`None`).
+                if set to True (default: :obj:`False`)
             lr (float): Learning rate (default: :obj:`0.01`)
             epochs (int): Total epochs (default: :obj:`100`)
             eval_steps (int): Interval for evaluation (default: :obj:`10`)
             use_negative: If set to True, then try to restrict calculation of
                 the loss function to only the positive and negative examples,
                 and exclude those that are neutral. This will be indicated in
                 the :obj:`y_mask` attribute of the data object, where the
@@ -70,17 +71,15 @@
         Raises:
             ValueError: More than one metrics is available but did not specify
                 metric_best.
             KeyError: metric_best did not match any of the specified metrics.
 
         """
         if metric_best is None or metric_best == "auto":
-            if "apop" in self.metrics:  # default best metric
-                self._metric_best = "apop"
-            elif len(self.metrics) != 1:
+            if len(self.metrics) != 1:
                 raise ValueError(
                     "Multiple metrics found but did not specify metric_best",
                 )
             else:
                 self._metric_best = list(self.metrics)[0]
         elif metric_best not in self.metrics:
             raise KeyError(f"No metrics named {metric_best!r}")
```

### Comparing `obnb-0.1.0/src/obnb/model_trainer/graphgym.py` & `obnb-0.1.0.dev1/src/obnb/model_trainer/graphgym.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/model_trainer/label_propagation.py` & `obnb-0.1.0.dev1/src/obnb/model_trainer/label_propagation.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/model_trainer/supervised_learning.py` & `obnb-0.1.0.dev1/src/obnb/model_trainer/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/typing.py` & `obnb-0.1.0.dev1/src/obnb/typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     Union,
 )
 
 import numpy as np
 
 try:
     from torch import Tensor
-except (ModuleNotFoundError, OSError):
+except ModuleNotFoundError:
     Tensor = Any
 
 try:
     from torch_geometric.data import Data as PyG_Data
-except (ModuleNotFoundError, OSError):
+except ModuleNotFoundError:
     PyG_Data = Any
 
 INT_TYPE = (int, np.int32, np.int64)
 FLOAT_TYPE = (float, np.float32, np.float64)
 NUMERIC_TYPE = INT_TYPE + FLOAT_TYPE
 
 EdgeData = List[Dict[int, float]]
```

### Comparing `obnb-0.1.0/src/obnb/util/checkers.py` & `obnb-0.1.0.dev1/src/obnb/util/checkers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Type checking functions.
 
 This module contains a collection of checkers to ensure that the input value to
 a function call is valid.
 
 """
-import warnings
 from typing import get_args
 
 import numpy as np
-from outdated import check_outdated
 
 from obnb.typing import INT_TYPE, NUMERIC_TYPE, Iterable, List, Optional, Tuple
 
 __all__ = [
     "checkConfig",
     "checkNullableType",
     "checkNumpyArrayIsNumeric",
@@ -25,26 +23,14 @@
     "checkTypesInNumpyArray",
     "checkTypesInSet",
     "checkValueNonnegative",
     "checkValuePositive",
 ]
 
 
-def checkVersion(version: str):
-    """Check if the current version is up to date."""
-    is_outdated, latest_version = check_outdated("obnb", version)
-    if is_outdated:
-        warnings.warn(
-            f"A new OBNB version {latest_version!r} is available "
-            f"(current version: {version!r}).",
-            UserWarning,
-            stacklevel=2,
-        )
-
-
 def checkValuePositive(name, val):
     """Check if the input value is positive."""
     if not val > 0:
         raise ValueError(f"{name!r} should be positive, got {val}")
 
 
 def checkValueNonnegative(name, val):
```

### Comparing `obnb-0.1.0/src/obnb/util/converter.py` & `obnb-0.1.0.dev1/src/obnb/util/converter.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/util/cx_explorer.py` & `obnb-0.1.0.dev1/src/obnb/util/cx_explorer.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/util/deprecated.py` & `obnb-0.1.0.dev1/src/obnb/util/deprecated.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/util/download.py` & `obnb-0.1.0.dev1/src/obnb/util/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 import requests
 from tqdm import tqdm
 
 from obnb.config import (
     DEFAULT_RETRY_DELAY,
     MAX_DOWNLOAD_RETRIES,
-    OBNB_DATA_URL_DICT,
-    OBNB_DATA_URL_DICT_STABLE,
+    NLEDATA_URL_DICT,
+    NLEDATA_URL_DICT_STABLE,
     STREAM_BLOCK_SIZE,
 )
 from obnb.exception import DataNotFoundError, ExceededMaxNumRetries
 from obnb.typing import LogLevel, Optional, Tuple, ZipType
 from obnb.util.logger import display_pbar, get_logger
 
 native_logger = get_logger(None, log_level="INFO")
@@ -45,16 +45,16 @@
 
     Returns:
         str: URL to download the archive data.
 
     """
     logger = logger or native_logger
 
-    if (base_url := OBNB_DATA_URL_DICT.get(version)) is None:
-        versions = list(OBNB_DATA_URL_DICT_STABLE) + ["latest"]
+    if (base_url := NLEDATA_URL_DICT.get(version)) is None:
+        versions = list(NLEDATA_URL_DICT_STABLE) + ["latest"]
         raise ValueError(
             f"Unrecognized version {version!r}, please choose from the "
             f"following versions:\n{pformat(versions)}",
         )
 
     data_url = urllib.parse.urljoin(base_url, f"{name}.zip")
     logger.info(f"Download URL: {data_url}")
```

### Comparing `obnb-0.1.0/src/obnb/util/idhandler.py` & `obnb-0.1.0.dev1/src/obnb/util/idhandler.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/util/parallel.py` & `obnb-0.1.0.dev1/src/obnb/util/parallel.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/util/registers.py` & `obnb-0.1.0.dev1/src/obnb/util/registers.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb/util/timer.py` & `obnb-0.1.0.dev1/src/obnb/util/timer.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/src/obnb.egg-info/PKG-INFO` & `obnb-0.1.0.dev1/src/obnb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: obnb
-Version: 0.1.0
+Version: 0.1.0.dev1
 Summary: A Python toolkit for biological network learning evaluation
 Author-email: Remy Liu <liurenmi@msu.edu>
 License: MIT
-Project-URL: home, https://github.com/krishnanlab/obnb
-Project-URL: bug-tracker, https://github.com/krishnanlab/obnb/issues
+Project-URL: home, https://github.com/krishnanlab/NetworkLearningEval
+Project-URL: bug-tracker, https://github.com/krishnanlab/NetworkLearningEval/issues
 Keywords: Data Processing,Gene Classification,Machine Learning,Network Biology,Network Repositories
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python
@@ -20,141 +20,142 @@
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: pyroe
 Provides-Extra: ext
 Provides-Extra: full
 License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/obnb.svg)](https://badge.fury.io/py/obnb)
-[![Documentation Status](https://readthedocs.org/projects/obnb/badge/?version=latest)](https://obnb.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/nleval.svg)](https://badge.fury.io/py/nleval)
+[![Documentation Status](https://readthedocs.org/projects/networklearningeval/badge/?version=latest)](https://networklearningeval.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-[![Tests](https://github.com/krishnanlab/obnb/actions/workflows/tests.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/tests.yml)
-[![Test Examples](https://github.com/krishnanlab/obnb/actions/workflows/examples.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/examples.yml)
-[![Test Data](https://github.com/krishnanlab/obnb/actions/workflows/test_data.yml/badge.svg)](https://github.com/krishnanlab/obnb/actions/workflows/test_data.yml)
+[![Tests](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/tests.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/tests.yml)
+[![Test Examples](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/examples.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/examples.yml)
+[![Test Data](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/test_data.yml/badge.svg)](https://github.com/krishnanlab/NetworkLearningEval/actions/workflows/test_data.yml)
 
 # Open Biomedical Network Benchmark
 
-The Open Biomedical Network Benchmark (OBNB) is a comprehensive resource for setting up benchmarking graph datasets using _biomedical networks_ and _gene annotations_.
-Our goal is to accelerate the adoption of advanced graph machine learning techniques, such as graph neural networks and graph embeddings, in network biology for gaining novel insights into genes' function, trait, and disease associations using biological networks.
-To make this adoption convenient, OBNB also provides dataset objects compatible with popular graph deep learning frameworks, including [PyTorch Geometric (PyG)](https://github.com/pyg-team/pytorch_geometric) and [Deep Graph Library (DGL)](https://github.com/dmlc/dgl).
-
-A comprehensive benchmarking study with a wide-range of graph neural networks and graph embedding methods on OBNB datasets can be found in our benchmarking repository [`obnbench`](https://github.com/krishnanlab/obnbench).
+## Installation
 
-## Package usage
+Clone the repository first and then install via `pip`
 
-### Construct default datasets
+```bash
+git clone https://github.com/krishnanlab/NetworkLearningEval && cd NetworkLearningEval
+pip install -e .
+```
 
-We provide a high-level dataset constructor to help users easily set up benchmarking graph datasets
-for a combination of network and label. In particular, the dataset will be set up with study-bias
-holdout split (6/2/2), where 60% of the most well-studied genes according to the number of
-associated PubMed publications are used for training, 20% of the least studied genes are used for
-testing, and the rest of the 20% genes are used for validation. For more customizable data loading
-and processing options, see the [customized dataset construction](#customized-dataset-construction)
-section below.
+The `-e` option means 'editable', i.e. no need to reinstall the library if you make changes to the source code.
+Feel free to not use the `-e` option and simply do `pip install .` if you do not plan on modifying the source code.
 
-```python
-from obnb.dataset import OpenBiomedNetBench
-from obnb.util.version import get_available_data_versions
+### Optional Pytorch Geometric installation
 
-root = "datasets"  # save dataset and cache under the datasets/ directory
-version = "current"  # use the last archived version
-# Optionally, set version to the specific data version number
-# Or, set version to "latest" to download the latest data from source and process it from scratch
+User need to install [Pytorch Geomtric](https://github.com/pyg-team/pytorch_geometric) to enable some GNN related features.
+To install PyG, first need to install [PyTorch](https://pytorch.org).
+For full details about installation instructions, visit the links above.
+Assuming the system has Python3.8 or above installed, with CUDA10.2, use the following to install both PyTorch and PyG.
 
-# Download and process network/label data. Use the adjacency matrix as the ML feature
-dataset = OpenBiomedNetBench(root=root, graph_name="BioGRID", label_name="DisGeNET",
-                             version=version, graph_as_feature=True, use_dense_graph=True)
+```bash
+conda install pytorch=1.12.1 torchvision cudatoolkit=10.2 -c pytorch
+pip install torch-geometric==2.0.4 torch-scatter torch-sparse torch-cluster -f https://data.pyg.org/whl/torch-1.12.1+cu102.html
+```
 
-# Check the specific archive data version used
-print(dataset.version)
+### Quick install using the installation script
 
-# Check all available stable archive data versions
-print(get_available_data_versions())
+```bash
+source install.sh cu102  # other options are [cpu,cu113]
 ```
 
-Users can also load the dataset objects into ones that are compatible with PyG or DGL (see below).
+## Quick Demonstration
 
-#### PyG dataset
+### Construct default datasets
 
-```python
-from obnb.dataset import OpenBiomedNetBenchPyG
-dataset = OpenBiomedNetBenchPyG(root, "BioGRID", "DisGeNET")
-```
+We provide a high-level dataset constructor to help user effortlessly set up a ML-ready dataset
+for a combination of network and label. In particular, the dataset will be set up with study-bias
+holdout split (6/2/2), where 60% of the most well studied genes according to the number of
+associated PubMed publications are used for training, 20% of the least studied genes are used for
+testing, and rest of the 20% genes are used for validation. For more customizable data loading
+and processing options, see the [customized dataset construction](#customized-dataset-construction)
+section below.
 
-**Note**: requires installing PyG first (see [installation instructions](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html))
+```python
+from obnb.util.dataset_constructors import default_constructor
 
-#### DGL dataset
+root = "datasets"  # save dataset and cache under the datasets/ directory
+version = "nledata-v0.1.0-dev3"  # archive data version, use 'latest' to pull latest data from source instead
 
-```python
-from obnb.dataset import OpenBiomedNetBenchDGL
-dataset = OpenBiomedNetBenchDGL(root, "BioGRID", "DisGeNET")
+# Download and process network/label data. Use the adjacency matrix as the ML feature
+dataset = default_constructor(root=root, version=version, graph_name="BioGRID", label_name="DisGeNET",
+                              graph_as_feature=True, use_dense_graph=True)
 ```
 
-**Note**: requires installing DGL first (see [installation instructions](https://www.dgl.ai/pages/start.html))
-
 ### Evaluating standard models
 
 Evaluation of simple machine learning methods such as logistic regression and label propagation
-can be done easily using the trainer objects.
+can be done easily using the trainer objects. The trainer objects take a dictionary of metrics
+as input for evaluating the models' performances, and can be set up as follows.
 
 ```python
+from obnb.metric import auroc
 from obnb.model_trainer import SupervisedLearningTrainer, LabelPropagationTrainer
 
-sl_trainer = SupervisedLearningTrainer()
-lp_trainer = LabelPropagationTrainer()
+metrics = {"auroc": auroc}  # use AUROC as our default evaluation metric
+sl_trainer = SupervisedLearningTrainer(metrics)
+lp_trainer = LabelPropagationTrainer(metrics)
 ```
 
-Then, use the `fit_and_eval` method of the trainer to evaluate a given ML model over all tasks
+Then, use the `eval_multi_ovr` method of the trainer to evaluate a given ML model over all tasks
 in a one-vs-rest setting.
 
 ```python
 from sklearn.linear_model import LogisticRegression
 from obnb.model.label_propagation import OneHopPropagation
 
 # Initialize models
 sl_mdl = LogisticRegression(penalty="l2", solver="lbfgs")
 lp_mdl = OneHopPropagation()
 
 # Evaluate the models over all tasks
-sl_results = sl_trainer.fit_and_eval(sl_mdl, dataset)
-lp_results = lp_trainer.fit_and_eval(lp_mdl, dataset)
+sl_results = sl_trainer.eval_multi_ovr(sl_mdl, dataset)
+lp_results = lp_trainer.eval_multi_ovr(lp_mdl, dataset)
 ```
 
 ### Evaluating GNN models
 
 Training and evaluation of Graph Neural Network (GNN) models can be done in a very similar fashion.
 
 ```python
 from torch_geometric.nn import GCN
 from obnb.model_trainer.gnn import SimpleGNNTrainer
 
-# Use 1-dimensional trivial node feature by default
-dataset = OpenBiomedNetBench(root=root, graph_name="BioGRID", label_name="DisGeNET", version=version)
+# Use 1-dimensional trivial node feature
+dataset = default_constructor(root=root, version=version, graph_name="BioGRID", label_name="DisGeNET")
 
 # Train and evaluate a GCN
 gcn_mdl = GCN(in_channels=1, hidden_channels=64, num_layers=5, out_channels=n_tasks)
-gcn_trainer = SimpleGNNTrainer(device="cuda", metric_best="apop")
+gcn_trainer = SimpleGNNTrainer(metrics, device="cuda", metric_best="auroc")
 gcn_results = gcn_trainer.train(gcn_mdl, dataset)
 ```
 
 ### Customized dataset construction
 
 #### Load network and labels
 
 ```python
 from obnb import data
 
+root = "datasets"  # save dataset and cache under the datasets/ directory
+
 # Load processed BioGRID data from archive.
-g = data.BioGRID(root, version=version)
+# Alternatively, set version="latest" to get and process the newest data from scratch.
+g = data.BioGRID(root, version="nledata-v0.1.0-dev3")
 
 # Load DisGeNET gene set collections.
-lsc = data.DisGeNET(root, version=version)
+lsc = data.DisGeNET(root, version="latest")
 ```
 
 #### Setting up data and splits
 
 ```python
 from obnb.util.converter import GenePropertyConverter
 from obnb.label.split import RatioHoldout
@@ -183,35 +184,30 @@
 #### Combine into dataset
 
 ```python
 from obnb import Dataset
 dataset = Dataset(graph=g, feature=g.to_dense_graph().to_feature(), label=lsc, splitter=splitter)
 ```
 
-## Installation
+## Data preparation and releasing notes
 
-OBNB can be installed easily via pip from [PyPI](https://pypi.org/project/obnb/):
+First, bump data version in `__init__.py` to the next data release version, e.g., `nledata-v0.1.0 -> nledata-v0.1.1-dev`.
+Then, download and process all latest data by running
 
 ```bash
-pip install obnb
+python script/release_data.py
 ```
 
-### Install with extension modules (optional)
+By default, the data ready to be uploaded (e.g., to [Zenodo](zenodo.org)) is saved under `data_release/archived`.
+After some necessary inspection and checking, if everything looks good, upload and publish the new archived data.
 
-OBNB provides interfaces with several other packages for network feature extractions, such as
-[PecanPy](https://github.com/krishnanlab/PecanPy) and [GraPE](https://github.com/AnacletoLAB/grape).
-To enable those extensions, install `obnb` with the `ext` extra option enabled:
+**Note:** `dev` data should be uploaded to the [sandbox](https://sandbox.zenodo.org/record/1097545#.YxYrqezMJzV) instead.
 
-```bash
-pip install obnb[ext]
-```
+Check items:
 
-### Install graph deep learning libraries (optional)
+- [ ] Update `__data_version__`
+- [ ] Run [`release_data.py`](script/release_data.py)
+- [ ] Upload archived data to Zenodo (be sure to edit the data version there also)
+- [ ] Update url dict in config (will improve in the future to get info from Zenodo directly)
+- [ ] Update network stats in data [test](test/test_data.py)
 
-Follow installation instructions for [PyG](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html) or [DGL](https://www.dgl.ai/pages/start.html) to set up the graph deep learning library of your choice.
-
-Alternatively, we also provide an [installation script](install.sh) that helps you installthe graph deep-learning dependencies in a new conda environment `obnb`:
-
-```bash
-git clone https://github.com/krishnanlab/obnb && cd obnb
-source install.sh cu117  # other options are [cpu,cu118]
-```
+Finally, commit and push the bumped version.
```

### Comparing `obnb-0.1.0/src/obnb.egg-info/SOURCES.txt` & `obnb-0.1.0.dev1/src/obnb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/obnb/__init__.py
+src/obnb/dataset.py
+src/obnb/dataset_pyg.py
 src/obnb/exception.py
 src/obnb/typing.py
 src/obnb.egg-info/PKG-INFO
 src/obnb.egg-info/SOURCES.txt
 src/obnb.egg-info/dependency_links.txt
 src/obnb.egg-info/not-zip-safe
 src/obnb.egg-info/requires.txt
@@ -37,28 +39,24 @@
 src/obnb/data/network/consensuspathdb.py
 src/obnb/data/network/funcoup.py
 src/obnb/data/network/hippie.py
 src/obnb/data/network/humanbase.py
 src/obnb/data/network/humannet.py
 src/obnb/data/network/humap.py
 src/obnb/data/network/huri.py
+src/obnb/data/network/intact.py
 src/obnb/data/network/omnipath.py
 src/obnb/data/network/pcnet.py
 src/obnb/data/network/proteomehd.py
 src/obnb/data/network/signor.py
 src/obnb/data/network/string.py
 src/obnb/data/ontology/__init__.py
 src/obnb/data/ontology/base.py
 src/obnb/data/ontology/gene_ontology.py
 src/obnb/data/ontology/mondo.py
-src/obnb/dataset/__init__.py
-src/obnb/dataset/base.py
-src/obnb/dataset/dataset.py
-src/obnb/dataset/dataset_dgl.py
-src/obnb/dataset/dataset_pyg.py
 src/obnb/ext/__init__.py
 src/obnb/ext/grape.py
 src/obnb/ext/orbital_features.py
 src/obnb/ext/pecanpy.py
 src/obnb/ext/sknetwork.py
 src/obnb/feature/__init__.py
 src/obnb/feature/base.py
@@ -94,22 +92,22 @@
 src/obnb/model_trainer/graphgym.py
 src/obnb/model_trainer/label_propagation.py
 src/obnb/model_trainer/supervised_learning.py
 src/obnb/util/__init__.py
 src/obnb/util/checkers.py
 src/obnb/util/converter.py
 src/obnb/util/cx_explorer.py
+src/obnb/util/dataset_constructors.py
 src/obnb/util/deprecated.py
 src/obnb/util/download.py
 src/obnb/util/idhandler.py
 src/obnb/util/logger.py
 src/obnb/util/parallel.py
 src/obnb/util/path.py
 src/obnb/util/registers.py
 src/obnb/util/timer.py
-src/obnb/util/version.py
 test/test_data.py
 test/test_dataset.py
 test/test_graph.py
 test/test_metric.py
 test/test_model.py
 test/test_wrapper.py
```

### Comparing `obnb-0.1.0/test/test_data.py` & `obnb-0.1.0.dev1/test/test_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 import pytest
 from parameterized import parameterized
 
 import obnb
 import obnb.data
 import obnb.graph
-from obnb.config import OBNB_DATA_URL_DICT
-from obnb.dataset.dataset import OpenBiomedNetBench
+from obnb.config import NLEDATA_URL_DICT
 from obnb.exception import DataNotFoundError
 from obnb.feature.base import BaseFeature
+from obnb.util.dataset_constructors import default_constructor
 from obnb.util.download import download_unzip
 from obnb.util.timer import Timeout
 
 opts = {
     "log_level": "DEBUG",
     "version": obnb.__data_version__,
 }
@@ -85,15 +85,15 @@
         # Clean at the end of the test class
         cls.tmp_dir_preserve = tempfile.mkdtemp()
         print(
             f"Created temporary directory for testing data: {cls.tmp_dir}, "
             f"{cls.tmp_dir_preserve}",
         )
 
-        data_url = urljoin(OBNB_DATA_URL_DICT[obnb.__data_version__], ".cache.zip")
+        data_url = urljoin(NLEDATA_URL_DICT[obnb.__data_version__], ".cache.zip")
         download_unzip(data_url, cls.tmp_dir_preserve)
 
     @classmethod
     def tearDownClass(cls):
         shutil.rmtree(cls.tmp_dir)
         shutil.rmtree(cls.tmp_dir_preserve)
         print(f"Removed temporary directories: {cls.tmp_dir}, {cls.tmp_dir_preserve}")
@@ -163,21 +163,20 @@
     datadir = tmpdir / "datasets"
 
     for graph_as_feature, use_dense_graph in product([True, False], [True, False]):
         with subtests.test(
             graph_as_feature=graph_as_feature,
             use_dense_graph=use_dense_graph,
         ):
-            dataset = OpenBiomedNetBench(
+            dataset = default_constructor(
                 root=datadir,
                 graph_name="BioPlex",
                 label_name="DisGeNET",
                 graph_as_feature=graph_as_feature,
                 use_dense_graph=use_dense_graph,
-                auto_generate_feature=None,
                 **opts,
             )
 
             if graph_as_feature:
                 assert isinstance(dataset.feature, BaseFeature)
             else:
                 assert dataset.feature is None
```

### Comparing `obnb-0.1.0/test/test_dataset.py` & `obnb-0.1.0.dev1/test/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 
-from obnb.dataset.base import Dataset
+from obnb.dataset import Dataset
 from obnb.exception import IDNotExistError
 from obnb.feature import MultiFeatureVec
 from obnb.graph.dense import DenseGraph
 from obnb.label.collection import LabelsetCollection
 
 
 class Data:
@@ -116,15 +116,15 @@
         answer = data.raw_data_list[idx]
         with subtests.test(idx=idx):
             assert dataset.get_feat(idx, mode="idxs").tolist() == answer
 
     # Index out of range
     pytest.raises(IndexError, dataset.get_feat, [3, 5])
 
-    dataset = Dataset(graph=data.graph, label=data.lsc, auto_generate_feature=None)
+    dataset = Dataset(graph=data.graph, label=data.lsc)
     with pytest.raises(ValueError, match="feature not set"):
         dataset.get_feat([0, 1])
 
 
 def test_get_feat_from_ids(subtests, data):
     dataset = Dataset(feature=data.feature, label=data.lsc)
     test_list = [["a", "c"], ["d"], ["a", "b", "c", "d", "e"]]
```

### Comparing `obnb-0.1.0/test/test_graph.py` & `obnb-0.1.0.dev1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/test/test_metric.py` & `obnb-0.1.0.dev1/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/test/test_model.py` & `obnb-0.1.0.dev1/test/test_model.py`

 * *Files identical despite different names*

### Comparing `obnb-0.1.0/test/test_wrapper.py` & `obnb-0.1.0.dev1/test/test_wrapper.py`

 * *Files identical despite different names*

