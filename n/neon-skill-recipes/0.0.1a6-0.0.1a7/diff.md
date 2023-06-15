# Comparing `tmp/neon-skill-recipes-0.0.1a6.tar.gz` & `tmp/neon-skill-recipes-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-recipes-0.0.1a6.tar", last modified: Thu Jun 15 22:46:49 2023, max compression
+gzip compressed data, was "neon-skill-recipes-0.0.1a7.tar", last modified: Thu Jun 15 22:59:30 2023, max compression
```

## Comparing `neon-skill-recipes-0.0.1a6.tar` & `neon-skill-recipes-0.0.1a7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:49.545602 neon-skill-recipes-0.0.1a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 22:46:49.545602 neon-skill-recipes-0.0.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:49.541602 neon-skill-recipes-0.0.1a6/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:49.541602 neon-skill-recipes-0.0.1a6/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/CurrentRecipe.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/CurrentStep.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/IngredientQuantity.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/NextStep.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/NoIngredients.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/NoInstructions.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/NoNextSteps.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/NoPreviousStep.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/NoRecipe.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/PreviousStep.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/ReciteStep.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/SearchFailed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/dialog/en-us/YouWillNeed.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:49.541602 neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 22:46:49.000000 neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 22:46:49.000000 neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:46:49.000000 neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:46:49.000000 neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:46:49.000000 neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:46:49.000000 neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/recipe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:46:49.545602 neon-skill-recipes-0.0.1a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/skill.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:49.541602 neon-skill-recipes-0.0.1a6/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:46:49.545602 neon-skill-recipes-0.0.1a6/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.random.recipe.intent
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.recipe.by.ingredient.intent
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.recipe.by.name.intent
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.the.current.step.intent
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.the.ingredients.intent
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.the.next.step.intent
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.the.previous.step.intent
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/get.the.recipe.name.intent
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 22:46:44.000000 neon-skill-recipes-0.0.1a6/vocab/en-us/recite.the.instructions.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:30.240312 neon-skill-recipes-0.0.1a7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 22:59:30.240312 neon-skill-recipes-0.0.1a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:30.236312 neon-skill-recipes-0.0.1a7/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:30.240312 neon-skill-recipes-0.0.1a7/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/CurrentRecipe.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/CurrentStep.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/IngredientQuantity.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/NextStep.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/NoIngredients.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/NoInstructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/NoNextSteps.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/NoPreviousStep.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/NoRecipe.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/PreviousStep.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/ReciteStep.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/SearchFailed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/dialog/en-us/YouWillNeed.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:30.240312 neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 22:59:30.000000 neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 22:59:30.000000 neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:59:30.000000 neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:59:30.000000 neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:59:30.000000 neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:59:30.000000 neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/recipe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:59:30.240312 neon-skill-recipes-0.0.1a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/skill.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:30.236312 neon-skill-recipes-0.0.1a7/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:59:30.240312 neon-skill-recipes-0.0.1a7/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.random.recipe.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.recipe.by.ingredient.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.recipe.by.name.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.the.current.step.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.the.ingredients.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.the.next.step.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.the.previous.step.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/get.the.recipe.name.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 22:59:25.000000 neon-skill-recipes-0.0.1a7/vocab/en-us/recite.the.instructions.intent
```

### Comparing `neon-skill-recipes-0.0.1a6/LICENSE.md` & `neon-skill-recipes-0.0.1a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-recipes-0.0.1a6/PKG-INFO` & `neon-skill-recipes-0.0.1a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-recipes
-Version: 0.0.1a6
+Version: 0.0.1a7
 Home-page: https://github.com/NeonGeckoCom/skill-recipes
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-recipes-0.0.1a6/README.md` & `neon-skill-recipes-0.0.1a7/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-recipes-0.0.1a6/__init__.py` & `neon-skill-recipes-0.0.1a7/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/PKG-INFO` & `neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-recipes
-Version: 0.0.1a6
+Version: 0.0.1a7
 Home-page: https://github.com/NeonGeckoCom/skill-recipes
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-recipes-0.0.1a6/neon_skill_recipes.egg-info/SOURCES.txt` & `neon-skill-recipes-0.0.1a7/neon_skill_recipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-recipes-0.0.1a6/recipe_utils.py` & `neon-skill-recipes-0.0.1a7/recipe_utils.py`

 * *Files identical despite different names*

### Comparing `neon-skill-recipes-0.0.1a6/setup.py` & `neon-skill-recipes-0.0.1a7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-recipes"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:RecipeSkill'
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

### Comparing `neon-skill-recipes-0.0.1a6/skill.json` & `neon-skill-recipes-0.0.1a7/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-recipes-0.0.1a6/version.py` & `neon-skill-recipes-0.0.1a7/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.1a6"
+__version__ = "0.0.1a7"
```

