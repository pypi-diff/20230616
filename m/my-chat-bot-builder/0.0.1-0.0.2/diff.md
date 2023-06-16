# Comparing `tmp/my_chat_bot_builder-0.0.1.tar.gz` & `tmp/my_chat_bot_builder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_chat_bot_builder-0.0.1.tar", last modified: Fri Jun 16 02:16:46 2023, max compression
+gzip compressed data, was "my_chat_bot_builder-0.0.2.tar", last modified: Fri Jun 16 03:25:00 2023, max compression
```

## Comparing `my_chat_bot_builder-0.0.1.tar` & `my_chat_bot_builder-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 02:16:46.820900 my_chat_bot_builder-0.0.1/
--rw-rw-rw-   0        0        0      577 2023-06-16 02:16:46.819895 my_chat_bot_builder-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      153 2023-06-14 03:46:20.000000 my_chat_bot_builder-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 02:16:46.817896 my_chat_bot_builder-0.0.1/my_chat_bot_builder.egg-info/
--rw-rw-rw-   0        0        0      577 2023-06-16 02:16:46.000000 my_chat_bot_builder-0.0.1/my_chat_bot_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-16 02:16:46.000000 my_chat_bot_builder-0.0.1/my_chat_bot_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 02:16:46.000000 my_chat_bot_builder-0.0.1/my_chat_bot_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-16 02:16:46.000000 my_chat_bot_builder-0.0.1/my_chat_bot_builder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 02:16:46.000000 my_chat_bot_builder-0.0.1/my_chat_bot_builder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 02:16:46.821221 my_chat_bot_builder-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-06-16 02:15:47.000000 my_chat_bot_builder-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 03:25:00.162388 my_chat_bot_builder-0.0.2/
+-rw-rw-rw-   0        0        0      577 2023-06-16 03:25:00.162388 my_chat_bot_builder-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2023-06-14 03:46:20.000000 my_chat_bot_builder-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 03:25:00.160305 my_chat_bot_builder-0.0.2/my_chat_bot_builder.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-06-16 03:25:00.000000 my_chat_bot_builder-0.0.2/my_chat_bot_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-16 03:25:00.000000 my_chat_bot_builder-0.0.2/my_chat_bot_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:25:00.000000 my_chat_bot_builder-0.0.2/my_chat_bot_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-16 03:25:00.000000 my_chat_bot_builder-0.0.2/my_chat_bot_builder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 03:25:00.000000 my_chat_bot_builder-0.0.2/my_chat_bot_builder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 03:25:00.162388 my_chat_bot_builder-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-06-16 02:46:00.000000 my_chat_bot_builder-0.0.2/setup.py
```

### Comparing `my_chat_bot_builder-0.0.1/PKG-INFO` & `my_chat_bot_builder-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_chat_bot_builder
-Version: 0.0.1
+Version: 0.0.2
 Summary: A chat bot builder based on Azure OpenAI
 Home-page: https://github.com/yourusername/my-chat-bot-builder
 Author: jack
 Author-email: jack.cx.chen@pccw.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `my_chat_bot_builder-0.0.1/my_chat_bot_builder.egg-info/PKG-INFO` & `my_chat_bot_builder-0.0.2/my_chat_bot_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-chat-bot-builder
-Version: 0.0.1
+Version: 0.0.2
 Summary: A chat bot builder based on Azure OpenAI
 Home-page: https://github.com/yourusername/my-chat-bot-builder
 Author: jack
 Author-email: jack.cx.chen@pccw.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `my_chat_bot_builder-0.0.1/setup.py` & `my_chat_bot_builder-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="my_chat_bot_builder",
-    version="0.0.1",
+    version="0.0.2",
     author="jack",
     author_email="jack.cx.chen@pccw.com",
     description="A chat bot builder based on Azure OpenAI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yourusername/my-chat-bot-builder",
     packages=find_packages(),
```

