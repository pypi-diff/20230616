# Comparing `tmp/git2vec-0.1.4.tar.gz` & `tmp/git2vec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2vec-0.1.4.tar", last modified: Fri Jun 16 17:59:31 2023, max compression
+gzip compressed data, was "git2vec-0.1.5.tar", last modified: Fri Jun 16 19:06:43 2023, max compression
```

## Comparing `git2vec-0.1.4.tar` & `git2vec-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:59:31.218937 git2vec-0.1.4/
--rw-rw-rw-   0        0        0     2805 2023-06-16 17:59:31.216941 git2vec-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2151 2023-06-09 14:25:12.000000 git2vec-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 17:59:31.191349 git2vec-0.1.4/git2vec/
--rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2vec-0.1.4/git2vec/__init__.py
--rw-rw-rw-   0        0        0     7697 2023-06-16 17:49:11.000000 git2vec-0.1.4/git2vec/loader.py
--rw-rw-rw-   0        0        0     3996 2023-06-09 14:25:12.000000 git2vec-0.1.4/git2vec/vectordb.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:59:31.214921 git2vec-0.1.4/git2vec.egg-info/
--rw-rw-rw-   0        0        0     2805 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 17:59:31.000000 git2vec-0.1.4/git2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 17:59:31.218937 git2vec-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-06-16 17:59:23.000000 git2vec-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:06:43.354836 git2vec-0.1.5/
+-rw-rw-rw-   0        0        0     2701 2023-06-16 19:06:43.354836 git2vec-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-06-16 18:53:23.000000 git2vec-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 19:06:43.332263 git2vec-0.1.5/git2vec/
+-rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2vec-0.1.5/git2vec/__init__.py
+-rw-rw-rw-   0        0        0     7697 2023-06-16 18:53:23.000000 git2vec-0.1.5/git2vec/loader.py
+-rw-rw-rw-   0        0        0     3996 2023-06-09 14:25:12.000000 git2vec-0.1.5/git2vec/vectordb.py
+drwxrwxrwx   0        0        0        0 2023-06-16 19:06:43.352842 git2vec-0.1.5/git2vec.egg-info/
+-rw-rw-rw-   0        0        0     2701 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 19:06:43.000000 git2vec-0.1.5/git2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 19:06:43.356341 git2vec-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-06-16 19:06:36.000000 git2vec-0.1.5/setup.py
```

### Comparing `git2vec-0.1.4/PKG-INFO` & `git2vec-0.1.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,83 @@
-Metadata-Version: 2.1
-Name: git2vec
-Version: 0.1.4
-Summary: A useful module for handling Git data.
-Home-page: https://github.com/voynow/git2vec
-Author: Jamie Voynow
-Author-email: voynow99@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+# Git2Vec
 
-# Git2Vec Repo
-
-Git2Vec is a Python module that allows you to load text files from a Git repository and create a searchable vector database using Langchain, Pinecone, and OpenAI.
+Git2Vec is a Python package for handling Git data. It provides functionality to load and process Git repositories, and supports concurrent file loading for improved performance. The package can be found on [PyPI](https://pypi.org/project/git2vec/).
 
 ## Installation
 
-Install from https://pypi.org/project/git2vec/ using pip
+To install Git2Vec, run the following command:
 
 ```bash
 pip install git2vec
 ```
 
-If cloned, you will need to install the following packages:
+## Setup
 
-```bash
-pip install -r requirements.txt
-```
+Before using Git2Vec, make sure to have the following dependencies installed:
+
+- langchain
+- pinecone-client
+- tiktoken
+- gitpython
+- python-dotenv
+- pandas
 
-If you are a developer, you will need to install the development requirements:
+You can install them using the following command:
 
 ```bash
-pip install -r requirements.dev.txt
+pip install -r requirements.txt
 ```
 
 ## Usage
 
-### Loading a Git repository
+### Loading Git Repositories
 
-To load a Git repository, use the `git2vec.loader.load()` function:
+The main functionality of Git2Vec is provided by the `loader.py` module. Here's an example of how to use the `pull_code_from_repo` function to load a Git repository:
 
 ```python
-from git2vec import loader
-
-repo_name = "https://github.com/voynow/turbo-docs"
+from git2vec.loader import pull_code_from_repo
 
-# Returns a list of Document objects
-repo_data = loader.load(repo_name)
+repo_url = "https://github.com/username/repo.git"
+branch = "main"
 
-# Or return a string of all the raw text
-raw_repo = loader.load(repo_name, return_str=True)
+repo_data = pull_code_from_repo(repo_url, branch)
 ```
 
-### Creating and managing a vector database
+### Getting Top Repositories
 
-To create a vector database from the loaded Git repository, use the following functions:
+You can use the `get_top_repos` function to fetch the top repositories based on certain criteria:
 
 ```python
-from git2vec import vectordb
+from git2vec.loader import get_top_repos
 
-# Create a vector store from the Git repo
-vectorstore = vectordb.create_vectorstore(repo_name)
+n_repos = 10
+last_n_days = 30
+language = "Python"
+sort = "stars"
+order = "desc"
 
-# Retrieve the vector store from Pinecone index
-vectorstore = vectordb.get_vectorstore()
+top_repos = get_top_repos(n_repos, last_n_days, language, sort, order)
 ```
 
-## Modules
+### Pipeline Fetch and Load
 
-### loader.py
+The `pipeline_fetch_and_load` function can be used to fetch and load repositories in a single step:
 
-The `loader.py` module contains the `TurboGitLoader` class which can be used to load text files from a Git repository. The `load()` function takes a repository URL and returns a list of `Document` objects or a string containing all the raw text.
+```python
+from git2vec.loader import pipeline_fetch_and_load
 
-### vectordb.py
+n_repos = 10
+last_n_days = 30
+language = "Python"
+sort = "stars"
+order = "desc"
 
-The `vectordb.py` module provides functions to create and manage a vector database using Langchain, Pinecone, and OpenAI. It contains functions for initializing Pinecone, upserting data, processing data, embedding and upserting, creating a vectorstore, and retrieving a vectorstore.
+github_data = pipeline_fetch_and_load(n_repos, last_n_days, language, sort, order)
+```
 
 ## Contributing
 
-If you find any issues or have any suggestions, feel free to open an issue or submit a pull request. We welcome any contributions!
+If you'd like to contribute to Git2Vec, feel free to fork the repository and submit a pull request. If you have any questions or issues, please open an issue on the GitHub repository.
 
 ## License
 
-This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
+Git2Vec is released under the MIT License.
```

### Comparing `git2vec-0.1.4/git2vec/loader.py` & `git2vec-0.1.5/git2vec/loader.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.4/git2vec/vectordb.py` & `git2vec-0.1.5/git2vec/vectordb.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.4/setup.py` & `git2vec-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2vec',
-    version='0.1.4',
+    version='0.1.5',
     description='A useful module for handling Git data.',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2vec',
     packages=find_packages(),
     install_requires=[
         'langchain',
         'pinecone-client',
         'tiktoken',
-        'gitpython'
+        'gitpython',
         "python-dotenv",
         "pandas",
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  
         'Intended Audience :: Developers',  
         'Topic :: Software Development :: Build Tools',
```

