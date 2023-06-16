# Comparing `tmp/arosics-1.9.0.tar.gz` & `tmp/arosics-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arosics-1.9.0.tar", last modified: Thu May  4 17:04:02 2023, max compression
+gzip compressed data, was "arosics-1.9.1.tar", last modified: Fri Jun 16 12:52:45 2023, max compression
```

## Comparing `arosics-1.9.0.tar` & `arosics-1.9.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.559054 arosics-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-05-04 17:03:38.000000 arosics-1.9.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-04 17:03:38.000000 arosics-1.9.0/.editorconfig
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.543054 arosics-1.9.0/.github/
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-04 17:03:38.000000 arosics-1.9.0/.github/ISSUE_TEMPLATE.md
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-04 17:03:38.000000 arosics-1.9.0/.github/create_release_from_gitlab_ci.sh
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-05-04 17:03:38.000000 arosics-1.9.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3297 2023-05-04 17:03:38.000000 arosics-1.9.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-04 17:03:38.000000 arosics-1.9.0/.zenodo.json
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-04 17:03:38.000000 arosics-1.9.0/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1882 2023-05-04 17:03:38.000000 arosics-1.9.0/CITATION
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-05-04 17:03:38.000000 arosics-1.9.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    24714 2023-05-04 17:03:38.000000 arosics-1.9.0/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)    10140 2023-05-04 17:03:38.000000 arosics-1.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-04 17:03:38.000000 arosics-1.9.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4118 2023-05-04 17:03:38.000000 arosics-1.9.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     7961 2023-05-04 17:04:02.559054 arosics-1.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6418 2023-05-04 17:03:38.000000 arosics-1.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.547054 arosics-1.9.0/arosics/
--rwxrwxrwx   0 root         (0) root         (0)    86052 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/CoReg.py
--rw-rw-rw-   0 root         (0) root         (0)    42345 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/CoReg_local.py
--rw-rw-rw-   0 root         (0) root         (0)    23187 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/DeShifter.py
--rwxrwxrwx   0 root         (0) root         (0)    70260 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/Tie_Point_Grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    20799 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/arosics_cli.py
--rwxrwxrwx   0 root         (0) root         (0)     6933 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-04 17:03:38.000000 arosics-1.9.0/arosics/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.547054 arosics-1.9.0/arosics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7961 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1807 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 17:04:02.000000 arosics-1.9.0/arosics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.547054 arosics-1.9.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6769 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.539054 arosics-1.9.0/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.539054 arosics-1.9.0/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.551054 arosics-1.9.0/docs/_build/html/_images/
--rw-r--r--   0 root         (0) root         (0)    43518 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/CoregPoints_table.png
--rw-r--r--   0 root         (0) root         (0)   772233 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
--rw-r--r--   0 root         (0) root         (0)     6615 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/arosics_logo.png
--rw-r--r--   0 root         (0) root         (0)   994099 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/output_40_1.png
--rw-r--r--   0 root         (0) root         (0)  1009524 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/output_44_1.png
--rw-r--r--   0 root         (0) root         (0)   297816 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.551054 arosics-1.9.0/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)     6615 2023-05-04 16:56:43.000000 arosics-1.9.0/docs/_build/html/_static/arosics_logo.png
--rw-r--r--   0 root         (0) root         (0)      286 2022-12-02 16:01:28.000000 arosics-1.9.0/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)       90 2022-12-02 16:01:28.000000 arosics-1.9.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2022-12-02 16:01:28.000000 arosics-1.9.0/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.551054 arosics-1.9.0/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/about.rst
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/api_cli_reference.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/cli_reference.rst
--rwxrwxrwx   0 root         (0) root         (0)     9929 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.559054 arosics-1.9.0/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)    43518 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/CoregPoints_table.png
--rw-rw-rw-   0 root         (0) root         (0)   954684 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif
--rw-rw-rw-   0 root         (0) root         (0)   772233 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
--rw-rw-rw-   0 root         (0) root         (0)     6615 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/arosics_logo.png
--rw-rw-rw-   0 root         (0) root         (0)   994099 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/output_40_1.png
--rw-rw-rw-   0 root         (0) root         (0)  1009524 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/output_44_1.png
--rw-rw-rw-   0 root         (0) root         (0)   297816 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/images/shift_vectors_testcase1__900x824.gif
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     6461 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:04:02.559054 arosics-1.9.0/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)    10547 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage/global_coreg.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage/input_data_requirements.rst
--rw-rw-rw-   0 root         (0) root         (0)     7859 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage/local_coreg.rst
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-04 17:03:38.000000 arosics-1.9.0/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-04 17:03:38.000000 arosics-1.9.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-05-04 17:04:02.559054 arosics-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4158 2023-05-04 17:03:38.000000 arosics-1.9.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-04 17:03:39.000000 arosics-1.9.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.883398 arosics-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-06-16 12:52:23.000000 arosics-1.9.1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-16 12:52:23.000000 arosics-1.9.1/.editorconfig
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.863400 arosics-1.9.1/.github/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-16 12:52:23.000000 arosics-1.9.1/.github/ISSUE_TEMPLATE.md
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-06-16 12:52:23.000000 arosics-1.9.1/.github/create_release_from_gitlab_ci.sh
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-16 12:52:23.000000 arosics-1.9.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3188 2023-06-16 12:52:23.000000 arosics-1.9.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-16 12:52:23.000000 arosics-1.9.1/.zenodo.json
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-16 12:52:23.000000 arosics-1.9.1/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2023-06-16 12:52:23.000000 arosics-1.9.1/CITATION
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-06-16 12:52:23.000000 arosics-1.9.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    25034 2023-06-16 12:52:23.000000 arosics-1.9.1/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10140 2023-06-16 12:52:23.000000 arosics-1.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-16 12:52:23.000000 arosics-1.9.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4118 2023-06-16 12:52:23.000000 arosics-1.9.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7961 2023-06-16 12:52:45.883398 arosics-1.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6418 2023-06-16 12:52:23.000000 arosics-1.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.867399 arosics-1.9.1/arosics/
+-rwxrwxrwx   0 root         (0) root         (0)    86052 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/CoReg.py
+-rw-rw-rw-   0 root         (0) root         (0)    42345 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/CoReg_local.py
+-rw-rw-rw-   0 root         (0) root         (0)    23187 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/DeShifter.py
+-rwxrwxrwx   0 root         (0) root         (0)    70325 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/Tie_Point_Grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20799 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/arosics_cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     6933 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-06-16 12:52:23.000000 arosics-1.9.1/arosics/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.867399 arosics-1.9.1/arosics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7961 2023-06-16 12:52:45.000000 arosics-1.9.1/arosics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-06-16 12:52:45.000000 arosics-1.9.1/arosics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:52:45.000000 arosics-1.9.1/arosics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-16 12:52:45.000000 arosics-1.9.1/arosics.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:52:45.000000 arosics-1.9.1/arosics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-16 12:52:45.000000 arosics-1.9.1/arosics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-16 12:52:45.000000 arosics-1.9.1/arosics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.871399 arosics-1.9.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6769 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.859400 arosics-1.9.1/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.863400 arosics-1.9.1/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.875399 arosics-1.9.1/docs/_build/html/_images/
+-rw-r--r--   0 root         (0) root         (0)    43518 2023-06-16 12:48:04.000000 arosics-1.9.1/docs/_build/html/_images/CoregPoints_table.png
+-rw-r--r--   0 root         (0) root         (0)   772233 2023-06-16 12:48:04.000000 arosics-1.9.1/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-06-16 12:48:04.000000 arosics-1.9.1/docs/_build/html/_images/arosics_logo.png
+-rw-r--r--   0 root         (0) root         (0)   994099 2023-06-16 12:48:04.000000 arosics-1.9.1/docs/_build/html/_images/output_40_1.png
+-rw-r--r--   0 root         (0) root         (0)  1009524 2023-06-16 12:48:04.000000 arosics-1.9.1/docs/_build/html/_images/output_44_1.png
+-rw-r--r--   0 root         (0) root         (0)   297816 2023-06-16 12:48:04.000000 arosics-1.9.1/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.875399 arosics-1.9.1/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-06-16 12:48:04.000000 arosics-1.9.1/docs/_build/html/_static/arosics_logo.png
+-rw-r--r--   0 root         (0) root         (0)      286 2022-10-16 10:21:34.000000 arosics-1.9.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)       90 2022-10-16 10:21:34.000000 arosics-1.9.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2022-10-16 10:21:34.000000 arosics-1.9.1/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.875399 arosics-1.9.1/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/about.rst
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/api_cli_reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/cli_reference.rst
+-rwxrwxrwx   0 root         (0) root         (0)     9929 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.879399 arosics-1.9.1/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)    43518 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/images/CoregPoints_table.png
+-rw-rw-rw-   0 root         (0) root         (0)   954684 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif
+-rw-rw-rw-   0 root         (0) root         (0)   772233 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+-rw-rw-rw-   0 root         (0) root         (0)     6615 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/images/arosics_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)   994099 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/images/output_40_1.png
+-rw-rw-rw-   0 root         (0) root         (0)  1009524 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/images/output_44_1.png
+-rw-rw-rw-   0 root         (0) root         (0)   297816 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/images/shift_vectors_testcase1__900x824.gif
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:52:45.883398 arosics-1.9.1/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)    10547 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/usage/global_coreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/usage/input_data_requirements.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/usage/local_coreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-16 12:52:23.000000 arosics-1.9.1/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-16 12:52:23.000000 arosics-1.9.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-16 12:52:45.883398 arosics-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4146 2023-06-16 12:52:23.000000 arosics-1.9.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-16 12:52:24.000000 arosics-1.9.1/tox.ini
```

### Comparing `arosics-1.9.0/.coveragerc` & `arosics-1.9.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/.github/create_release_from_gitlab_ci.sh` & `arosics-1.9.1/.github/create_release_from_gitlab_ci.sh`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/.gitignore` & `arosics-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/.gitlab-ci.yml` & `arosics-1.9.1/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,18 @@
   - cleanup
 
 
 test_arosics:
   stage: test
   coverage: '/TOTAL\s+\d+\s+\d+\s+(\d+%)/'
   script:
-    - source /opt/conda/bin/activate ci_env
+    - source activate ci_env
 
     # update py_tools_ds and geoarray
-    - pip install -U py_tools_ds -q
-    - pip install -U geoarray -q
-
-    - pip install scipy  # TODO remove as soon as CI runner is rebuilt
+    - mamba update py-tools-ds geoarray
 
     # run tests
     - make pytest
 
     # create the docs
     - make docs
   artifacts:
@@ -40,52 +37,55 @@
     expire_in: 30 days
     when: always
 
 
 test_styles:
   stage: test
   script:
-    - source /opt/conda/bin/activate ci_env
+    - source activate ci_env
     - make lint
   artifacts:
     paths:
     - tests/linting/flake8.log
     - tests/linting/pycodestyle.log
     - tests/linting/pydocstyle.log
     when: always
 
 
 test_urls:
   stage: test
   script:
-    - source /opt/conda/bin/activate ci_env
+    - source activate ci_env
     - pip install -U urlchecker
     - make urlcheck
   when: always
 
 
 test_arosics_install:
   stage: test
   script:
-    - source /opt/conda/bin/activate
-    - mamba update -n base -c conda-forge --all
+    - source activate
+    - mamba update -n base mamba conda
 
     # create arosics environment from environment_arosics.yml
     - mamba env create --name arosics_test -f tests/CI_docker/context/environment_arosics.yml
     - conda activate arosics_test
 
     # install arosics
     - pip install -e .
     - cd ..
     - pwd
     - ls
 
     # test importability
     - python -c "import arosics; print(arosics)"
     - python -c "from arosics import COREG, COREG_LOCAL"
+
+    # check if dependencies are properly installed
+    - pip check || exit
   only:
     - main
 
 
 pages:  # this job must be called 'pages' to advise GitLab to upload content to GitLab Pages
   stage: deploy
   dependencies:
@@ -124,15 +124,15 @@
 
 
 deploy_pypi:
   stage: deploy
   dependencies:
     - test_arosics
   script:
-    - source /opt/conda/bin/activate ci_env
+    - source activate ci_env
     - pip install -U twine
     - python setup.py sdist
     - twine upload dist/*  # requires creds as environment variables
   only:
     - /^v\d+\.\d+\.\d+([abc]\d*)?$/  # PEP-440 compliant version (tags)
   except:
     - dev
```

