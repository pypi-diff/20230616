# Comparing `tmp/aifunc-0.4.5.tar.gz` & `tmp/aifunc-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.4.5.tar", max compression
+gzip compressed data, was "aifunc-0.4.6.tar", max compression
```

## Comparing `aifunc-0.4.5.tar` & `aifunc-0.4.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.5/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.5/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.5/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.5/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.5/aifunc/generate_question.py
--rw-r--r--   0        0        0     6690 2023-06-15 05:02:10.949575 aifunc-0.4.5/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-15 05:06:50.997504 aifunc-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.6/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.6/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.6/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.6/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.6/aifunc/generate_question.py
+-rw-r--r--   0        0        0     6798 2023-06-16 07:41:58.734075 aifunc-0.4.6/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-16 07:42:20.712233 aifunc-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.6/PKG-INFO
```

### Comparing `aifunc-0.4.5/aifunc/add_ai_function.py` & `aifunc-0.4.6/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.4.5/aifunc/utility.py` & `aifunc-0.4.6/aifunc/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,21 +127,23 @@
     yaml_data = response.text
     data = yaml.safe_load(yaml_data)
   else:
     print("Failed to load YAML file.")
     exit(0)
 
   instruction = data["instruction"]
+  instruction = "Your input and output are both json. " + instruction
   example_pairs = data["example_pairs"]
   properties = data["properties"]
-  for example in example_pairs:
-    user_content = example["user_content"]
-    assistant_content = example["assistant_content"]
-    example["user_content"] = str(user_content)
-    example["assistant_content"] = str(assistant_content)
+  if example_pairs != None:
+    for example in example_pairs:
+      user_content = example["user_content"]
+      assistant_content = example["assistant_content"]
+      example["user_content"] = str(user_content)
+      example["assistant_content"] = str(assistant_content)
 
   def fixed_format_ai_wrapper(prompt):
     message = [{"role": "system", "content": instruction}]
     for example in example_pairs:
       user_content = example["user_content"]
       assistant_content = example["assistant_content"]
       message.append({"role": "user", "content": user_content})
```

