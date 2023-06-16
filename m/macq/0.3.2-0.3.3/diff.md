# Comparing `tmp/macq-0.3.2.tar.gz` & `tmp/macq-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macq-0.3.2.tar", last modified: Fri May 26 19:44:29 2023, max compression
+gzip compressed data, was "macq-0.3.3.tar", last modified: Fri Jun 16 19:19:04 2023, max compression
```

## Comparing `macq-0.3.2.tar` & `macq-0.3.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.606325 macq-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 19:43:50.000000 macq-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-26 19:44:29.606325 macq-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-26 19:43:50.000000 macq-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.586324 macq-0.3.2/macq/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 19:43:50.000000 macq-0.3.2/macq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.594325 macq-0.3.2/macq/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/amdn.py
--rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/arms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/learned_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/learned_fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    31604 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/locm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/slaf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.594325 macq-0.3.2/macq/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.594325 macq-0.3.2/macq/generate/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/fd_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/planning_domains_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/random_goal_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/trace_from_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/vanilla_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.598325 macq-0.3.2/macq/observation/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/action_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/atomic_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/id_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/identity_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/noisy_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/noisy_partial_disordered_parallel_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/noisy_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/observed_tracelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/partial_observation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.602325 macq-0.3.2/macq/trace/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/disordered_parallel_actions_observation_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/partial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/trace_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.606325 macq-0.3.2/macq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/common_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/complex_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/pysat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/tokenization_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/tokenization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/trace_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/trace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.590324 macq-0.3.2/macq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 19:43:50.000000 macq-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:44:29.606325 macq-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-26 19:43:50.000000 macq-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.606325 macq-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-26 19:43:50.000000 macq-0.3.2/tests/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 19:18:40.000000 macq-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-16 19:19:04.689309 macq-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-16 19:18:40.000000 macq-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.681309 macq-0.3.3/macq/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 19:18:40.000000 macq-0.3.3/macq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/amdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/arms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/learned_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/learned_fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31588 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/locm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-06-16 19:18:40.000000 macq-0.3.3/macq/extract/slaf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/generate/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/fd_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/planning_domains_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/random_goal_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/trace_from_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/pddl/vanilla_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-16 19:18:40.000000 macq-0.3.3/macq/generate/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.685309 macq-0.3.3/macq/observation/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/action_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/atomic_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/id_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/identity_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/noisy_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/noisy_partial_disordered_parallel_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/noisy_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/observed_tracelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-16 19:18:40.000000 macq-0.3.3/macq/observation/partial_observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/macq/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/disordered_parallel_actions_observation_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/partial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 19:18:40.000000 macq-0.3.3/macq/trace/trace_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/macq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/complex_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/tokenization_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/tokenization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/trace_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-16 19:18:40.000000 macq-0.3.3/macq/utils/trace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.681309 macq-0.3.3/macq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 19:19:04.000000 macq-0.3.3/macq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 19:18:40.000000 macq-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 19:19:04.689309 macq-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-16 19:18:40.000000 macq-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:19:04.689309 macq-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-16 19:18:40.000000 macq-0.3.3/tests/test_readme.py
```

### Comparing `macq-0.3.2/LICENSE` & `macq-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/PKG-INFO` & `macq-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.2
+Version: 0.3.3
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.2/README.md` & `macq-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/__init__.py` & `macq-0.3.3/macq/extract/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,28 @@
 
 from .learned_fluent import LearnedFluent, LearnedLiftedFluent
 from .learned_action import LearnedAction, LearnedLiftedAction
 from .model import Model, LearnedAction
 from .extract import Extract, modes
 from .exceptions import IncompatibleObservationToken
 from .model import Model
+from .amdn import AMDN
+from .arms import ARMS
+from .locm import LOCM
+from .slaf import SLAF
+from .observer import Observer
 
 __all__ = [
     "LearnedAction",
     "LearnedLiftedAction",
     "LearnedFluent",
     "LearnedLiftedFluent",
     "Model",
     "Extract",
     "modes",
     "IncompatibleObservationToken",
+    "ARMS",
+    "AMDN",
+    "LOCM",
+    "SLAF",
+    "Observer",
 ]
```

### Comparing `macq-0.3.2/macq/extract/amdn.py` & `macq-0.3.3/macq/extract/amdn.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/arms.py` & `macq-0.3.3/macq/extract/arms.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/exceptions.py` & `macq-0.3.3/macq/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/extract.py` & `macq-0.3.3/macq/extract/extract.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Dict, List, Union
 
 from ..observation import ObservedTraceList
 from ..trace import Action, State
