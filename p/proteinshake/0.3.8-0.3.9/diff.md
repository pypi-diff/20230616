# Comparing `tmp/proteinshake-0.3.8.tar.gz` & `tmp/proteinshake-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinshake-0.3.8.tar", last modified: Fri Mar 24 14:25:49 2023, max compression
+gzip compressed data, was "proteinshake-0.3.9.tar", last modified: Fri Mar 24 16:14:50 2023, max compression
```

## Comparing `proteinshake-0.3.8.tar` & `proteinshake-0.3.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.227697 proteinshake-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-24 14:25:36.000000 proteinshake-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-03-24 14:25:49.227697 proteinshake-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-24 14:25:36.000000 proteinshake-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.219696 proteinshake-0.3.8/proteinshake/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.223696 proteinshake-0.3.8/proteinshake/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/alphafold.py
--rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/enzyme_commission.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/gene_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/protein_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/protein_ligand_decoys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/protein_ligand_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/protein_protein_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/rcsb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/scop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/datasets/tm_align.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.223696 proteinshake-0.3.8/proteinshake/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/dgl.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/np.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/nx.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/frameworks/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.223696 proteinshake-0.3.8/proteinshake/representations/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/representations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/representations/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/representations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/representations/voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.227697 proteinshake-0.3.8/proteinshake/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/binding_site_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/enzyme_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/gene_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/ligand_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/pfam_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/protein_protein_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/structural_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/structure_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/structure_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/tasks/virtual_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.227697 proteinshake-0.3.8/proteinshake/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/transforms/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/transforms/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.227697 proteinshake-0.3.8/proteinshake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/utils/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-24 14:25:36.000000 proteinshake-0.3.8/proteinshake/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.223696 proteinshake-0.3.8/proteinshake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-03-24 14:25:49.000000 proteinshake-0.3.8/proteinshake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-24 14:25:49.000000 proteinshake-0.3.8/proteinshake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 14:25:49.000000 proteinshake-0.3.8/proteinshake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-24 14:25:49.000000 proteinshake-0.3.8/proteinshake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-24 14:25:49.000000 proteinshake-0.3.8/proteinshake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-24 14:25:49.227697 proteinshake-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-24 14:25:36.000000 proteinshake-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:49.227697 proteinshake-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 14:25:36.000000 proteinshake-0.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-24 14:25:36.000000 proteinshake-0.3.8/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-24 14:25:36.000000 proteinshake-0.3.8/tests/test_frameworks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-24 14:25:36.000000 proteinshake-0.3.8/tests/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-03-24 14:25:36.000000 proteinshake-0.3.8/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-24 14:25:36.000000 proteinshake-0.3.8/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.966511 proteinshake-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-24 16:14:39.000000 proteinshake-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-03-24 16:14:50.966511 proteinshake-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-24 16:14:39.000000 proteinshake-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.958511 proteinshake-0.3.9/proteinshake/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.962511 proteinshake-0.3.9/proteinshake/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/alphafold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/enzyme_commission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/gene_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/protein_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/protein_ligand_decoys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/protein_ligand_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/protein_protein_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/rcsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/scop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/datasets/tm_align.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.962511 proteinshake-0.3.9/proteinshake/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/dgl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/frameworks/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.962511 proteinshake-0.3.9/proteinshake/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/representations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/representations/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/representations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/representations/voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.966511 proteinshake-0.3.9/proteinshake/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/binding_site_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/enzyme_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/gene_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/ligand_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/pfam_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/protein_protein_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/structural_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/structure_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/structure_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/tasks/virtual_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.966511 proteinshake-0.3.9/proteinshake/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/transforms/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/transforms/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.966511 proteinshake-0.3.9/proteinshake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/utils/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-24 16:14:40.000000 proteinshake-0.3.9/proteinshake/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.958511 proteinshake-0.3.9/proteinshake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-03-24 16:14:50.000000 proteinshake-0.3.9/proteinshake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-24 16:14:50.000000 proteinshake-0.3.9/proteinshake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:14:50.000000 proteinshake-0.3.9/proteinshake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-24 16:14:50.000000 proteinshake-0.3.9/proteinshake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-24 16:14:50.000000 proteinshake-0.3.9/proteinshake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-24 16:14:50.966511 proteinshake-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-24 16:14:40.000000 proteinshake-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:50.966511 proteinshake-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:14:40.000000 proteinshake-0.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-24 16:14:40.000000 proteinshake-0.3.9/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-24 16:14:40.000000 proteinshake-0.3.9/tests/test_frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-24 16:14:40.000000 proteinshake-0.3.9/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-03-24 16:14:40.000000 proteinshake-0.3.9/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-24 16:14:40.000000 proteinshake-0.3.9/tests/test_transforms.py
```

### Comparing `proteinshake-0.3.8/LICENSE` & `proteinshake-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/PKG-INFO` & `proteinshake-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinshake
-Version: 0.3.8
+Version: 0.3.9
 Summary: Deep learning ready datasets of 3D protein structures.
 Home-page: https://proteinshake.readthedocs.io/en/latest/index.html
 Author: Tim Kucera, Carlos Oliver, Dexiong Chen, Karsten Borgwardt
 Author-email: kucera@biochem.mpg.de
 Keywords: bioinformatics,deep-learning,computational-biology,macromolecular-structure
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinshake Version: 0.3.8 Summary: Deep learning
+Metadata-Version: 2.1 Name: proteinshake Version: 0.3.9 Summary: Deep learning
 ready datasets of 3D protein structures. Home-page: https://
 proteinshake.readthedocs.io/en/latest/index.html Author: Tim Kucera, Carlos
 Oliver, Dexiong Chen, Karsten Borgwardt Author-email: kucera@biochem.mpg.de
 Keywords: bioinformatics,deep-learning,computational-biology,macromolecular-
 structure Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `proteinshake-0.3.8/README.md` & `proteinshake-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/__init__.py` & `proteinshake-0.3.9/proteinshake/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/alphafold.py` & `proteinshake-0.3.9/proteinshake/datasets/alphafold.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/dataset.py` & `proteinshake-0.3.9/proteinshake/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/enzyme_commission.py` & `proteinshake-0.3.9/proteinshake/datasets/enzyme_commission.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/gene_ontology.py` & `proteinshake-0.3.9/proteinshake/datasets/gene_ontology.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/protein_family.py` & `proteinshake-0.3.9/proteinshake/datasets/protein_family.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/protein_ligand_decoys.py` & `proteinshake-0.3.9/proteinshake/datasets/protein_ligand_decoys.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/protein_ligand_interface.py` & `proteinshake-0.3.9/proteinshake/datasets/protein_ligand_interface.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/protein_protein_interface.py` & `proteinshake-0.3.9/proteinshake/datasets/protein_protein_interface.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/rcsb.py` & `proteinshake-0.3.9/proteinshake/datasets/rcsb.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/scop.py` & `proteinshake-0.3.9/proteinshake/datasets/scop.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/datasets/tm_align.py` & `proteinshake-0.3.9/proteinshake/datasets/tm_align.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/frameworks/dataset.py` & `proteinshake-0.3.9/proteinshake/frameworks/dataset.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/frameworks/np.py` & `proteinshake-0.3.9/proteinshake/frameworks/np.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/frameworks/pyg.py` & `proteinshake-0.3.9/proteinshake/frameworks/pyg.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/frameworks/tf.py` & `proteinshake-0.3.9/proteinshake/frameworks/tf.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/frameworks/torch.py` & `proteinshake-0.3.9/proteinshake/frameworks/torch.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/representations/graph.py` & `proteinshake-0.3.9/proteinshake/representations/graph.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/representations/point.py` & `proteinshake-0.3.9/proteinshake/representations/point.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/representations/voxel.py` & `proteinshake-0.3.9/proteinshake/representations/voxel.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/__init__.py` & `proteinshake-0.3.9/proteinshake/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/binding_site_detection.py` & `proteinshake-0.3.9/proteinshake/tasks/binding_site_detection.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/enzyme_class.py` & `proteinshake-0.3.9/proteinshake/tasks/enzyme_class.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/gene_ontology.py` & `proteinshake-0.3.9/proteinshake/tasks/gene_ontology.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/ligand_affinity.py` & `proteinshake-0.3.9/proteinshake/tasks/ligand_affinity.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/pfam_task.py` & `proteinshake-0.3.9/proteinshake/tasks/pfam_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from sklearn import metrics
 from functools import cached_property
+import numpy as np
 
 from proteinshake.datasets import ProteinFamilyDataset
 from proteinshake.tasks import Task
 
 class ProteinFamilyTask(Task):
     """ Predict the protein family classification of a protein structure. This is a protein-level multi-class prediction.
 
@@ -38,13 +39,15 @@
         return 20
 
     def target(self, protein):
         return self.token_map[protein['protein']['Pfam'][0]]
 
     def evaluate(self, y_true, y_pred):
         """ Using metrics from https://doi.org/10.1073/pnas.1821905116 """
+        y_true = np.array(y_true, dtype=int)
+        y_pred = np.array(y_pred, dtype=int)
         return {
             'precision': metrics.precision_score(y_true, y_pred, average='macro', zero_division=0),
             'recall': metrics.recall_score(y_true, y_pred, average='macro', zero_division=0),
             'accuracy': metrics.accuracy_score(y_true, y_pred),
             #'AUROC': metrics.roc_auc_score(y_true, y_pred, average='macro', multi_class='ovo'),
         }
```

