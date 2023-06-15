# Comparing `tmp/vernum-2.2.2.tar.gz` & `tmp/vernum-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vernum-2.2.2.tar", last modified: Sun Feb 10 00:25:28 2019, max compression
+gzip compressed data, was "vernum-3.0.0.tar", last modified: Thu Jun 15 22:27:17 2023, max compression
```

## Comparing `vernum-2.2.2.tar` & `vernum-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-10 00:25:28.000000 vernum-2.2.2/
--rw-r--r--   0 root         (0) root         (0)     1696 2019-02-10 00:25:28.000000 vernum-2.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1111 2019-02-10 00:25:23.000000 vernum-2.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2019-02-10 00:25:28.000000 vernum-2.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      754 2019-02-10 00:25:23.000000 vernum-2.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-02-10 00:25:23.000000 vernum-2.2.2/vernum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2019-02-10 00:25:23.000000 vernum-2.2.2/vernum/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1696 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      238 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        7 2019-02-10 00:25:28.000000 vernum-2.2.2/vernum.egg-info/top_level.txt
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 22:27:17.448186 vernum-3.0.0/
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-15 22:24:30.000000 vernum-3.0.0/.version
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-06-15 03:00:08.000000 vernum-3.0.0/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-15 22:27:17.447683 vernum-3.0.0/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1111 2023-06-15 03:00:08.000000 vernum-3.0.0/README.md
+-rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-15 22:26:45.000000 vernum-3.0.0/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-15 22:27:17.448308 vernum-3.0.0/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 22:27:17.436440 vernum-3.0.0/vernum/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 03:00:08.000000 vernum-3.0.0/vernum/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-06-15 21:44:28.000000 vernum-3.0.0/vernum/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2203 2023-06-15 22:16:32.000000 vernum-3.0.0/vernum/handler.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 22:27:17.447025 vernum-3.0.0/vernum.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1373 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      250 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       47 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        7 2023-06-15 22:27:17.000000 vernum-3.0.0/vernum.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vernum-2.2.2/PKG-INFO` & `vernum-3.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: vernum
-Version: 2.2.2
-Summary: Version numbering and git tagging for project releases
-Home-page: http://gitlab.com/fpotter/tools/vernum
-Author: Francis Potter
-Author-email: vernum@fpotter.com
+Version: 3.0.0
+Summary: Easy semantic versioning for projects in Git
+Author-email: Steampunk Wizard <vernum@steampunkwizard.ca>
 License: MIT
-Description: # VERNUM
-        
-        Version numbering and git tagging for project releases
-        
-        ## Installation
-        
-        Requires Python 3 to run the command; your project can be anything.
-        
-        ```
-        sudo pip3 install vernum
-        ```
-        
-        ## What it does
-        
-        - Maintain a file at the root of a project called simply "version" with the version number, e.g. "5.6.2"
-        - Update the release file for major, minor, or patch releases - patch is the default
-        - Always create and push a git tag with the version number in it
-        
-        ## Usage
-        
-        Requirements:
-        
-        - CD to the root of the project before running it
-        - Be on the branch that you use for releases (i.e. `master`)
-        - Be fully up-to-date in git (i.e. merged, committed, and pushed)
-        
-        Then run the command:
-        
-        - `vernum major` to update the major version level, i.e. 5.6.2 -> 6.0.0
-        - `vernum minor` to update the minor version level, i.e. 5.6.2 -> 5.7.0
-        - `vernum patch` to update the patch version level, i.e. 5.6.2 -> 5.6.3
-        
-        Note that `patch` is the default so you can just say `vernum` for a patch release
-        
-        Reference the `version` file within your code when it needs to know the version. For example, see `setup.py` in this project.
-        
-Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# VERNUM
+
+Version numbering and git tagging for project releases
+
+## Installation
+
+Requires Python 3 to run the command; your project can be anything.
+
+```
+sudo pip3 install vernum
+```
+
+## What it does
+
+- Maintain a file at the root of a project called simply "version" with the version number, e.g. "5.6.2"
+- Update the release file for major, minor, or patch releases - patch is the default
+- Always create and push a git tag with the version number in it
+
+## Usage
+
+Requirements:
+
+- CD to the root of the project before running it
+- Be on the branch that you use for releases (i.e. `master`)
+- Be fully up-to-date in git (i.e. merged, committed, and pushed)
+
+Then run the command:
+
+- `vernum major` to update the major version level, i.e. 5.6.2 -> 6.0.0
+- `vernum minor` to update the minor version level, i.e. 5.6.2 -> 5.7.0
+- `vernum patch` to update the patch version level, i.e. 5.6.2 -> 5.6.3
+
+Note that `patch` is the default so you can just say `vernum` for a patch release
+
+Reference the `version` file within your code when it needs to know the version. For example, see `setup.py` in this project.
```

### Comparing `vernum-2.2.2/README.md` & `vernum-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vernum-2.2.2/vernum/__main__.py` & `vernum-3.0.0/vernum/handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 
 import os
-import subprocess
+from subprocess import run
 from argparse import ArgumentParser
+import re
+from dataclasses import dataclass
+
+FORMAT = re.compile(r"^v?(\d+)\.(\d+)\.(\d+)$")
 
 LEVELS = ['major','minor','patch']
 