+from .model import Model
+
 from .amdn import AMDN
 from .arms import ARMS
 from .locm import LOCM
-from .model import Model
-from .observer import Observer
 from .slaf import SLAF
-
+from .observer import Observer
 
 @dataclass
 class SAS:
     pre_state: State
     action: Action
     post_state: State
```

### Comparing `macq-0.3.2/macq/extract/learned_action.py` & `macq-0.3.3/macq/extract/learned_action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/learned_fluent.py` & `macq-0.3.3/macq/extract/learned_fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/locm.py` & `macq-0.3.3/macq/extract/locm.py`

 * *Files 1% similar despite different names*

```diff
@@ -716,15 +716,15 @@
             print()
 
             print("OS:")
             pprint(OS)
             print()
 
             print("bindings:")
-            pprint(bindings[sorts["rooma"]])
+            pprint(bindings)
             print()
 
         bound_param_sorts = {
             sort: {
                 state: [
                     binding.hypothesis.G_
                     for binding in bindings.get(sort, {}).get(state, [])
```

### Comparing `macq-0.3.2/macq/extract/model.py` & `macq-0.3.3/macq/extract/model.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/observer.py` & `macq-0.3.3/macq/extract/observer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/extract/slaf.py` & `macq-0.3.3/macq/extract/slaf.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/csv.py` & `macq-0.3.3/macq/generate/csv.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/pddl/fd_random_walk.py` & `macq-0.3.3/macq/generate/pddl/fd_random_walk.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/pddl/generator.py` & `macq-0.3.3/macq/generate/pddl/generator.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/pddl/planning_domains_api.py` & `macq-0.3.3/macq/generate/pddl/planning_domains_api.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/pddl/random_goal_sampling.py` & `macq-0.3.3/macq/generate/pddl/random_goal_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/pddl/trace_from_goal.py` & `macq-0.3.3/macq/generate/pddl/trace_from_goal.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/pddl/vanilla_sampling.py` & `macq-0.3.3/macq/generate/pddl/vanilla_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/generate/plan.py` & `macq-0.3.3/macq/generate/plan.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/__init__.py` & `macq-0.3.3/macq/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/action_observation.py` & `macq-0.3.3/macq/observation/action_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/atomic_partial_observation.py` & `macq-0.3.3/macq/observation/atomic_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/identity_observation.py` & `macq-0.3.3/macq/observation/identity_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/noisy_observation.py` & `macq-0.3.3/macq/observation/noisy_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/noisy_partial_disordered_parallel_observation.py` & `macq-0.3.3/macq/observation/noisy_partial_disordered_parallel_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/noisy_partial_observation.py` & `macq-0.3.3/macq/observation/noisy_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/observation.py` & `macq-0.3.3/macq/observation/observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/observed_tracelist.py` & `macq-0.3.3/macq/observation/observed_tracelist.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/observation/partial_observation.py` & `macq-0.3.3/macq/observation/partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/__init__.py` & `macq-0.3.3/macq/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/action.py` & `macq-0.3.3/macq/trace/action.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/disordered_parallel_actions_observation_lists.py` & `macq-0.3.3/macq/trace/disordered_parallel_actions_observation_lists.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/fluent.py` & `macq-0.3.3/macq/trace/fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/state.py` & `macq-0.3.3/macq/trace/state.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/step.py` & `macq-0.3.3/macq/trace/step.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/trace.py` & `macq-0.3.3/macq/trace/trace.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/trace/trace_list.py` & `macq-0.3.3/macq/trace/trace_list.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/utils/__init__.py` & `macq-0.3.3/macq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/utils/progress.py` & `macq-0.3.3/macq/utils/progress.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/utils/pysat.py` & `macq-0.3.3/macq/utils/pysat.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/utils/timer.py` & `macq-0.3.3/macq/utils/timer.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/utils/trace_errors.py` & `macq-0.3.3/macq/utils/trace_errors.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq/utils/trace_utils.py` & `macq-0.3.3/macq/utils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/macq.egg-info/PKG-INFO` & `macq-0.3.3/macq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.3.2
+Version: 0.3.3
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
```

### Comparing `macq-0.3.2/macq.egg-info/SOURCES.txt` & `macq-0.3.3/macq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macq-0.3.2/setup.py` & `macq-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.2"
+VERSION = "0.3.3"
 
 NAME = "macq"
 
 DESCRIPTION = "Action model acquisition from state trace data."
 
 DEPENDENCIES = [
     "tarski",
```

### Comparing `macq-0.3.2/tests/test_readme.py` & `macq-0.3.3/tests/test_readme.py`

 * *Files identical despite different names*