### Comparing `arosics-1.9.0/.zenodo.json` & `arosics-1.9.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/CITATION` & `arosics-1.9.1/CITATION`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/CONTRIBUTING.rst` & `arosics-1.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/HISTORY.rst` & `arosics-1.9.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+1.9.1 (2023-06-16)
+------------------
+
+* Removed dill from requirements.
+* !37: Fixed issue #82 (IndexError: cannot do a non-empty take from an empty axes) which happened in case COREG_LOCAL
+  could not find a single tie point.
+* !38: Updated CI (now faster) and environment file (now uses conda where ever possible).
+
+
 1.9.0 (2023-05-04)
 ------------------
 
 * Re-implemented interpolation of tie point attributes into space (!23).
   Three techniques are now supported: RBF, GPR, and Ordinary Kriging. Added scikit-learn to dependencies.
 * Fixed GDAL warning related to PROJ_DATA/PROJ_LIB environment variables (!34).
 * Added parameter 'rs_random_state' (RANSAC random state) and set it to 0 by default (!35).
```

### Comparing `arosics-1.9.0/LICENSE` & `arosics-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/Makefile` & `arosics-1.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/PKG-INFO` & `arosics-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arosics
-Version: 1.9.0
+Version: 1.9.1
 Summary: An Automated and Robust Open-Source Image Co-Registration Software for Multi-Sensor Satellite Data
 Home-page: https://git.gfz-potsdam.de/danschef/arosics
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: Apache-2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/danschef/arosics
 Project-URL: Issue Tracker, https://git.gfz-potsdam.de/danschef/arosics/-/issues