### Comparing `proteinshake-0.3.8/proteinshake/tasks/protein_protein_interface.py` & `proteinshake-0.3.9/proteinshake/tasks/protein_protein_interface.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/structural_class.py` & `proteinshake-0.3.9/proteinshake/tasks/structural_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from sklearn import metrics
 from functools import cached_property
+import numpy as np
 
 from proteinshake.datasets import SCOPDataset
 from proteinshake.tasks import Task
 
 class StructuralClassTask(Task):
     """ Predict the SCOP class of a protein structure. This is a protein-level multi-class prediction.
 
@@ -38,13 +39,15 @@
         return 20
 
     def target(self, protein):
         return self.token_map[protein['protein'][self.scop_level]]
 
     def evaluate(self, y_true, y_pred):
         """ Using metrics from https://doi.org/10.1073/pnas.1821905116 """
+        y_true = np.array(y_true, dtype=int)
+        y_pred = np.array(y_pred, dtype=int)
         return {
             'precision': metrics.precision_score(y_true, y_pred, average='macro', zero_division=0),
             'recall': metrics.recall_score(y_true, y_pred, average='macro', zero_division=0),
             'accuracy': metrics.accuracy_score(y_true, y_pred),
             #'AUROC': metrics.roc_auc_score(self.test_targets, y_pred, average='macro', multi_class='ovo'),
         }
