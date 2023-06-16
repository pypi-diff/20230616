# Comparing `tmp/emotional-0.3.0.tar.gz` & `tmp/emotional-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotional-0.3.0.tar", last modified: Tue May 30 16:28:29 2023, max compression
+gzip compressed data, was "emotional-0.3.1.tar", last modified: Fri Jun 16 14:24:52 2023, max compression
```

## Comparing `emotional-0.3.0.tar` & `emotional-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1064 2022-09-16 23:07:01.534539 emotional-0.3.0/LICENSE
--rw-r--r--   0        0        0     2981 2023-05-29 23:31:26.683409 emotional-0.3.0/README.md
--rw-r--r--   0        0        0       98 2023-05-27 03:08:22.776955 emotional-0.3.0/emotional/__init__.py
--rw-r--r--   0        0        0      368 2023-05-27 02:52:07.423635 emotional-0.3.0/emotional/_compat.py
--rw-r--r--   0        0        0       26 2022-09-16 23:25:13.176855 emotional-0.3.0/emotional/_version.py
--rw-r--r--   0        0        0      534 2022-12-14 23:26:05.855303 emotional-0.3.0/emotional/changelog.py
--rw-r--r--   0        0        0     5016 2023-05-29 23:31:26.683409 emotional-0.3.0/emotional/config.py
--rw-r--r--   0        0        0     2864 2023-05-27 22:47:44.207044 emotional-0.3.0/emotional/defaults.py
--rw-r--r--   0        0        0     1476 2022-10-15 12:56:13.266978 emotional-0.3.0/emotional/github.py
--rw-r--r--   0        0        0     1644 2022-10-15 12:56:13.253645 emotional-0.3.0/emotional/gitlab.py
--rw-r--r--   0        0        0     1154 2022-10-15 12:56:13.246978 emotional-0.3.0/emotional/jira.py
--rw-r--r--   0        0        0     8199 2023-05-27 23:13:14.873415 emotional-0.3.0/emotional/plugin.py
--rw-r--r--   0        0        0     1290 2023-05-29 23:31:26.683409 emotional-0.3.0/emotional/templates/changelog.md.jinja
--rw-r--r--   0        0        0      679 2022-09-30 23:32:44.967373 emotional-0.3.0/emotional/templates/example.jinja
--rw-r--r--   0        0        0     1285 2023-05-29 23:36:13.810761 emotional-0.3.0/emotional/templates/info.md.jinja
--rw-r--r--   0        0        0      492 2023-05-27 03:38:07.830591 emotional-0.3.0/emotional/utils.py
--rw-r--r--   0        0        0     3155 2023-05-30 16:28:29.450905 emotional-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-19 23:34:18.625328 emotional-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1760 2023-05-26 13:49:14.058121 emotional-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     2326 2023-05-26 23:19:31.330807 emotional-0.3.0/tests/fixtures/changelogs/default.md
--rw-r--r--   0        0        0     2322 2023-05-27 02:17:11.627205 emotional-0.3.0/tests/fixtures/changelogs/group_by_scope.md
--rw-r--r--   0        0        0     2326 2023-05-29 23:19:47.101655 emotional-0.3.0/tests/fixtures/changelogs/order_by_scope.md
--rw-r--r--   0        0        0     2326 2023-05-27 02:17:11.627205 emotional-0.3.0/tests/fixtures/changelogs/release_emoji.md
--rw-r--r--   0        0        0     2585 2023-05-27 23:13:14.806748 emotional-0.3.0/tests/test_bump.py
--rw-r--r--   0        0        0    20509 2023-05-29 23:35:29.773993 emotional-0.3.0/tests/test_changelog.py
--rw-r--r--   0        0        0     5595 2023-05-27 03:43:41.674835 emotional-0.3.0/tests/test_commit.py
--rw-r--r--   0        0        0     1381 2022-12-18 16:24:15.888821 emotional-0.3.0/tests/test_config.py
--rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.885488 emotional-0.3.0/tests/test_github.py
--rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.888821 emotional-0.3.0/tests/test_gitlab.py
--rw-r--r--   0        0        0     2588 2022-12-18 16:24:15.888821 emotional-0.3.0/tests/test_jira.py
--rw-r--r--   0        0        0      644 2023-05-27 03:02:52.109422 emotional-0.3.0/tests/test_plugin.py
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 emotional-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-09-16 23:07:01.534539 emotional-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2981 2023-05-29 23:31:26.683409 emotional-0.3.1/README.md
+-rw-r--r--   0        0        0       98 2023-05-27 03:08:22.776955 emotional-0.3.1/emotional/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-27 02:52:07.423635 emotional-0.3.1/emotional/_compat.py
+-rw-r--r--   0        0        0       26 2022-09-16 23:25:13.176855 emotional-0.3.1/emotional/_version.py
+-rw-r--r--   0        0        0      550 2023-06-16 14:21:57.779235 emotional-0.3.1/emotional/changelog.py
+-rw-r--r--   0        0        0     5016 2023-05-29 23:31:26.683409 emotional-0.3.1/emotional/config.py
+-rw-r--r--   0        0        0     2864 2023-05-27 22:47:44.207044 emotional-0.3.1/emotional/defaults.py
+-rw-r--r--   0        0        0     1476 2022-10-15 12:56:13.266978 emotional-0.3.1/emotional/github.py
+-rw-r--r--   0        0        0     1644 2022-10-15 12:56:13.253645 emotional-0.3.1/emotional/gitlab.py
+-rw-r--r--   0        0        0     1154 2022-10-15 12:56:13.246978 emotional-0.3.1/emotional/jira.py
+-rw-r--r--   0        0        0     8199 2023-05-27 23:13:14.873415 emotional-0.3.1/emotional/plugin.py
+-rw-r--r--   0        0        0      570 2023-05-30 22:46:58.266154 emotional-0.3.1/emotional/templates/changelog.md.jinja
+-rw-r--r--   0        0        0      679 2022-09-30 23:32:44.967373 emotional-0.3.1/emotional/templates/example.jinja
+-rw-r--r--   0        0        0     1285 2023-05-29 23:36:13.810761 emotional-0.3.1/emotional/templates/info.md.jinja
+-rw-r--r--   0        0        0     1089 2023-05-30 22:50:49.123348 emotional-0.3.1/emotional/templates/macros.md.jinja
+-rw-r--r--   0        0        0      492 2023-05-27 03:38:07.830591 emotional-0.3.1/emotional/utils.py
+-rw-r--r--   0        0        0     2940 2023-06-16 14:24:52.018660 emotional-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-19 23:34:18.625328 emotional-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1760 2023-05-26 13:49:14.058121 emotional-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     2325 2023-05-30 22:43:26.895646 emotional-0.3.1/tests/fixtures/changelogs/default.md
+-rw-r--r--   0        0        0     2321 2023-05-30 22:43:21.108965 emotional-0.3.1/tests/fixtures/changelogs/group_by_scope.md
+-rw-r--r--   0        0        0     2325 2023-05-30 22:43:15.548951 emotional-0.3.1/tests/fixtures/changelogs/order_by_scope.md
+-rw-r--r--   0        0        0     2325 2023-05-30 22:43:05.728927 emotional-0.3.1/tests/fixtures/changelogs/release_emoji.md
+-rw-r--r--   0        0        0     2505 2023-06-16 13:53:54.654049 emotional-0.3.1/tests/test_bump.py
+-rw-r--r--   0        0        0    20509 2023-05-29 23:35:29.773993 emotional-0.3.1/tests/test_changelog.py
+-rw-r--r--   0        0        0     5595 2023-05-27 03:43:41.674835 emotional-0.3.1/tests/test_commit.py
+-rw-r--r--   0        0        0     1381 2022-12-18 16:24:15.888821 emotional-0.3.1/tests/test_config.py
+-rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.885488 emotional-0.3.1/tests/test_github.py
+-rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.888821 emotional-0.3.1/tests/test_gitlab.py
+-rw-r--r--   0        0        0     2588 2022-12-18 16:24:15.888821 emotional-0.3.1/tests/test_jira.py
+-rw-r--r--   0        0        0      644 2023-05-27 03:02:52.109422 emotional-0.3.1/tests/test_plugin.py
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 emotional-0.3.1/PKG-INFO
```

### Comparing `emotional-0.3.0/LICENSE` & `emotional-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/README.md` & `emotional-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/changelog.py` & `emotional-0.3.1/emotional/changelog.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 
 TEMPLATE = "changelog.md.jinja"
 
 
 def render_changelog(tree: Iterable, config: EmotionalConfig | None = None) -> str:
     config = config or EmotionalConfig()
     changelog: str = render_template(TEMPLATE, tree=tree, config=config, settings=config.settings)
