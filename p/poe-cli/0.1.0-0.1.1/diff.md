# Comparing `tmp/poe-cli-0.1.0.tar.gz` & `tmp/poe-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe-cli-0.1.0.tar", last modified: Sun May 28 19:26:59 2023, max compression
+gzip compressed data, was "poe-cli-0.1.1.tar", last modified: Fri Jun 16 11:21:27 2023, max compression
```

## Comparing `poe-cli-0.1.0.tar` & `poe-cli-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-05-28 19:26:59.102476 poe-cli-0.1.0/
--rw-rw-r--   0 salastro  (1000) salastro  (1000)      686 2023-05-28 17:31:16.000000 poe-cli-0.1.0/LICENSE
--rw-rw-r--   0 salastro  (1000) salastro  (1000)     1380 2023-05-28 19:26:59.102476 poe-cli-0.1.0/PKG-INFO
--rw-rw-r--   0 salastro  (1000) salastro  (1000)      508 2023-05-28 19:14:36.000000 poe-cli-0.1.0/README.md
--rw-rw-r--   0 salastro  (1000) salastro  (1000)       90 2023-05-28 18:27:04.000000 poe-cli-0.1.0/pyproject.toml
--rw-rw-r--   0 salastro  (1000) salastro  (1000)     1289 2023-05-28 19:26:59.102476 poe-cli-0.1.0/setup.cfg
-drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-05-28 19:26:59.100476 poe-cli-0.1.0/src/
-drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-05-28 19:26:59.101476 poe-cli-0.1.0/src/poe_cli/
--rw-rw-r--   0 salastro  (1000) salastro  (1000)        0 2023-05-28 17:04:40.000000 poe-cli-0.1.0/src/poe_cli/__init__.py
--rw-rw-r--   0 salastro  (1000) salastro  (1000)     2720 2023-05-28 16:32:00.000000 poe-cli-0.1.0/src/poe_cli/main.py
-drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-05-28 19:26:59.102476 poe-cli-0.1.0/src/poe_cli.egg-info/
--rw-rw-r--   0 salastro  (1000) salastro  (1000)     1380 2023-05-28 19:26:59.000000 poe-cli-0.1.0/src/poe_cli.egg-info/PKG-INFO
--rw-rw-r--   0 salastro  (1000) salastro  (1000)      298 2023-05-28 19:26:59.000000 poe-cli-0.1.0/src/poe_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 salastro  (1000) salastro  (1000)        1 2023-05-28 19:26:59.000000 poe-cli-0.1.0/src/poe_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 salastro  (1000) salastro  (1000)       42 2023-05-28 19:26:59.000000 poe-cli-0.1.0/src/poe_cli.egg-info/entry_points.txt
--rw-rw-r--   0 salastro  (1000) salastro  (1000)      266 2023-05-28 19:26:59.000000 poe-cli-0.1.0/src/poe_cli.egg-info/requires.txt
--rw-rw-r--   0 salastro  (1000) salastro  (1000)        8 2023-05-28 19:26:59.000000 poe-cli-0.1.0/src/poe_cli.egg-info/top_level.txt
+drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-06-16 11:21:27.202882 poe-cli-0.1.1/
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)      686 2023-05-28 17:31:16.000000 poe-cli-0.1.1/LICENSE
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)     1622 2023-06-16 11:21:27.202882 poe-cli-0.1.1/PKG-INFO
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)      750 2023-05-28 20:35:23.000000 poe-cli-0.1.1/README.md
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)       90 2023-05-28 18:27:04.000000 poe-cli-0.1.1/pyproject.toml
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)     1289 2023-06-16 11:21:27.202882 poe-cli-0.1.1/setup.cfg
+drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-06-16 11:21:27.200882 poe-cli-0.1.1/src/
+drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-06-16 11:21:27.201882 poe-cli-0.1.1/src/poe_cli/
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)        0 2023-05-28 17:04:40.000000 poe-cli-0.1.1/src/poe_cli/__init__.py
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)     4212 2023-06-16 10:52:22.000000 poe-cli-0.1.1/src/poe_cli/main.py
+drwxrwxr-x   0 salastro  (1000) salastro  (1000)        0 2023-06-16 11:21:27.202882 poe-cli-0.1.1/src/poe_cli.egg-info/
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)     1622 2023-06-16 11:21:27.000000 poe-cli-0.1.1/src/poe_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)      298 2023-06-16 11:21:27.000000 poe-cli-0.1.1/src/poe_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)        1 2023-06-16 11:21:27.000000 poe-cli-0.1.1/src/poe_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)       42 2023-06-16 11:21:27.000000 poe-cli-0.1.1/src/poe_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)      266 2023-06-16 11:21:27.000000 poe-cli-0.1.1/src/poe_cli.egg-info/requires.txt
+-rw-rw-r--   0 salastro  (1000) salastro  (1000)        8 2023-06-16 11:21:27.000000 poe-cli-0.1.1/src/poe_cli.egg-info/top_level.txt
```

### Comparing `poe-cli-0.1.0/LICENSE` & `poe-cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poe-cli-0.1.0/PKG-INFO` & `poe-cli-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line interface for Poe.
 Home-page: https://github.com/salastro/poe-cli
 Author: SalahDin Rezk
 Author-email: salah2112004@gmail.com
 Project-URL: Bug Tracker, https://github.com/salastro/poe-cli/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -12,26 +12,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # POE-CLI
 Command line interface for Poe.
 
