# Comparing `tmp/pyscal3-3.0.0.tar.gz` & `tmp/pyscal3-3.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal3-3.0.0.tar", last modified: Sat Apr 29 22:01:57 2023, max compression
+gzip compressed data, was "pyscal3-3.0.0.dev6.tar", last modified: Fri Jun 16 11:30:28 2023, max compression
```

## Comparing `pyscal3-3.0.0.tar` & `pyscal3-3.0.0.dev6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.361606 pyscal3-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-29 22:01:53.000000 pyscal3-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-29 22:01:53.000000 pyscal3-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-29 22:01:57.361606 pyscal3-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-29 22:01:53.000000 pyscal3-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.349605 pyscal3-3.0.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.349605 pyscal3-3.0.0/lib/voro++/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-29 22:01:53.000000 pyscal3-3.0.0/lib/voro++/voro++.cc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-29 22:01:53.000000 pyscal3-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 22:01:57.365606 pyscal3-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-29 22:01:53.000000 pyscal3-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.349605 pyscal3-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.353605 pyscal3-3.0.0/src/pyscal/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    49087 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/crystal_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/csl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.353605 pyscal3-3.0.0/src/pyscal/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/data/annotations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/data/element_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/data/structure_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.357606 pyscal3-3.0.0/src/pyscal/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/formats/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/formats/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/formats/mdtraj.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/formats/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/grain_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/modsystem_binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    38179 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/neighbor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.357606 pyscal3-3.0.0/src/pyscal/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/operations/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/operations/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/sh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/solids.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/structure_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/traj_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-29 22:01:53.000000 pyscal3-3.0.0/src/pyscal/voronoi.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.357606 pyscal3-3.0.0/src/pyscal3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-29 22:01:57.000000 pyscal3-3.0.0/src/pyscal3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-29 22:01:57.000000 pyscal3-3.0.0/src/pyscal3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 22:01:57.000000 pyscal3-3.0.0/src/pyscal3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 22:01:57.000000 pyscal3-3.0.0/src/pyscal3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-29 22:01:57.000000 pyscal3-3.0.0/src/pyscal3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 22:01:57.000000 pyscal3-3.0.0/src/pyscal3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 22:01:57.361606 pyscal3-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_angular.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_chiparams.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_crystal_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_disorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_nucsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_q12.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_q3.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_q_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_traj_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-29 22:01:53.000000 pyscal3-3.0.0/tests/test_voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-16 11:30:24.000000 pyscal3-3.0.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 11:30:24.000000 pyscal3-3.0.0.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-16 11:30:24.000000 pyscal3-3.0.0.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.543497 pyscal3-3.0.0.dev6/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.543497 pyscal3-3.0.0.dev6/lib/voro++/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/lib/voro++/voro++.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.543497 pyscal3-3.0.0.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.543497 pyscal3-3.0.0.dev6/src/pyscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49087 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/crystal_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/csl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/src/pyscal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/data/annotations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/data/element_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/data/structure_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/src/pyscal/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/formats/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/formats/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/formats/mdtraj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/formats/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/grain_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/modsystem_binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38179 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/neighbor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/src/pyscal/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/operations/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/operations/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/sh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/solids.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/structure_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/traj_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/src/pyscal/voronoi.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/src/pyscal3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-16 11:30:28.000000 pyscal3-3.0.0.dev6/src/pyscal3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-16 11:30:28.000000 pyscal3-3.0.0.dev6/src/pyscal3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:30:28.000000 pyscal3-3.0.0.dev6/src/pyscal3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:30:28.000000 pyscal3-3.0.0.dev6/src/pyscal3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 11:30:28.000000 pyscal3-3.0.0.dev6/src/pyscal3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 11:30:28.000000 pyscal3-3.0.0.dev6/src/pyscal3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:30:28.547497 pyscal3-3.0.0.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_chiparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_crystal_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_nucsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_q12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_q3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_q_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_traj_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-16 11:30:25.000000 pyscal3-3.0.0.dev6/tests/test_voronoi.py
```

### Comparing `pyscal3-3.0.0/LICENSE` & `pyscal3-3.0.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/PKG-INFO` & `pyscal3-3.0.0.dev6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal3
-Version: 3.0.0
+Version: 3.0.0.dev6
 Summary: Python library written in C++ for calculation of local atomic structural environment
 Home-page: https://pyscal.org
 Download-URL: https://anaconda.org/conda-forge/pyscal
 Author: Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal3-3.0.0/README.md` & `pyscal3-3.0.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/setup.py` & `pyscal3-3.0.0.dev6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal3',
-    version='3.0.0',
+    version='3.0.0.dev.6',
     author='Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Python library written in C++ for calculation of local atomic structural environment',
     long_description=readme,
     long_description_content_type = "text/markdown",
     # tell setuptools to look for any packages under 'src'
     packages=find_packages('src'),
