# Comparing `tmp/git2vec-0.1.5.tar.gz` & `tmp/git2vec-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2vec-0.1.5.tar", last modified: Fri Jun 16 19:06:43 2023, max compression
+gzip compressed data, was "git2vec-0.1.6.tar", last modified: Fri Jun 16 19:25:16 2023, max compression
```

## Comparing `git2vec-0.1.5.tar` & `git2vec-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 19:06:43.354836 git2vec-0.1.5/
--rw-rw-rw-   0        0        0     2701 2023-06-16 19:06:43.354836 git2vec-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2047 2023-06-16 18:53:23.000000 git2vec-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 19:06:43.332263 git2vec-0.1.5/git2vec/
--rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2vec-0.1.5/git2vec/__init__.py
--rw-rw-rw-   0        0        0     7697 2023-06-16 18:53:23.000000 git2vec-0.1.5/git2vec/loader.py
--rw-rw-rw-   0        0        0     3996 2023-06-09 14:25:12.000000 git2vec-0.1.5/git2vec/vectordb.py
-drwxrwxrwx   0        0        0        0 2023-06-16 19:06:43.352842 git2vec-0.1.5/git2vec.egg-info/
--rw-rw-rw-   0        0        0     2701 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 19:06:43.356341 git2vec-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-06-16 19:06:36.000000 git2vec-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:25:16.429123 git2vec-0.1.6/
+-rw-rw-rw-   0        0        0     2701 2023-06-16 19:25:16.428113 git2vec-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-06-16 18:53:23.000000 git2vec-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 19:25:16.405499 git2vec-0.1.6/git2vec/
+-rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2vec-0.1.6/git2vec/__init__.py
+-rw-rw-rw-   0        0        0     7575 2023-06-16 19:15:37.000000 git2vec-0.1.6/git2vec/loader.py
+-rw-rw-rw-   0        0        0     3996 2023-06-09 14:25:12.000000 git2vec-0.1.6/git2vec/vectordb.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:25:16.426114 git2vec-0.1.6/git2vec.egg-info/
+-rw-rw-rw-   0        0        0     2701 2023-06-16 19:25:16.000000 git2vec-0.1.6/git2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-16 19:25:16.000000 git2vec-0.1.6/git2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:25:16.000000 git2vec-0.1.6/git2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-16 19:25:16.000000 git2vec-0.1.6/git2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 19:25:16.000000 git2vec-0.1.6/git2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 19:25:16.430117 git2vec-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-06-16 19:25:13.000000 git2vec-0.1.6/setup.py
```

### Comparing `git2vec-0.1.5/PKG-INFO` & `git2vec-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.5
+Version: 0.1.6
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.5/README.md` & `git2vec-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.5/git2vec/loader.py` & `git2vec-0.1.6/git2vec/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,14 +128,18 @@
     """
     Load the git repo data using TurboGitLoader
 
     :param repo: URL to the repo
     :param branch: default branch name
     :param return_str: return raw text or not
     """
+    # remove any old repos
+    if os.path.exists(REPODATA_FOLDER):
+        shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
+
     folder_name = "/".join(repo.split("/")[3:5])
     output_path = f"{REPODATA_FOLDER}{folder_name}/"
 
     # git pull, load, and delete repo
     repo = git_pull(repo, branch, output_path)
     repo_docs = load_concurrently(repo, output_path)
     shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
@@ -158,18 +162,14 @@
             for kk, vv in dd.items()
             for k, v in flatten_dict(vv, separator, kk).items()
         }
         if isinstance(dd, dict)
         else {prefix: dd}
     )
 
-def repos_to_df(repos):
-    repos = [flatten_dict(repo) for repo in repos['items']]
-    repos_df = pd.DataFrame(repos)
-
 
 def get_access_token():
     """Can be stored in a .env file or as an environment variable"""
     dotenv.load_dotenv()
     access_token = os.getenv("GITHUB_ACCESS_TOKEN")
     if not access_token:
         raise ValueError(
@@ -228,17 +228,14 @@
 def pipeline_fetch_and_load(
     n_repos: int,
     last_n_days: int,
     language: str = None,
     sort: str = "stars",
     order: str = "desc",
 ) -> Dict[str, Dict]:
-    # remove any old repos
-    if os.path.exists(REPODATA_FOLDER):
-        shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
 
     response = get_top_repos(
         n_repos=n_repos,
         last_n_days=last_n_days,
         language=language,
         sort=sort,
         order=order,
```

### Comparing `git2vec-0.1.5/git2vec/vectordb.py` & `git2vec-0.1.6/git2vec/vectordb.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.5/git2vec.egg-info/PKG-INFO` & `git2vec-0.1.6/git2vec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.5
+Version: 0.1.6
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2vec-0.1.5/setup.py` & `git2vec-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2vec',
-    version='0.1.5',
+    version='0.1.6',
     description='A useful module for handling Git data.',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2vec',
     packages=find_packages(),
     install_requires=[
         'langchain',
```