-    return changelog
+    return changelog.rstrip() + "\n"
 
 
 def monkeypatch():
     from commitizen import changelog
 
     changelog.render_changelog = render_changelog
```

### Comparing `emotional-0.3.0/emotional/config.py` & `emotional-0.3.1/emotional/config.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/defaults.py` & `emotional-0.3.1/emotional/defaults.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/github.py` & `emotional-0.3.1/emotional/github.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/gitlab.py` & `emotional-0.3.1/emotional/gitlab.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/jira.py` & `emotional-0.3.1/emotional/jira.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/plugin.py` & `emotional-0.3.1/emotional/plugin.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/templates/example.jinja` & `emotional-0.3.1/emotional/templates/example.jinja`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/emotional/templates/info.md.jinja` & `emotional-0.3.1/emotional/templates/info.md.jinja`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/pyproject.toml` & `emotional-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dependencies = [
     "commitizen>=3.0",
     "typing-extensions>=4.4.0; python_version<'3.10'",
 ]
 dynamic = []
 requires-python = ">=3.7"
 readme = "README.md"
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."commitizen.plugin"]
 emotional = "emotional.plugin:Emotional"
 
@@ -33,17 +33,16 @@
 [tool.pdm.dev-dependencies]
 test = [
     "pytest>=7.1.2",
     "pytest-sugar>=0.9.5",
     "pytest-cov>=3.0.0",
 ]
 lint = [
-    "black==23.3.0",
     "mypy==1.3.0",
-    "absolufy-imports>=0.3.1",
+    "black==23.3.0",
     "ruff==0.0.270",
 ]
 
 [tool.pdm.scripts]
 pre_cover = "coverage erase"
 
 [tool.pdm.scripts.test]
