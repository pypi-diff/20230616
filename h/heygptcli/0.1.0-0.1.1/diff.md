# Comparing `tmp/heygptcli-0.1.0.tar.gz` & `tmp/heygptcli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heygptcli-0.1.0.tar", max compression
+gzip compressed data, was "heygptcli-0.1.1.tar", max compression
```

## Comparing `heygptcli-0.1.0.tar` & `heygptcli-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        5 2023-06-09 08:08:09.178950 heygptcli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 08:08:09.178950 heygptcli-0.1.0/heygpt/__init__.py
--rw-r--r--   0        0        0      717 2023-06-09 08:08:09.178950 heygptcli-0.1.0/heygpt/api.py
--rwxr-xr-x   0        0        0     5045 2023-06-09 08:08:09.178950 heygptcli-0.1.0/heygpt/cli.py
--rw-r--r--   0        0        0     2144 2023-06-09 08:08:09.182950 heygptcli-0.1.0/heygpt/constant.py
--rw-r--r--   0        0        0     2339 2023-06-09 08:08:09.182950 heygptcli-0.1.0/heygpt/core.py
--rw-r--r--   0        0        0     2064 2023-06-09 08:08:09.182950 heygptcli-0.1.0/heygpt/serve.py
--rw-r--r--   0        0        0      153 2023-06-09 08:08:09.182950 heygptcli-0.1.0/heygpt/serve_prompts.py
--rw-r--r--   0        0        0      849 2023-06-09 08:08:09.182950 heygptcli-0.1.0/heygpt/utils.py
--rw-r--r--   0        0        0      707 2023-06-09 08:08:09.182950 heygptcli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 heygptcli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-16 18:46:16.771883 heygptcli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/__init__.py
+-rw-r--r--   0        0        0      717 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/api.py
+-rwxr-xr-x   0        0        0     4840 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/cli.py
+-rw-r--r--   0        0        0     2249 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/constant.py
+-rw-r--r--   0        0        0     2804 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/core.py
+-rw-r--r--   0        0        0     1897 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/serve.py
+-rw-r--r--   0        0        0      153 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/serve_prompts.py
+-rw-r--r--   0        0        0      849 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/utils.py
+-rw-r--r--   0        0        0      677 2023-06-16 18:46:16.771883 heygptcli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.1/PKG-INFO
```

### Comparing `heygptcli-0.1.0/heygpt/api.py` & `heygptcli-0.1.1/heygpt/api.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.0/heygpt/cli.py` & `heygptcli-0.1.1/heygpt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,17 +35,16 @@
     no_prompt: bool = typer.Option(
         False, "--no-prompt", "-n", help="Ask without anyprompt templates."
     ),
     text: str = typer.Option(
         str, help="Optional provide text query as an input argument."
     ),
     tag: Annotated[Optional[List[str]], typer.Option()] = [],
-    md: bool = typer.Option(False, help="output format in markdown"),
     save: bool = typer.Option(
-        False, help="save output to file availabe formats: md, txt, html"
+        False, "--output", "-o", help="save output to file availabe formats: md"
     ),
 ):
     tags: str = " #".join(tag)
     command: str = ""
 
     # print(tags)
     # return
@@ -74,38 +73,33 @@
                 break
         if not _found_prompt:
             rich.print(f"No prompt '{act}' found")
             return
 
     if tags.strip() != "":
         command += f"\nFor: #{tags}"
-    if md:
-        command += "use markdown format for output."
+
     if not sys.stdin.isatty():
         text = sys.stdin.read()
     elif text == "":
         rich.print(f"Selected: {command}") if not no_prompt else ...
         print()
         text = Prompt.ask("[blue]Enter text")
 
     # log.debug(text)
     if bard:
-        content = completion_bard(command=command, text=text)
+        content = completion_bard(command=command, text=text, _print=True)
     else:
-        completion = completion_openai_gpt(command=command, text=text)
-        content = completion.choices[0].message.content
+        completion = completion_openai_gpt(command=command, text=text, _print=True)
+        content = completion
 
     # typer.echo("\n---------- output ----------\n")
-    if md:
-        print_md(content)
-    else:
-        rich.print(content)
 
     if save:
-        file_name = "output.txt"
+        file_name = "output.md"
         with open(f"{file_name}", "w") as f:
             f.write(content)
         rich.print(f"\n\nINFO: Output saved to: {file_name}")
 
 
 @app.command(help="Generate new prompts.")
 def create_prompt(text):
@@ -123,15 +117,15 @@
     print()
     rich.print(text)
 
 
 @app.command(help="Use heygpt as api server.")
 def api():
     uvicorn.run(
-        "heygpt.serve:app", port=5000, host="0.0.0.0", reload=True, log_level="info"
+        "heygpt.api:app", port=5000, host="0.0.0.0", reload=True, log_level="info"
     )
 
 
 @app.command(help="Use heygpt as UI.")
 def stream():
     # run streamlit app
     path = str(Path(__file__).parent) + "/serve.py"
```

### Comparing `heygptcli-0.1.0/heygpt/constant.py` & `heygptcli-0.1.1/heygpt/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import csv
 import json
 from dataclasses import dataclass, field
 
+from dotenv import load_dotenv
 import requests
 from pydantic import BaseModel
 from heygpt.utils import log
 
+load_dotenv()
+
 
 @dataclass
 class Prompt:
     Title: str
     Command: str
     ExtraCommands: str = field(default_factory=str)
     Tags: list[str] = field(default_factory=list)
@@ -31,14 +34,16 @@
 )
 
 genrtare_prompt_url = os.environ.get(
     "PROMPT_GENERATE_URL",
     "https://api-inference.huggingface.co/models/merve/chatgpt-prompt-generator-v12",
 )
 
+openai_model = os.getenv("OPENAI_MODEL", "gpt-3.5-turbo")
+
 
 def get_config_path(app: str = "heygpt"):
     if os.name == "nt":  # Windows
         return os.path.expanduser(f"~\\AppData\\Roaming\\{app}\\config.json")
     elif os.name == "posix":  # Linux, macOS, etc.
         return os.path.expanduser(f"~/.config/{app}/config.json")
     else:
```

### Comparing `heygptcli-0.1.0/heygpt/core.py` & `heygptcli-0.1.1/heygpt/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,88 @@
 import os
 
 import requests
 import openai
-from dotenv import load_dotenv
 from bardapi import Bard
 from rich.console import Console
 from rich.markdown import Markdown
 from prompt_toolkit import prompt
 from prompt_toolkit.completion import FuzzyWordCompleter
 
-
-from heygpt.constant import configs, genrtare_prompt_url
+from heygpt.constant import configs, genrtare_prompt_url, openai_model
 
 console = Console()
 
-load_dotenv()
-
 openai.api_key = os.getenv("OPENAI_API_KEY", configs.get("openai_key"))
 
 
+def sh(command):
+    return os.popen(command).read()
+
+
+def print_md(markdown: str, **kwargs):
+    md = Markdown(markdown)
+    console.print(md, **kwargs)
+
+
 def ask_prompt_input(items: list, title="Select item"):
     completer = FuzzyWordCompleter(items)
     text = prompt(f"{title}: ", completer=completer, complete_while_typing=True)
     return text
 
 
-def completion_openai_gpt(text: str = None, command: str = ""):
+def completion_openai_gpt(text: str = None, command: str = "", _print=False):
+    """
+    ref: https://docs.openai.com/api-reference/completions/create
+    """
+    out = ""
+
     if not text:
         raise Exception("No text found")
 
-    # payload = f"{command} ```{text}```"
-
     completion = openai.ChatCompletion.create(
-        model="gpt-3.5-turbo",
+        model=openai_model,
+        stream=True,
         messages=[
-            {"role": "user", "content": command + "\n" + text},
-            # {"role": "user", "content": text},
+            {
+                "role": "system",
+                "content": "Output has to be in markdown supported format",
+            },
+            {"role": "user", "content": command + "\nTask: " + text},
         ],
         # stop="",
     )
 
