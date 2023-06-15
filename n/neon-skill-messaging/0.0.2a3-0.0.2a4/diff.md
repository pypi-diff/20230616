# Comparing `tmp/neon-skill-messaging-0.0.2a3.tar.gz` & `tmp/neon-skill-messaging-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-messaging-0.0.2a3.tar", last modified: Thu Jun 15 22:39:22 2023, max compression
+gzip compressed data, was "neon-skill-messaging-0.0.2a4.tar", last modified: Thu Jun 15 22:44:07 2023, max compression
```

## Comparing `neon-skill-messaging-0.0.2a3.tar` & `neon-skill-messaging-0.0.2a4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:39:22.989585 neon-skill-messaging-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 22:39:22.989585 neon-skill-messaging-0.0.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29710 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:39:22.977585 neon-skill-messaging-0.0.2a3/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:39:22.985585 neon-skill-messaging-0.0.2a3/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/ConfirmCall.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/ConfirmEmail.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/ConfirmMessage.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/ConfirmSend.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/ContactNotFound.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/DiscardDraft.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/EmailSent.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/ErrorDialog.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/GetEmailBody.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/GetEmailSubject.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/GetRecipientAddress.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/OnlyMobile.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/dialog/en-us/TextSent.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:39:22.985585 neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 22:39:22.000000 neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 22:39:22.000000 neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:39:22.000000 neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 22:39:22.000000 neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:39:22.000000 neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 22:39:22.000000 neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:39:22.989585 neon-skill-messaging-0.0.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/skill.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:39:22.981585 neon-skill-messaging-0.0.2a3/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:39:22.989585 neon-skill-messaging-0.0.2a3/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/Neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/draft.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/email.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/klat.voc
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/message.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/sms.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:39:17.000000 neon-skill-messaging-0.0.2a3/vocab/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:44:07.916272 neon-skill-messaging-0.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 22:44:07.916272 neon-skill-messaging-0.0.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29710 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:44:07.912272 neon-skill-messaging-0.0.2a4/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:44:07.912272 neon-skill-messaging-0.0.2a4/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/ConfirmCall.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/ConfirmEmail.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/ConfirmMessage.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/ConfirmSend.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/ContactNotFound.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/DiscardDraft.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/EmailSent.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/ErrorDialog.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/GetEmailBody.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/GetEmailSubject.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/GetRecipientAddress.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/OnlyMobile.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/dialog/en-us/TextSent.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:44:07.916272 neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 22:44:07.000000 neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 22:44:07.000000 neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:44:07.000000 neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 22:44:07.000000 neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 22:44:07.000000 neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 22:44:07.000000 neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:44:07.916272 neon-skill-messaging-0.0.2a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/skill.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:44:07.912272 neon-skill-messaging-0.0.2a4/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:44:07.916272 neon-skill-messaging-0.0.2a4/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/Neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/draft.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/email.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/klat.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/message.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/sms.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 22:44:04.000000 neon-skill-messaging-0.0.2a4/vocab/en-us/yes.voc
```

### Comparing `neon-skill-messaging-0.0.2a3/LICENSE.md` & `neon-skill-messaging-0.0.2a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-messaging-0.0.2a3/PKG-INFO` & `neon-skill-messaging-0.0.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-messaging
-Version: 0.0.2a3
+Version: 0.0.2a4
 Home-page: https://github.com/NeonGeckoCom/skill-messaging
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-messaging-0.0.2a3/README.md` & `neon-skill-messaging-0.0.2a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-messaging-0.0.2a3/__init__.py` & `neon-skill-messaging-0.0.2a4/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/PKG-INFO` & `neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-messaging
-Version: 0.0.2a3
+Version: 0.0.2a4
 Home-page: https://github.com/NeonGeckoCom/skill-messaging
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-messaging-0.0.2a3/neon_skill_messaging.egg-info/SOURCES.txt` & `neon-skill-messaging-0.0.2a4/neon_skill_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-messaging-0.0.2a3/setup.py` & `neon-skill-messaging-0.0.2a4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-messaging"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:MessagingSkill'
+BASE_PATH = path.abspath(path.dirname(__file__))
 
 
 def get_requirements(requirements_filename: str):
-    requirements_file = path.join(path.abspath(path.dirname(__file__)),
-                                  requirements_filename)
+    requirements_file = path.join(BASE_PATH, requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
         requirements = r.readlines()
     requirements = [r.strip() for r in requirements if r.strip()
                     and not r.strip().startswith("#")]
 
     for i in range(0, len(requirements)):
         r = requirements[i]
@@ -55,31 +55,31 @@
                     r.replace("github.com",
                               f"{getenv('GITHUB_TOKEN')}@github.com")
     return requirements
 
 
 def find_resource_files():
     resource_base_dirs = ("locale", "ui", "vocab", "dialog", "regex")
-    base_dir = path.dirname(__file__)
+    base_dir = BASE_PATH
     package_data = ["skill.json"]
     for res in resource_base_dirs:
         if path.isdir(path.join(base_dir, res)):
             for (directory, _, files) in walk(path.join(base_dir, res)):
                 if files:
                     package_data.append(
                         path.join(directory.replace(base_dir, "").lstrip('/'),
                                   '*'))
 #    print(package_data)
     return package_data
 
 
-with open("README.md", "r") as f:
+with open(path.join(BASE_PATH, "README.md"), "r") as f:
     long_description = f.read()
 
-with open("./version.py", "r", encoding="utf-8") as v:
+with open(path.join(BASE_PATH, "version.py"), "r", encoding="utf-8") as v:
     for line in v.readlines():
         if line.startswith("__version__"):
             if '"' in line:
                 version = line.split('"')[1]
             else:
                 version = line.split("'")[1]
```

### Comparing `neon-skill-messaging-0.0.2a3/skill.json` & `neon-skill-messaging-0.0.2a4/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-messaging-0.0.2a3/version.py` & `neon-skill-messaging-0.0.2a4/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.2a3"
+__version__ = "0.0.2a4"
```