```

### Comparing `arosics-1.9.0/README.rst` & `arosics-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/CoReg.py` & `arosics-1.9.1/arosics/CoReg.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/CoReg_local.py` & `arosics-1.9.1/arosics/CoReg_local.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/DeShifter.py` & `arosics-1.9.1/arosics/DeShifter.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/Tie_Point_Grid.py` & `arosics-1.9.1/arosics/Tie_Point_Grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,31 +431,33 @@
                                      'SSIM_IMPROVED', 'RELIABILITY', 'LAST_ERR'])
 
         # merge DataFrames (dtype must be equal to records.dtypes; We need np.object due to None values)
         GDF = GDF.astype(object).merge(records.astype(object), on='POINT_ID', how="inner")
         GDF = GDF.replace([np.nan, None], int(self.outFillVal))  # fillna fails with geopandas==0.6.0
         GDF.crs = crs  # gets lost when using GDF.astype(np.object), so we have to reassign that
 
+        n_matches = len(GDF[GDF.LAST_ERR == int(self.outFillVal)])
+
         if not self.q:
-            print("Found %s matches." % len(GDF[GDF.LAST_ERR == int(self.outFillVal)]))
+            print(f"Found {n_matches} matches.")
 
         # filter tie points according to given filter level
-        if self.tieP_filter_level > 0:
+        if n_matches > 0 and self.tieP_filter_level > 0:
             if not self.q:
                 print('Performing validity checks...')
             TPR = Tie_Point_Refiner(GDF[GDF.ABS_SHIFT != self.outFillVal], **self.outlDetect_settings)
             GDF_filt, new_columns = TPR.run_filtering(level=self.tieP_filter_level)
             GDF = GDF.merge(GDF_filt[['POINT_ID'] + new_columns], on='POINT_ID', how="outer")
 
         GDF = GDF.replace([np.nan, None], int(self.outFillVal))  # fillna fails with geopandas==0.6.0
 
         self.CoRegPoints_table = GDF
 
         if not self.q:
