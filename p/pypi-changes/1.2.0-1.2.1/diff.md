# Comparing `tmp/pypi_changes-1.2.0.tar.gz` & `tmp/pypi_changes-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_changes-1.2.0.tar", last modified: Tue Jun 28 23:47:02 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pypi_changes-1.2.0.tar` & `pypi_changes-1.2.1.tar`

### file list

```diff
@@ -1,60 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.042094 pypi_changes-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.038094 pypi_changes-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.038094 pypi_changes-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-06-28 23:47:02.042094 pypi_changes-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.038094 pypi_changes-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    61998 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/docs/demo.gif
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-06-28 23:47:02.042094 pypi_changes-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.038094 pypi_changes-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.038094 pypi_changes-1.2.0/src/pypi_changes/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/_distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5852 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/_pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.038094 pypi_changes-1.2.0/src/pypi_changes/_print/
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/_print/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/_print/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/_print/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-28 23:47:00.000000 pypi_changes-1.2.0/src/pypi_changes/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/src/pypi_changes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.038094 pypi_changes-1.2.0/src/pypi_changes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-06-28 23:47:01.000000 pypi_changes-1.2.0/src/pypi_changes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-06-28 23:47:02.000000 pypi_changes-1.2.0/src/pypi_changes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 23:47:01.000000 pypi_changes-1.2.0/src/pypi_changes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-28 23:47:01.000000 pypi_changes-1.2.0/src/pypi_changes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-06-28 23:47:01.000000 pypi_changes-1.2.0/src/pypi_changes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-28 23:47:01.000000 pypi_changes-1.2.0/src/pypi_changes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:47:02.042094 pypi_changes-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8933 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/pypi_info_missing_package.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   162624 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/pypi_info_pytz.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/pypi_info_self.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_pkg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_print rich.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_print_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_pypi_changes.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-28 23:46:52.000000 pypi_changes-1.2.0/whitelist.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.markdownlint.yaml
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.readthedocs.yml
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tox.ini
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/whitelist.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/docs/changelog.rst
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/docs/conf.py
+-rw-r--r--   0        0        0    61998 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/docs/demo.gif
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/docs/index.rst
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/__main__.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_cli.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_distributions.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_info.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_pkg.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_print/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_print/json.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/src/pypi_changes/_print/tree.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/pypi_info_missing_package.yaml
+-rw-r--r--   0        0        0   162624 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/pypi_info_pytz.yaml
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/pypi_info_self.yaml
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_distributions.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_info.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_main.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_pkg.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_print_json.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_print_rich.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_pypi_changes.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/tests/test_version.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/LICENSE
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/README.md
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 pypi_changes-1.2.1/PKG-INFO
```

### Comparing `pypi_changes-1.2.0/.github/CONTRIBUTING.md` & `pypi_changes-1.2.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pypi_changes-1.2.0/.github/workflows/check.yml` & `pypi_changes-1.2.1/.github/workflows/check.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 name: check
 on:
   push:
+    tags-ignore: ["**"]
   pull_request:
   schedule:
     - cron: "0 8 * * *"
 
 concurrency:
   group: check-${{ github.ref }}
   cancel-in-progress: true
