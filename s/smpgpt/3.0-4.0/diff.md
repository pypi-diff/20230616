# Comparing `tmp/smpgpt-3.0.tar.gz` & `tmp/smpgpt-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpgpt-3.0.tar", last modified: Fri Jun 16 20:55:10 2023, max compression
+gzip compressed data, was "smpgpt-4.0.tar", last modified: Fri Jun 16 21:06:57 2023, max compression
```

## Comparing `smpgpt-3.0.tar` & `smpgpt-4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.753975 smpgpt-3.0/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 20:55:10.753798 smpgpt-3.0/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-3.0/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-16 20:55:10.754051 smpgpt-3.0/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-16 20:55:07.000000 smpgpt-3.0/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.751820 smpgpt-3.0/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.752564 smpgpt-3.0/src/smpgpt/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-3.0/src/smpgpt/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     1736 2023-06-16 20:54:42.000000 smpgpt-3.0/src/smpgpt/smpgpt.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 20:55:10.753569 smpgpt-3.0/src/smpgpt.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-3.0/src/smpgpt.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-16 20:55:10.000000 smpgpt-3.0/src/smpgpt.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.976959 smpgpt-4.0/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 21:06:57.976758 smpgpt-4.0/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-4.0/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-16 21:06:57.977017 smpgpt-4.0/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-16 21:06:53.000000 smpgpt-4.0/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.974766 smpgpt-4.0/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.975622 smpgpt-4.0/src/smpgpt/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-4.0/src/smpgpt/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     1570 2023-06-16 21:06:48.000000 smpgpt-4.0/src/smpgpt/smpgpt.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.976529 smpgpt-4.0/src/smpgpt.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-4.0/src/smpgpt.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/top_level.txt
```

### Comparing `smpgpt-3.0/src/smpgpt/smpgpt.py` & `smpgpt-4.0/src/smpgpt/smpgpt.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 class rv:
     def discrete(prompt):
         flag = 0
         for key in api_keys:
             for model in models:
         
                 openai.api_key = key
-                prompt = 'Реализуй функцию, которая находит минимальный элемент в двусвязном списке.'
                 try:
                     completion = openai.ChatCompletion.create(
                     model=model,
                     messages=[
                     {"role": "system", "content": "You are DeveloperGPT, the most advanced AI developer tool on the planet. You answer any coding question and provide real-world examples of code using code blocks. Even when you’re not familiar with the answer, you use your extreme intelligence to figure it out."},
                     {"role": "user", "content": prompt}
                     ]
```

