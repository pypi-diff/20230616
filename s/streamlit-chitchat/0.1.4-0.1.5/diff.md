# Comparing `tmp/streamlit-chitchat-0.1.4.tar.gz` & `tmp/streamlit_chitchat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chitchat-0.1.4.tar", max compression
+gzip compressed data, was "streamlit_chitchat-0.1.5.tar", max compression
```

## Comparing `streamlit-chitchat-0.1.4.tar` & `streamlit_chitchat-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      820 2023-06-07 15:44:01.184625 streamlit-chitchat-0.1.4/README.md
--rw-r--r--   0        0        0      620 2023-06-07 16:29:53.419050 streamlit-chitchat-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-07 16:29:09.035394 streamlit-chitchat-0.1.4/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit-chitchat-0.1.4/streamlit_chitchat/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0     5187 2023-06-06 22:15:39.989109 streamlit-chitchat-0.1.4/streamlit_chitchat/streamlit_chitchat/chitchat.py
--rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit-chitchat-0.1.4/streamlit_chitchat/tests/__init__.py
--rw-r--r--   0        0        0     1146 2023-06-07 00:13:14.318438 streamlit-chitchat-0.1.4/streamlit_chitchat/tests/main.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.4/setup.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 streamlit-chitchat-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1453 2023-06-16 13:15:15.292597 streamlit_chitchat-0.1.5/README.md
+-rw-r--r--   0        0        0      627 2023-06-16 17:43:13.082582 streamlit_chitchat-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-16 16:45:14.267359 streamlit_chitchat-0.1.5/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0     4313 2023-06-16 17:23:40.629032 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/chitchat.py
+-rw-r--r--   0        0        0     1992 2023-06-16 17:24:05.212800 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/data.py
+-rw-r--r--   0        0        0      793 2023-06-16 16:38:43.394926 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit_chitchat-0.1.5/streamlit_chitchat/tests/__init__.py
+-rw-r--r--   0        0        0     3508 2023-06-16 17:06:21.414933 streamlit_chitchat-0.1.5/streamlit_chitchat/tests/main.py
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 streamlit_chitchat-0.1.5/PKG-INFO
```

### Comparing `streamlit-chitchat-0.1.4/pyproject.toml` & `streamlit_chitchat-0.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "streamlit-chitchat"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
-authors = ["k4144 <you@example.com>"]
+authors = ["k4144 <github.k4144@gmail.com>"]
 readme = "README.md"
 packages = [{include = "streamlit_chitchat"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [metadata]
 name = 'streamlit-chitchat'
-version = '0.1.0'
+version = '0.1.4'
 author = 'k4144'
-author_email = 'your_email@example.com'
+author_email = 'github.k4144@gmail.com'
 description = 'simple streamlit helper'
 long_description = ['file: README.md', 'LICENSE.txt']
 long_description_content_type = 'text/markdown'
 url = 'https://github.com/k4144/streamlit-chitchat'
```