-            if GDF.empty:
+            if n_matches == 0 or GDF.empty:
                 warnings.warn('No valid GCPs could by identified.')
             else:
                 if self.tieP_filter_level > 0:
                     print("%d valid tie points remain after filtering." % len(GDF[GDF.OUTLIER.__eq__(False)]))
 
         return self.CoRegPoints_table
```

### Comparing `arosics-1.9.0/arosics/__init__.py` & `arosics-1.9.1/arosics/__init__.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/arosics_cli.py` & `arosics-1.9.1/arosics/arosics_cli.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/geometry.py` & `arosics-1.9.1/arosics/geometry.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/plotting.py` & `arosics-1.9.1/arosics/plotting.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics/version.py` & `arosics-1.9.1/arosics/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.9.0'
-__versionalias__ = '2023-05-04_01'
+__version__ = '1.9.1'
+__versionalias__ = '2023-06-16_01'
```

### Comparing `arosics-1.9.0/arosics.egg-info/PKG-INFO` & `arosics-1.9.1/arosics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arosics
-Version: 1.9.0
+Version: 1.9.1
 Summary: An Automated and Robust Open-Source Image Co-Registration Software for Multi-Sensor Satellite Data
 Home-page: https://git.gfz-potsdam.de/danschef/arosics
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: Apache-2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/danschef/arosics
 Project-URL: Issue Tracker, https://git.gfz-potsdam.de/danschef/arosics/-/issues
