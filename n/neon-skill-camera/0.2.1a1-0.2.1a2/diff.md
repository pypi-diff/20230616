# Comparing `tmp/neon-skill-camera-0.2.1a1.tar.gz` & `tmp/neon-skill-camera-0.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-camera-0.2.1a1.tar", last modified: Thu Jun 15 22:52:18 2023, max compression
+gzip compressed data, was "neon-skill-camera-0.2.1a2.tar", last modified: Thu Jun 15 23:00:20 2023, max compression
```

## Comparing `neon-skill-camera-0.2.1a1.tar` & `neon-skill-camera-0.2.1a2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.823773 neon-skill-camera-0.2.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 22:52:18.823773 neon-skill-camera-0.2.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16984 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.815774 neon-skill-camera-0.2.1a1/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.819774 neon-skill-camera-0.2.1a1/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/DefaultDuration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/LaunchCamera.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/NoCamera.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/NothingToShow.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/PictureInsteadOfVideo.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/ServerNotSupported.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/ShowLatest.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/StartRecording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/hour.list
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/minute.list
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/dialog/en-us/second.list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.819774 neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 22:52:18.000000 neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-15 22:52:18.000000 neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:52:18.000000 neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 22:52:18.000000 neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:52:18.000000 neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 22:52:18.000000 neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:52:18.823773 neon-skill-camera-0.2.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.823773 neon-skill-camera-0.2.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/ui/Camera.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/ui/ControlBar.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.823773 neon-skill-camera-0.2.1a1/ui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/ui/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/ui/images/capture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/ui/images/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.823773 neon-skill-camera-0.2.1a1/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (123)   341166 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/ui/sounds/clicking.wav
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.815774 neon-skill-camera-0.2.1a1/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:52:18.823773 neon-skill-camera-0.2.1a1/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/vocab/en-us/ShowLastIntent.intent
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/vocab/en-us/TakePicIntent.intent
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/vocab/en-us/TakeVidIntent.intent
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:52:13.000000 neon-skill-camera-0.2.1a1/vocab/en-us/duration.entity
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.373039 neon-skill-camera-0.2.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 23:00:20.373039 neon-skill-camera-0.2.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16984 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.369039 neon-skill-camera-0.2.1a2/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.369039 neon-skill-camera-0.2.1a2/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/DefaultDuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/LaunchCamera.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/NoCamera.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/NothingToShow.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/PictureInsteadOfVideo.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/ServerNotSupported.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/ShowLatest.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/StartRecording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/hour.list
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/minute.list
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/dialog/en-us/second.list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.369039 neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 23:00:20.000000 neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-15 23:00:20.000000 neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:00:20.000000 neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 23:00:20.000000 neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 23:00:20.000000 neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 23:00:20.000000 neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 23:00:20.373039 neon-skill-camera-0.2.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.369039 neon-skill-camera-0.2.1a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/ui/Camera.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/ui/ControlBar.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.369039 neon-skill-camera-0.2.1a2/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/ui/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/ui/images/capture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/ui/images/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.369039 neon-skill-camera-0.2.1a2/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)   341166 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/ui/sounds/clicking.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.369039 neon-skill-camera-0.2.1a2/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:00:20.373039 neon-skill-camera-0.2.1a2/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/vocab/en-us/ShowLastIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/vocab/en-us/TakePicIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/vocab/en-us/TakeVidIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 23:00:16.000000 neon-skill-camera-0.2.1a2/vocab/en-us/duration.entity
```

### Comparing `neon-skill-camera-0.2.1a1/LICENSE.md` & `neon-skill-camera-0.2.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/PKG-INFO` & `neon-skill-camera-0.2.1a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-camera
-Version: 0.2.1a1
+Version: 0.2.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-camera
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-camera-0.2.1a1/README.md` & `neon-skill-camera-0.2.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/__init__.py` & `neon-skill-camera-0.2.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/PKG-INFO` & `neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-camera
-Version: 0.2.1a1
+Version: 0.2.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-camera
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-camera-0.2.1a1/neon_skill_camera.egg-info/SOURCES.txt` & `neon-skill-camera-0.2.1a2/neon_skill_camera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/setup.py` & `neon-skill-camera-0.2.1a2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-camera"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:UsbCamSkill'
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

### Comparing `neon-skill-camera-0.2.1a1/skill.json` & `neon-skill-camera-0.2.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/ui/Camera.qml` & `neon-skill-camera-0.2.1a2/ui/Camera.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/ui/ControlBar.qml` & `neon-skill-camera-0.2.1a2/ui/ControlBar.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/ui/images/back.svg` & `neon-skill-camera-0.2.1a2/ui/images/back.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/ui/images/capture.svg` & `neon-skill-camera-0.2.1a2/ui/images/capture.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/ui/images/close.svg` & `neon-skill-camera-0.2.1a2/ui/images/close.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/ui/sounds/clicking.wav` & `neon-skill-camera-0.2.1a2/ui/sounds/clicking.wav`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-0.2.1a1/version.py` & `neon-skill-camera-0.2.1a2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.2.1a1"
+__version__ = "0.2.1a2"
```

### Comparing `neon-skill-camera-0.2.1a1/vocab/en-us/ShowLastIntent.intent` & `neon-skill-camera-0.2.1a2/vocab/en-us/ShowLastIntent.intent`

 * *Files identical despite different names*