+[![Upload Python Package](https://github.com/salastro/poe-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/salastro/poe-cli/actions/workflows/python-publish.yml)
 
 https://github.com/salastro/poe-cli/assets/63563250/d4a2333c-0707-410a-818e-3fb0a644a2c4
 
 
 ## Installation
+### From pip
+```
+pip install poe-cli
+```
+### From source
 ```
 git clone https://github.com/salastro/poe-cli.git
 cd poe-cli
 pip install -e .
 ```
 
 ## Usage
```

### Comparing `poe-cli-0.1.0/setup.cfg` & `poe-cli-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = poe-cli
-version = 0.1.0
+version = 0.1.1
 author = SalahDin Rezk
 author_email = salah2112004@gmail.com
 description = Command line interface for Poe.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/salastro/poe-cli
 project_urls = 
@@ -21,15 +21,15 @@
 	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.7
 install_requires = 
 	argparse>=1.4.0
 	certifi>=2023.5.7
 	charset-normalizer>=3.1.0
 	idna>=3.4
 	markdown-it-py>=2.2.0
 	mdurl>=0.1.2
```

### Comparing `poe-cli-0.1.0/src/poe_cli/main.py` & `poe-cli-0.1.1/src/poe_cli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,132 @@
 import argparse
-import json
 import sys
 
 import poe
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.table import Table
 
 
-def parse_args() -> argparse.Namespace:
-    """TODO: Docstring for parse_args.
-    :returns: TODO
+def parse_args() -> argparse.ArgumentParser:
+    """
+    Parse command line arguments for the script.
 
+    :returns: An argparse.ArgumentParser instance.
     """
     parser = argparse.ArgumentParser(
         description="Command line interface for Poe.")
     parser.add_argument("-t", "--token", type=str, help="POE token",
                         required=True)
     parser.add_argument("-l", "--list", help="List bots", action="store_true")
     parser.add_argument("-b", "--bot", type=str,
                         default="chinchilla", help="Bot ID")
+    parser.add_argument("-B", "--break", help="Force chat break",
+                        dest="no_break", action="store_true")
     parser.add_argument("-m", "--message", type=str, help="Message to send")
+    parser.add_argument("-c", "--chat", help="Chat mode", action="store_true")
     return parser
 
 
 def load_token(token: str, console: Console) -> poe.Client:
+    """
+    Load the POE (Poe) token and create a Poe client.
+
+    :param token: The POE token as a string.
+    :param console: A rich Console object for displaying progress.
+    :returns: A connected poe.Client instance.
+    """
     with console.status("[bold red]POE[/bold red][green] is loading..."):
         client = poe.Client(token)
         console.print("[bold red]POE[/bold red][green] is ready!")
     return client
 
 
 def list_bots(client: poe.Client) -> Table:
-    """TODO: Docstring for list_bots.
-
-    :client: TODO
-    :returns: TODO
+    """
+    Get a list of available bots and format them as a rich Table.
 
+    :param client: A connected poe.Client instance.
+    :returns: A rich Table containing the bot ID and bot name.
     """
-    bots = json.dumps(client.bot_names)
-    bots = json.loads(bots)
+    bots = client.bot_names
     table = Table(title="Bots")
     table.add_column("Bot ID", justify="center", style="cyan", no_wrap=True)
-    table.add_column("Bot Name", justify="center",
-                     style="magenta", no_wrap=True)
+    table.add_column("Bot Name", justify="center", style="magenta",
+                     no_wrap=True)
     for bot in bots:
         table.add_row(bot, bots[bot])
     return table
 
 
+def live_panel(console: Console, client: poe.Client, bot: str,
+               message: str, with_chat_break: bool = True) -> None:
+    """
+    Display the live panel with the chat conversation.
+
+    :param console: A rich Console object for displaying the live panel.
+    :param client: A connected poe.Client instance.
+    :param bot: The bot ID to send the message to.
+    :param message: The message to send to the bot.
+    """
+    # Create a Panel to show the message in
+    panel = Panel("")
+
+    # Create a Live context manager with the Panel to update text
+    with Live(panel, console=console) as live:
+        response = ""
+        for chunk in client.send_message(bot, message,
+                                         with_chat_break=with_chat_break):
+            response += chunk["text_new"]
+            panel = Panel(Markdown(response))
+            live.update(panel)
+
+
 def main():
     # Parse arguments
     parser = parse_args()
     args = parser.parse_args()
 
     # Assign arguments
     TOKEN = args.token
     MESSAGE = args.message
     BOT = args.bot
     LIST_BOTS = args.list
+    CHAT = args.chat
+    BREAK = args.no_break
 
-    # if there is no argument, print help
-    if not LIST_BOTS and not MESSAGE:
+    # If there is no argument, print help
+    if (not LIST_BOTS and not MESSAGE) and not CHAT:
         parser.print_help()
-        sys.exit(1)
+        sys.exit(2)
 
     # Create console, for cool stuff
     console = Console()
     # Create POE client
     client = load_token(TOKEN, console)
 
     # List bots
     if LIST_BOTS:
         console.print(list_bots(client))
         sys.exit(0)
 
-    # Create a Panel to show the message in
-    panel = Panel("")
-
-    # Create a Live context manager with the Panel to update text
-    with Live(panel, console=console) as live:
-        response = ""
-        for chunk in client.send_message(BOT, MESSAGE,
-                                         with_chat_break=True):
-            response += chunk["text_new"]
-            panel = Panel(Markdown(response))
-            live.update(panel)
+    if CHAT:
+        client.send_chat_break(BOT)
+        while True:
+            # Ask for another message
+            MESSAGE = input("> ")
+            # If the message is empty, exit
+            if not MESSAGE:
+                exit(0)
+            # Display the live panel with the chat conversation
+            live_panel(console, client, BOT, MESSAGE, False)
+    else:
+        live_panel(console, client, BOT, MESSAGE, not BREAK)
 
 
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         Console().print("\n[bold red]POE[/bold red][green] shut down.")
```

### Comparing `poe-cli-0.1.0/src/poe_cli.egg-info/PKG-INFO` & `poe-cli-0.1.1/src/poe_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line interface for Poe.
 Home-page: https://github.com/salastro/poe-cli
 Author: SalahDin Rezk
 Author-email: salah2112004@gmail.com
 Project-URL: Bug Tracker, https://github.com/salastro/poe-cli/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -12,26 +12,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # POE-CLI
 Command line interface for Poe.
 
+[![Upload Python Package](https://github.com/salastro/poe-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/salastro/poe-cli/actions/workflows/python-publish.yml)
 
 https://github.com/salastro/poe-cli/assets/63563250/d4a2333c-0707-410a-818e-3fb0a644a2c4
 
 
 ## Installation
+### From pip
+```
+pip install poe-cli
+```
+### From source
 ```
 git clone https://github.com/salastro/poe-cli.git
 cd poe-cli
 pip install -e .
 ```
 
 ## Usage
```