```

### Comparing `arosics-1.9.0/arosics.egg-info/SOURCES.txt` & `arosics-1.9.1/arosics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/arosics.egg-info/requires.txt` & `arosics-1.9.1/arosics.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 cartopy
 cmocean
-dill
 folium!=0.12.0,>=0.6.0
 gdal
-geojson
 geoarray>=0.15.0
+geojson
 geopandas
 matplotlib
 numpy
 packaging
 pandas
 plotly
 pyfftw
```

### Comparing `arosics-1.9.0/docs/Makefile` & `arosics-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/_build/html/_images/CoregPoints_table.png` & `arosics-1.9.1/docs/_build/html/_images/CoregPoints_table.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif` & `arosics-1.9.1/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/_build/html/_images/arosics_logo.png` & `arosics-1.9.1/docs/_build/html/_images/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/_build/html/_images/output_40_1.png` & `arosics-1.9.1/docs/_build/html/_images/output_40_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/_build/html/_images/output_44_1.png` & `arosics-1.9.1/docs/_build/html/_images/output_44_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif` & `arosics-1.9.1/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/_build/html/_static/arosics_logo.png` & `arosics-1.9.1/docs/_build/html/_static/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/about.rst` & `arosics-1.9.1/docs/about.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/cli_reference.rst` & `arosics-1.9.1/docs/cli_reference.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/conf.py` & `arosics-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/images/CoregPoints_table.png` & `arosics-1.9.1/docs/images/CoregPoints_table.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif` & `arosics-1.9.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif` & `arosics-1.9.1/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/images/arosics_logo.png` & `arosics-1.9.1/docs/images/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/images/output_40_1.png` & `arosics-1.9.1/docs/images/output_40_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/images/output_44_1.png` & `arosics-1.9.1/docs/images/output_44_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/images/shift_vectors_testcase1__900x824.gif` & `arosics-1.9.1/docs/images/shift_vectors_testcase1__900x824.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/installation.rst` & `arosics-1.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/make.bat` & `arosics-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/usage/global_coreg.rst` & `arosics-1.9.1/docs/usage/global_coreg.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/usage/input_data_requirements.rst` & `arosics-1.9.1/docs/usage/input_data_requirements.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/usage/local_coreg.rst` & `arosics-1.9.1/docs/usage/local_coreg.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/docs/usage.rst` & `arosics-1.9.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.0/setup.py` & `arosics-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,18 @@
 version = {}
 with open("arosics/version.py") as version_file:
     exec(version_file.read(), version)
 
 req = [
     'cartopy',
     'cmocean',
-    'dill',
     'folium>=0.6.0,!=0.12.0',
     'gdal',
-    'geojson',
     'geoarray>=0.15.0',
+    'geojson',
     'geopandas',
     'matplotlib',
     'numpy',
     'packaging',
     'pandas',
     'plotly',
     'pyfftw',
```

