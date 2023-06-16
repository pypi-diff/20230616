# Comparing `tmp/pythorhead-0.0.4.tar.gz` & `tmp/pythorhead-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.0.4.tar", last modified: Wed Jun 14 21:43:22 2023, max compression
+gzip compressed data, was "pythorhead-0.1.0.tar", last modified: Fri Jun 16 13:14:09 2023, max compression
```

## Comparing `pythorhead-0.0.4.tar` & `pythorhead-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.384036 pythorhead-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-14 21:42:58.000000 pythorhead-0.0.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-14 21:42:58.000000 pythorhead-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-14 21:43:04.000000 pythorhead-0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-14 21:42:58.000000 pythorhead-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40742 2023-06-14 21:43:22.388036 pythorhead-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-14 21:42:58.000000 pythorhead-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-14 21:42:58.000000 pythorhead-0.0.4/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-14 21:43:04.000000 pythorhead-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 21:42:58.000000 pythorhead-0.0.4/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-14 21:42:58.000000 pythorhead-0.0.4/pythorhead/lemmy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:43:22.388036 pythorhead-0.0.4/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40742 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 21:43:22.000000 pythorhead-0.0.4/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:43:22.388036 pythorhead-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-16 13:13:50.000000 pythorhead-0.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-16 13:13:50.000000 pythorhead-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-16 13:13:56.000000 pythorhead-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 13:13:50.000000 pythorhead-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-16 13:14:09.796255 pythorhead-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 13:13:50.000000 pythorhead-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-16 13:13:50.000000 pythorhead-0.1.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-16 13:13:56.000000 pythorhead-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 13:13:50.000000 pythorhead-0.1.0/pythorhead/types/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:14:09.796255 pythorhead-0.1.0/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40749 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 13:14:09.000000 pythorhead-0.1.0/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 13:13:50.000000 pythorhead-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:14:09.796255 pythorhead-0.1.0/setup.cfg
```

### Comparing `pythorhead-0.0.4/.github/workflows/pypi.yml` & `pythorhead-0.1.0/.github/workflows/pypi.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         fetch-depth: 0
     - name: "📣 Release on push"
       id: release
       uses: rymndhng/release-on-push-action@v0.28.0
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
-        bump_version_scheme: patch
+        bump_version_scheme: norelease
         use_github_release_notes: true
     - name: "✏️ Generate release changelog"
       if: ${{ steps.release.outputs.version != '' }}
       uses: heinrichreimer/github-changelog-generator-action@v2.3
       with:
         token: ${{ secrets.GITHUB_TOKEN }}
     - name: "💾 Commit new version"
```

### Comparing `pythorhead-0.0.4/.gitignore` & `pythorhead-0.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# vscode
+.vscode
```

### Comparing `pythorhead-0.0.4/CHANGELOG.md` & `pythorhead-0.1.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Changelog
 
+## [v0.1.0](https://github.com/db0/pythorhead/tree/v0.1.0) (2023-06-16)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.0.5...v0.1.0)
+
+**Merged pull requests:**
+
+- Refactoring [\#3](https://github.com/db0/pythorhead/pull/3) ([NicKoehler](https://github.com/NicKoehler))
+
+## [v0.0.5](https://github.com/db0/pythorhead/tree/v0.0.5) (2023-06-15)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.0.4...v0.0.5)
+
+**Merged pull requests:**
+
+- Fix typo in log\_in function [\#2](https://github.com/db0/pythorhead/pull/2) ([AshtonTX](https://github.com/AshtonTX))
+
 ## [v0.0.4](https://github.com/db0/pythorhead/tree/v0.0.4) (2023-06-14)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.0.3...v0.0.4)
 
 ## [v0.0.3](https://github.com/db0/pythorhead/tree/v0.0.3) (2023-06-14)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.0.2...v0.0.3)
```

### Comparing `pythorhead-0.0.4/LICENSE` & `pythorhead-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.0.4/PKG-INFO` & `pythorhead-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.0.4
+Version: 0.1.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,9 +685,9 @@
 
 ```python
 from pythorhead import Lemmy
 
 lemmy = Lemmy("https://lemmy.dbzer0.com")
 lemmy.log_in("username", "password")
 community_id = lemmy.discover_community("botart")
-lemmy.post(community_id, "Hello Lemmy World")
+lemmy.post.create(community_id, "Hello Lemmy World")
 ```
```

### Comparing `pythorhead-0.0.4/logo.png` & `pythorhead-0.1.0/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.0.4/pyproject.toml` & `pythorhead-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.0.4"
+version = "v0.1.0"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.0.4/pythorhead/lemmy.py` & `pythorhead-0.1.0/pythorhead/lemmy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,31 @@
 import requests
 from loguru import logger
 
-class Lemmy:
+from pythorhead.auth import Authentication
+from pythorhead.post import Post
+
 
-    _auth_token = None
-    _api_base_url = None
+class Lemmy:
+    post: Post
+    _auth: Authentication
     _known_communities = {}
 
-    def __init__(self, api_base_url):
-        self._api_base_url = api_base_url
+    def __init__(self, api_base_url: str) -> None:
+        self._auth = Authentication()
+        self._auth.api_base_url = f"{api_base_url}/api/v3"
+        self.post = Post()
 
+    def log_in(self, username_or_email: str, password: str) -> bool:
+        return Authentication().log_in(username_or_email, password)
 
-    def log_in(self, username_or_email, password):
-        payload = {
-            "username_or_email": username_or_email,
-            "password": password
-        }
-        try:
-            re = requests.post(f"{self._api_base_url}/api/v3/user/login", json=payload)
-            self._auth_token = re.json()["jwt"]
-        except Exception as err:
-            logger.error(f"Something went wrong while logginf in as {username_or_email}: {err}")
-            return False
-        return True
-
-    def discover_community(self, community_name):
+    def discover_community(self, community_name: str) -> int | None:
         if community_name in self._known_communities:
             return self._known_communities[community_name]
         try:
-            req = requests.get(f"{self._api_base_url}/api/v3/community?name={community_name}")
+            req = requests.get(f"{self._auth.api_base_url}/community?name={community_name}")
             community_id = req.json()["community_view"]["community"]["id"]
             self._known_communities[community_name] = community_id
         except Exception as err:
             logger.error(f"Error when looking up community '{community_name}': {err}")
-            return None
+            return
         return community_id
-
-    def post(self, community_id, post_name, post_url = None, post_body = None):
-        new_post = {
-            "auth": self._auth_token,
-            "community_id": community_id,
-            "name": post_name,
-        }
-        if post_url:
-             new_post["url"] = post_url
-        if post_body:
-             new_post["body"] = post_body
-        re = requests.post(f"{self._api_base_url}/api/v3/post", json=new_post)
-        if not re.ok:
-            logger.error(f"Error encountered while posting: {re.text}")
-        return re.ok
```

### Comparing `pythorhead-0.0.4/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.1.0/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.0.4
+Version: 0.1.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,9 +685,9 @@
 
 ```python
 from pythorhead import Lemmy
 
 lemmy = Lemmy("https://lemmy.dbzer0.com")
 lemmy.log_in("username", "password")
 community_id = lemmy.discover_community("botart")
-lemmy.post(community_id, "Hello Lemmy World")
+lemmy.post.create(community_id, "Hello Lemmy World")
 ```
```

