# Comparing `tmp/aifunc-0.5.0.tar.gz` & `tmp/aifunc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.5.0.tar", max compression
+gzip compressed data, was "aifunc-0.5.1.tar", max compression
```

## Comparing `aifunc-0.5.0.tar` & `aifunc-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.5.0/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.5.0/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.5.0/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.5.0/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.5.0/aifunc/generate_question.py
--rw-r--r--   0        0        0     6838 2023-06-16 07:45:15.467144 aifunc-0.5.0/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-16 07:45:29.240131 aifunc-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.5.1/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.5.1/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.5.1/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.5.1/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.5.1/aifunc/generate_question.py
+-rw-r--r--   0        0        0     6890 2023-06-16 15:30:05.230835 aifunc-0.5.1/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-16 15:30:32.789486 aifunc-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.1/PKG-INFO
```

### Comparing `aifunc-0.5.0/aifunc/add_ai_function.py` & `aifunc-0.5.1/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.5.0/aifunc/utility.py` & `aifunc-0.5.1/aifunc/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     yaml_data = response.text
     data = yaml.safe_load(yaml_data)
   else:
     print("Failed to load YAML file.")
     exit(0)
 
   instruction = data["instruction"]
-  instruction = "Your input and output are both json. " + instruction
+  instruction = "Your input and output are both json and from now you only speak in the language of json. " + instruction
   example_pairs = data["example_pairs"]
   properties = data["properties"]
   if example_pairs != None:
     for example in example_pairs:
       user_content = example["user_content"]
       assistant_content = example["assistant_content"]
       example["user_content"] = str(user_content)
@@ -174,16 +174,16 @@
         if response.get("function_call"):
           arguments = eval(response["function_call"]["arguments"])
           return arguments
         else:
           raise
       except Exception as e:
         if i < 4:  # if it's not the last attempt
-          print(f"Attempt {i} failed, retrying in 5 seconds...")
-          time.sleep(5)  # wait for 5 seconds before next attempt
+          print(f"Attempt {i} failed, retrying in 1 seconds...")
+          time.sleep(1)  # wait for 5 seconds before next attempt
         else:  # if it's the last attempt
           print("All attempts failed.")
           raise e  # re-raise the last exception
     raise Exception(
       "Unable to execute fixed_format_ai_wrapper after 5 attempts.")
 
   return fixed_format_ai_wrapper
```

