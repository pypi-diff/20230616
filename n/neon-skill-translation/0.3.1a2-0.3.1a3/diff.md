# Comparing `tmp/neon-skill-translation-0.3.1a2.tar.gz` & `tmp/neon-skill-translation-0.3.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-translation-0.3.1a2.tar", last modified: Thu Jun 15 22:59:10 2023, max compression
+gzip compressed data, was "neon-skill-translation-0.3.1a3.tar", last modified: Fri Jun 16 01:01:08 2023, max compression
```

## Comparing `neon-skill-translation-0.3.1a2.tar` & `neon-skill-translation-0.3.1a3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/locale/en-us/dialog/language_not_supported.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/locale/en-us/dialog/phrase_in_language.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/locale/en-us/languages.value
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/locale/en-us/vocab/female.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/locale/en-us/vocab/male.voc
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/locale/en-us/vocab/translate_phrase.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-15 22:59:10.000000 neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-15 22:59:10.000000 neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:59:10.000000 neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 22:59:10.000000 neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 22:59:10.000000 neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 22:59:10.000000 neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:10.435848 neon-skill-translation-0.3.1a2/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/ui/Translation.qml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:59:06.000000 neon-skill-translation-0.3.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/dialog/language_not_supported.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/dialog/phrase_in_language.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/languages.value
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.843175 neon-skill-translation-0.3.1a3/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/vocab/female.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/vocab/male.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/locale/en-us/vocab/translate_phrase.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 01:01:08.000000 neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:01:08.847175 neon-skill-translation-0.3.1a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/ui/Translation.qml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-16 01:01:00.000000 neon-skill-translation-0.3.1a3/version.py
```

### Comparing `neon-skill-translation-0.3.1a2/LICENSE.md` & `neon-skill-translation-0.3.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a2/PKG-INFO` & `neon-skill-translation-0.3.1a3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-translation
-Version: 0.3.1a2
+Version: 0.3.1a3
 Home-page: https://github.com/NeonGeckoCom/skill-translation
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-translation-0.3.1a2/README.md` & `neon-skill-translation-0.3.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a2/__init__.py` & `neon-skill-translation-0.3.1a3/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/PKG-INFO` & `neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-translation
-Version: 0.3.1a2
+Version: 0.3.1a3
 Home-page: https://github.com/NeonGeckoCom/skill-translation
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-translation-0.3.1a2/neon_skill_translation.egg-info/SOURCES.txt` & `neon-skill-translation-0.3.1a3/neon_skill_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a2/setup.py` & `neon-skill-translation-0.3.1a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-translation"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
-PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:Translation'
+PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:TranslationSkill'
 BASE_PATH = path.abspath(path.dirname(__file__))
 
 
 def get_requirements(requirements_filename: str):
     requirements_file = path.join(BASE_PATH, requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
         requirements = r.readlines()
```

### Comparing `neon-skill-translation-0.3.1a2/skill.json` & `neon-skill-translation-0.3.1a3/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a2/test/test_skill.py` & `neon-skill-translation-0.3.1a3/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a2/ui/Translation.qml` & `neon-skill-translation-0.3.1a3/ui/Translation.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-translation-0.3.1a2/version.py` & `neon-skill-translation-0.3.1a3/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.1a2"
+__version__ = "0.3.1a3"
```

