# Comparing `tmp/msfvenomgui-0.2.1.tar.gz` & `tmp/msfvenomgui-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfvenomgui-0.2.1.tar", max compression
+gzip compressed data, was "msfvenomgui-0.2.2.tar", max compression
```

## Comparing `msfvenomgui-0.2.1.tar` & `msfvenomgui-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-07 00:42:09.938622 msfvenomgui-0.2.1/LICENSE
--rw-r--r--   0        0        0      633 2023-06-16 17:51:01.399056 msfvenomgui-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:46:11.344208 msfvenomgui-0.2.1/msfvenomgui/__init__.py
--rw-r--r--   0        0        0     3955 2023-06-16 17:51:01.399056 msfvenomgui-0.2.1/msfvenomgui/command_builder.py
--rw-r--r--   0        0        0     6770 2023-06-16 18:01:32.487844 msfvenomgui-0.2.1/msfvenomgui/gui.py
--rwxr-xr-x   0        0        0      108 2023-06-16 17:51:01.399056 msfvenomgui-0.2.1/msfvenomgui/main.py
--rw-r--r--   0        0        0      502 2023-06-16 18:08:28.719469 msfvenomgui-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 msfvenomgui-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 00:42:09.938622 msfvenomgui-0.2.2/LICENSE
+-rw-r--r--   0        0        0      633 2023-06-16 17:51:01.399056 msfvenomgui-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 00:46:11.344208 msfvenomgui-0.2.2/msfvenomgui/__init__.py
+-rw-r--r--   0        0        0     3955 2023-06-16 17:51:01.399056 msfvenomgui-0.2.2/msfvenomgui/command_builder.py
+-rw-r--r--   0        0        0     6697 2023-06-16 18:14:30.575185 msfvenomgui-0.2.2/msfvenomgui/gui.py
+-rwxr-xr-x   0        0        0      113 2023-06-16 18:14:30.575185 msfvenomgui-0.2.2/msfvenomgui/main.py
+-rw-r--r--   0        0        0      502 2023-06-16 18:14:50.319229 msfvenomgui-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 msfvenomgui-0.2.2/PKG-INFO
```

### Comparing `msfvenomgui-0.2.1/LICENSE` & `msfvenomgui-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msfvenomgui-0.2.1/README.md` & `msfvenomgui-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `msfvenomgui-0.2.1/msfvenomgui/command_builder.py` & `msfvenomgui-0.2.2/msfvenomgui/command_builder.py`

 * *Files identical despite different names*

### Comparing `msfvenomgui-0.2.1/msfvenomgui/gui.py` & `msfvenomgui-0.2.2/msfvenomgui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import command_builder
 import tkinter as tk
 import tkinter.ttk as ttk
 
+from command_builder import *
 from subprocess import Popen, PIPE
 
 
 class GUI:
     def __init__(self):
-        self.cmd = command_builder.CommandBuilder()
+        self.cmd = CommandBuilder()
 
         self.main_window = tk.Tk()
         self.main_window.title("msfvenom-gui")
 
         self.parent_frame = ttk.Frame(self.main_window)
         self.parent_frame.pack(side="left", expand=1)
 
@@ -22,29 +22,29 @@
         self.label_msfvenom_exe = ttk.Label(master=self.widget_frame, text="Path to msfvenom:", justify="right")
         self.var_msfvenom_exe = tk.StringVar(value=self.cmd.msfvenom_path)
         self.entry_msfvenom_exe = ttk.Entry(master=self.widget_frame, textvariable=self.var_msfvenom_exe, width=25)
 
         # row 2: payload
         self.label_payload = ttk.Label(master=self.widget_frame, text="Payload:", justify="right")
         self.combobox_payload = ttk.Combobox(master=self.widget_frame,
-                                             values=command_builder.PAYLOADS, width=25)
+                                             values=PAYLOADS, width=25)
         self.combobox_payload.current(1)
 
         # row 3: exe format
         self.label_exe_format = ttk.Label(master=self.widget_frame, text="Executable format:", justify="right")
-        self.combobox_exe_format = ttk.Combobox(master=self.widget_frame, values=command_builder.EXE_FORMAT, width=25)
+        self.combobox_exe_format = ttk.Combobox(master=self.widget_frame, values=EXE_FORMAT, width=25)
 
         # row 4: transform format
         self.label_transform_format = ttk.Label(master=self.widget_frame, text="Transform format:", justify="right")
-        self.combobox_transform_format = ttk.Combobox(master=self.widget_frame, values=command_builder.TRANSFORM_FORMAT,
+        self.combobox_transform_format = ttk.Combobox(master=self.widget_frame, values=TRANSFORM_FORMAT,
                                                       width=25)
 
         # row 5: encoder
         self.label_encoder = ttk.Label(master=self.widget_frame, text="Encoding:", justify="right")
-        self.combobox_encoder = ttk.Combobox(master=self.widget_frame, values=command_builder.ENCODING, width=25)
+        self.combobox_encoder = ttk.Combobox(master=self.widget_frame, values=ENCODING, width=25)
 
         # row 6: LHOST and RHOST
         self.label_lhost = ttk.Label(master=self.widget_frame, text="LHOST:", justify="right")
         self.var_lhost = tk.StringVar(value="127.0.0.1")
         self.entry_lhost = ttk.Entry(master=self.widget_frame, textvariable=self.var_lhost, width=25)
 
         self.label_lport = ttk.Label(master=self.widget_frame, text="LPORT:", justify="right")
```

### Comparing `msfvenomgui-0.2.1/PKG-INFO` & `msfvenomgui-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfvenomgui
-Version: 0.2.1
+Version: 0.2.2
 Summary: msfvenomgui provides a graphical UI over Metasploit's msfvenom tool.
 License: GPL-3.0-only
 Author: bluesentinelsec
 Author-email: bluesentinel@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