-def update_version(level):
-    if os.path.isfile('version'):
-        with open('version') as versionfile:
-            oldversion = versionfile.read().strip()
-    elif os.path.exists('version'):
-        raise(RuntimeError("Can't create file 'version'"))
-    else:
-        oldversion="0.0.0"
-    major, minor, patch = [int(x) for x in oldversion.split('.')]
-    if level == 'major':
-        major += 1
-        minor = 0
-        patch = 0
-    elif level == 'minor':
-        minor += 1
-        patch = 0
-    else: patch += 1
-    newversion = '%i.%i.%i' % (major, minor, patch)
-    with open('version', 'w') as versionfile:
-        versionfile.write(newversion)
-    return newversion
-
-def git(command):
-    process = subprocess.run(['git'] + command.split(), stdout=subprocess.PIPE)
-    if process.returncode != 0:
-        raise(RuntimeError('Failure of git command: ' + command))
-    return process.stdout.decode()
-
-def do(level=None):
-    status = git('status -s')
-    if status:
-        raise RuntimeError('Git working tree must be clean to release')
-    version = update_version(level)
-    print('Version updated to ' + version)
-    print(git('add version'))
-    print(git('commit -m v' + version))
-    print(git('tag -a v%s -m v%s' % (version, version)))
-    print(git('push --follow-tags'))
-    print('Release complete')
+@dataclass
+class Handler:
+
+    dry_run:bool = False
+
+    def git(self, command, dry_ok=False):
+        print('git ' + command)
+        if dry_ok or not self.dry_run:
+            result = run(['git'] + command.split(),
+                                    capture_output=True, text=True)
+            if result.returncode != 0:
+                raise SystemExit(result.stderr)
+            return result.stdout.strip()
+
+    def get_previous_version(self):
+        branch = self.git("branch --show-current", dry_ok=True)
+        tags = self.git(f"tag --sort=-creatordate --merged {branch}", dry_ok=True)
+        for tag in tags.split('\n'):
+            if match:=FORMAT.match(tag):
+                return (int(x) for x in match.groups())
+
+    def update_version(self, level):
+        major, minor, patch = self.get_previous_version() or (0,0,0)
+        if level == 'major':
+            major += 1
+            minor = 0
+            patch = 0
+        elif level == 'minor':
+            minor += 1
+            patch = 0
+        else: patch += 1
+        newversion = '%i.%i.%i' % (major, minor, patch)
+        if self.dry_run:
+            print(f"Write {newversion} to .version")
+        else:
+            with open('.version', 'w') as versionfile:
+                versionfile.write(newversion)
+        return newversion
+
+    def do(self, level=None):
+        status = self.git('status -s')
+        if status:
+            raise SystemExit('Git working tree must be clean to update version')
+        version = self.update_version(level)
+        print('Version updated to ' + version)
+        print(self.git(f"tag -a v{version} -m v{version}"))
+        print(self.git('push --tags'))
+        print('Release complete')
 
-def run():
+def main():
     parser = ArgumentParser()
     parser.add_argument('level', choices=LEVELS, default='patch', nargs='?')
-    level = parser.parse_args().level
-    do(level)
+    parser.add_argument('--dry-run','-n', action='store_true')
+    namespace = parser.parse_args()
+    handler = Handler(namespace.dry_run)
+    handler.do(namespace.level)
 
-if __name__=='__main__':
-    run()
```

### Comparing `vernum-2.2.2/vernum.egg-info/PKG-INFO` & `vernum-3.0.0/vernum.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: vernum
-Version: 2.2.2
-Summary: Version numbering and git tagging for project releases
-Home-page: http://gitlab.com/fpotter/tools/vernum
-Author: Francis Potter
-Author-email: vernum@fpotter.com
+Version: 3.0.0
+Summary: Easy semantic versioning for projects in Git
+Author-email: Steampunk Wizard <vernum@steampunkwizard.ca>
 License: MIT
-Description: # VERNUM
-        
-        Version numbering and git tagging for project releases
-        
-        ## Installation
-        
-        Requires Python 3 to run the command; your project can be anything.
-        
-        ```
-        sudo pip3 install vernum
-        ```
-        
-        ## What it does
-        
-        - Maintain a file at the root of a project called simply "version" with the version number, e.g. "5.6.2"
-        - Update the release file for major, minor, or patch releases - patch is the default
-        - Always create and push a git tag with the version number in it
-        
-        ## Usage
-        
-        Requirements:
-        
-        - CD to the root of the project before running it
-        - Be on the branch that you use for releases (i.e. `master`)
-        - Be fully up-to-date in git (i.e. merged, committed, and pushed)
-        
-        Then run the command:
-        
-        - `vernum major` to update the major version level, i.e. 5.6.2 -> 6.0.0
-        - `vernum minor` to update the minor version level, i.e. 5.6.2 -> 5.7.0
-        - `vernum patch` to update the patch version level, i.e. 5.6.2 -> 5.6.3
-        
-        Note that `patch` is the default so you can just say `vernum` for a patch release
-        
-        Reference the `version` file within your code when it needs to know the version. For example, see `setup.py` in this project.
-        
-Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# VERNUM
+
+Version numbering and git tagging for project releases
+
+## Installation
+
+Requires Python 3 to run the command; your project can be anything.
+
+```
+sudo pip3 install vernum
+```
+
+## What it does
+
+- Maintain a file at the root of a project called simply "version" with the version number, e.g. "5.6.2"
+- Update the release file for major, minor, or patch releases - patch is the default
+- Always create and push a git tag with the version number in it
+
+## Usage
+
+Requirements:
+
+- CD to the root of the project before running it
+- Be on the branch that you use for releases (i.e. `master`)
+- Be fully up-to-date in git (i.e. merged, committed, and pushed)
+
+Then run the command:
+
+- `vernum major` to update the major version level, i.e. 5.6.2 -> 6.0.0
+- `vernum minor` to update the minor version level, i.e. 5.6.2 -> 5.7.0
+- `vernum patch` to update the patch version level, i.e. 5.6.2 -> 5.6.3
+
+Note that `patch` is the default so you can just say `vernum` for a patch release
+
+Reference the `version` file within your code when it needs to know the version. For example, see `setup.py` in this project.
```

