# Comparing `tmp/lifeguard-openai-1.0.1.tar.gz` & `tmp/lifeguard-openai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-openai-1.0.1.tar", last modified: Wed Jun  7 13:58:01 2023, max compression
+gzip compressed data, was "lifeguard-openai-1.0.2.tar", last modified: Fri Jun 16 14:35:39 2023, max compression
```

## Comparing `lifeguard-openai-1.0.1.tar` & `lifeguard-openai-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/lifeguard_openai/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/lifeguard_openai/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/actions/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/lifeguard_openai/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 13:58:01.000000 lifeguard-openai-1.0.1/lifeguard_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:58:01.557923 lifeguard-openai-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 13:57:39.000000 lifeguard-openai-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:35:39.215844 lifeguard-openai-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 14:35:39.215844 lifeguard-openai-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:35:39.211844 lifeguard-openai-1.0.2/lifeguard_openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/lifeguard_openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:35:39.211844 lifeguard-openai-1.0.2/lifeguard_openai/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/lifeguard_openai/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/lifeguard_openai/actions/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:35:39.215844 lifeguard-openai-1.0.2/lifeguard_openai/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/lifeguard_openai/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/lifeguard_openai/infrastructure/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/lifeguard_openai/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:35:39.211844 lifeguard-openai-1.0.2/lifeguard_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 14:35:39.000000 lifeguard-openai-1.0.2/lifeguard_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 14:35:39.000000 lifeguard-openai-1.0.2/lifeguard_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:35:39.000000 lifeguard-openai-1.0.2/lifeguard_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 14:35:39.000000 lifeguard-openai-1.0.2/lifeguard_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 14:35:39.000000 lifeguard-openai-1.0.2/lifeguard_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:35:39.215844 lifeguard-openai-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-16 14:35:17.000000 lifeguard-openai-1.0.2/setup.py
```

### Comparing `lifeguard-openai-1.0.1/PKG-INFO` & `lifeguard-openai-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-openai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Lifeguard integration with OpenAI
 Home-page: https://github.com/LifeguardSystem/lifeguard-openai
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-openai-1.0.1/lifeguard_openai/actions/errors.py` & `lifeguard-openai-1.0.2/lifeguard_openai/infrastructure/prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,33 @@
     LIFEGUARD_OPENAI_TOKEN,
     LIFEGUARD_OPENAI_MODEL,
     LIFEGUARD_OPENAI_TEMPERATURE,
     LIFEGUARD_OPENAI_TOP_P,
     LIFEGUARD_OPENAI_FREQUENCY_PENALTY,
     LIFEGUARD_OPENAI_PRESENCE_PENALTY,
     LIFEGUARD_OPENAI_MAX_TOKENS,
-    LIFEGUARD_OPENAI_EXPLAIN_ERROR_PROMPT,
 )
 
 openai.api_key = LIFEGUARD_OPENAI_TOKEN
 
 
-def _get_explanation(traceback):
-    if traceback:
-        response = openai.Completion.create(
-            model=LIFEGUARD_OPENAI_MODEL,
-            prompt=f"{LIFEGUARD_OPENAI_EXPLAIN_ERROR_PROMPT}\n\n{traceback}",
-            temperature=LIFEGUARD_OPENAI_TEMPERATURE,
-            top_p=LIFEGUARD_OPENAI_TOP_P,
-            frequency_penalty=LIFEGUARD_OPENAI_FREQUENCY_PENALTY,
-            presence_penalty=LIFEGUARD_OPENAI_PRESENCE_PENALTY,
-            max_tokens=LIFEGUARD_OPENAI_MAX_TOKENS,
-        )
-        if response.choices:
-            return response.choices[0].text
-        else:
-            return "No explanation available"
-    return "No traceback available"
-
-
-def explain_error(validation_response, _settings):
-    traceback = validation_response.details.get("traceback", "")
-    if isinstance(traceback, list):
-        validation_response.details["explanation"] = [
-            _get_explanation(entry) for entry in traceback
-        ]
-    else:
-        validation_response.details["explanation"] = _get_explanation(traceback)
+def execute_prompt(prompt, options=None):
+    default_options = {
+        "model": LIFEGUARD_OPENAI_MODEL,
+        "temperature": LIFEGUARD_OPENAI_TEMPERATURE,
+        "top_p": LIFEGUARD_OPENAI_TOP_P,
+        "frequency_penalty": LIFEGUARD_OPENAI_FREQUENCY_PENALTY,
+        "presence_penalty": LIFEGUARD_OPENAI_PRESENCE_PENALTY,
+        "max_tokens": LIFEGUARD_OPENAI_MAX_TOKENS,
+    }
+
+    if not options:
+        options = {}
+    options["prompt"] = prompt
+
+    default_options.update(options)
+
+    response = openai.Completion.create(**default_options)
+
+    if response.choices:
+        return response.choices[0].text
+    return ""
```

### Comparing `lifeguard-openai-1.0.1/lifeguard_openai/settings.py` & `lifeguard-openai-1.0.2/lifeguard_openai/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-openai-1.0.1/lifeguard_openai.egg-info/PKG-INFO` & `lifeguard-openai-1.0.2/lifeguard_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-openai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Lifeguard integration with OpenAI
 Home-page: https://github.com/LifeguardSystem/lifeguard-openai
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-openai-1.0.1/setup.py` & `lifeguard-openai-1.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-openai",
-    version="1.0.1",
+    version="1.0.2",
     url="https://github.com/LifeguardSystem/lifeguard-openai",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with OpenAI",
```

