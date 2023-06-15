# Comparing `tmp/neon-skill-spelling-0.1.1a1.tar.gz` & `tmp/neon-skill-spelling-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-spelling-0.1.1a1.tar", last modified: Thu Jun 15 22:03:16 2023, max compression
+gzip compressed data, was "neon-skill-spelling-0.1.1a2.tar", last modified: Thu Jun 15 22:08:07 2023, max compression
```

## Comparing `neon-skill-spelling-0.1.1a1.tar` & `neon-skill-spelling-0.1.1a2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-15 22:03:16.000000 neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 22:03:16.000000 neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:03:16.000000 neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 22:03:16.000000 neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:03:16.000000 neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:03:16.000000 neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.073614 neon-skill-spelling-0.1.1a1/regex/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/ca-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/da-dk/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/da-dk/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/de-de/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/el-gr/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/el-gr/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/en-us/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/es-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/fa-ir/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/fr-fr/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/gl-es/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/gl-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/hu-hu/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/it-it/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/nl-nl/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/pl-pl/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/pt-br/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/pt-br/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/ro-ro/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/ru-ru/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/sv-se/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/sv-se/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/regex/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/regex/tr-tr/word.rx
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/skill.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.073614 neon-skill-spelling-0.1.1a1/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/ca-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/da-dk/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/da-dk/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/de-de/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/el-gr/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/el-gr/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/en-us/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/es-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/fa-ir/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/fr-fr/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/gl-es/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/gl-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/hu-hu/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/it-it/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/nl-nl/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/pl-pl/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/pt-br/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/pt-br/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/ro-ro/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/ru-ru/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/sv-se/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/sv-se/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:03:16.077614 neon-skill-spelling-0.1.1a1/vocab/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:03:12.000000 neon-skill-spelling-0.1.1a1/vocab/tr-tr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-15 22:08:07.000000 neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 22:08:07.000000 neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:08:07.000000 neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 22:08:07.000000 neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:08:07.000000 neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:08:07.000000 neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.059785 neon-skill-spelling-0.1.1a2/regex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/ca-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/da-dk/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/de-de/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/el-gr/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/en-us/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/es-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/fa-ir/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/fr-fr/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/gl-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/hu-hu/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/it-it/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/nl-nl/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/pl-pl/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/pt-br/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/ro-ro/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/regex/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/ru-ru/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/regex/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/sv-se/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/regex/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/regex/tr-tr/word.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/skill.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.063784 neon-skill-spelling-0.1.1a2/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/ca-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/da-dk/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/de-de/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/el-gr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/en-us/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/es-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/fa-ir/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/fr-fr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/gl-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/hu-hu/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/it-it/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/nl-nl/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/pl-pl/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/pt-br/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/ro-ro/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/ru-ru/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/sv-se/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:08:07.067784 neon-skill-spelling-0.1.1a2/vocab/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:08:02.000000 neon-skill-spelling-0.1.1a2/vocab/tr-tr/Spell.voc
```

### Comparing `neon-skill-spelling-0.1.1a1/LICENSE` & `neon-skill-spelling-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-0.1.1a1/LICENSE.md` & `neon-skill-spelling-0.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-0.1.1a1/PKG-INFO` & `neon-skill-spelling-0.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-spelling
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-spelling
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-spelling-0.1.1a1/README.md` & `neon-skill-spelling-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-0.1.1a1/__init__.py` & `neon-skill-spelling-0.1.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/PKG-INFO` & `neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-spelling
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-spelling
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-spelling-0.1.1a1/neon_skill_spelling.egg-info/SOURCES.txt` & `neon-skill-spelling-0.1.1a2/neon_skill_spelling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-0.1.1a1/setup.py` & `neon-skill-spelling-0.1.1a2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-spelling"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:SpellingSkill'
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
@@ -55,31 +55,31 @@
                     r.replace("github.com",
                               f"{getenv('GITHUB_TOKEN')}@github.com")
     return requirements
 
 
 def find_resource_files():
     resource_base_dirs = ("locale", "ui", "vocab", "dialog", "regex")
-    base_dir = path.dirname(__file__)
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
```

### Comparing `neon-skill-spelling-0.1.1a1/skill.json` & `neon-skill-spelling-0.1.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-0.1.1a1/version.py` & `neon-skill-spelling-0.1.1a2/version.py`

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

