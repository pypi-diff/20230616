# Comparing `tmp/selfcord.py-0.1.9.tar.gz` & `tmp/selfcord.py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.9.tar", last modified: Thu Jun  1 19:05:19 2023, max compression
+gzip compressed data, was "selfcord.py-0.2.0.tar", last modified: Fri Jun 16 16:12:03 2023, max compression
```

## Comparing `selfcord.py-0.1.9.tar` & `selfcord.py-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.860261 selfcord.py-0.1.9/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.864261 selfcord.py-0.1.9/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.864261 selfcord.py-0.1.9/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    22255 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/selfcord/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.860261 selfcord.py-0.1.9/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 19:05:19.000000 selfcord.py-0.1.9/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:05:19.868261 selfcord.py-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-01 19:05:09.000000 selfcord.py-0.1.9/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.9/PKG-INFO` & `selfcord.py-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -15,15 +15,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.7-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.0-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
@@ -133,13 +133,13 @@
     await ctx.reply(f"{bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 
 bot.run(token)
 ```
 ## Some Useful Links
 - [Documentation](https://github.com/Shell1010/Selfcord/wiki)
 - [Other Documentation (messy)](https://github.com/Shell1010/Selfcord/tree/main/docs)
-- [PyPi](https://pypi.org/project/selfcord/)
+- [PyPi](https://pypi.org/project/selfcord.py/)
 - [Official Discord Server](https://discord.gg/FCFnnBGzkg)
 - [A simple selfbot designed to showcase the library's features](https://github.com/Shell1010/Aeterna-Selfbot)
 
 ## Contributing
 Contributors are always Welcome
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.9 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.0 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.7-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.0-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
@@ -44,11 +44,11 @@
 ```python import selfcord token = "insert token" bot = selfcord.Bot(prefixes=
 ["!", "?"]) @bot.on("ready") async def ball(time): print(f"Connected To
 {bot.user}\n Startup took {time:0.2f} seconds") @bot.cmd(description="Snipe",
 aliases=['s']) async def snipe(ctx): await ctx.reply(f"
 {bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 bot.run(token) ``` ## Some Useful Links - [Documentation](https://github.com/
 Shell1010/Selfcord/wiki) - [Other Documentation (messy)](https://github.com/
-Shell1010/Selfcord/tree/main/docs) - [PyPi](https://pypi.org/project/selfcord/
-) - [Official Discord Server](https://discord.gg/FCFnnBGzkg) - [A simple
-selfbot designed to showcase the library's features](https://github.com/
+Shell1010/Selfcord/tree/main/docs) - [PyPi](https://pypi.org/project/
+selfcord.py/) - [Official Discord Server](https://discord.gg/FCFnnBGzkg) - [A
+simple selfbot designed to showcase the library's features](https://github.com/
 Shell1010/Aeterna-Selfbot) ## Contributing Contributors are always Welcome
```

### Comparing `selfcord.py-0.1.9/README.md` & `selfcord.py-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.7-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.0-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
@@ -122,13 +122,13 @@
     await ctx.reply(f"{bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 
 bot.run(token)
 ```
 ## Some Useful Links
 - [Documentation](https://github.com/Shell1010/Selfcord/wiki)
 - [Other Documentation (messy)](https://github.com/Shell1010/Selfcord/tree/main/docs)
-- [PyPi](https://pypi.org/project/selfcord/)
+- [PyPi](https://pypi.org/project/selfcord.py/)
 - [Official Discord Server](https://discord.gg/FCFnnBGzkg)
 - [A simple selfbot designed to showcase the library's features](https://github.com/Shell1010/Aeterna-Selfbot)
 
 ## Contributing
 Contributors are always Welcome
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.7-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.0-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
@@ -40,11 +40,11 @@
 ```python import selfcord token = "insert token" bot = selfcord.Bot(prefixes=
 ["!", "?"]) @bot.on("ready") async def ball(time): print(f"Connected To
 {bot.user}\n Startup took {time:0.2f} seconds") @bot.cmd(description="Snipe",
 aliases=['s']) async def snipe(ctx): await ctx.reply(f"
 {bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 bot.run(token) ``` ## Some Useful Links - [Documentation](https://github.com/
 Shell1010/Selfcord/wiki) - [Other Documentation (messy)](https://github.com/
-Shell1010/Selfcord/tree/main/docs) - [PyPi](https://pypi.org/project/selfcord/
-) - [Official Discord Server](https://discord.gg/FCFnnBGzkg) - [A simple
-selfbot designed to showcase the library's features](https://github.com/
+Shell1010/Selfcord/tree/main/docs) - [PyPi](https://pypi.org/project/
+selfcord.py/) - [Official Discord Server](https://discord.gg/FCFnnBGzkg) - [A
+simple selfbot designed to showcase the library's features](https://github.com/
 Shell1010/Aeterna-Selfbot) ## Contributing Contributors are always Welcome
```

### Comparing `selfcord.py-0.1.9/selfcord/api/errors.py` & `selfcord.py-0.2.0/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/selfcord/api/events.py` & `selfcord.py-0.2.0/selfcord/api/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,26 +89,26 @@
         """
         self.user = user
         message = Message(data, self.bot, http)
         self.user.messages.append(message)
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit("message", message)
-        if not self.bot.userbot:
-            if message.author.id == self.bot.user.id:
-                for prefix in self.bot.prefixes:
-                    # Attempts to invoke the command if has prefix and from the user
-                    if message.content.startswith(prefix):
-                        await self.bot.process_commands(message)
-        else:
+        if self.bot.userbot:
             for prefix in self.bot.prefixes:
                 # Attempts to invoke the command if has prefix
                 if message.content.startswith(prefix):
                     await self.bot.process_commands(message)
 
+        elif message.author.id == self.bot.user.id:
+            for prefix in self.bot.prefixes:
+                # Attempts to invoke the command if has prefix and from the user
+                if message.content.startswith(prefix):
+                    await self.bot.process_commands(message)
+
     async def handle_message_delete(self, data: dict, user: Client, http: http):
         """Handles what happens when a message is deleted. Very little data will be logged if the message is not in the bots cache.
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
@@ -149,40 +149,37 @@
 
         Args:
             channel (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
-        if channel.get("type") == 0:
+        if channel.get("type") == 0 or channel.get("type") not in [1, 2, 3]:
             id = channel.get("guild_id")
             for guild in self.user.guilds:
                 if guild.id == id:
                     channel = TextChannel(channel, self.bot, self.http)
                     guild.channels.append(channel)
 
-        elif channel.get("type") == 1:
+        elif channel.get("type") != 0 and channel.get("type") == 1:
             self.user.private_channels.append(DMChannel(channel, self.bot, http))
 
-        elif channel.get("type") == 2:
+        elif (
+            channel.get("type") != 0
+            and channel.get("type") != 1
+            and channel.get("type") == 2
+        ):
             id = channel.get("guild_id")
             for guild in self.user.guilds:
                 if guild.id == id:
                     channel = VoiceChannel(channel, self.bot, self.http)
                     guild.channels.append(channel)
 
-        elif channel.get("type") == 3:
-            self.user.private_channels.append(GroupChannel(channel, self.bot, http))
-
         else:
-            id = channel.get("guild_id")
-            for guild in self.user.guilds:
-                if guild.id == id:
-                    channel = TextChannel(channel, self.bot, self.http)
-                    guild.channels.append(channel)
+            self.user.private_channels.append(GroupChannel(channel, self.bot, http))
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit("channel_create", channel)
 
     async def handle_guild_member_list_update(
         self, data: dict, user: Client, http: http
     ):
@@ -355,32 +352,32 @@
         """Handles the presence updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
-        PLAYING = 0
-        STREAMING = 1
         LISTENING = 2
-        WATCHING = 3
         CUSTOM = 4
 
         last_modified = data.get("last_modified")
         status = data.get("status")
         check = data.get("user").get("username")
-        if check != None:
-            user = User(data.get("user"), self.bot, self.http)
-        else:
+        if check is None:
             user = data.get("user").get("id")
 
+        else:
+            user = User(data.get("user"), self.bot, self.http)
         client_status = data.get("client_status")
         activity = data.get("activities")
         activities = []
         if activity != None:
+            PLAYING = 0
+            STREAMING = 1
+            WATCHING = 3
             for activity in activity:
                 type = activity.get("type")
                 if type == PLAYING:
                     type = "PLAYING"
                 elif type == STREAMING:
                     type = "STREAMING"
                 elif type == WATCHING:
@@ -399,18 +396,18 @@
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.token = data["token"]
         self.endpoint = data["endpoint"]
-        if data["guild_id"] != None:
-            self.server_id = data["guild_id"]
-        else:
+        if data["guild_id"] is None:
             self.server_id = data["channel_id"]
+        else:
+            self.server_id = data["guild_id"]
         await asyncio.sleep(1)
         self.voice = Voice(
             self.session_id,
             self.token,
             self.endpoint,
             self.server_id,
             self.bot,
```

### Comparing `selfcord.py-0.1.9/selfcord/api/gateway.py` & `selfcord.py-0.2.0/selfcord/api/gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,53 +41,52 @@
             application_id (str): Application ID
             key (str): Key for the large image
 
         Returns:
             dict[str, int]: Dict for the activity object for payload
         """
         type = 0
-        button_urls = [button for button in buttons.values()]
-        buttons: list = [button for button in buttons.keys()]
+        button_urls = list(buttons.values())
+        buttons: list = list(buttons.keys())
         req = requests.get(
             f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
         )
         for item in req.json():
             if item["name"] == key:
                 key = item["id"]
 
-        if len(button_urls) == 0 or len(buttons) == 0:
-            payload = {
+        return (
+            {
                 "name": name,
                 "details": details,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "type": type,
                 "created_at": int(time.time()),
             }
-        else:
-            payload = {
+            if not button_urls or not buttons
+            else {
                 "name": name,
                 "details": details,
                 "type": type,
                 "buttons": buttons,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
                 "created_at": int(time.time()),
             }
-
-        return payload
+        )
 
     @staticmethod
     def Stream(
         name: str,
         details: str,
         state: str,
         url: str,
@@ -108,38 +107,38 @@
             application_id (str): Application ID
             key (str): Key for the large image
 
         Returns:
             dict[str, int]: Dict for the activity object for payload
         """
         type = 1
-        button_urls = [button for button in buttons.values()]
-        buttons: list = [button for button in buttons.keys()]
+        button_urls = list(buttons.values())
+        buttons: list = list(buttons.keys())
         req = requests.get(
             f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
         )
         for item in req.json():
             if item["name"] == key:
                 key = item["id"]
 
-        if len(button_urls) == 0 or len(buttons) == 0:
-            payload = {
+        return (
+            {
                 "name": name,
                 "details": details,
                 "type": type,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "created_at": int(time.time()),
                 "url": url,
             }
-        else:
-            payload = {
+            if not button_urls or not buttons
+            else {
                 "name": name,
                 "details": details,
                 "type": type,
                 "buttons": buttons,
                 "url": url,
                 "state": state,
                 "application_id": application_id,
@@ -147,16 +146,15 @@
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
                 "created_at": int(time.time()),
             }
-
-        return payload
+        )
 
     @staticmethod
     def Listen(
         name: str,
         details: str,
         state: str,
         buttons: dict,
@@ -175,53 +173,52 @@
             application_id (str): Application ID
             key (str): Key for the large image
 
         Returns:
             dict[str, int]: Dict for the activity object for payload
         """
         type = 2
-        button_urls = [button for button in buttons.values()]
-        buttons: list = [button for button in buttons.keys()]
+        button_urls = list(buttons.values())
+        buttons: list = list(buttons.keys())
         req = requests.get(
             f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
         )
         for item in req.json():
             if item["name"] == key:
                 key = item["id"]
 
-        if len(button_urls) == 0 or len(buttons) == 0:
-            payload = {
+        return (
+            {
                 "name": name,
                 "details": details,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "type": type,
                 "created_at": int(time.time()),
             }
-        else:
-            payload = {
+            if not button_urls or not buttons
+            else {
                 "name": name,
                 "details": details,
                 "type": type,
                 "buttons": buttons,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
                 "created_at": int(time.time()),
             }
-
-        return payload
+        )
 
     @staticmethod
     def Watch(
         name: str,
         details: str,
         state: str,
         buttons: dict,
@@ -241,54 +238,53 @@
             key (str): Key for the large image
 
         Returns:
             dict[str, int]: Dict for the activity object for payload
         """
         type = 3
 
-        button_urls = [button for button in buttons.values()]
-        buttons: list = [button for button in buttons.keys()]
+        button_urls = list(buttons.values())
+        buttons: list = list(buttons.keys())
 
         req = requests.get(
             f"https://discordapp.com/api/oauth2/applications/{application_id}/assets"
         )
         for item in req.json():
             if item["name"] == key:
                 key = item["id"]
 
-        if len(button_urls) == 0 or len(buttons) == 0:
-            payload = {
+        return (
+            {
                 "name": name,
                 "details": details,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "type": type,
                 "created_at": int(time.time()),
             }
-        else:
-            payload = {
+            if not button_urls or not buttons
+            else {
                 "name": name,
                 "details": details,
                 "type": type,
                 "buttons": buttons,
                 "state": state,
                 "application_id": application_id,
                 "assets": {
                     "large_image": key,
                 },
                 "metadata": {
                     "button_urls": button_urls,
                 },
                 "created_at": int(time.time()),
             }
-
-        return payload
+        )
 
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from zlib import _Decompress
 
@@ -318,35 +314,43 @@
         self.zlib: _Decompress = zlib.decompressobj()
         self.zlib_suffix: bytes = b"\x00\x00\xff\xff"
         self.last_ack: float = time.perf_counter()
         self.last_send: float = time.perf_counter()
         self.latency = float("inf")
         self.resume_url = None
         self.alive = False
+        self.fired = False
 
     async def recv_msg(self):
         """
         Receives Message from gateway, encodes as json and does things depending on op code
         """
         item = await self.ws.recv()
         buffer = bytearray()
         buffer.extend(item)
         if len(item) < 4 or item[-4:] != self.zlib_suffix:
             return
 
         if item:
-            item = self.zlib.decompress(item)
+            if self.fired:
+                log.info(f"{item}")
+            try:
+                item = self.zlib.decompress(item)
+            except Exception as e:
+                log.error(f"Could not decompress\n{e}")
             item = json.loads(item)  # Get json message from gateway
 
             op = item.get("op")  # Op code
             data = item.get("d")  # Data
             event = item.get("t")  # The event
             s = item.get("s")
             if op == self.RECONNECT:
+                await self.close()
                 await self.reconnect(s)
+                self.fired = True
                 log.error("Reconnect websocket")
 
             elif op == self.INVALIDATE_SESSION:
                 if data:
                     await self.close()
                     log.error("Session Invalidated")
 
@@ -371,15 +375,15 @@
                     method = getattr(self.handler, handle)
 
                     val = await asyncio.gather(
                         asyncio.create_task(method(data, self.user, self.http)),
                         return_exceptions=True,
                     )  # A background task is created to run the handler
                     for item in val:
-                        if item == None:
+                        if item is None:
                             break
                         else:
                             await self.bot.emit("error", item)
 
                     # asyncio.create_task(method(data, self.user, self.http))
                 # Handlers are all situated in events.py
 
@@ -461,14 +465,15 @@
         await self.ws.send(json.dumps(payload))
 
     async def reconnect(self, seq: int):
         """Reconnect to discord gateway"""
         self.ws = await websockets.connect(
             f"{self.bot.resume_url}?encoding=json&v=9&compress=zlib-stream"
         )
+        self.alive = True
         payload = {
             "op": 6,
             "d": {"token": self.token, "session_id": self.bot.session_id, "seq": seq},
         }
         await self.send_json(payload)
 
     async def connect(self):
@@ -578,15 +583,15 @@
                 "self_video": True,
             },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Initiated video call")
             log.info(f"Began video call to GUILD: {guild} and CHANNEL: {channel}")
-        if guild == None:
+        if guild is None:
             await self.http.request(
                 method="post",
                 endpoint=f"/channels/{channel}/call/ring",
                 json={"recipients": None},
             )
             if self.debug:
                 log.debug("Sent Ring")
@@ -609,15 +614,15 @@
                 "self_video": False,
             },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Initiated call")
             log.info(f"Began call to GUILD: {guild} and CHANNEL: {channel}")
-        if guild == None:
+        if guild is None:
             await self.http.request(
                 method="post",
                 endpoint=f"/channels/{channel}/call/ring",
                 json={"recipients": None},
             )
             if self.debug:
                 log.debug("Sent Ring")
@@ -625,29 +630,30 @@
     async def stream_call(self, channel: str, guild=None):
         """Initiates a discord stream call
 
         Args:
             channel (str): Channel ID
             guild (str, optional): Guild ID. Defaults to None.
         """
+        await self.call(channel, guild)
         type = "guild" if guild != None else "call"
         payload = {
             "op": 18,
             "d": {
                 "guild_id": guild,
                 "channel_id": channel,
                 "preferred_region": "rotterdam",
                 "type": type,
             },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Initiated call")
             log.info(f"Began call to GUILD: {guild} and CHANNEL: {channel}")
-        if guild == None:
+        if guild is None:
             await self.http.request(
                 method="post",
                 endpoint=f"/channels/{channel}/call/ring",
                 json={"recipients": None},
             )
 
             payload = {
```

### Comparing `selfcord.py-0.1.9/selfcord/api/http.py` & `selfcord.py-0.2.0/selfcord/api/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -91,28 +91,31 @@
         Raises:
             LoginFailure: If you suck
 
         Returns:
             dict: Data, json data
         """
         url = self.base_url + endpoint
-
         headers = {
             "cookie": f"{self.cookie}",
             "authorization": self.token,
             "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36",
             "Content-Type": "application/json",
             "X-Super-Properties": self.xproperties,
             "X-Discord-Locale": "en-GB",
+            "X-context-properties": "eyJsb2NhdGlvbiI6Ikludml0ZSBCdXR0b24gRW1iZWQiLCJsb2NhdGlvbl9ndWlsZF9pZCI6bnVsbCwibG9jYXRpb25fY2hhbm5lbF9pZCI6IjEwOTkwOTMxODEyNTUxNDM1MjUiLCJsb2NhdGlvbl9jaGFubmVsX3R5cGUiOjEsImxvY2F0aW9uX21lc3NhZ2VfaWQiOiIxMTE2NTE0MDMyODk2MTgwMjU0In0=",
+            "connection": "keep-alive",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "origin": "https://discord.com",
+            "DNT": "1",
             "x-debug-options": "logGatewayEvents,logOverlayEvents,logAnalyticsEvents,bugReporterEnabled",
             "x-fingerprint": self.fingerprint,
+            "x-discord-timezone": "Europe/London",
             "TE": "trailers",
         }
 
         async with ClientSession(
             timeout=aiohttp.ClientTimeout(
                 total=10000, connect=10000, sock_read=10000, sock_connect=10000
             ),
@@ -121,15 +124,15 @@
             ),
             headers=headers,
         ) as session:
             request = getattr(session, method)
             while True:
                 async with request(url, *args, **kwargs) as resp:
                     if self.debug:
-                        log.debug(f"Sent Request URL: {url} Payload: {args} {kwargs}")
+                        log.debug(f"Sent Request Method: {method} URL: {url} Payload: {args} {kwargs}")
 
                     if resp.status == 429:
                         try:
                             json = await resp.json()
                             await asyncio.sleep(json["retry_after"])
                             if self.debug:
                                 log.error(f"429 Ratelimited: {json}")
@@ -143,18 +146,14 @@
                                 log.info(
                                     f"Attempted to send request to URL: {url} PAYLOAD: {kwargs}"
                                 )
                             break
 
                     elif resp.status == 401:
                         json = await resp.json()
-                        if self.debug:
-                            log.info(
-                                f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
-                            )
                         log.error(f"{json} -- {resp.status}")
                         break
 
                     elif resp.status == 403:
                         json = await resp.json()
                         log.error(f"403 Unauthorized: {json}")
                         if self.debug:
```

### Comparing `selfcord.py-0.1.9/selfcord/api/voice/voice.py` & `selfcord.py-0.2.0/selfcord/api/voice/voice.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/selfcord/bot.py` & `selfcord.py-0.2.0/selfcord/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,36 +11,19 @@
 from traceback import format_exception
 from typing import TYPE_CHECKING
 
 import aiohttp
 from aioconsole import aexec
 
 from .api import Activity, gateway, http
-from .models import (
-    Client,
-    DMChannel,
-    GroupChannel,
-    Guild,
-    InteractionUtil,
-    Option,
-    Search,
-    SlashCommand,
-    TextChannel,
-    User,
-    VoiceChannel,
-)
-from .utils import (
-    Command,
-    CommandCollection,
-    Context,
-    Event,
-    Extension,
-    ExtensionCollection,
-    logging,
-)
+from .models import (Client, DMChannel, GroupChannel, Guild, InteractionUtil,
+                     Option, Search, SlashCommand, TextChannel, User,
+                     VoiceChannel)
+from .utils import (Command, CommandCollection, Context, Event, Extension,
+                    ExtensionCollection, logging)
 
 if TYPE_CHECKING:
     from .api.gateway import gateway
     from .api.http import http
 
 log = logging.getLogger("Bot")
 
@@ -94,18 +77,16 @@
             data = await self.http.static_login(token)
             self.user = Client(data)
             await self.gateway.start(token, self.user, self)
             if self.debug:
                 log.debug("Started Bot")
                 log.info(f"Logged in as {self.user}")
 
-        try:
+        with contextlib.suppress(KeyboardInterrupt):
             asyncio.run(runner())
-        except KeyboardInterrupt:
-            pass
 
     @property
     def latency(self):
         """Latency of heartbeat ack, gateway latency essentially"""
         return self.gateway.latency
 
     # For events
@@ -124,48 +105,48 @@
                     msg += f"[ .Commands ]\n"
                     for command in self.commands:
                         msg += f". {command.name}: {command.description}\n"
                     msg += "\n[ .Extensions ]\n"
                     for ext in self.extensions:
                         msg += f"[ {ext.name} ] : [ {ext.description} ]\n"
 
-                    msg += f"```"
+                    msg += "```"
                     return await ctx.reply(f"{msg}")
 
                 else:
                     name = cat.lower()
                     for ext in self.extensions:
                         if name == ext.name.lower():
                             msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
                             msg += f"[ {self.user} ]\n\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n\n[ .Prefixes ] : {self.prefixes}\n\n"
                             msg += f"[ .Commands ]\n"
                             for command in ext.commands:
                                 if command.ext == ext.ext:
                                     msg += f". {command.name}: {command.description}\n"
 
-                            msg += f"```"
+                            msg += "```"
                             return await ctx.reply(f"{msg}")
                     else:
                         for cmd in self.commands:
                             if name == cmd.name.lower():
                                 msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
                                 msg += f"[ {self.user} ]\n\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n\n[ .Prefixes ] : {self.prefixes}\n\n"
                                 msg += f"[ .{cmd.name} ]\n"
                                 msg += f"[ Description ] :  {cmd.description} \n"
                                 msg += f"[ Long Description ] :\n{cmd.func.__doc__}\n"
                                 msg += f"[ Aliases ] : {cmd.aliases} \n"
                                 args = inspect.signature(cmd.func)
                                 msg += f"\n[ Example Usage ] :\n[ {self.prefixes[0]}{cmd.aliases[0]}"
                                 for arg in args.parameters.keys():
-                                    if arg == "self" or arg == "ctx":
+                                    if arg in ["self", "ctx"]:
                                         continue
                                     msg += f" <{arg}>"
-                                msg += f" ]"
+                                msg += " ]"
 
-                                msg += f"```"
+                                msg += "```"
                                 return await ctx.reply(f"{msg}")
                         for ext in self.extensions:
                             for cmd in ext.commands:
                                 if name == cmd.name.lower():
                                     msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
                                     msg += f"[ {self.user} ]\n\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n\n[ .Prefixes ] : {self.prefixes}\n\n"
                                     msg += f"[ .{cmd.name} ]\n"
@@ -173,20 +154,20 @@
                                     msg += (
                                         f"[ Long Description ] :\n{cmd.func.__doc__}\n"
                                     )
                                     msg += f"[ Aliases ] :  {cmd.aliases} \n"
                                     args = inspect.signature(cmd.func)
                                     msg += f"\n[ Example Usage ] :\n[ {self.prefixes[0]}{cmd.aliases[0]}"
                                     for arg in args.parameters.keys():
-                                        if arg == "self" or arg == "ctx":
+                                        if arg in ["self", "ctx"]:
                                             continue
                                         msg += f" <{arg}>"
-                                    msg += f" ]"
+                                    msg += " ]"
 
-                                    msg += f"```"
+                                    msg += "```"
                                     return await ctx.reply(f"{msg}")
 
         if self.eval:
 
             def clean_code(content):
                 if content.startswith("```") and content.endswith("```"):
                     return "\n".join(content.split("\n")[1:])[:-3]
@@ -196,15 +177,15 @@
             @self.cmd(description="Executes and runs code", aliases=["exec"])
             async def eval(ctx, *, code):
                 """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution."""
                 code = clean_code(code)
 
                 try:
                     with contextlib.redirect_stdout(io.StringIO()) as f:
-                        await aexec(code)
+                        await aexec(source=code, local=globals() )
                         result = f"```{f.getvalue()}\n```"
                 except Exception as e:
                     error = "".join(format_exception(e, e, e.__traceback__))
                     result = f"```\n{error}```"
 
                 await ctx.reply(result)
 
@@ -234,15 +215,15 @@
 
     async def emit(self, event, *args, **kwargs):
         """Used to essentially push values to the decorator when the event fires
 
         Args:
             event (str): The event name
         """
-        on_event = "on_{}".format(event)
+        on_event = f"on_{event}"
 
         # try:
         if hasattr(self, on_event):
             await getattr(self, on_event)(*args, **kwargs)
         if event in self._events.keys():
             for Event in self._events[event]:
                 if Event.coro.__code__.co_varnames[0] == "self":
@@ -446,39 +427,36 @@
         Returns:
 
             User: The User object
         """
 
         data = await self.http.request(method="get", endpoint=f"/users/{user_id}")
 
-        user = User(data, bot=self, http=self.http)
-        return user
+        return User(data, bot=self, http=self.http)
 
     async def create_guild(
         self, name: str, icon_url: str = None, template: str = "2TffvPucqHkN"
     ):
         """Creates a guild"""
-        if icon_url is not None:
-            image = await self.http.encode_image(icon_url)
-        else:
-            image = None
-        await self.http.request(
+        image = None if icon_url is None else await self.http.encode_image(icon_url)
+        json = await self.http.request(
             method="post",
-            endpoint=f"/guilds",
+            endpoint="/guilds",
             headers={
                 "origin": "https://discord.com",
                 "referer": "https://discord.com/channels/@me",
             },
             json={"name": name, "icon": image, "template": template},
         )
         if self.debug:
             log.debug("Finished Creating Guild")
             log.info(
                 f"Created Guild NAME: {name} TEMPLATE: {template} ICON: {icon_url}"
             )
+        return Guild(json, self, self.http)
 
     async def add_friend(self, user_id: str):
         """
         Function to add a specific user as a friend.
 
         Args:
             user_id (str): ID of the possible random user.
@@ -504,15 +482,15 @@
         """Edits user profile"""
         fields = {}
         if bio != None:
             fields["bio"] = bio
         if accent != None:
             fields["accent"] = accent
         await self.http.request(
-            method="patch", endpoint=f"/users/@me/profile", json=fields
+            method="patch", endpoint="/users/@me/profile", json=fields
         )
         if self.debug:
             log.debug("Finished Edit profile")
 
     async def change_pfp(self, avatar_url=None):
         """Disclaimer: This may phone lock your account :(
 
@@ -559,14 +537,29 @@
             )
             if self.debug:
                 log.debug("Created DM Channel")
             return DMChannel(data, bot=self, http=self.http)
         else:
             log.error("Recipient ID not specified")
 
+    async def join_guild(self, code: str) -> Guild | None:
+        """Helper function to join guilds
+        
+        Args:
+            code (str): Invite Code
+        Returns:
+            Guild object | None
+        """
+        data = await self.http.request("post", f"/invites/{code}", json = {
+            "session_id": f"{self.session_id}"
+        }
+        )
+        if data is not None:
+            return Guild(data['guild'], self, self.http)
+        return None
     async def redeem_nitro(self, code: str):
         """Helper function to redeem nitro
 
         Args:
             code (str): Nitro code
         """
         async with aiohttp.ClientSession() as session:
```

### Comparing `selfcord.py-0.1.9/selfcord/models/channel.py` & `selfcord.py-0.2.0/selfcord/models/channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from __future__ import annotations
 
 import asyncio
+import os
+import random
 from traceback import format_exception
 from typing import TYPE_CHECKING
 
+import aiofiles
+import aiohttp
+
 from ..utils import logging
 from .message import Message
 from .user import User
 from .webhook import Webhook
 
 if TYPE_CHECKING:
     from ..api.http import http
@@ -20,89 +25,123 @@
 class Messageable:
     """Parent class specific for those classes that include a textchat for sending messages."""
 
     def __init__(self, http: http, bot: Bot) -> None:
         self.http: http = http
         self.bot: Bot = bot
 
-    async def history(self) -> list[Message] | None:
+    @property
+    def make_nonce(self):
+        """Generate pseudorandom number."""
+        return str(random.randint(0, 100000000))
+
+    async def history(self, amount: int = 100) -> list[Message] | None:
         """
         Get channel message history.
 
         Args:
-            No arguments required
+            amount(int) : Amount of messages to gather. Default is 100.
 
         Returns:
             messages(list) : List of messages from the channel.
             None : If client does not have view permission for the channel or no data found
         """
-        messages = []
-        data = await self.http.request(
-            method="get", endpoint=f"/channels/{self.id}/messages?limit=100"
-        )
+        if amount >= 100:
+            data = await self.http.request(
+                method="get", endpoint=f"/channels/{self.id}/messages?limit=100"
+            )
+        else:
+            data = await self.http.request(
+                method="get", endpoint=f"/channels/{self.id}/messages?limit={amount + 5}"
+            )
+
         if data is None:
             return None
 
-        for msg in data:
-            messages.append(Message(msg, self.bot, self.http))
+        messages = [Message(msg, self.bot, self.http) for msg in data]
         while True:
+            
+
             data = await self.http.request(
                 method="get",
                 endpoint=f"/channels/{self.id}/messages?limit=100&before={data[-1]['id']}",
             )
-            if len(data) > 0:
-                for msg in data:
-                    messages.append(Message(msg, self.bot, self.http))
-            else:
+
+            if len(data) <= 0:
+                break
+            messages.extend(Message(msg, self.bot, self.http) for msg in data)
+            if len(messages) >= amount:
                 break
 
         return messages
 
+    async def upload_image(self, paths: list[str]) -> list[dict[str, int | str]]:
+        files = []
+        id = 0
+        for path in paths:
+            async with aiofiles.open(path, "rb") as f:
+                file = await f.read()
+                size = len(file)
+                name = os.path.basename(path)
+            files.append({"file_size" : size, "filename": f"{name}", "id": id})
+            id += 1
+        json = await self.http.request("post", f"/channels/{self.id}/attachments", json={"files": files})
+        items = []
+        for key, atch in enumerate(json['attachments']):
+            upload_url = atch['upload_url']
+            id = atch['id']
+            upload_filename = atch['upload_filename']
+            async with aiohttp.ClientSession() as session:
+                async with aiofiles.open(paths[key], "rb") as f:
+                    file = await f.read()
+                async with session.put(upload_url, data=file): 
+                    pass
+            items.append({"uploaded_filename": upload_filename, "filename": os.path.basename(upload_filename) , "id": id})
+        return items
+
+        
+
     async def purge(self, amount: int = 0) -> None:
         """
         Delete a number of messages, starting from the most recent.
 
         Args:
             amount(int) : Number of messages to purge/delete.
 
         Returns:
             No return value
         """
-        messages = await self.history()
-        msgs = []
-        for msg in messages:
-            if str(msg.author.id) == str(self.bot.user.id):
-                msgs.append(msg)
-
+        messages = await self.history(amount)
+        if messages is None:
+            return
+        msgs = [msg for msg in messages if str(msg.author.id) == str(self.bot.user.id)]
         if amount != 0:
             for i in range(0, len(msgs[:amount]), 3):
                 await asyncio.gather(
                     *(
                         asyncio.create_task(message.delete())
                         for message in msgs[:amount][i : i + 3]
                     )
                 )
-        else:
-            for i in range(0, len(msgs), 3):
-                await asyncio.gather(
-                    *(
-                        asyncio.create_task(message.delete())
-                        for message in msgs[i : i + 3]
-                    )
+                await asyncio.sleep(0.3)
+            return
+
+
+        for i in range(0, len(msgs), 3):
+            await asyncio.gather(
+                *(
+                    asyncio.create_task(message.delete())
+                    for message in msgs[i : i + 3]
                 )
+            )
+            await asyncio.sleep(0.3)
 
-    #            for i in range(0, len(msgs[:amount]), 2):
-    #                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[:amount][i:i + 2]))
-    #                await asyncio.sleep(0.2)
-    #        else:
-    #            for i in range(0, len(msgs), 2):
-    #                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[i:i + 2]))
-    #                await asyncio.sleep(0.2)
 
-    async def spam(self, amount: int, content: str, tts=False) -> None:
+
+    async def spam(self, amount: int, content: str, file_paths: list[str] = [], tts=False) -> None:
         """
         Send multiple of the same message.
 
         Args:
             - amount(int) : Number of spam messages to send.
             - content(str) : The message to send.
             - tts(bool) = False : Specify whether it is a TTS message.
@@ -110,109 +149,106 @@
         Returns:
             No return value.
         """
         amount: list[int] = [i + 1 for i in range(amount)]
         for i in range(0, len(amount), 3):
             await asyncio.gather(
                 *(
-                    asyncio.create_task(self.send(tts=tts, content=content))
-                    for amoun in amount[i : i + 3]
+                    asyncio.create_task(self.send(tts=tts, content=content, file_paths=file_paths))
+                    for _ in amount[i : i + 3]
                 )
             )
             await asyncio.sleep(0.3)
 
-    async def send(self, content=None, tts=False) -> Message:
+    async def send(self, content=None, file_paths: list[str] = [], tts=False) -> Message:
         """
         Send a message to the text channel.
 
         Args:
             - content(str) : Message content. Should be string type or similar. Discord `embed` type is not allowed.
             - tts(bool) : Specify whether message is text-to-speech or not
 
         Returns:
             Message object.
         """
+        json = {"content": content, "nonce": self.make_nonce, "tts": tts}
+        if file_paths != []:
+            vals = await self.upload_image(file_paths)
+            json |= {"attachments" : vals}
+
         if hasattr(self, "guild_id"):
             resp = await self.http.request(
                 method="post",
                 endpoint=f"/channels/{self.id}/messages",
                 headers={
                     "origin": "https://discord.com",
                     "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}",
                 },
-                json={"content": content, "tts": tts},
+                json=json
             )
             resp.update({"guild_id": self.guild_id})
 
         else:
             resp = await self.http.request(
                 method="post",
                 endpoint=f"/channels/{self.id}/messages",
                 headers={
                     "origin": "https://discord.com",
                     "referer": f"https://discord.com/channels/{self.id}",
                 },
-                json={"content": content, "tts": tts},
+                json=json
             )
 
         return Message(resp, self.bot, self.http)
 
-    async def reply(self, message: str, content=None, tts=False) -> Message:
+    async def reply(self, message: Message, content: str, file_paths: list[str] = [], tts=False) -> Message:
         """Reply to a specific message
 
         Args:
             message (str): Message to reply to
             content (_type_, optional): Message content to reply with. Defaults to None.
             tts (bool, optional): Specify whether message is text-to-speech or not. Defaults to False.
 
         Returns:
             Message object.
         """
+        json = {
+            "content": content,
+            "tts": tts,
+            "nonce": self.make_nonce,
+            "message_reference": {
+                "channel_id": f"{self.id}",
+                "message_id": f"{message.id}",
+            },
+        }
+
+        if file_paths != []:
+            vals = await self.upload_image(file_paths)
+            json |= {"attachments" : vals}
+
         if hasattr(self, "guild_id"):
             resp = await self.http.request(
                 method="post",
                 endpoint=f"/channels/{self.id}/messages",
                 headers={
                     "origin": "https://discord.com",
                     "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}",
                 },
-                json={
-                    "content": content,
-                    "tts": tts,
-                    "message_reference": {
-                        "channel_id": f"{self.id}",
-                        "message_id": f"{message.id}",
-                    },
-                    "allowed_mentions": {
-                        "parse": ["users", "roles", "everyone"],
-                        "replied_user": False,
-                    },
-                },
+                json=json
             )
             resp.update({"guild_id": self.guild_id})
         else:
             resp = await self.http.request(
                 method="post",
                 endpoint=f"/channels/{self.id}/messages",
                 headers={
                     "origin": "https://discord.com",
                     "referer": f"https://discord.com/channels/{self.id}",
                 },
-                json={
-                    "content": content,
-                    "tts": tts,
-                    "message_reference": {
-                        "channel_id": f"{self.id}",
-                        "message_id": f"{message.id}",
-                    },
-                    "allowed_mentions": {
-                        "parse": ["users", "roles", "everyone"],
-                        "replied_user": False,
-                    },
-                },
+                json=json
             )
         return Message(resp, self.bot, self.http)
 
 
 class Voiceable(Messageable):
     """Parent class specific for those classes that include a voice chat, or call functionality"""
 
@@ -326,15 +362,15 @@
             No arguments required
 
         Returns:
             No return value
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
-
+    
     async def edit(
         self,
         name: str = None,
         parent_id: int = None,
         position: int = None,
         topic: str = None,
     ):
```

### Comparing `selfcord.py-0.1.9/selfcord/models/client.py` & `selfcord.py-0.2.0/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/selfcord/models/emoji.py` & `selfcord.py-0.2.0/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/selfcord/models/guild.py` & `selfcord.py-0.2.0/selfcord/models/guild.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,45 +61,40 @@
         self.mfa_level = data.get("mfa_level")
         self.features = data.get("features")
         self.member_count = data.get("member_count")
         self.unavailable = data.get("unavailable")
         self.verification_level = data.get("verification_level")
         self.explicit_content_filter = data.get("explicit_content_filter")
         self.owner_id = data.get("owner_id")
-
+        members, channels, roles, emojis = (data.get("members") if data.get("members") is not None else [], data.get("channels") if data.get("channels") is not None else [],data.get("roles") if data.get("roles") is not None else [], data.get("emojis") if data.get("emojis") is not None else [])
+        
         for member, channel, role, emoji in zip_longest(
-            data.get("members"),
-            data.get("channels"),
-            data.get("roles"),
-            data.get("emojis"),
+            members,
+            channels,
+            roles,
+            emojis
         ):
             if member != None:
                 user = User(member, self.bot, self.http)
 
                 self.members.append(user)
 
             if channel != None:
                 type = channel.get("type")
-                if type == self.TEXTCHANNEL:
+                if type == self.TEXTCHANNEL or type not in [
+                    self.VOICECHANNEL,
+                    self.CATEGORY,
+                ]:
                     channel = TextChannel(channel, self.bot, self.http)
-                    channel.guild_id = self.id
-                    self.channels.append(channel)
                 elif type == self.VOICECHANNEL:
                     channel = VoiceChannel(channel, self.bot, self.http)
-                    channel.guild_id = self.id
-                    self.channels.append(channel)
-                elif type == self.CATEGORY:
-                    channel = Category(channel, self.bot, self.http)
-                    channel.guild_id = self.id
-                    self.channels.append(channel)
                 else:
-                    channel = TextChannel(channel, self.bot, self.http)
-                    channel.guild_id = self.id
-                    self.channels.append(channel)
-
+                    channel = Category(channel, self.bot, self.http)
+                channel.guild_id = self.id
+                self.channels.append(channel)
             if role != None:
                 role = Role(role, self.bot, self.http, guild_id=self.id)
                 self.roles.append(role)
 
             if emoji != None:
                 emoji = Emoji(emoji, self.bot, self.http)
                 emoji.guild_id = self.id
@@ -150,19 +145,17 @@
     async def txt_channel_create(self, name: str, parent_id: str = None):
         """Creates a Text Channel in the guild
 
         Args:
             name (str): Name of the channel
             parent_id (str, optional): ID of the category. Defaults to None.
         """
-        payload = {"name": name}
-        payload.update({"permission_overwrites": []})
-        payload.update({"type": 0})
+        payload = {"name": name, "permission_overwrites": [], "type": 0}
         if parent_id != None:
-            payload.update({"parent_id": parent_id})
+            payload["parent_id"] = parent_id
 
         channel = await self.http.request(
             method="post", endpoint=f"/guilds/{self.id}/channels", json=payload
         )
         return TextChannel(channel, self.bot, self.http)
 
     async def vc_channel_create(self, name: str):
```

### Comparing `selfcord.py-0.1.9/selfcord/models/interactions.py` & `selfcord.py-0.2.0/selfcord/models/interactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,15 @@
         self.value: str = None
 
     def __str__(self):
         return f"{self.name}"
 
     def __iter__(self):
         if self.options is not None:
-            for option in self.options:
-                yield option
+            yield from self.options
         else:
             yield None
 
 
 class SlashCommand:
     def __init__(self, data: dict) -> None:
         self.id: str = data["id"]
@@ -65,16 +64,15 @@
             else None
         )
         self.guild_id: str | None = data.get("guild_id")
         self.target_id: str | None = data.get("target_id")
 
     def __iter__(self):
         if self.options is not None:
-            for option in self.options:
-                yield option
+            yield from self.options
         else:
             yield None
 
     def __str__(self):
         return f"{self.name}"
 
     def __eq__(self, other):
@@ -141,30 +139,26 @@
             "type": 2,
             "application_id": bot_id,
             "channel_id": channel_id,
             "nonce": nonce,
             "session_id": self.bot.session_id,
         }
         if guild_id is not None:
-            payload.update({"guild_id": guild_id})
-
+            payload["guild_id"] = guild_id
         data = {
             "version": command.version,
             "id": command.id,
             "name": command.name,
             "type": command.type,
             "options": [],
             "application_command": command.raw_data,
             "attachments": [],
         }
-        if value is not None:
-            last_val = value[-1]
         if option is not None:
             dic = {"options": []}
-            last_opt = option[-1]
             for index, (opt, value) in enumerate(zip_longest(option, value)):
                 if index == 0:
                     if value is None:
                         dic["options"].append(
                             {"name": opt.name, "type": opt.type, "options": []}
                         )
                     else:
@@ -173,16 +167,16 @@
                         )
                 elif value is not None:
                     for opten in dic["options"]:
                         opten["options"].append(
                             {"name": opt.name, "type": opt.type, "value": value}
                         )
 
-            data.update(dic)
-        payload.update({"data": data})
+            data |= dic
+        payload["data"] = data
         randstr = "".join(random.sample(string.ascii_letters + string.digits, k=16))
         boundary_val = f"----WebkitFormBoundary{randstr}"
         req_data = f'--{boundary_val}\r\nContent-Disposition: form-data; name="payload_json"\r\n\r\n{json.dumps(payload)}\r\n--{boundary_val}--'
         await self.http.request(
             "post",
             "/interactions",
             headers={"content-type": f"multipart/form-data; boundary={boundary_val}"},
```

### Comparing `selfcord.py-0.1.9/selfcord/models/member.py` & `selfcord.py-0.2.0/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/selfcord/models/message.py` & `selfcord.py-0.2.0/selfcord/models/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import time
 import urllib
+from itertools import zip_longest
 
 from .user import User
 
 
 class Attachment:
     def __init__(self, data) -> None:
         self.proxy_url = data.get("proxy_url")
@@ -36,65 +37,75 @@
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         self.tts = data.get("tts")
         self.referenced_message = data.get("referenced_message")
-        self.mentions = data.get("mentions")
         self.author = User(data.get("author"), self.bot, self.http)
         self.id = data.get("id")
         self.flags = data.get("flags")
         self.embeds = data.get("embeds")
         self.content = data.get("content")
         self.components = data.get("components")
         self.timestamp = time.time()
         self.channel_id = data.get("channel_id")
 
         attachments = data.get("attachments")
-        self.attachments = [Attachment(atch) for atch in attachments]
+        self.attachments = []
+        self.mentions = []
+        for mention, atch in zip_longest(data.get("mentions"), attachments):
+            if atch is not None:
+                self.attachments.append(Attachment(atch))
+            if mention is not None:
+                self.mentions.append(User(mention, self.bot, self.http))
         self.guild_id = data.get("guild_id")
 
         self.channel = self.bot.get_channel(self.channel_id)
 
         self.guild = self.bot.get_guild(self.guild_id)
 
     async def delete(self):
         """Delete the Message Object"""
         await self.http.request(
             method="delete", endpoint=f"/channels/{self.channel_id}/messages/{self.id}"
         )
 
-    async def edit(self, content: str) -> Message:
+    async def edit(self, content: str, file_paths: list[str] = []) -> Message:
         """Edits the specified message
 
         Args:
             content (str): Content to edit message to.
         """
-        if self.guild_id != None:
+        json = { "content":  content }
+        if file_paths != []:
+            vals = await self.channel.upload_image(file_paths)
+            json |= {"attachments" : vals}
+
+        if self.guild_id is None:
             resp = await self.http.request(
                 method="patch",
                 endpoint=f"/channels/{self.channel_id}/messages/{self.id}",
                 headers={
                     "origin": "https://discord.com",
-                    "referer": f"https://discord.com/channels/{self.channel_id}/{self.guild_id}",
+                    "referer": f"https://discord.com/channels/{self.channel_id}",
                 },
-                json={"content": content},
+                json=json,
             )
-            resp.update({"guild_id": self.guild_id})
         else:
             resp = await self.http.request(
                 method="patch",
                 endpoint=f"/channels/{self.channel_id}/messages/{self.id}",
                 headers={
                     "origin": "https://discord.com",
-                    "referer": f"https://discord.com/channels/{self.channel_id}",
+                    "referer": f"https://discord.com/channels/{self.channel_id}/{self.guild_id}",
                 },
-                json={"content": content},
+                json=json,
             )
+            resp.update({"guild_id": self.guild_id})
         return Message(resp, self.bot, self.http)
 
     async def react(self, emoji: str):
         """React to a message with an emoji
 
         Args:
             emoji (str): The emoji
```

### Comparing `selfcord.py-0.1.9/selfcord/models/permission.py` & `selfcord.py-0.2.0/selfcord/models/permission.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,13 +47,12 @@
             "SEND_MESSAGES_IN_THREADS": 0x4000000000,
             "USE_EMBEDDED_ACTIVITIES": 0x8000000000,
             "MODERATE_MEMBERS": 0x10000000000,
         }
         self.permissions = self.calculate_permissions(data)
 
     def calculate_permissions(self, perm_value: int):
-        permissions = []
-        for perm, value in self.perms.items():
-            if (perm_value & value) == value:
-                permissions.append(perm)
-
-        return permissions
+        return [
+            perm
+            for perm, value in self.perms.items()
+            if (perm_value & value) == value
+        ]
```

### Comparing `selfcord.py-0.1.9/selfcord/models/role.py` & `selfcord.py-0.2.0/selfcord/models/role.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,30 +25,30 @@
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
         role = data.get("role")
 
-        self.id = data.get("id") if role == None else role.get("id")
+        self.id = data.get("id") if role is None else role.get("id")
         self.permissions = (
             Permission(int(data.get("permissions"))).permissions
-            if role == None
+            if role is None
             else Permission(int(role.get("permissions"))).permissions
         )
-        self.name = data.get("name") if role == None else role.get("name")
+        self.name = data.get("name") if role is None else role.get("name")
         self.mentionable = (
-            data.get("mentionable") if role == None else role.get("mentionable")
+            data.get("mentionable") if role is None else role.get("mentionable")
         )
-        self.managed = data.get("managed") if role == None else role.get("managed")
-        self.icon = data.get("icon") if role == None else role.get("icon")
-        self.flags = data.get("flags") if role == None else role.get("flags")
+        self.managed = data.get("managed") if role is None else role.get("managed")
+        self.icon = data.get("icon") if role is None else role.get("icon")
+        self.flags = data.get("flags") if role is None else role.get("flags")
 
-        self.color = data.get("color") if role == None else role.get("color")
-        self.hoist = data.get("hoist") if role == None else role.get("hoist")
+        self.color = data.get("color") if role is None else role.get("color")
+        self.hoist = data.get("hoist") if role is None else role.get("hoist")
         if self.guild_id is None:
             self.guild_id = data.get("guild_id")
 
     def __str__(self) -> str:
         return f"{self.name}"
 
     async def delete(self):
```

### Comparing `selfcord.py-0.1.9/selfcord/models/webhook.py` & `selfcord.py-0.2.0/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/selfcord/utils/command.py` & `selfcord.py-0.2.0/selfcord/utils/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,46 +40,42 @@
 class ExtensionCollection:
     """Extension collection, where extensions are stored into. Utilised for Extender, Extensions as a whole. This is also used within help commands and command invocation."""
 
     def __init__(self):
         self.extensions = {}
 
     def __iter__(self):
-        for cmd in self.extensions.values():
-            yield cmd
+        yield from self.extensions.values()
 
     def _is_already_registered(self, ext: Extension) -> bool:
         """Whether the specified Extension is already registered
 
         Args:
             ext (Extension): Extension to check
 
         Returns:
             bool: True or False
         """
         for extension in self.extensions.values():
-            if ext.name == extension:
-                return True
-            else:
-                return False
+            return ext.name == extension
         else:
             return False
 
     def add(self, ext: Extension):
         """Adds an extension
 
         Args:
             ext (Extension): Extension to add
 
         Raises:
             ValueError: Extension must be subclass of extension
             ValueError: A name or alias is already registered
         """
         if not isinstance(ext, Extension):
-            log.error(f"ext is not an Extension or subclass of Extension")
+            log.error("ext is not an Extension or subclass of Extension")
         if self._is_already_registered(ext):
             log.error("Name or Alias is already registered")
         # Add extension to the collection
         self.extensions[ext.name] = ext
 
     def get(self, alias: str) -> Extension | None:
         """Get an extension
@@ -118,32 +114,28 @@
         self.commands: dict[CommandCollection, function] = {}
         self.recent_commands: dict[CommandCollection, function] = {}
 
     def __len__(self):
         return len(self.commands)
 
     def __iter__(self):
-        for cmd in self.commands.values():
-            yield cmd
+        yield from self.commands.values()
 
     def _is_already_registered(self, cmd: Command) -> bool:
         """Whether the specified Command is already registered
 
         Args:
             cmd (Command): Command to check
 
         Returns:
             bool: True or False
         """
         for command in self.commands.values():
             for alias in cmd.aliases:
-                if alias in command.aliases:
-                    return True
-                else:
-                    return False
+                return alias in command.aliases
             else:
                 return False
         else:
             return False
 
     def append(self, collection):
         """Append to commands, and recent_commands
@@ -179,16 +171,15 @@
 
     def recents(self):
         """View commands recently acquired
 
         Yields:
             Generator: [Command]
         """
-        for cmd in self.recent_commands.values():
-            yield cmd
+        yield from self.recent_commands.values()
 
     def copy(self):
         """Copy commands from recents to main collection"""
         self.commands.update(self.recent_commands)
         self.clear()
 
     def clear(self):
@@ -372,15 +363,15 @@
     @property
     def command_content(self) -> str | None:
         """The content minus the prefix and command name, essentially the args
 
         Returns:
             str: String of content
         """
-        if self.alias == None:
+        if self.alias is None:
             return
         try:
             cut = len(self.prefix + self.alias)
             return self.content[cut:]
         except:
             return None
 
@@ -412,30 +403,29 @@
             _type_: _description_
         """
         args: list[Any] = []
         kwargs: dict[Any, Any] = {}
 
         if self.command.signature is not None:
             signature = self.command.signature
-        if self.command_content != "":
-            splitted = self.command_content.split(" ")[1:]
-
-            for index, item in enumerate(splitted):
-                user_regex = re.findall(r"<@[0-9]{18,19}>", item)
-                if len(user_regex) > 0:
-                    x = re.findall(r"[0-9]{18,19}", item)
-                    if len(x) > 0:
-                        val = x[0]
-                        splitted[index] = val
-                break
-        else:
+        if self.command_content == "":
             return args, kwargs
 
+        splitted = self.command_content.split(" ")[1:]
+
+        for index, item in enumerate(splitted):
+            user_regex = re.findall(r"<@[0-9]{18,19}>", item)
+            if len(user_regex) > 0:
+                x = re.findall(r"[0-9]{18,19}", item)
+                if len(x) > 0:
+                    val = x[0]
+                    splitted[index] = val
+            break
         for index, (name, param) in enumerate(signature):
-            if name == "ctx" or name == "self":
+            if name in ["ctx", "self"]:
                 continue
 
             if param.kind is param.POSITIONAL_OR_KEYWORD:
                 try:
                     arg: str | Any = self.convert(param, splitted.pop(0))
                     args.append(arg)
                 except Exception:
@@ -472,52 +462,52 @@
                 args.insert(0, self)
         try:
             await func(*args, **kwargs)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not run command \n{error}")
 
-    async def reply(self, content: str, tts=False) -> Message:
+    async def reply(self, content: str, file_paths: list[str] = [], tts=False) -> Message:
         """Helper function to reply to your own message containing the command
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        message: Message = await self.channel.reply(self.message, content, tts)
+        message: Message = await self.channel.reply(self.message, content, file_paths, tts)
         return message
 
-    async def send(self, content: str, tts=False) -> Message:
+    async def send(self, content: str, file_paths: list[str] = [], tts=False) -> Message:
         """Helper function to send message to the current channel
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        message: Message = await self.channel.send(content=content, tts=tts)
+        message: Message = await self.channel.send(content=content, file_paths=file_paths, tts=tts)
         return message
 
-    async def spam(self, amount: int, content: str):
+    async def spam(self, amount: int, content: str, file_paths: list[str] = [], tts: bool = False):
         """Helper function to spam messages in the current channel (uses asyncio.gather !!!!)
 
         Args:
             amount (int): Amount of messages to spam
             content (str): The message you would like to send
         """
-        await self.channel.spam(amount, content)
+        await self.channel.spam(amount, content, file_paths, tts)
 
     async def purge(self, amount: int = 0):
         """Helper function to purge messages in the current channel, uses asyncio gather.
 
         Args:
             amount (int): The amount of messages to purge, defaults to All.
         """
         await self.channel.purge(amount)
 
-    async def edit(self, content: str) -> Message:
+    async def edit(self, content: str, file_paths: list[str] = []) -> Message:
         """Helper function to edit the message you sent
 
         Args:
             content (str): Content to edit to
         """
-        message = await self.message.edit(content)
+        message = await self.message.edit(content, file_paths)
         return message
```

### Comparing `selfcord.py-0.1.9/selfcord/utils/logging.py` & `selfcord.py-0.2.0/selfcord/utils/logging.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.2.0/selfcord.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -15,15 +15,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.1.7-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.0-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
@@ -133,13 +133,13 @@
     await ctx.reply(f"{bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 
 bot.run(token)
 ```
 ## Some Useful Links
 - [Documentation](https://github.com/Shell1010/Selfcord/wiki)
 - [Other Documentation (messy)](https://github.com/Shell1010/Selfcord/tree/main/docs)
-- [PyPi](https://pypi.org/project/selfcord/)
+- [PyPi](https://pypi.org/project/selfcord.py/)
 - [Official Discord Server](https://discord.gg/FCFnnBGzkg)
 - [A simple selfbot designed to showcase the library's features](https://github.com/Shell1010/Aeterna-Selfbot)
 
 ## Contributing
 Contributors are always Welcome
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.1.9 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.0 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.1.7-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.0-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
@@ -44,11 +44,11 @@
 ```python import selfcord token = "insert token" bot = selfcord.Bot(prefixes=
 ["!", "?"]) @bot.on("ready") async def ball(time): print(f"Connected To
 {bot.user}\n Startup took {time:0.2f} seconds") @bot.cmd(description="Snipe",
 aliases=['s']) async def snipe(ctx): await ctx.reply(f"
 {bot.user.deleted_messages[-1].author}: {bot.user.deleted_messages[-1]}")
 bot.run(token) ``` ## Some Useful Links - [Documentation](https://github.com/
 Shell1010/Selfcord/wiki) - [Other Documentation (messy)](https://github.com/
-Shell1010/Selfcord/tree/main/docs) - [PyPi](https://pypi.org/project/selfcord/
-) - [Official Discord Server](https://discord.gg/FCFnnBGzkg) - [A simple
-selfbot designed to showcase the library's features](https://github.com/
+Shell1010/Selfcord/tree/main/docs) - [PyPi](https://pypi.org/project/
+selfcord.py/) - [Official Discord Server](https://discord.gg/FCFnnBGzkg) - [A
+simple selfbot designed to showcase the library's features](https://github.com/
 Shell1010/Aeterna-Selfbot) ## Contributing Contributors are always Welcome
```

### Comparing `selfcord.py-0.1.9/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.2.0/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.9/setup.py` & `selfcord.py-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 "selfcord",
                 "selfcord.api",
                 "selfcord.utils",
                 "selfcord.models",
                 "selfcord.api.voice",
             ]
         ),
-        version="0.1.9",
+        version="0.2.0",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell",
         extras_require={"voice": ["pynacl==1.5.0", "opuslib==3.0.1"]},
         license="MIT",
         install_requires=[
             "aiohttp==3.7.4.post0",
```

