# Comparing `tmp/neon-skill-instructions-0.1.1a1.tar.gz` & `tmp/neon-skill-instructions-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-instructions-0.1.1a1.tar", last modified: Thu Jun 15 22:37:11 2023, max compression
+gzip compressed data, was "neon-skill-instructions-0.1.1a2.tar", last modified: Thu Jun 15 22:40:26 2023, max compression
```

## Comparing `neon-skill-instructions-0.1.1a1.tar` & `neon-skill-instructions-0.1.1a2.tar`

### file list

```diff
@@ -1,71 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.720073 neon-skill-instructions-0.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 22:37:11.720073 neon-skill-instructions-0.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/instruction_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.712073 neon-skill-instructions-0.1.1a1/instructions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.712073 neon-skill-instructions-0.1.1a1/instructions/en/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/instructions/en/demo1_en-us.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/instructions/en/demo2_en-us.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.712073 neon-skill-instructions-0.1.1a1/instructions/pl/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/instructions/pl/demo1_pl.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/instructions/pl/demo2_pl.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.712073 neon-skill-instructions-0.1.1a1/instructions/uk/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/instructions/uk/demo1_uk.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/instructions/uk/demo2_uk.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.712073 neon-skill-instructions-0.1.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.716073 neon-skill-instructions-0.1.1a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/cancel.voc
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/choose.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/file_exists.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/finished.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/instruction_names.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/instructions_keyword.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/no_file.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/no_instruction.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/repeat.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/run_instructions.intent
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/start.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/en-us/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.716073 neon-skill-instructions-0.1.1a1/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/choose.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/file_exists.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/finished.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/instruction_names.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/instructions_keyword.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/no_file.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/no_instruction.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/repeat.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/run_instructions.intent
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/start.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/pl-pl/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.720073 neon-skill-instructions-0.1.1a1/locale/uk-uk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/choose.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/file_exists.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/finished.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/instruction_names.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/instructions_keyword.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/no_file.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/no_instruction.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/repeat.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/run_instructions.intent
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/start.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/locale/uk-uk/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.720073 neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 22:37:11.000000 neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-15 22:37:11.000000 neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:37:11.000000 neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 22:37:11.000000 neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:37:11.000000 neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:37:11.000000 neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:37:11.720073 neon-skill-instructions-0.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:37:11.720073 neon-skill-instructions-0.1.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:37:07.000000 neon-skill-instructions-0.1.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:26.642637 neon-skill-instructions-0.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 22:40:26.642637 neon-skill-instructions-0.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/instruction_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:26.638636 neon-skill-instructions-0.1.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:26.638636 neon-skill-instructions-0.1.1a2/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/cancel.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/choose.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/file_exists.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/finished.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/instruction_names.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/instructions_keyword.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/no_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/no_instruction.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/repeat.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/run_instructions.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/start.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:26.638636 neon-skill-instructions-0.1.1a2/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/choose.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/file_exists.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/finished.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/instruction_names.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/instructions_keyword.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/no_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/no_instruction.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/repeat.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/run_instructions.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/start.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/pl-pl/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:26.642637 neon-skill-instructions-0.1.1a2/locale/uk-uk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/choose.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/file_exists.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/finished.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/instruction_names.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/instructions_keyword.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/no_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/no_instruction.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/repeat.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/run_instructions.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/start.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/locale/uk-uk/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:26.642637 neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 22:40:26.000000 neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-15 22:40:26.000000 neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:40:26.000000 neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 22:40:26.000000 neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:40:26.000000 neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:40:26.000000 neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:40:26.642637 neon-skill-instructions-0.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:40:26.642637 neon-skill-instructions-0.1.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:40:22.000000 neon-skill-instructions-0.1.1a2/version.py
```

### Comparing `neon-skill-instructions-0.1.1a1/LICENSE.md` & `neon-skill-instructions-0.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a1/PKG-INFO` & `neon-skill-instructions-0.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-instructions
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-instructions
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-instructions-0.1.1a1/README.md` & `neon-skill-instructions-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a1/__init__.py` & `neon-skill-instructions-0.1.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a1/instruction_checks.py` & `neon-skill-instructions-0.1.1a2/instruction_checks.py`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/PKG-INFO` & `neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-instructions
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-instructions
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-instructions-0.1.1a1/neon_skill_instructions.egg-info/SOURCES.txt` & `neon-skill-instructions-0.1.1a2/neon_skill_instructions.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 LICENSE.md
 README.md
 __init__.py
 instruction_checks.py
 setup.py
 skill.json
 version.py
-instructions/en/demo1_en-us.jsonl
-instructions/en/demo2_en-us.jsonl
-instructions/pl/demo1_pl.jsonl
-instructions/pl/demo2_pl.jsonl
-instructions/uk/demo1_uk.jsonl
-instructions/uk/demo2_uk.jsonl
 locale/en-us/cancel.voc
 locale/en-us/choose.dialog
 locale/en-us/file_exists.dialog
 locale/en-us/finished.dialog
 locale/en-us/instruction_names.dialog
 locale/en-us/instructions_keyword.voc
 locale/en-us/neon.voc
```

