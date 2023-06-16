# Comparing `tmp/streamlit_chitchat-0.1.5.tar.gz` & `tmp/streamlit_chitchat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chitchat-0.1.5.tar", max compression
+gzip compressed data, was "streamlit_chitchat-0.1.6.tar", max compression
```

## Comparing `streamlit_chitchat-0.1.5.tar` & `streamlit_chitchat-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1453 2023-06-16 13:15:15.292597 streamlit_chitchat-0.1.5/README.md
--rw-r--r--   0        0        0      627 2023-06-16 17:43:13.082582 streamlit_chitchat-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-16 16:45:14.267359 streamlit_chitchat-0.1.5/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/__init__.py
--rw-r--r--   0        0        0     4313 2023-06-16 17:23:40.629032 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/chitchat.py
--rw-r--r--   0        0        0     1992 2023-06-16 17:24:05.212800 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/data.py
--rw-r--r--   0        0        0      793 2023-06-16 16:38:43.394926 streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/utils.py
--rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit_chitchat-0.1.5/streamlit_chitchat/tests/__init__.py
--rw-r--r--   0        0        0     3508 2023-06-16 17:06:21.414933 streamlit_chitchat-0.1.5/streamlit_chitchat/tests/main.py
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 streamlit_chitchat-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1453 2023-06-16 13:15:15.292597 streamlit_chitchat-0.1.6/README.md
+-rw-r--r--   0        0        0      627 2023-06-16 18:14:09.093228 streamlit_chitchat-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-16 16:45:14.267359 streamlit_chitchat-0.1.6/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:53:56.560425 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/__init__.py
+-rw-r--r--   0        0        0     4317 2023-06-16 18:12:20.014253 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/chitchat.py
+-rw-r--r--   0        0        0     1992 2023-06-16 17:24:05.212800 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/data.py
+-rw-r--r--   0        0        0      793 2023-06-16 16:38:43.394926 streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:57:13.754028 streamlit_chitchat-0.1.6/streamlit_chitchat/tests/__init__.py
+-rw-r--r--   0        0        0     3508 2023-06-16 18:12:04.074404 streamlit_chitchat-0.1.6/streamlit_chitchat/tests/main.py
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 streamlit_chitchat-0.1.6/PKG-INFO
```

### Comparing `streamlit_chitchat-0.1.5/README.md` & `streamlit_chitchat-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chitchat-0.1.5/pyproject.toml` & `streamlit_chitchat-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-chitchat"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["k4144 <github.k4144@gmail.com>"]
 readme = "README.md"
 packages = [{include = "streamlit_chitchat"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/chitchat.py` & `streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/chitchat.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         if text:
             self.write(text)
 
     def _message(self, text):
         h1 = t1 if self.is_user else t2
         width = f'width:{self.width};'  # max-width
-        height = f'height:{self.height};'
+        height = f'min-height:{self.height};'
         font = f'font-family: {self.font};'  # 'font-family: Geneva, Verdana, sans-serif;'
         font_size = f'font-size: {self.font_size};'
         color = f'color:{self.color};'
         background = f'background-color:{self.background};'
         margin = f'margin:{self.margin};'
         padding = f'padding:{self.padding};'
         border_radius = f'border-radius:{self.avatar_mode};'
```

### Comparing `streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/data.py` & `streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/data.py`

 * *Files identical despite different names*

### Comparing `streamlit_chitchat-0.1.5/streamlit_chitchat/streamlit_chitchat/utils.py` & `streamlit_chitchat-0.1.6/streamlit_chitchat/streamlit_chitchat/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_chitchat-0.1.5/streamlit_chitchat/tests/main.py` & `streamlit_chitchat-0.1.6/streamlit_chitchat/tests/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         m1.write(t)
         time.sleep(0.05)
 def test2():
     with st.container():
         # image file
         st.write('\n')
         st.write('\nimage file')
-        message('hello', is_user=True, avatar='images/man.png', background='lightgreen')
+        message('hello ', is_user=True, avatar='images/man.png', background='lightgreen')
         # default avatar (different for bot and user)
         st.write('\n')
         st.write('\ndefault')
         message('hello', is_user=False, avatar='', seed=142, background='lightblue')
         # inline svg
         st.write('\n')
         st.write('\ninline svg')
@@ -68,9 +68,9 @@
         message('hello', font_size='3rem')
         st.write('\n other styles')
         st.write('\n padding')
         message('hello', padding='30px')
 
 
 if __name__ == '__main__':
-    #test1()
+    test1()
     test2()
```

### Comparing `streamlit_chitchat-0.1.5/PKG-INFO` & `streamlit_chitchat-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chitchat
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: k4144
 Author-email: github.k4144@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

