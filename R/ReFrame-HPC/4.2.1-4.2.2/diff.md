# Comparing `tmp/ReFrame-HPC-4.2.1.tar.gz` & `tmp/ReFrame-HPC-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReFrame-HPC-4.2.1.tar", last modified: Fri May 26 19:57:16 2023, max compression
+gzip compressed data, was "ReFrame-HPC-4.2.2.tar", last modified: Fri Jun 16 16:23:46 2023, max compression
```

## Comparing `ReFrame-HPC-4.2.1.tar` & `ReFrame-HPC-4.2.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.368482 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.368482 ReFrame-HPC-4.2.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/bin/reframe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.368482 ReFrame-HPC-4.2.1/reframe/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.376482 ReFrame-HPC-4.2.1/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.376482 ReFrame-HPC-4.2.1/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    94467 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.380482 ReFrame-HPC-4.2.1/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.384482 ReFrame-HPC-4.2.1/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    55074 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.384482 ReFrame-HPC-4.2.1/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.384482 ReFrame-HPC-4.2.1/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.341693 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.341693 ReFrame-HPC-4.2.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/bin/reframe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.341693 ReFrame-HPC-4.2.2/reframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.353694 ReFrame-HPC-4.2.2/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23120 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.357694 ReFrame-HPC-4.2.2/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94662 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.357694 ReFrame-HPC-4.2.2/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.361694 ReFrame-HPC-4.2.2/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55077 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.361694 ReFrame-HPC-4.2.2/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/setup.cfg
```

### Comparing `ReFrame-HPC-4.2.1/LICENSE` & `ReFrame-HPC-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/PKG-INFO` & `ReFrame-HPC-4.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.2.1
+Version: 4.2.2
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/reframe-hpc/reframe?include_prereleases)
 ![GitHub commits since latest release](https://img.shields.io/github/commits-since/reframe-hpc/reframe/latest)
 ![GitHub contributors](https://img.shields.io/github/contributors-anon/reframe-hpc/reframe)<br/>
 [![PyPI version](https://badge.fury.io/py/ReFrame-HPC.svg)](https://badge.fury.io/py/ReFrame-HPC)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc)](https://pepy.tech/project/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc/month)](https://pepy.tech/project/reframe-hpc)<br/>
-[![Slack](https://reframe-slack.herokuapp.com/badge.svg)](https://reframe-slack.herokuapp.com/)<br/>
+[![Slack](https://badgen.net/badge/icon/slack?icon=slack&label)](https://join.slack.com/t/reframetalk/shared_invite/zt-1tar8s71w-At0tolJ~~zxT2oG_2Ly9sw)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![DOI](https://zenodo.org/badge/89384186.svg)](https://zenodo.org/badge/latestdoi/89384186)<br/>
 [![Twitter Follow](https://img.shields.io/twitter/follow/ReFrameHPC?style=social)](https://twitter.com/ReFrameHPC)
 
 # ReFrame in a Nutshell
 
 ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems.
```

### Comparing `ReFrame-HPC-4.2.1/README.md` & `ReFrame-HPC-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/README_minimal.md` & `ReFrame-HPC-4.2.2/README_minimal.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/reframe-hpc/reframe?include_prereleases)
 ![GitHub commits since latest release](https://img.shields.io/github/commits-since/reframe-hpc/reframe/latest)
 ![GitHub contributors](https://img.shields.io/github/contributors-anon/reframe-hpc/reframe)<br/>
 [![PyPI version](https://badge.fury.io/py/ReFrame-HPC.svg)](https://badge.fury.io/py/ReFrame-HPC)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc)](https://pepy.tech/project/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc/month)](https://pepy.tech/project/reframe-hpc)<br/>
-[![Slack](https://reframe-slack.herokuapp.com/badge.svg)](https://reframe-slack.herokuapp.com/)<br/>
+[![Slack](https://badgen.net/badge/icon/slack?icon=slack&label)](https://join.slack.com/t/reframetalk/shared_invite/zt-1tar8s71w-At0tolJ~~zxT2oG_2Ly9sw)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![DOI](https://zenodo.org/badge/89384186.svg)](https://zenodo.org/badge/latestdoi/89384186)<br/>
 [![Twitter Follow](https://img.shields.io/twitter/follow/ReFrameHPC?style=social)](https://twitter.com/ReFrameHPC)
 
 # ReFrame in a Nutshell
 
 ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems.
```

### Comparing `ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/PKG-INFO` & `ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.2.1
+Version: 4.2.2
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/reframe-hpc/reframe?include_prereleases)
 ![GitHub commits since latest release](https://img.shields.io/github/commits-since/reframe-hpc/reframe/latest)
 ![GitHub contributors](https://img.shields.io/github/contributors-anon/reframe-hpc/reframe)<br/>
 [![PyPI version](https://badge.fury.io/py/ReFrame-HPC.svg)](https://badge.fury.io/py/ReFrame-HPC)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc)](https://pepy.tech/project/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc/month)](https://pepy.tech/project/reframe-hpc)<br/>
-[![Slack](https://reframe-slack.herokuapp.com/badge.svg)](https://reframe-slack.herokuapp.com/)<br/>
+[![Slack](https://badgen.net/badge/icon/slack?icon=slack&label)](https://join.slack.com/t/reframetalk/shared_invite/zt-1tar8s71w-At0tolJ~~zxT2oG_2Ly9sw)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![DOI](https://zenodo.org/badge/89384186.svg)](https://zenodo.org/badge/latestdoi/89384186)<br/>
 [![Twitter Follow](https://img.shields.io/twitter/follow/ReFrameHPC?style=social)](https://twitter.com/ReFrameHPC)
 
 # ReFrame in a Nutshell
 
 ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems.
```

### Comparing `ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/SOURCES.txt` & `ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/bin/reframe` & `ReFrame-HPC-4.2.2/bin/reframe`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/__init__.py` & `ReFrame-HPC-4.2.2/reframe/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.2.1'
+VERSION = '4.2.2'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `ReFrame-HPC-4.2.1/reframe/core/backends.py` & `ReFrame-HPC-4.2.2/reframe/core/backends.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/buildsystems.py` & `ReFrame-HPC-4.2.2/reframe/core/buildsystems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/builtins.py` & `ReFrame-HPC-4.2.2/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/config.py` & `ReFrame-HPC-4.2.2/reframe/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import os
 import re
 import socket
 
 import reframe
 import reframe.core.settings as settings
 import reframe.utility as util
+import reframe.utility.jsonext as jsonext
 from reframe.core.environments import normalize_module_list
 from reframe.core.exceptions import ConfigError, ReframeFatalError
 from reframe.core.logging import getlogger
 from reframe.utility import ScopedDict
 
 
 def _match_option(opt, opt_map):
@@ -221,15 +222,15 @@
             return self._site_config
 
     def __repr__(self):
         return (f'{type(self).__name__}(site_config={self._site_config!r}, '
                 f'sources={self._sources!r})')
 
     def __str__(self):
-        return json.dumps(self._pick_config(), indent=2)
+        return jsonext.dumps(self._pick_config(), indent=2)
 
     # Delegate everything to either the original config or to the reduced one
     # if a system is selected
 
     def __iter__(self):
         return iter(self._pick_config())
```

### Comparing `ReFrame-HPC-4.2.1/reframe/core/containers.py` & `ReFrame-HPC-4.2.2/reframe/core/containers.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/decorators.py` & `ReFrame-HPC-4.2.2/reframe/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/deferrable.py` & `ReFrame-HPC-4.2.2/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/environments.py` & `ReFrame-HPC-4.2.2/reframe/core/environments.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/exceptions.py` & `ReFrame-HPC-4.2.2/reframe/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/fields.py` & `ReFrame-HPC-4.2.2/reframe/core/fields.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/fixtures.py` & `ReFrame-HPC-4.2.2/reframe/core/fixtures.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/hooks.py` & `ReFrame-HPC-4.2.2/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/launchers/__init__.py` & `ReFrame-HPC-4.2.2/reframe/core/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/launchers/local.py` & `ReFrame-HPC-4.2.2/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/launchers/mpi.py` & `ReFrame-HPC-4.2.2/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/launchers/ssh.py` & `ReFrame-HPC-4.2.2/reframe/core/launchers/ssh.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/logging.py` & `ReFrame-HPC-4.2.2/reframe/core/logging.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/meta.py` & `ReFrame-HPC-4.2.2/reframe/core/meta.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/modules.py` & `ReFrame-HPC-4.2.2/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/namespaces.py` & `ReFrame-HPC-4.2.2/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/parameters.py` & `ReFrame-HPC-4.2.2/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/pipeline.py` & `ReFrame-HPC-4.2.2/reframe/core/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,17 +194,17 @@
     #: :attr:`valid_systems` except that the ``a:b`` entries are invalid.
     #:
     #: :type: :class:`List[str]`
     #: :default: ``required``
     #:
     #: .. seealso::
     #:    - `Environment features
-    #:      <config_reference.html#environments-.features>`__
+    #:      <config_reference.html#config.environments.features>`__
     #:    - `Environment extras
-    #:      <config_reference.html#environments-.extras>`__
+    #:      <config_reference.html#config.environments.extras>`__
     #:
     #: .. versionchanged:: 2.12
     #:    Programming environments can now be specified using wildcards.
     #:
     #: .. versionchanged:: 2.17
     #:    Support for wildcards is dropped.
     #:
@@ -264,17 +264,17 @@
     #:    valid_systems = ['sys1', '-feat']
     #:
     #: :type: :class:`List[str]`
     #: :default: ``None``
     #:
     #: .. seealso::
     #:    - `System partition features
-    #:      <config_reference.html#systems-.partitions-.features>`__
+    #:      <config_reference.html#config.systems.partitions.features>`__
     #:    - `System partition extras
-    #:      <config_reference.html#systems-.partitions-.extras>`__
+    #:      <config_reference.html#config.systems.partitions.extras>`__
     #:
     #: .. versionchanged:: 3.3
     #:    Default value changed from ``[]`` to ``None``.
     #:
     #: .. versionchanged:: 3.6
     #:    Default value changed from ``None`` to ``required``.
     #:
@@ -1641,43 +1641,50 @@
             self._outputdir = runtime.make_outputdir(
                 self.current_system.name, self._current_partition.name,
                 self._current_environ.name, self.short_name
             )
         except OSError as e:
             raise PipelineError('failed to set up paths') from e
 
-    def _create_job(self, name, force_local=False, **job_opts):
+    def _create_job(self, job_type, force_local=False, **job_opts):
         '''Setup the job related to this check.'''
 
         if force_local:
             scheduler = getscheduler('local')()
             launcher = getlauncher('local')()
         else:
             scheduler = self._current_partition.scheduler
             launcher = self._current_partition.launcher_type()
 
         self.logger.debug(
-            f'Setting up job {name!r} '
+            f'Setting up {type} job for test {self.name!r} '
             f'(scheduler: {scheduler.registered_name!r}, '
             f'launcher: {launcher.registered_name!r})'
         )
+
+        if job_type == 'build':
+            script_name = 'rfm_build.sh'
+        elif job_type == 'run':
+            script_name = 'rfm_job.sh'
+
         return Job.create(scheduler,
                           launcher,
-                          name=name,
+                          name=f'rfm_{self.short_name}',
+                          script_filename=script_name,
                           workdir=self._stagedir,
                           sched_access=self._current_partition.access,
                           **job_opts)
 
     def _setup_build_job(self, **job_opts):
-        self._build_job = self._create_job(f'rfm_build',
-                                           self.local or self.build_locally,
-                                           **job_opts)
+        self._build_job = self._create_job(
+            'build', self.local or self.build_locally, **job_opts
+        )
 
     def _setup_run_job(self, **job_opts):
-        self._job = self._create_job(f'rfm_job', self.local, **job_opts)
+        self._job = self._create_job(f'run', self.local, **job_opts)
 
     def _setup_container_platform(self):
         try:
             self.container_platform.emit_prepare_commands(self.stagedir)
         except NotImplementedError:
             cplatf_name = self.current_partition.container_runtime
             if cplatf_name:
```

### Comparing `ReFrame-HPC-4.2.1/reframe/core/runtime.py` & `ReFrame-HPC-4.2.2/reframe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/__init__.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 
 #
 # Scheduler implementations
 #
 
 import abc
+import os
 import time
 
 import reframe.core.runtime as runtime
 import reframe.core.shell as shell
 import reframe.utility.jsonext as jsonext
 import reframe.utility.typecheck as typ
 from reframe.core.exceptions import JobError, JobNotStartedError
@@ -326,17 +327,19 @@
                  sched_flex_alloc_nodes=None,
                  sched_access=[],
                  sched_options=None):
 
         self._cli_options = list(sched_options) if sched_options else []
         self._name = name
         self._workdir = workdir
-        self._script_filename = script_filename or '%s.sh' % name
-        self._stdout = stdout or '%s.out' % name
-        self._stderr = stderr or '%s.err' % name
+        self._script_filename = script_filename or f'{name}.sh'
+
+        basename, _ = os.path.splitext(self._script_filename)
+        self._stdout = stdout or f'{basename}.out'
+        self._stderr = stderr or f'{basename}.err'
 
         # Backend scheduler related information
         self._sched_flex_alloc_nodes = sched_flex_alloc_nodes
         self._sched_access = sched_access
 
         # Live job information; to be filled during job's lifetime by the
         # scheduler
```

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/flux.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/local.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/lsf.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/oar.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/pbs.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/registry.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/sge.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/schedulers/slurm.py` & `ReFrame-HPC-4.2.2/reframe/core/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/settings.py` & `ReFrame-HPC-4.2.2/reframe/core/settings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/shell.py` & `ReFrame-HPC-4.2.2/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/systems.py` & `ReFrame-HPC-4.2.2/reframe/core/systems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/variables.py` & `ReFrame-HPC-4.2.2/reframe/core/variables.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/core/warnings.py` & `ReFrame-HPC-4.2.2/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/argparse.py` & `ReFrame-HPC-4.2.2/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/autodetect.py` & `ReFrame-HPC-4.2.2/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/ci.py` & `ReFrame-HPC-4.2.2/reframe/frontend/ci.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/cli.py` & `ReFrame-HPC-4.2.2/reframe/frontend/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,15 +827,15 @@
             default = {'token'}
             value = rt.get_option(config_param, default)
             if value is default:
                 printer.error(
                     f'no such configuration parameter found: {config_param}'
                 )
             else:
-                printer.info(json.dumps(value, indent=2))
+                printer.info(jsonext.dumps(value, indent=2))
 
         sys.exit(0)
 
     if options.detect_host_topology:
         from reframe.utility.cpuinfo import cpuinfo
 
         s_cpuinfo = cpuinfo()
```

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/dependencies.py` & `ReFrame-HPC-4.2.2/reframe/frontend/dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,22 @@
             pruned_graph.setdefault(node, util.OrderedSet())
             for adj in graph[node]:
                 pruned_graph[node].add(adj)
                 curr_depth += 1
                 if adj not in pruned_graph:
                     unvisited.append(adj)
 
+    # Re-calculate the in-degree of the pruned graph nodes
+    for u in pruned_graph:
+        u.in_degree = 0
+
+    for u, adjacent in pruned_graph.items():
+        for v in adjacent:
+            v.in_degree += 1
+
     return pruned_graph
 
 
 @time_function
 def toposort(graph, is_subgraph=False):
     '''Return a list of the graph nodes topologically sorted.
```

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/executors/__init__.py` & `ReFrame-HPC-4.2.2/reframe/frontend/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/executors/policies.py` & `ReFrame-HPC-4.2.2/reframe/frontend/executors/policies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/filters.py` & `ReFrame-HPC-4.2.2/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/loader.py` & `ReFrame-HPC-4.2.2/reframe/frontend/loader.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/printer.py` & `ReFrame-HPC-4.2.2/reframe/frontend/printer.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/runreport.py` & `ReFrame-HPC-4.2.2/reframe/frontend/runreport.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/statistics.py` & `ReFrame-HPC-4.2.2/reframe/frontend/statistics.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/frontend/testgenerators.py` & `ReFrame-HPC-4.2.2/reframe/frontend/testgenerators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/schemas/config.json` & `ReFrame-HPC-4.2.2/reframe/schemas/config.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/schemas/junit.xsd` & `ReFrame-HPC-4.2.2/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/schemas/runreport.json` & `ReFrame-HPC-4.2.2/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/__init__.py` & `ReFrame-HPC-4.2.2/reframe/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/color.py` & `ReFrame-HPC-4.2.2/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/cpuinfo.py` & `ReFrame-HPC-4.2.2/reframe/utility/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/jsonext.py` & `ReFrame-HPC-4.2.2/reframe/utility/jsonext.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
     if isinstance(obj, BaseException):
         return str(obj)
 
     if inspect.istraceback(obj):
         return traceback.format_tb(obj)
 
+    if inspect.isfunction(obj):
+        return f'py::{obj.__qualname__}'
+
     newobj = encode_dict(obj)
     if newobj is not None:
         return newobj
 
     return None
```

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/osext.py` & `ReFrame-HPC-4.2.2/reframe/utility/osext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/profile.py` & `ReFrame-HPC-4.2.2/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/sanity.py` & `ReFrame-HPC-4.2.2/reframe/utility/sanity.py`

 * *Files 0% similar despite different names*

```diff
@@ -786,15 +786,15 @@
 
 @deferrable
 def extractall_s(patt, string, tag=0, conv=None):
     '''Extract all values from the capturing group ``tag`` of a matching regex
     ``patt`` in ``string``.
 
     :arg patt: as in :func:`extractall`.
-'   :arg string: The string to examine.
+    :arg string: The string to examine.
     :arg tag: as in :func:`extractall`.
     :arg conv: as in :func:`extractall`.
     :returns: same as :func:`extractall`.
 
     .. versionadded:: 3.4.1
     '''
     return list(evaluate(x) for x in extractiter_s(patt, string, tag, conv))
```

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/typecheck.py` & `ReFrame-HPC-4.2.2/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/udeps.py` & `ReFrame-HPC-4.2.2/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/reframe/utility/versioning.py` & `ReFrame-HPC-4.2.2/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.1/setup.cfg` & `ReFrame-HPC-4.2.2/setup.cfg`

 * *Files identical despite different names*