```

### Comparing `pyscal3-3.0.0/src/pyscal/atoms.py` & `pyscal3-3.0.0.dev6/src/pyscal/atoms.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/attributes.py` & `pyscal3-3.0.0.dev6/src/pyscal/attributes.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/core.py` & `pyscal3-3.0.0.dev6/src/pyscal/core.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/crystal_structures.py` & `pyscal3-3.0.0.dev6/src/pyscal/crystal_structures.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/csl.py` & `pyscal3-3.0.0.dev6/src/pyscal/csl.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/data/annotations.yaml` & `pyscal3-3.0.0.dev6/src/pyscal/data/annotations.yaml`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/data/element_data.yaml` & `pyscal3-3.0.0.dev6/src/pyscal/data/element_data.yaml`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/data/structure_data.yaml` & `pyscal3-3.0.0.dev6/src/pyscal/data/structure_data.yaml`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/formats/ase.py` & `pyscal3-3.0.0.dev6/src/pyscal/formats/ase.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/formats/lammps.py` & `pyscal3-3.0.0.dev6/src/pyscal/formats/lammps.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/formats/mdtraj.py` & `pyscal3-3.0.0.dev6/src/pyscal/formats/mdtraj.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/formats/vasp.py` & `pyscal3-3.0.0.dev6/src/pyscal/formats/vasp.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/grain_boundary.py` & `pyscal3-3.0.0.dev6/src/pyscal/grain_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,18 @@
         self.gb_plane = gb_plane
         self.gb_index_limit = gb_index_limit
         valid = self.check_if_gb_is_valid(gb_plane)
         if not valid:
             raise TypeError("GB cannot be created with the given input!")
         return valid
     
-    def populate_grain_boundary(self, lattice, repetitions=(1,1,1), lattice_parameter=1, overlap=0.0):
+    def populate_grain_boundary(self, lattice, element=None, repetitions=(1,1,1), lattice_parameter=1, overlap=0.0):
         if lattice in pcs.structures.keys():
             structure = lattice
-            element = None
+            element = element
             basis = pcs.structures[lattice]['positions']
             sdict = pcs.structures[lattice]
         elif lattice in pcs.elements.keys():
             structure = pcs.elements[lattice]['structure']
             element = lattice
             lattice_parameter = pcs.elements[lattice]['lattice_constant']
             basis = pcs.structures[structure]['positions']
```

### Comparing `pyscal3-3.0.0/src/pyscal/misc.py` & `pyscal3-3.0.0.dev6/src/pyscal/misc.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/modsystem_binding.cpp` & `pyscal3-3.0.0.dev6/src/pyscal/modsystem_binding.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/neighbor.cpp` & `pyscal3-3.0.0.dev6/src/pyscal/neighbor.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/operations/operations.py` & `pyscal3-3.0.0.dev6/src/pyscal/operations/operations.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/operations/symmetry.py` & `pyscal3-3.0.0.dev6/src/pyscal/operations/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/routines.py` & `pyscal3-3.0.0.dev6/src/pyscal/routines.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/sh.cpp` & `pyscal3-3.0.0.dev6/src/pyscal/sh.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/solids.cpp` & `pyscal3-3.0.0.dev6/src/pyscal/solids.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/structure_creator.py` & `pyscal3-3.0.0.dev6/src/pyscal/structure_creator.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/traj_process.py` & `pyscal3-3.0.0.dev6/src/pyscal/traj_process.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/trajectory.py` & `pyscal3-3.0.0.dev6/src/pyscal/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/visualization.py` & `pyscal3-3.0.0.dev6/src/pyscal/visualization.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal/voronoi.cpp` & `pyscal3-3.0.0.dev6/src/pyscal/voronoi.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/src/pyscal3.egg-info/PKG-INFO` & `pyscal3-3.0.0.dev6/src/pyscal3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal3
-Version: 3.0.0
+Version: 3.0.0.dev6
 Summary: Python library written in C++ for calculation of local atomic structural environment
 Home-page: https://pyscal.org
 Download-URL: https://anaconda.org/conda-forge/pyscal
 Author: Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal3-3.0.0/src/pyscal3.egg-info/SOURCES.txt` & `pyscal3-3.0.0.dev6/src/pyscal3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_chiparams.py` & `pyscal3-3.0.0.dev6/tests/test_chiparams.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_disorder.py` & `pyscal3-3.0.0.dev6/tests/test_disorder.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_masking.py` & `pyscal3-3.0.0.dev6/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_neighbors.py` & `pyscal3-3.0.0.dev6/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_nucsize.py` & `pyscal3-3.0.0.dev6/tests/test_nucsize.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_q12.py` & `pyscal3-3.0.0.dev6/tests/test_q12.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_q_system.py` & `pyscal3-3.0.0.dev6/tests/test_q_system.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_read_file.py` & `pyscal3-3.0.0.dev6/tests/test_read_file.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_symmetry.py` & `pyscal3-3.0.0.dev6/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_system.py` & `pyscal3-3.0.0.dev6/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_traj_process.py` & `pyscal3-3.0.0.dev6/tests/test_traj_process.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.0.0/tests/test_voronoi.py` & `pyscal3-3.0.0.dev6/tests/test_voronoi.py`

 * *Files identical despite different names*