### Comparing `neon-skill-instructions-0.1.1a1/setup.py` & `neon-skill-instructions-0.1.1a2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-instructions"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:InstructionsSkill'
+BASE_PATH = path.abspath(path.dirname(__file__))
 
 
 def get_requirements(requirements_filename: str):
-    requirements_file = path.join(path.abspath(path.dirname(__file__)),
-                                  requirements_filename)
+    requirements_file = path.join(BASE_PATH, requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
         requirements = r.readlines()
     requirements = [r.strip() for r in requirements if r.strip()
                     and not r.strip().startswith("#")]
 
     for i in range(0, len(requirements)):
         r = requirements[i]
@@ -54,33 +54,32 @@
                 requirements[i] = \
                     r.replace("github.com",
                               f"{getenv('GITHUB_TOKEN')}@github.com")
     return requirements
 
 
 def find_resource_files():
-    resource_base_dirs = ("locale", "ui", "vocab", "dialog", "regex",
-                          "instructions")
-    base_dir = path.dirname(__file__)
+    resource_base_dirs = ("locale", "ui", "vocab", "dialog", "regex")
+    base_dir = BASE_PATH
     package_data = ["skill.json"]
     for res in resource_base_dirs:
         if path.isdir(path.join(base_dir, res)):
             for (directory, _, files) in walk(path.join(base_dir, res)):
                 if files:
                     package_data.append(
                         path.join(directory.replace(base_dir, "").lstrip('/'),
                                   '*'))
 #    print(package_data)
     return package_data
 
 
-with open("README.md", "r") as f:
+with open(path.join(BASE_PATH, "README.md"), "r") as f:
     long_description = f.read()
 
-with open("./version.py", "r", encoding="utf-8") as v:
+with open(path.join(BASE_PATH, "version.py"), "r", encoding="utf-8") as v:
     for line in v.readlines():
         if line.startswith("__version__"):
             if '"' in line:
                 version = line.split('"')[1]
             else:
                 version = line.split("'")[1]
 
@@ -95,8 +94,8 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={SKILL_PKG: ""},
     packages=[SKILL_PKG],
     package_data={SKILL_PKG: find_resource_files()},
     include_package_data=True,
     entry_points={"ovos.plugin.skill": PLUGIN_ENTRY_POINT}
-)
+)
```

### Comparing `neon-skill-instructions-0.1.1a1/skill.json` & `neon-skill-instructions-0.1.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a1/test/test_skill.py` & `neon-skill-instructions-0.1.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a1/version.py` & `neon-skill-instructions-0.1.1a2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a1"
+__version__ = "0.1.1a2"
```