@@ -98,15 +97,14 @@
 [tool.commitizen]
 name = "emotional"
 github = "noirbizarre/emotional"
 version_provider = "scm"
 
 [tool.black]
 line-length = 100
-exclude = "/(\n    \\.git\n  | \\.github\n  | \\.mypy_cache\n  | \\.pytest_cache\n  | \\.tox\n  | \\.venv\n  | __pycache__\n  | __pypackages__\n  | build\n  | dist\n  | reports\n)/\n"
 
 [tool.pytest.ini_options]
 addopts = "-ra"
 norecursedirs = ".git build dist"
 testpaths = [
     "emotional/",
     "tests/",
```

### Comparing `emotional-0.3.0/tests/conftest.py` & `emotional-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/tests/fixtures/changelogs/default.md` & `emotional-0.3.1/tests/fixtures/changelogs/default.md`

 * *Files 0% similar despite different names*

```diff
@@ -124,8 +124,7 @@
 ## 🚀 v0.9.2 (2017-11-11)
 
 ## 🚀 v0.9.1 (2017-11-11)
 
 ### 🐛 Bug fixes
 
 - **setup.py**: future is now required for every python version
-
```

### Comparing `emotional-0.3.0/tests/fixtures/changelogs/group_by_scope.md` & `emotional-0.3.1/tests/fixtures/changelogs/group_by_scope.md`

 * *Files 0% similar despite different names*

```diff
@@ -159,8 +159,7 @@
 ## 🚀 v0.9.1 (2017-11-11)
 
 ### 🐛 Bug fixes
 
 #### setup.py
 
 - future is now required for every python version
-
```

### Comparing `emotional-0.3.0/tests/fixtures/changelogs/order_by_scope.md` & `emotional-0.3.1/tests/fixtures/changelogs/order_by_scope.md`

 * *Files 0% similar despite different names*

```diff
@@ -124,8 +124,7 @@
 ## 🚀 v0.9.2 (2017-11-11)
 
 ## 🚀 v0.9.1 (2017-11-11)
 
 ### 🐛 Bug fixes
 
 - **setup.py**: future is now required for every python version
-
```

### Comparing `emotional-0.3.0/tests/fixtures/changelogs/release_emoji.md` & `emotional-0.3.1/tests/fixtures/changelogs/release_emoji.md`

 * *Files 0% similar despite different names*

```diff
@@ -124,8 +124,7 @@
 ## 🎉 v0.9.2 (2017-11-11)
 
 ## 🎉 v0.9.1 (2017-11-11)
 
 ### 🐛 Bug fixes
 
 - **setup.py**: future is now required for every python version
-
```

### Comparing `emotional-0.3.0/tests/test_bump.py` & `emotional-0.3.1/tests/test_bump.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,15 +67,13 @@
         (MAJOR_INCREMENTS_EXCLAMATION_SAMPLE_2, "MAJOR"),
         (NONE_INCREMENT, None),
     ),
 )
 def test_find_increment(messages, expected_type, config):
     cz = Emotional(config)
     commits = [GitCommit(rev="test", title=message) for message in messages]
-    print("bump_pattern:", cz.bump_pattern)
-    print("bump_map:", cz.bump_map)
     increment_type = bump.find_increment(
         commits,
         regex=cz.bump_pattern,
         increments_map=cz.bump_map,
     )
     assert increment_type == expected_type
```

### Comparing `emotional-0.3.0/tests/test_changelog.py` & `emotional-0.3.1/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/tests/test_commit.py` & `emotional-0.3.1/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/tests/test_config.py` & `emotional-0.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/tests/test_github.py` & `emotional-0.3.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/tests/test_gitlab.py` & `emotional-0.3.1/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/tests/test_jira.py` & `emotional-0.3.1/tests/test_jira.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/tests/test_plugin.py` & `emotional-0.3.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `emotional-0.3.0/PKG-INFO` & `emotional-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotional
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Commitizen plugin for conventional commit with emojis and integrations
 Author-Email: Axel H. <noirbizarre@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Requires-Dist: commitizen>=3.0
 Requires-Dist: typing-extensions>=4.4.0; python_version < "3.10"
 Description-Content-Type: text/markdown
```