```

### Comparing `proteinshake-0.3.8/proteinshake/tasks/structure_search.py` & `proteinshake-0.3.9/proteinshake/tasks/structure_search.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/structure_similarity.py` & `proteinshake-0.3.9/proteinshake/tasks/structure_similarity.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/task.py` & `proteinshake-0.3.9/proteinshake/tasks/task.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/tasks/virtual_screen.py` & `proteinshake-0.3.9/proteinshake/tasks/virtual_screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     """
 
     DatasetClass = ProteinLigandDecoysDataset
 
     def __init__(self, *args, **kwargs):
         kwargs['split'] = 'none'
         super().__init__(*args, **kwargs)
+        self.test_targets = [self.target(p) for p in self.proteins]
 
     @property
     def task_type(self):
         return ('protein', 'virtual_screen')
 
     def target(self, protein):
         """ The target here is a sorted list of smiles where the true ligands
@@ -93,9 +94,9 @@
 
             scores_dict = {lig_ids[i]: score for i, score in enumerate(y_pred[i])}
             ranks_dict = {lig_id: i < cutoff_index for i, lig_id in  enumerate(sorted(lig_ids, key = lambda x: scores_dict[x]))}
 
             mean_active_rank = np.mean([ranks_dict[lig_id] for lig_id in active_ids])
             efs.append(mean_active_rank)
 
-        return {'enrichment_factor-@{self.cutoff_fraction}': np.mean(efs)}
+        return {f'enrichment_factor-@{cutoff_fraction}': np.mean(efs)}
```

### Comparing `proteinshake-0.3.8/proteinshake/transforms/coords.py` & `proteinshake-0.3.9/proteinshake/transforms/coords.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/transforms/transforms.py` & `proteinshake-0.3.9/proteinshake/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/utils/embeddings.py` & `proteinshake-0.3.9/proteinshake/utils/embeddings.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/utils/io.py` & `proteinshake-0.3.9/proteinshake/utils/io.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake/utils/similarity.py` & `proteinshake-0.3.9/proteinshake/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/proteinshake.egg-info/PKG-INFO` & `proteinshake-0.3.9/proteinshake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinshake
-Version: 0.3.8
+Version: 0.3.9
 Summary: Deep learning ready datasets of 3D protein structures.
 Home-page: https://proteinshake.readthedocs.io/en/latest/index.html
 Author: Tim Kucera, Carlos Oliver, Dexiong Chen, Karsten Borgwardt
 Author-email: kucera@biochem.mpg.de
 Keywords: bioinformatics,deep-learning,computational-biology,macromolecular-structure
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinshake Version: 0.3.8 Summary: Deep learning
+Metadata-Version: 2.1 Name: proteinshake Version: 0.3.9 Summary: Deep learning
 ready datasets of 3D protein structures. Home-page: https://
 proteinshake.readthedocs.io/en/latest/index.html Author: Tim Kucera, Carlos
 Oliver, Dexiong Chen, Karsten Borgwardt Author-email: kucera@biochem.mpg.de
 Keywords: bioinformatics,deep-learning,computational-biology,macromolecular-
 structure Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `proteinshake-0.3.8/proteinshake.egg-info/SOURCES.txt` & `proteinshake-0.3.9/proteinshake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/setup.cfg` & `proteinshake-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/setup.py` & `proteinshake-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 URL = 'https://proteinshake.readthedocs.io/en/latest/index.html'
 
 install_requires = [
     'biopandas>=0.4.1',
     'pandas>=1.4.3',
     'rdkit-pypi>=2022.3.3',
     'tqdm>=4.64.0',
```

### Comparing `proteinshake-0.3.8/tests/test_datasets.py` & `proteinshake-0.3.9/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/tests/test_frameworks.py` & `proteinshake-0.3.9/tests/test_frameworks.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/tests/test_preprocess.py` & `proteinshake-0.3.9/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/tests/test_tasks.py` & `proteinshake-0.3.9/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `proteinshake-0.3.8/tests/test_transforms.py` & `proteinshake-0.3.9/tests/test_transforms.py`

 * *Files identical despite different names*