@@ -13,22 +14,22 @@
   test:
     name: test with ${{ matrix.py }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         py:
+          - "3.12.0-beta.2"
+          - "3.11"
           - "3.10"
           - "3.9"
-          - "3.8"
-          - "3.7"
         os:
-          - ubuntu-20.04
-          - windows-2022
-          - macos-10.15
+          - ubuntu-latest
+          - windows-latest
+          - macos-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v4
         with:
@@ -50,48 +51,25 @@
       matrix:
         tox_env:
           - type
           - dev
           - docs
           - pkg_meta
         os:
-          - ubuntu-20.04
-          - windows-2022
+          - ubuntu-latest
+          - windows-latest
         exclude:
           - { os: windows, tox_env: pkg_meta }
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - name: Setup Python 3.10
+      - name: Setup Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install tox
         run: python -m pip install tox
       - name: Run check for ${{ matrix.tox_env }}
         run: tox -e ${{ matrix.tox_env }}
         env:
           UPGRADE_ADVISORY: "yes"
-
-  publish:
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-    needs: [check, test]
-    runs-on: ubuntu-20.04
-    steps:
-      - name: Setup python to build package
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.10"
-      - name: Install build
-        run: python -m pip install build
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Build package
-        run: pyproject-build -s -w . -o dist
-      - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          skip_existing: true
-          user: __token__
-          password: ${{ secrets.pypi_password }}
```

### Comparing `pypi_changes-1.2.0/CODE_OF_CONDUCT.md` & `pypi_changes-1.2.1/CODE_OF_CONDUCT.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 project or its community. Examples of representing a project or community include using an official project e-mail
 address, posting via an official social media account, or acting as an appointed representative at an online or offline
 event. Representation of a project may be further defined and clarified by project maintainers.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at
-gaborjbernat@gmail.com. The project team will review and investigate all complaints, and will respond in a way that it
-deems appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the
-reporter of an incident. Further details of specific enforcement policies may be posted separately.
+`gaborjbernat@gmail.com` deems appropriate to the circumstances. The project team is obligated to maintain
+confidentiality with regard to the reporter of an incident. Further details of specific enforcement policies may be
+posted separately.
 
 Project maintainers who do not follow or enforce the Code of Conduct in good faith may face temporary or permanent
 repercussions as determined by other members of the project's leadership.
 
 ## Attribution
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4, available at
```

### Comparing `pypi_changes-1.2.0/LICENSE` & `pypi_changes-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_changes-1.2.0/README.md` & `pypi_changes-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pypi_changes-1.2.0/docs/conf.py` & `pypi_changes-1.2.1/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""Configuration for documentation generation."""  # noqa: INP001
 from __future__ import annotations
 
-from datetime import date, datetime
+from datetime import datetime, timezone
 
 from pypi_changes import __version__
 
 company = "gaborbernat"
 name = "pypi-changes"
+now = datetime.now(tz=timezone.utc)
 version = ".".join(__version__.split(".")[:2])
 release = __version__
-copyright = f"2021-{date.today().year}, {company}"
+copyright = f"2021-{now.year}, {company}"  # noqa: A001
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx_argparse_cli",
@@ -33,33 +35,33 @@
 today_fmt = "%B %d, %Y"
 
 html_theme = "furo"
 html_theme_options = {
     "navigation_with_keys": True,
 }
 html_title = "pypi changes"
-html_last_updated_fmt = datetime.now().isoformat()
+html_last_updated_fmt = now.isoformat()
 
 autoclass_content = "class"
 autodoc_member_order = "bysource"
 autodoc_default_options = {
     "member-order": "bysource",
     "undoc-members": True,
     "show-inheritance": True,
 }
 autodoc_typehints = "none"
 always_document_param_types = False
 typehints_fully_qualified = True
 autosectionlabel_prefix_document = True
 
 extlinks = {
-    "issue": ("https://github.com/gaborbernat/pypi_changes/issues/%s", "#"),
-    "pull": ("https://github.com/gaborbernat/pypi_changes/pull/%s", "PR #"),
-    "user": ("https://github.com/%s", "@"),
-    "pypi": ("https://pypi.org/project/%s", ""),
+    "issue": ("https://github.com/gaborbernat/pypi_changes/issues/%s", "#%s"),
+    "pull": ("https://github.com/gaborbernat/pypi_changes/pull/%s", "PR #%s"),
+    "user": ("https://github.com/%s", "@%s"),
+    "pypi": ("https://pypi.org/project/%s", "%s"),
 }
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "packaging": ("https://packaging.pypa.io/en/latest", None),
 }
 nitpicky = True
 nitpick_ignore = []
```

### Comparing `pypi_changes-1.2.0/docs/demo.gif` & `pypi_changes-1.2.1/docs/demo.gif`

 * *Files identical despite different names*

### Comparing `pypi_changes-1.2.0/src/pypi_changes/_cli.py` & `pypi_changes-1.2.1/src/pypi_changes/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 from argparse import Action, ArgumentDefaultsHelpFormatter, ArgumentError, ArgumentParser, Namespace
 from pathlib import Path
-from typing import Sequence
+from typing import TYPE_CHECKING
 
 from platformdirs import user_cache_path
 
 from ._version import version
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 
 class Options(Namespace):
     python: Path
     jobs: int
     cache_path: Path
     cache_duration: int
     sort: str
@@ -68,20 +71,20 @@
 
     return parser
 
 
 class _Python(Action):
     def __call__(
         self,
-        parser: ArgumentParser,  # noqa: U100
-        namespace: Namespace,  # noqa: U100
+        parser: ArgumentParser,  # noqa: ARG002
+        namespace: Namespace,
         values: str | Sequence[str] | None,
-        option_string: str | None = None,  # noqa: U100
+        option_string: str | None = None,  # noqa: ARG002
     ) -> None:
-        assert isinstance(values, str)
+        assert isinstance(values, str)  # noqa: S101
         path = Path(values).absolute()
         if not path.exists():
             raise ArgumentError(self, f"path {path} does not exist")
         setattr(namespace, self.dest, path)
 
 
 class _HelpFormatter(ArgumentDefaultsHelpFormatter):
```

### Comparing `pypi_changes-1.2.0/src/pypi_changes/_distributions.py` & `pypi_changes-1.2.1/src/pypi_changes/_distributions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 
 import json
 import re
-import sys
+from importlib.metadata import Distribution, PathDistribution
 from pathlib import Path
 from subprocess import check_output
-from typing import Generator, Iterable
+from typing import TYPE_CHECKING
 
 from rich.console import Console
 
-from ._cli import Options
-
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
-    from importlib.metadata import Distribution, PathDistribution
-else:  # pragma: no cover (<py38)
-    from importlib_metadata import Distribution, PathDistribution
+if TYPE_CHECKING:
+    from collections.abc import Generator, Iterable
 
+    from ._cli import Options
 
 _PKG_REGEX = re.compile(r"^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])(\.egg-info|\.dist-info)$", flags=re.IGNORECASE)
 
 
 def collect_distributions(options: Options) -> list[PathDistribution]:
     distributions: list[PathDistribution] = []
     with Console().status("Discovering distributions") as status:
@@ -28,25 +25,24 @@
             status.update(f"Discovering distributions {len(distributions)}")
             distributions.append(dist)
     return distributions
 
 
 def _get_py_info(python: str) -> list[Path]:
     cmd = [python, "-c", "import sys, json; print(json.dumps(sys.path))"]
-    paths = [Path(i) for i in json.loads(check_output(cmd, text=True))]
-    return paths
+    return [Path(i) for i in json.loads(check_output(cmd, text=True))]  # noqa: S603
 
 
 def _iter_distributions(paths: Iterable[Path]) -> Generator[PathDistribution, None, None]:
     found: set[str] = set()
     done_paths: set[Path] = set()
-    for path in paths:
-        if not path.exists():
+    for raw_path in paths:
+        if not raw_path.exists():
             continue
-        path = path.resolve()
+        path = raw_path.resolve()
         if path not in done_paths:
             done_paths.add(path)
             for candidate in path.iterdir():
                 if not candidate.is_dir():
                     continue
                 match = _PKG_REGEX.match(candidate.name)
                 if match:
```

### Comparing `pypi_changes-1.2.0/src/pypi_changes/_info.py` & `pypi_changes-1.2.1/src/pypi_changes/_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 import os
-import sys
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from contextlib import ExitStack, contextmanager
 from datetime import datetime, timedelta, timezone
-from typing import Any, Generator, Iterator, Sequence
+from typing import TYPE_CHECKING, Any
 
 from packaging.version import InvalidVersion, Version
 from pypi_simple import PyPISimple
-from requests import Session
-from requests_cache import CachedSession  # type: ignore # no implicit re-export
+from requests_cache import CachedSession
 from rich.progress import BarColumn, Progress, Task, TextColumn, TimeRemainingColumn
 from rich.text import Text
 
-from ._cli import Options
 from ._pkg import Package
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
+if TYPE_CHECKING:
+    from collections.abc import Generator, Iterator, Sequence
     from importlib.metadata import PathDistribution
-else:  # pragma: no cover (<py38)
-    from importlib_metadata import PathDistribution
+
+    from requests import Session
+
+    from ._cli import Options
 
 PYPI_INDEX = "https://pypi.org/simple"
 
 
 def pypi_info(distributions: Sequence[PathDistribution], options: Options) -> Generator[Package, None, None]:
     with ExitStack() as stack:
         enter = stack.enter_context
@@ -49,28 +49,27 @@
         executor = enter(ThreadPoolExecutor(max_workers=options.jobs, thread_name_prefix="version-getter"))
         future_to_url = {executor.submit(one_info, client, session, dist): dist for dist in distributions}
         for future in as_completed(future_to_url):
             dist = future_to_url[future]
             progress.update(task, advance=1)
             try:
                 result: Exception | dict[str, Any] | None = future.result()
-            except Exception as exc:
+            except Exception as exc:  # noqa: BLE001
                 result = exc
             yield Package(dist, result)
 
 
 class SpeedColumn(TextColumn):
     def __init__(self) -> None:
         super().__init__("[bold cyan]")
 
     def render(self, task: Task) -> Text:
         if task.speed is None:
             return Text("no speed")
-        else:
-            return Text(f"{task.speed:.3f} steps/s")
+        return Text(f"{task.speed:.3f} steps/s")
 
 
 @contextmanager
 def _pypi_client(session: Session) -> Iterator[PyPISimple | None]:
     url = os.environ.get("PIP_INDEX_URL")
     if url is not None and url.lstrip("/") != PYPI_INDEX:
         with PyPISimple(endpoint=url, session=session) as client:
@@ -113,29 +112,30 @@
         version = Version(value[0])
     except InvalidVersion:
         version = Version("0.0.1")
     return version, value[1][0]["upload_time_iso_8601"]
 
 
 def _merge_with_index_server(
-    name: str, pypi_client: PyPISimple, releases: dict[str, list[dict[str, Any]]]
+    name: str,
+    pypi_client: PyPISimple,
+    releases: dict[str, list[dict[str, Any]]],
 ) -> dict[str, list[dict[str, Any]]]:
     index_info = pypi_client.get_project_page(name)
-    if index_info is not None:
-        index_releases = defaultdict(list)
-        for pkg in index_info.packages:
-            release = {"packagetype": pkg.package_type, "version": pkg.version, "upload_time_iso_8601": None}
-            if pkg.version is not None:  # some Artifactory might not set this for .egg-info uploads, ignore those
-                index_releases[pkg.version].append(release)
-
-        missing = {ver: values for ver, values in index_releases.items() if ver not in releases}
-        if missing:
-            missing.update(releases)
-            missing = dict(sorted(missing.items(), key=sort_by_version_release, reverse=True))
-            releases = missing
+    index_releases = defaultdict(list)
+    for pkg in index_info.packages:
+        release = {"packagetype": pkg.package_type, "version": pkg.version, "upload_time_iso_8601": None}
+        if pkg.version is not None:  # some Artifactory might not set this for .egg-info uploads, ignore those
+            index_releases[pkg.version].append(release)
+
+    missing = {ver: values for ver, values in index_releases.items() if ver not in releases}
+    if missing:
+        missing.update(releases)
+        missing = dict(sorted(missing.items(), key=sort_by_version_release, reverse=True))
+        return missing
     return releases
 
 
 __all__ = [
     "pypi_info",
     "Package",
 ]
```

### Comparing `pypi_changes-1.2.0/src/pypi_changes/_pkg.py` & `pypi_changes-1.2.1/src/pypi_changes/_pkg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 from __future__ import annotations
 
-import sys
 from datetime import datetime, timezone
-from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from packaging.version import Version
 
-if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
+if TYPE_CHECKING:
     from importlib.metadata import PathDistribution
-else:  # pragma: no cover (<py38)
-    from importlib_metadata import PathDistribution
+    from pathlib import Path
 
 
 class Package:
     def __init__(self, dist: PathDistribution, info: dict[str, Any] | None | Exception) -> None:
         self.dist: PathDistribution = dist
         self.info: dict[str, Any] | None = None if isinstance(info, Exception) else info
         self.exc = info if isinstance(info, Exception) else None
 
     @property
     def last_release_at(self) -> datetime:
         last_release = self.last_release
         if last_release is None:
             return datetime.now(timezone.utc)
-        return self.last_release["upload_time_iso_8601"]  # type: ignore # Any instead of datetime
+        return self.last_release["upload_time_iso_8601"]  # type: ignore[no-any-return,index] # Any instead of datetime
 
     @property
     def last_release(self) -> dict[str, Any] | None:
         if self.info is None or not self.info["releases"]:
             return None
         for version_str, releases in self.info["releases"].items():
             version = Version(version_str)
             if not version.is_devrelease and not version.is_prerelease:
-                return releases[0]  # type: ignore
-        return next(iter(self.info["releases"].values()))[0]  # type: ignore
+                return releases[0]  # type: ignore[no-any-return]
+        return next(iter(self.info["releases"].values()))[0]  # type: ignore[no-any-return]
 
     @property
     def name(self) -> str:
-        return self.dist.metadata["Name"]  # type: ignore
+        return self.dist.metadata["Name"]
 
     @property
     def version(self) -> str:
         return self.dist.version
 
     @property
     def path(self) -> Path:
-        return self.dist._path  # type: ignore # it exists
+        return self.dist._path  # type: ignore[no-any-return,attr-defined] # it exists  # noqa: SLF001
 
     @property
     def current_release(self) -> dict[str, Any]:
         if self.info is not None:
             release_info = self.info["releases"].get(self.version)
             if release_info is not None:
                 return release_info[0] or {}
```

### Comparing `pypi_changes-1.2.0/src/pypi_changes/_print/__init__.py` & `pypi_changes-1.2.1/src/pypi_changes/_print/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
-from datetime import datetime
-from typing import Iterable
+from typing import TYPE_CHECKING
 
-from .._cli import Options
-from .._pkg import Package
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+    from datetime import datetime
+
+    from pypi_changes._cli import Options
+    from pypi_changes._pkg import Package
 
 
 class _Reversor:
     def __init__(self, obj: str) -> None:
         self.obj = obj
 
     def __eq__(self, other: object) -> bool:
```

### Comparing `pypi_changes-1.2.0/src/pypi_changes/_print/json.py` & `pypi_changes-1.2.1/src/pypi_changes/_print/json.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 import json
 from datetime import datetime, timezone
-from typing import Any, Iterable
+from typing import TYPE_CHECKING, Any
 
 from humanize import naturaldelta
 
-from .._cli import Options
-from .._pkg import Package
 from . import get_sorted_pkg_list
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    from pypi_changes._cli import Options
+    from pypi_changes._pkg import Package
+
 
 def release_info(release: dict[str, Any] | None, now: datetime) -> dict[str, Any]:
     if release is None:
         return {}
     release_at = release.get("upload_time_iso_8601")
     release_since = naturaldelta(now - release_at) if release_at else None
     return {
@@ -33,15 +37,15 @@
         pkg_list.append(
             {
                 "name": pkg.name,
                 "version": pkg.version,
                 "up_to_date": pkg.version == latest_release.get("version") if latest_release is not None else True,
                 "current": current_release,
                 "latest": latest_release,
-            }
+            },
         )
-    print(json.dumps(pkg_list, indent=2))
+    print(json.dumps(pkg_list, indent=2))  # noqa: T201
 
 
 __all__ = [
     "print_json",
 ]
```

### Comparing `pypi_changes-1.2.0/src/pypi_changes/_print/tree.py` & `pypi_changes-1.2.1/src/pypi_changes/_print/tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from __future__ import annotations
 
 from datetime import datetime, timezone
-from typing import Iterable
+from typing import TYPE_CHECKING
 
 from humanize import naturaldelta
 from rich import print as rich_print
 from rich.markup import escape
 from rich.text import Text
 from rich.tree import Tree
 
-from .._cli import Options
-from .._pkg import Package
 from . import get_sorted_pkg_list
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    from pypi_changes._cli import Options
+    from pypi_changes._pkg import Package
+
 
 def print_tree(distributions: Iterable[Package], options: Options) -> None:
     now = datetime.now(timezone.utc)
     tree = Tree(f"🐍 Distributions within {escape(str(options.python))}", guide_style="cyan")
     for pkg in get_sorted_pkg_list(distributions, options, now):
         text = Text(pkg.name, "yellow")
         text.stylize(f"link https://pypi.org/project/{pkg.name}/#history")
```

### Comparing `pypi_changes-1.2.0/tests/conftest.py` & `pypi_changes-1.2.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from __future__ import annotations
 
 import sys
-from pathlib import Path
+from typing import TYPE_CHECKING
 from unittest.mock import MagicMock, create_autospec
 
 import pytest
-from _pytest.monkeypatch import MonkeyPatch
 
 from pypi_changes._cli import Options
-from tests import MakeDist
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from _pytest.monkeypatch import MonkeyPatch
+
+    from tests import MakeDist
 
 
 @pytest.fixture(autouse=True)
 def _no_index(monkeypatch: MonkeyPatch) -> None:
     monkeypatch.delenv("PIP_INDEX_URL", raising=False)
 
 
@@ -30,12 +35,12 @@
 
 @pytest.fixture()
 def make_dist() -> MakeDist:
     def func(path: Path, name: str, version: str) -> MagicMock:
         of_type = f"importlib{'.' if sys.version_info >= (3, 8) else '_'}metadata.PathDistribution"
         dist: MagicMock = create_autospec(of_type)
         dist.metadata = {"Name": name}
-        dist._path = path / "dist"
+        dist._path = path / "dist"  # noqa: SLF001
         dist.version = version
         return dist
 
     return func
```

### Comparing `pypi_changes-1.2.0/tests/pypi_info_missing_package.yaml` & `pypi_changes-1.2.1/tests/pypi_info_missing_package.yaml`

 * *Files identical despite different names*

### Comparing `pypi_changes-1.2.0/tests/pypi_info_pytz.yaml` & `pypi_changes-1.2.1/tests/pypi_info_pytz.yaml`

 * *Files identical despite different names*

### Comparing `pypi_changes-1.2.0/tests/pypi_info_self.yaml` & `pypi_changes-1.2.1/tests/pypi_info_self.yaml`

 * *Files identical despite different names*

### Comparing `pypi_changes-1.2.0/tests/test_cli.py` & `pypi_changes-1.2.1/tests/test_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 from unittest.mock import call
 
 import pytest
-from _pytest.capture import CaptureFixture
-from pytest_mock import MockerFixture
 
 from pypi_changes import __version__
 from pypi_changes._cli import Options, parse_cli_arguments
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from _pytest.capture import CaptureFixture
+    from pytest_mock import MockerFixture
+
 
 def test_cli_ok_default(tmp_path: Path, mocker: MockerFixture) -> None:
     user_cache_path = mocker.patch("pypi_changes._cli.user_cache_path", return_value=tmp_path / "cache")
 
     options = parse_cli_arguments([str(tmp_path)])
 
     assert isinstance(options, Options)
```

### Comparing `pypi_changes-1.2.0/tests/test_distributions.py` & `pypi_changes-1.2.1/tests/test_distributions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import sys
 from pathlib import Path
-
-from pytest_mock import MockerFixture
+from typing import TYPE_CHECKING
 
 from pypi_changes._cli import Options
 from pypi_changes._distributions import collect_distributions
 from tests import PathDistribution
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
 
 def test_distributions() -> None:
     distributions = list(collect_distributions(Options(python=Path(sys.executable))))
     assert all(isinstance(i, PathDistribution) for i in distributions)
 
 
 def _make_dist(path: Path, name: str) -> Path:
@@ -32,8 +34,8 @@
 
 def test_distribution_duplicate_pkg(mocker: MockerFixture, tmp_path: Path) -> None:
     dist_1, dist_2 = _make_dist(tmp_path / "1", "a"), _make_dist(tmp_path / "2", "a")
     mocker.patch("pypi_changes._distributions._get_py_info", return_value=[dist_1.parent, dist_2.parent])
     distributions = list(collect_distributions(Options(python=Path(sys.executable))))
     assert len(distributions) == 1
     assert distributions[0].metadata["Name"] == "a"
-    assert distributions[0]._path == dist_1  # type: ignore # we're accessing a private property not type hinted
+    assert distributions[0]._path == dist_1  # type: ignore[attr-defined]  # noqa: SLF001
```

### Comparing `pypi_changes-1.2.0/tests/test_info.py` & `pypi_changes-1.2.1/tests/test_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from __future__ import annotations
 
 import os
 from datetime import datetime, timezone
 from pathlib import Path
+from typing import TYPE_CHECKING
 from unittest.mock import create_autospec
 
 import pytest
 from pypi_simple import DistributionPackage, ProjectPage, PyPISimple
-from pytest_mock import MockerFixture
 from vcr import use_cassette
 
-from pypi_changes._cli import Options
 from pypi_changes._info import _merge_with_index_server, pypi_info
 from pypi_changes._pkg import Package
-from tests import MakeDist
+
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from pypi_changes._cli import Options
+    from tests import MakeDist
 
 
 @pytest.fixture()
-def _force_pypi_index(mocker: MockerFixture, _no_index: None) -> None:  # noqa: U101
+def _force_pypi_index(mocker: MockerFixture, _no_index: None) -> None:
     mocker.patch("pypi_changes._info.PYPI_INDEX", "")
     mocker.patch.dict(os.environ, {"PIP_INDEX_URL": "https://pypi.org/simple"})
 
 
 @pytest.mark.usefixtures("_force_pypi_index")
 def test_info_self(tmp_path: Path, option_simple: Options, make_dist: MakeDist) -> None:
     dist = make_dist(tmp_path, "pypi-changes", "1.0.0")
@@ -30,30 +34,30 @@
     with use_cassette(str(Path(__file__).parent / "pypi_info_self.yaml"), mode="once"):
         packages = list(pypi_info(distributions, option_simple))
 
     assert isinstance(packages, list)
     assert len(packages) == 1
     pkg = packages[0]
     assert isinstance(pkg, Package)
-    assert repr(pkg) == f"Package(name='pypi-changes', path={repr(tmp_path / 'dist')})"
+    assert repr(pkg) == f"Package(name='pypi-changes', path={tmp_path / 'dist'!r})"
 
 
 @pytest.mark.usefixtures("_force_pypi_index")
 @pytest.mark.usefixtures("_no_proxy")
 def test_info_missing(tmp_path: Path, option_simple: Options, make_dist: MakeDist) -> None:
     dist = make_dist(tmp_path, "missing-package", "1.0.0")
     distributions = [dist]
 
     with use_cassette(str(Path(__file__).parent / "pypi_info_missing_package.yaml"), mode="once"):
         packages = list(pypi_info(distributions, option_simple))
 
     assert isinstance(packages, list)
     assert len(packages) == 1
     pkg = packages[0]
-    assert pkg.info == {"releases": {}}
+    assert pkg.info is None
     current = datetime.now(timezone.utc)
     last_release_at = pkg.last_release_at
     assert current <= last_release_at
 
 
 @pytest.mark.usefixtures("_no_proxy")
 def test_info_pypi_server_invalid_version(tmp_path: Path, option_simple: Options, make_dist: MakeDist) -> None:
@@ -67,15 +71,18 @@
     pkg = packages[0]
     assert pkg.exc is None
     assert pkg.info is not None
     assert "2004b" in pkg.info["releases"]  # this is an invalid version
 
 
 def test_info_pypi_server_timeout(
-    tmp_path: Path, mocker: MockerFixture, option_simple: Options, make_dist: MakeDist
+    tmp_path: Path,
+    mocker: MockerFixture,
+    option_simple: Options,
+    make_dist: MakeDist,
 ) -> None:
     dist = make_dist(tmp_path, "a", "1.0")
     mock_cached_session = mocker.patch("pypi_changes._info.CachedSession")
     mock_cached_session.return_value.__enter__.return_value.get.side_effect = TimeoutError
 
     packages = list(pypi_info([dist], option_simple))
 
@@ -84,16 +91,16 @@
     pkg = packages[0]
     assert pkg.info is None
     assert isinstance(pkg.exc, TimeoutError)
 
 
 def test_merge_with_pypi() -> None:
     versions = [("2", "sdist"), ("1", "sdist"), (None, None), ("3", "wheel")]
-    packages = [create_autospec(DistributionPackage, spec_set=True, version=v, package_type=t) for v, t in versions]
-    page = create_autospec(ProjectPage, spec_set=True, packages=packages)
+    packages = [create_autospec(DistributionPackage, version=v, package_type=t) for v, t in versions]
+    page = create_autospec(ProjectPage, packages=packages)
     client = create_autospec(PyPISimple, spec_set=True)
     client.get_project_page.return_value = page
 
     start = {"0": [{"packagetype": "sdist", "upload_time_iso_8601": None, "version": "0"}]}
     result = _merge_with_index_server("a", client, start)
     assert result == {
         "0": [{"packagetype": "sdist", "upload_time_iso_8601": None, "version": "0"}],
```

### Comparing `pypi_changes-1.2.0/tests/test_pkg.py` & `pypi_changes-1.2.1/tests/test_pkg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from pypi_changes._pkg import Package
-from tests import MakeDist
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tests import MakeDist
 
 
 def test_ignore_dev_release(make_dist: MakeDist, tmp_path: Path) -> None:
     releases = {"releases": {"1.0.0dev1": [{"version": "1.0.0dev1"}], "0.9.0": [{"version": "0.9.0"}]}}
     pkg = Package(make_dist(tmp_path, "a", "1.0.0"), info=releases)
     assert pkg.last_release == {"version": "0.9.0"}
```

### Comparing `pypi_changes-1.2.0/tests/test_print rich.py` & `pypi_changes-1.2.1/tests/test_print_rich.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 import sys
 from datetime import datetime, timezone
 from pathlib import Path
+from typing import TYPE_CHECKING
 from unittest.mock import create_autospec
 
-from _pytest.capture import CaptureFixture
-from pytest_mock import MockerFixture
-
-from pypi_changes._cli import Options
 from pypi_changes._pkg import Package
 from pypi_changes._print.tree import print_tree
 from tests import PathDistribution
 
+if TYPE_CHECKING:
+    from _pytest.capture import CaptureFixture
+    from pytest_mock import MockerFixture
+
+    from pypi_changes._cli import Options
+
 
 def test_print(capsys: CaptureFixture[str], option_simple: Options, mocker: MockerFixture) -> None:
     mocked_datetime = mocker.patch("pypi_changes._print.tree.datetime")
     mocked_datetime.now.return_value = datetime(2021, 11, 6, 10, tzinfo=timezone.utc)
     option_simple.python = Path(sys.executable)
     option_simple.sort = "updated"
     packages = [
```

### Comparing `pypi_changes-1.2.0/tests/test_print_json.py` & `pypi_changes-1.2.1/tests/test_print_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from __future__ import annotations
 
 import json
 import sys
 from datetime import datetime, timezone
 from pathlib import Path
+from typing import TYPE_CHECKING
 from unittest.mock import create_autospec
 
-from _pytest.capture import CaptureFixture
-from pytest_mock import MockerFixture
-
-from pypi_changes._cli import Options
 from pypi_changes._pkg import Package
 from pypi_changes._print.json import print_json, release_info
 from tests import PathDistribution
 
+if TYPE_CHECKING:
+    from _pytest.capture import CaptureFixture
+    from pytest_mock import MockerFixture
+
+    from pypi_changes._cli import Options
+
 
 def test_print_json(capsys: CaptureFixture[str], option_simple: Options, mocker: MockerFixture) -> None:
     mocked_datetime = mocker.patch("pypi_changes._print.json.datetime")
     mocked_datetime.now.return_value = datetime(2021, 11, 6, 10, tzinfo=timezone.utc)
     option_simple.python = Path(sys.executable)
     option_simple.sort = "unsorted"
     packages = [
         Package(
             create_autospec(PathDistribution, spec_set=True, version=v_cur, metadata={"Name": n}),
             info={
                 "releases": {
                     v_last: [{"version": v_last, "upload_time_iso_8601": t_last}],
                     v_cur: [{"version": v_cur, "upload_time_iso_8601": t_cur}],
-                }
+                },
             },
         )
         for n, (v_last, t_last), (v_cur, t_cur) in [
             (
                 "a",
                 ("2", datetime(2021, 10, 5, 10, tzinfo=timezone.utc)),
                 ("1", datetime(2020, 3, 8, 10, tzinfo=timezone.utc)),
```

### Comparing `pypi_changes-1.2.0/tests/test_pypi_changes.py` & `pypi_changes-1.2.1/tests/test_pypi_changes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from virtualenv import cli_run
 
 from pypi_changes import main
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_pypi_changes_self_output_default(tmp_path: Path) -> None:
     venv = cli_run([str(tmp_path / "venv")], setup_logging=False)
     main([str(venv.creator.exe), "--cache-path", str(tmp_path / "a.sqlite")])
 
 
 def test_pypi_changes_self_output_json(tmp_path: Path) -> None:
```

### Comparing `pypi_changes-1.2.0/tox.ini` & `pypi_changes-1.2.1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
+    py312
+    py311
     py310
     py39
     py38
     py37
     type
     pkg_meta
 skip_missing_interpreters = true
-minversion = 3.22
 
 [testenv]
 description = run the tests with pytest under {envname}
-passenv =
+package = wheel
+wheel_build_env = .pkg
+extras =
+    testing
+pass_env =
     PYTEST_*
     SSL_CERT_FILE
-setenv =
+set_env =
     COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
-    COVERAGE_PROCESS_START = {toxinidir}{/}setup.cfg
-extras =
-    testing
+    COVERAGE_PROCESS_START = {toxinidir}{/}pyproject.toml
 commands =
     pytest {tty:--color=yes} {posargs: --junitxml {toxworkdir}{/}junit.{envname}.xml \
       --cov {envsitepackagesdir}{/}pypi_changes --cov {toxinidir}{/}tests \
-      --cov-config=setup.cfg --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
+      --cov-config=pyproject.toml --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
       --cov-report html:{envtmpdir}{/}htmlcov \
       --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
-passenv =
-    {[testenv]passenv}
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=2.13
+    pre-commit>=3.3.3
+pass_env =
+    {[testenv]passenv}
+    PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure {tty:--color=always} {posargs}
 
 [testenv:type]
 description = run type check on code base
-setenv =
-    {tty:MYPY_FORCE_COLOR = 1}
 deps =
-    mypy==0.930
-    types-requests
+    mypy==1.3
+    types-requests>=2.31.0.1
+set_env =
+    {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy src/pypi_changes
     mypy tests
 
 [testenv:pkg_meta]
 description = check that the long description is valid
 skip_install = true
 deps =
-    build[virtualenv]>=0.7
-    check-wheel-contents>=0.3.2
-    twine>=3.7
+    build[virtualenv]>=0.10
+    check-wheel-contents>=0.4
+    twine>=4.0.2
 commands =
     python -m build -o {envtmpdir} -s -w .
     twine check {envtmpdir}{/}*
     check-wheel-contents --no-config {envtmpdir}
 
 [testenv:docs]
 description = build documentation
@@ -72,23 +75,23 @@
     sphinx-build -d "{envtmpdir}{/}doctree" docs "{toxworkdir}{/}docs_out" --color -b html {posargs}
     python -c 'print(r"documentation available under file://{toxworkdir}{/}docs_out{/}index.html")'
 
 [testenv:release]
 description = do a release, required posarg of the version number
 skip_install = true
 deps =
-    gitpython>=3.1
-    packaging>=21.3
-    towncrier>=21.3
+    gitpython>=3.1.31
+    packaging>=23.1
+    towncrier>=23.6
 commands =
     python {toxinidir}/tasks/release.py --version {posargs}
 
 [testenv:dev]
 description = dev environment with all deps at {envdir}
-usedevelop = true
+package = editable
 deps =
     {[testenv:release]deps}
 extras =
     docs
     testing
 commands =
     python -m pip list --format=columns
```

