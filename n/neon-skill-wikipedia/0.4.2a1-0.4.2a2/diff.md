# Comparing `tmp/neon-skill-wikipedia-0.4.2a1.tar.gz` & `tmp/neon-skill-wikipedia-0.4.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-wikipedia-0.4.2a1.tar", last modified: Thu Jun 15 22:46:22 2023, max compression
+gzip compressed data, was "neon-skill-wikipedia-0.4.2a2.tar", last modified: Thu Jun 15 22:58:40 2023, max compression
```

## Comparing `neon-skill-wikipedia-0.4.2a1.tar` & `neon-skill-wikipedia-0.4.2a2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:22.721851 neon-skill-wikipedia-0.4.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-15 22:46:22.721851 neon-skill-wikipedia-0.4.2a1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     5671 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:22.709851 neon-skill-wikipedia-0.4.2a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:22.713851 neon-skill-wikipedia-0.4.2a1/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/ca-es/More.voc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/ca-es/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/ca-es/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/ca-es/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/ca-es/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/ca-es/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/ca-es/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:22.717851 neon-skill-wikipedia-0.4.2a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/en-us/More.voc
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/en-us/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/en-us/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/en-us/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/en-us/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/en-us/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/locale/en-us/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:22.717851 neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-15 22:46:22.000000 neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-15 22:46:22.000000 neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:46:22.000000 neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 22:46:22.000000 neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:46:22.000000 neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 22:46:22.000000 neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/pic.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:46:22.721851 neon-skill-wikipedia-0.4.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:22.717851 neon-skill-wikipedia-0.4.2a1/ui/
--rw-r--r--   0 runner    (1001) docker     (123)   907480 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/ui/jumping.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:46:18.000000 neon-skill-wikipedia-0.4.2a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:58:40.989043 neon-skill-wikipedia-0.4.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-15 22:58:40.989043 neon-skill-wikipedia-0.4.2a2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5671 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:58:40.985042 neon-skill-wikipedia-0.4.2a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:58:40.985042 neon-skill-wikipedia-0.4.2a2/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/ca-es/More.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/ca-es/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/ca-es/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/ca-es/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/ca-es/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/ca-es/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/ca-es/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:58:40.989043 neon-skill-wikipedia-0.4.2a2/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/en-us/More.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/en-us/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/en-us/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/en-us/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/en-us/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/en-us/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/locale/en-us/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:58:40.989043 neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-15 22:58:40.000000 neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-15 22:58:40.000000 neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:58:40.000000 neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 22:58:40.000000 neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:58:40.000000 neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 22:58:40.000000 neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/pic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:58:40.989043 neon-skill-wikipedia-0.4.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:58:40.989043 neon-skill-wikipedia-0.4.2a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)   907480 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/ui/jumping.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:58:35.000000 neon-skill-wikipedia-0.4.2a2/version.py
```

### Comparing `neon-skill-wikipedia-0.4.2a1/LICENSE` & `neon-skill-wikipedia-0.4.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/LICENSE.md` & `neon-skill-wikipedia-0.4.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/PKG-INFO` & `neon-skill-wikipedia-0.4.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-wikipedia
-Version: 0.4.2a1
+Version: 0.4.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-wikipedia
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-wikipedia-0.4.2a1/README.md` & `neon-skill-wikipedia-0.4.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/__init__.py` & `neon-skill-wikipedia-0.4.2a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/locale/ca-es/wikiroulette.intent` & `neon-skill-wikipedia-0.4.2a2/locale/ca-es/wikiroulette.intent`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/PKG-INFO` & `neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-wikipedia
-Version: 0.4.2a1
+Version: 0.4.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-wikipedia
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-wikipedia-0.4.2a1/neon_skill_wikipedia.egg-info/SOURCES.txt` & `neon-skill-wikipedia-0.4.2a2/neon_skill_wikipedia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/setup.py` & `neon-skill-wikipedia-0.4.2a2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-wikipedia"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:WikipediaSkill'
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

### Comparing `neon-skill-wikipedia-0.4.2a1/skill.json` & `neon-skill-wikipedia-0.4.2a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/ui/jumping.gif` & `neon-skill-wikipedia-0.4.2a2/ui/jumping.gif`

 * *Files identical despite different names*

### Comparing `neon-skill-wikipedia-0.4.2a1/version.py` & `neon-skill-wikipedia-0.4.2a2/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.4.2a1"
+__version__ = "0.4.2a2"
```