-    return completion
+    for chunk in completion:
+        # Process each chunk as needed
+        c = chunk["choices"][0]["delta"].get("content", "")
+        out += c
+        if _print:
+            console.print(c, end="", markup=True)
+
+    return out
 
 
-def completion_bard(text: str, command: str = ""):
+def completion_bard(text: str, command: str = "", _print=False):
     """
     ref: https://github.com/dsdanielpark/Bard-API
     Bard is a GPT-3 model trained on 38 million lines of fantasy text.
 
     This function requires "_BARD_API_KEY" which can get from below steps:
     Go to https://bard.google.com/
         : Go to Application → Cookies → __Secure-1PSID. Copy the value of that cookie.
     """
     if os.environ.get("_BARD_API_KEY") == None:
         if configs.get("bard_key"):
             os.environ["_BARD_API_KEY"] = configs.get("bard_key")
 
-    return Bard().get_answer(command + "\n" + text)["content"]
+    completer = Bard().get_answer(command + "\nTask: " + text)["content"]
+    if _print:
+        print_md(completer)
+    return completer
 
 
 def make_prompt(text: str):
     json_data = {
         "inputs": f"""{text}""",
     }
 
@@ -77,16 +99,7 @@
     return res[0]
 
 
 def wisper(audio_file):
     with open(f"{audio_file}", "rb") as file:
         transcript = openai.Audio.transcribe("whisper-1", file)
     return transcript["text"]
-
-
-def sh(command):
-    return os.popen(command).read()
-
-
-def print_md(markdown: str):
-    md = Markdown(markdown)
-    console.print(md)
```

### Comparing `heygptcli-0.1.0/heygpt/serve.py` & `heygptcli-0.1.1/heygpt/serve.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import streamlit as st
 from heygpt.core import completion_openai_gpt, completion_bard
 from heygpt.serve_prompts import prompts_title
 
-# import streamlit_toggle as tog
-
 
 def local_css(file_name="", style=""):
     if file_name != "":
         with open(file_name) as f:
             st.markdown(f"<style>{f.read()}</style>", unsafe_allow_html=True)
     else:
         st.markdown(f"<style>{style}</style>", unsafe_allow_html=True)
@@ -37,34 +35,29 @@
     use_bard = st.checkbox("Ask Bard", value=False)
     prompt = st.radio(
         label="**Promots**", options=["None"] + list(prompts_title.keys())
     )
 
 
 with st.container():
-    # toggle_md = tog.st_toggle_switch(
-    #     label="format",
-    #     default_value=False,
-    # )
-
     content = ""
 
     with col2:
         if prompt != "None":
             _selected_prompt = prompts_title[prompt]
             print_prompt.write(f"**Selected**: {_selected_prompt}")
         else:
             _selected_prompt = ""
 
         if submit:
             if not use_bard:
                 completion = completion_openai_gpt(command=_selected_prompt, text=ask)
             else:
                 completion = completion_bard(command=_selected_prompt, text=ask)
-            content = completion.choices[0].message.content
+            content = completion
             st.markdown(content)
 
     with col3:
         if content != "":
             st.download_button(
                 label="Download text",
                 data=content.encode("utf-8"),
```

### Comparing `heygptcli-0.1.0/heygpt/utils.py` & `heygptcli-0.1.1/heygpt/utils.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.0/pyproject.toml` & `heygptcli-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "heygptcli"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Rishang <rishang@localhost.com>"]
 readme = "README.md"
 packages = [
   { include = "heygpt" }
 ]
 
 [tool.poetry.scripts]
 heygpt = "heygpt.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
-fastapi = {extras = ["all"], version = "^0.95.2"}
+fastapi = "^0.95.2"
 uvicorn = "^0.22.0"
 typer = "^0.9.0"
 python-dotenv = "^1.0.0"
 bardapi = "^0.1.11"
 openai = "^0.27.8"
 rich = "^13.4.1"
 prompt-toolkit = "^3.0.38"
```

### Comparing `heygptcli-0.1.0/PKG-INFO` & `heygptcli-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: heygptcli
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Rishang
 Author-email: rishang@localhost.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bardapi (>=0.1.11,<0.2.0)
-Requires-Dist: fastapi[all] (>=0.95.2,<0.96.0)
+Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: streamlit (>=1.23.1,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
-# api
+# heygpt cli/ui
+
+[https://github.com/Rishang/heygpt](https://github.com/Rishang/heygpt)
```

