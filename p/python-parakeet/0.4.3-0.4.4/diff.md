# Comparing `tmp/python-parakeet-0.4.3.tar.gz` & `tmp/python-parakeet-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-parakeet-0.4.3.tar", last modified: Thu Jan 19 17:30:51 2023, max compression
+gzip compressed data, was "python-parakeet-0.4.4.tar", last modified: Fri Jun 16 11:31:50 2023, max compression
```

## Comparing `python-parakeet-0.4.3.tar` & `python-parakeet-0.4.4.tar`

### file list

```diff
@@ -1,416 +1,427 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.032940 python-parakeet-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.956940 python-parakeet-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.github/workflows/conda.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.github/workflows/quay-io-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.github/workflows/snapcraft.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-01-19 17:30:51.032940 python-parakeet-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/conda/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/configuration.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/docs/source/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/ext/pydantic_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   153379 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/images/parakeet.png
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/images/parakeet_small.png
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/publications.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.cmake-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-19 17:30:26.000000 python-parakeet-0.4.3/pybind11/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.960940 python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/labeler_merged.yml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.964939 python-parakeet-0.4.3/pybind11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.964939 python-parakeet-0.4.3/pybind11/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.964939 python-parakeet-0.4.3/pybind11/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.964939 python-parakeet-0.4.3/pybind11/docs/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.964939 python-parakeet-0.4.3/pybind11/docs/advanced/cast/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.968939 python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)    74047 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/classes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.968939 python-parakeet-0.4.3/pybind11/docs/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/cmake/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/compiling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    58510 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.956940 python-parakeet-0.4.3/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.968939 python-parakeet-0.4.3/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    57522 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.968939 python-parakeet-0.4.3/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    42083 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    29086 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    69754 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   105769 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    67597 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.968939 python-parakeet-0.4.3/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pybind11/setup_helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.976940 python-parakeet-0.4.3/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/constructor_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.976940 python-parakeet-0.4.3/pybind11/tests/extra_python_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.976940 python-parakeet-0.4.3/pybind11/tests/extra_setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/local_bindings.h
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_async.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_call_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_class.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_copy_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_eval_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16731 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_iostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_modules.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_stl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_union.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-19 17:30:27.000000 python-parakeet-0.4.3/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-01-19 17:30:51.032940 python-parakeet-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/snap/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.956940 python-parakeet-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.980939 python-parakeet-0.4.3/src/parakeet/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-19 17:30:50.000000 python-parakeet-0.4.3/src/parakeet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/analyse/_average_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/analyse/_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/analyse/_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/analyse/_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/analyse/_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/beam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/command_line/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/command_line/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/analyse/_average_all_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/analyse/_average_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/analyse/_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/analyse/_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/analyse/_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/analyse/_refine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/command_line/config/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/config/_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/config/_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/config/_show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/command_line/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/metadata/_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/command_line/pdb/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/pdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/pdb/_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/pdb/_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/command_line/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/sample/_add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/sample/_mill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/sample/_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/sample/_show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/sample/_sputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/command_line/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/simulate/_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/simulate/_exit_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/simulate/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/simulate/_optics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/simulate/_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/command_line/simulate/_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:50.984940 python-parakeet-0.4.3/src/parakeet/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.028940 python-parakeet-0.4.3/src/parakeet/data/files/
--rw-r--r--   0 runner    (1001) docker     (123)  6040922 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/data/files/3jb9.cif
--rw-r--r--   0 runner    (1001) docker     (123)  3095859 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/data/files/4v1w.cif
--rw-r--r--   0 runner    (1001) docker     (123) 18908004 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/data/files/4v5d.cif
--rw-r--r--   0 runner    (1001) docker     (123)  7821805 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/data/files/6qt9.cif
--rw-r--r--   0 runner    (1001) docker     (123)  2781544 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/data/files/6z6u.pdb
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/data/files/water.cif
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/dqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/error.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.028940 python-parakeet-0.4.3/src/parakeet/freeze/
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/freeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/freeze/freeze_ext.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/freeze/sphere_packer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/inelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24853 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/landau.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/lens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/microscope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.028940 python-parakeet-0.4.3/src/parakeet/sample/
--rw-r--r--   0 runner    (1001) docker     (123)    56317 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/sample/_add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/sample/_mill.py
--rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/sample/_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/sample/_sputter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/sample/distribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.028940 python-parakeet-0.4.3/src/parakeet/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/_exit_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    19043 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/_optics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/simulate/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.028940 python-parakeet-0.4.3/src/parakeet/util/
--rw-r--r--   0 runner    (1001) docker     (123)    35630 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/src/parakeet/util/calibrate_ice_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.028940 python-parakeet-0.4.3/src/python_parakeet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-01-19 17:30:50.000000 python-parakeet-0.4.3/src/python_parakeet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-01-19 17:30:50.000000 python-parakeet-0.4.3/src/python_parakeet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 17:30:50.000000 python-parakeet-0.4.3/src/python_parakeet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-01-19 17:30:50.000000 python-parakeet-0.4.3/src/python_parakeet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-19 17:30:50.000000 python-parakeet-0.4.3/src/python_parakeet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-19 17:30:50.000000 python-parakeet-0.4.3/src/python_parakeet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:30:51.032940 python-parakeet-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_beam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_inelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_landau.py
--rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_sample_distribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-01-19 17:30:25.000000 python-parakeet-0.4.3/tests/test_sphere_packer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.069758 python-parakeet-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/quay-io-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/snapcraft.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/conda/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/docs/source/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/ext/pydantic_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   153379 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/images/parakeet.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50471 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/images/parakeet_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/images/parakeet_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/publications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/39.feature
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/44.doc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/50.feature
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/newsfragments/51.feature
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.cmake-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/pybind11/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/labeler_merged.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.077758 python-parakeet-0.4.4/pybind11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/advanced/cast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    74047 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.081758 python-parakeet-0.4.4/pybind11/docs/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/compiling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    58510 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.069758 python-parakeet-0.4.4/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.089758 python-parakeet-0.4.4/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57522 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.089758 python-parakeet-0.4.4/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42083 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29086 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69754 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105769 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67597 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.089758 python-parakeet-0.4.4/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/local_bindings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_class.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.105759 python-parakeet-0.4.4/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16731 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-16 11:31:26.000000 python-parakeet-0.4.4/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.073758 python-parakeet-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/src/parakeet/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/parakeet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/src/parakeet/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_average_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/analyse/_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/beam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.109758 python-parakeet-0.4.4/src/parakeet/command_line/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_all_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/analyse/_refine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/config/_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/metadata/_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/pdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/pdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/pdb/_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/pdb/_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_mill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/sample/_sputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/command_line/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_cbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_exit_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_optics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/command_line/simulate/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.113758 python-parakeet-0.4.4/src/parakeet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.149759 python-parakeet-0.4.4/src/parakeet/data/files/
+-rw-r--r--   0 runner    (1001) docker     (123)  6040922 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/3jb9.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  3095859 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/4v1w.cif
+-rw-r--r--   0 runner    (1001) docker     (123) 18908004 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/4v5d.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  7821805 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/6qt9.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  2781544 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/6z6u.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/data/files/water.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/dqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/error.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.149759 python-parakeet-0.4.4/src/parakeet/freeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/freeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/freeze/freeze_ext.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/freeze/sphere_packer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/inelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25723 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/landau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/microscope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.149759 python-parakeet-0.4.4/src/parakeet/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)    57480 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_mill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/_sputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/sample/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25109 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/src/parakeet/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_cbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_exit_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_optics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/phase_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/simulate/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/src/parakeet/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    37870 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/src/parakeet/util/calibrate_ice_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/src/python_parakeet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-16 11:31:50.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 11:31:49.000000 python-parakeet-0.4.4/src/python_parakeet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:31:50.153759 python-parakeet-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_beam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_inelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_landau.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_sample_distribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-16 11:31:24.000000 python-parakeet-0.4.4/tests/test_sphere_packer.py
```

### Comparing `python-parakeet-0.4.3/.github/workflows/conda.yml` & `python-parakeet-0.4.4/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/.github/workflows/docker-publish.yml` & `python-parakeet-0.4.4/.github/workflows/docker-publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
       - name: Checkout repository
         uses: actions/checkout@v3
 
       # Install the cosign tool except on PR
       # https://github.com/sigstore/cosign-installer
       - name: Install cosign
         if: github.event_name != 'pull_request'
-        uses: sigstore/cosign-installer@main
+        uses: sigstore/cosign-installer@f3c664df7af409cb4873aa5068053ba9d61a57b6
+        with:
+          cosign-release: 'v1.13.1'
 
 
       # Workaround: https://github.com/docker/build-push-action/issues/461
       - name: Setup Docker buildx
         uses: docker/setup-buildx-action@79abd3f86f79a9d68a23c75a09a9a85889262adf
 
       # Login against a Docker registry except on PR
```

### Comparing `python-parakeet-0.4.3/.github/workflows/python-package.yml` & `python-parakeet-0.4.4/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -56,11 +56,11 @@
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Check typing with mypy
       run: |
-        mypy src/ tests/ --ignore-missing --implicit-optional
+        mypy src/ tests/ 
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `python-parakeet-0.4.3/.github/workflows/python-publish.yml` & `python-parakeet-0.4.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/.github/workflows/quay-io-publish.yml` & `python-parakeet-0.4.4/.github/workflows/quay-io-publish.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/.github/workflows/snapcraft.yml` & `python-parakeet-0.4.4/.github/workflows/snapcraft.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/.github/workflows/sphinx.yml` & `python-parakeet-0.4.4/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/.gitignore` & `python-parakeet-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/.pre-commit-config.yaml` & `python-parakeet-0.4.4/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 repos:
 -   repo: https://github.com/ambv/black
-    rev: 22.12.0
+    rev: 23.1.0
     hooks:
     - id: black
       args: [--safe]
       language_version: python3
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.1.0
     hooks:
     - id: flake8
       args: ['--max-line-length=88', '--select=W291,W292,W293,F401']
       language_version: python3
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: 'v0.991'
     hooks:
     -   id: mypy
-        args: [--ignore-missing-imports, --implicit-optional]
-        additional_dependencies: [ types-PyYAML ]
+        args: []
+        additional_dependencies: [ types-PyYAML, pydantic ]
         exclude: docs
```

### Comparing `python-parakeet-0.4.3/CMakeLists.txt` & `python-parakeet-0.4.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/LICENSE` & `python-parakeet-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/README.md` & `python-parakeet-0.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 <div align="center">
 
-# Parakeet :parrot:
-
-![Parakeet](docs/source/images/parakeet_small.png)
+![Parakeet :parrot:](docs/source/images/parakeet_logo.png)
 
 > **Parakeet** is a digital twin for cryo electron tomography and stands for **P**rogram for **A**nalysis and **R**econstruction of **A**rtificial data for **K**ryo **E**l**E**ctron **T**omography
 
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/rosalindfranklininstitute/parakeet.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/rosalindfranklininstitute/parakeet/context:python)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/rosalindfranklininstitute/parakeet.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/rosalindfranklininstitute/parakeet/alerts/)
-
 [![PyPI version shields.io](https://img.shields.io/pypi/v/python-parakeet.svg)](https://pypi.python.org/pypi/python-parakeet/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/python-parakeet.svg)](https://pypi.python.org/pypi/python-parakeet/)
 [![PyPI download month](https://img.shields.io/pypi/dm/python-parakeet.svg)](https://pypi.python.org/pypi/python-parakeet/)
 
 [![Building](https://github.com/rosalindfranklininstitute/parakeet/actions/workflows/python-package.yml/badge.svg)](https://github.com/rosalindfranklininstitute/parakeet/actions/workflows/python-package.yml)
 [![Publishing](https://github.com/rosalindfranklininstitute/parakeet/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rosalindfranklininstitute/parakeet/actions/workflows/python-publish.yml)
 
@@ -70,13 +65,17 @@
 You can receive notifications from the [Github discussions](https://github.com/rosalindfranklininstitute/parakeet/discussions)
 by clicking "watch" on this repository.
 
 ## Issues
 
 Please use the [GitHub issue tracker](https://github.com/rosalindfranklininstitute/parakeet/issues) to submit bugs or request features.
 
+## Changes
+
+Checkout the [changelog](CHANGES.rst) for a list of recent changes to parakeet.
+
 ## License
 
 Copyright Diamond Light Source and Rosalind Franklin Institute, 2019.
 
 Distributed under the terms of the GPLv3 license, parakeet is free and open source software.
```

### Comparing `python-parakeet-0.4.3/conda/meta.yaml` & `python-parakeet-0.4.4/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/Makefile` & `python-parakeet-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/make.bat` & `python-parakeet-0.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/source/conf.py` & `python-parakeet-0.4.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/source/configuration.rst` & `python-parakeet-0.4.4/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/source/ext/pydantic_settings.py` & `python-parakeet-0.4.4/docs/source/ext/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/source/images/parakeet.png` & `python-parakeet-0.4.4/docs/source/images/parakeet.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/source/images/parakeet_small.png` & `python-parakeet-0.4.4/docs/source/images/parakeet_small.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/source/index.rst` & `python-parakeet-0.4.4/docs/source/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    sphinx-quickstart on Fri Feb 25 09:31:39 2022.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to parakeet's documentation!
 ====================================
 
-.. image:: images/parakeet.png
+.. image:: images/parakeet_logo.png
    :width: 300
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    installation
```

### Comparing `python-parakeet-0.4.3/docs/source/installation.rst` & `python-parakeet-0.4.4/docs/source/installation.rst`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - A C++ compiler (e.g. g++)
 - FFTW
 - Python development libraries
 - The CUDA toolkit
 
 On ubuntu 20.04, the dependencies can be install on a clean install as follows
 (you may need to contact your system administrator if you do not have admin
-priviliges):
+privileges):
 
 
 .. code-block:: bash
   
   # Install GCC
   sudo apt-get install build-essential
   
@@ -32,15 +32,15 @@
   wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/cuda-ubuntu2004.pin
   sudo mv cuda-ubuntu2004.pin /etc/apt/preferences.d/cuda-repository-pin-600
   sudo apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/3bf863cc.pub
   sudo add-apt-repository "deb https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2004/x86_64/ /"
   sudo apt-get update
   sudo apt-get -y install cuda
 
-Enviornment variables
+Environment variables
 ---------------------
 
 If you have multiple compiler versions or the compilers you want to use are not
 automatically picked up by cmake, you can explicitly state the compiler
 versions you would like to use as follows, where in this case we are using gcc
 as the C++ compiler:
 
@@ -50,15 +50,15 @@
   export CUDACXX=/usr/local/cuda-11/bin/nvcc
   export FFTWDIR=/usr/local/
 
 Depending on your GPU and the version of the CUDA toolkit you are using, it may
 also be necessary to set the CMAKE_CUDA_ARCHITECTURES variable. This variable
 is by default set to "OFF" in the CMakeLists.txt file which has the effect of
 compiling CUDA kernels on the fly. If you have an old GPU, this may not work
-and you will receive CUDA errors when attemping to run the simulations on the
+and you will receive CUDA errors when attempting to run the simulations on the
 GPU. In this case simply set the variable to the architecture supported by your
 GPU as follows (the example below is for the compute_37 architecture):
 
 .. code-block:: bash
   
   export CMAKE_CUDA_ARCHITECTURES=37
 
@@ -152,61 +152,93 @@
   # Install parakeet
   conda install -c conda-forge -c james.parkhurst python-parakeet
 
 
 Install as a Docker container
 -----------------------------
 
-Parakeet can also be installed and used via Docker
-(https://www.docker.com/get-started). To download parakeet's docker container
-you can do the following:
+Parakeet can also be run via Docker
+(https://www.docker.com/get-started). To pull the docker container with the latest version
+parakeet, you can do the following:
 
 .. code-block:: bash
   
-  docker pull ghcr.io/rosalindfranklininstitute/parakeet:master
+  docker pull quay.io/rosalindfranklininstitute/parakeet:latest
+
+You may also pull the docker container of a specific version of parakeet. To do this in the above
+command replace the 'latest' with one of the tags that you can find here
+( https://quay.io/repository/rosalindfranklininstitute/parakeet?tab=tags).
 
 To use parakeet with docker with GPU support the host machine should have the
-approprate Nvidia drivers installed and docker needs to be installed with the
+appropriate Nvidia drivers installed and docker needs to be installed with the
 nvidia container toolkit
 (https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html).
 
 To easily input and output data from the container the volume mechanism can be
 used, where a workspace directory of the host machine is mounted to a directory
 in the container (in the folder /mnt in the example below). For this reason it
-is advised that all the relevent files (e.g. config.yaml, sample.h5, etc.)
+is advised that all the relevant files (e.g. config.yaml, sample.h5, etc.)
 should be present in the host workspace directory.
 
-Below is an example on how to use parakeet with docker to run parakeet commands:
+Below is an example on how to use parakeet after, its docker image has been pulled, to run parakeet commands:
 
 .. code-block:: bash
 
-  docker run --gpus all -v $(pwd):/mnt --workdir=/mnt parakeet:master \
-    parakeet.config.new 
+  docker run --gpus all -v $(pwd):/mnt --workdir=/mnt parakeet:latest \
+    parakeet.config.new
+
+You may also pull and run parakeet with a single command.
+
+.. code-block:: bash
+
+  docker run --gpus all -v $(pwd):/mnt --workdir=/mnt \
+    quay.io/rosalindfranklininstitute/parakeet:latest parakeet.config.new
 
 
 Install as a Singularity image
 ------------------------------
 
-Parakeet can also be installed and used via Singularity
-(https://sylabs.io/guides/2.6/user-guide/installation.html). To download
+Parakeet can also be run via Singularity
+(https://sylabs.io/guides/2.6/user-guide/installation.html). To build
 parakeet's singularity container you can do the following:
 
 .. code-block:: bash
 
-  singularity build parakeet.sif docker://ghcr.io/rosalindfranklininstitute/parakeet:master
+  singularity build parakeet.sif docker://quay.io/rosalindfranklininstitute/parakeet:latest
+
+Again similar to docker, you may build the singularity container of a specific version of parakeet
+by replacing the 'latest' in the command above with one of the tags that you can find here
+( https://quay.io/repository/rosalindfranklininstitute/parakeet?tab=tags).
+
+Also like with docker, to use parakeet with singularity and GPU support, the
+host machine should have the appropriate Nvidia drivers installed.
+
+Below is an example on how to use parakeet, after its singularity image has been build, to run parakeet commands:
+
+.. code-block:: bash
+
+  # You can open an interactive shell in the singularity container like this:
+  singularity shell --nv --bind=/data/directory:/mnt --pwd=/mnt parakeet.sif
 
-Again similar to docker, to use parakeet with singularity and GPU support, the
-host machine should have the approprate Nvidia drivers installed.
+  # Or you can execute multiple commands
+  singularity exec --nv --bind=/data/directory:/mnt --pwd=/mnt parakeet.sif \
+    bash -c "parakeet.config.new && parakeet.sample.new"
 
-Below is an example on how to use parakeet with singularity to run parakeet commands:
+You may also build and run parakeet with a single command.
 
 .. code-block:: bash
 
-  singularity run --nv parakeet.sif \
-    parakeet.config.new
+  # You can open an interactive shell in the singularity container like this:
+  singularity shell --nv --bind=/data/directory:/mnt --pwd=/mnt \
+    docker://quay.io/rosalindfranklininstitute/parakeet:latest
+
+  # Or you can execute multiple commands
+  singularity exec --nv --bind=/data/directory:/mnt --pwd=/mnt \
+    docker://quay.io/rosalindfranklininstitute/parakeet:latest \
+    bash -c "parakeet.config.new && parakeet.sample.new"
 
 
 Install as Singularity sandbox
 ------------------------------
 
 If you need to modify the singularity container for development purposes, it is
 possible to build a parakeet sandbox as follows:
@@ -249,15 +281,15 @@
 
 You can build a new container depending on the parakeet docker container as
 follows. In your python source code repository create a file called Dockerfile
 with the following contents:
 
 .. code-block:: bash
 
-  FROM ghcr.io/rosalindfranklininstitute/parakeet:master
+  FROM quay.io/rosalindfranklininstitute/parakeet:latest
 
   WORKDIR /myapp
   COPY . .
 
   RUN apt update
   RUN git submodule update --init --recursive
   RUN pip install .
@@ -268,15 +300,28 @@
 
   sudo docker build . -t me/myapp
 
 Now we can build the singularity image from the docker image
 
 .. code-block:: bash
 
-  singularity build myapp.sif docker-deamon://me/myapp:latest
+  singularity build myapp.sif docker-daemon://me/myapp:latest
+
+
+Install as a Apptainer image
+------------------------------
+
+Parakeet can also be run via Apptainer. Apptainer is the new name for the Singularity
+project after is official move to the Linux Foundation
+(https://apptainer.org/news/community-announcement-20211130/).
+
+You may build and run parakeet via an Apptainer container the same way you would
+build and run parakeet via an Singularity container, but instead of the command
+'singularity' the command 'apptainer' should be used. The arguments of the command
+'apptainer' is the exact same with the command 'singularity'.
 
 
 Install as a snap
 -----------------
 
 You can install the parakeet snap from the snapcraft repository as follows:
 
@@ -298,144 +343,186 @@
 Note that the snap installation only exposes the top level parakeet command:
 
 .. code-block:: bash
 
   parakeet -h
 
 
-Install on Baskerville (native)
+Install on Baskerville HPC (native)
 -------------------------------
 
-In order to install parakeet on the baskerville tier 2 supercomputer with
-singularity, start an interactive job as follows (you will need to know your
-account number and qos to do this):
+In order to install parakeet on the Baskerville tier 2 supercomputer (https://www.baskerville.ac.uk/)
+within a virtual python environment (https://docs.baskerville.ac.uk/self-install/),
+start an interactive job as follows (you will need to know your
+account-project code and qos to do this):
 
 .. code-block:: bash
   
-  salloc --account=${ACCOUNT} --qos=${QOS} --gpus=1 --time=1:0:0
-  srun --pty bash -i
+  srun --account=${ACCOUNT} --qos=${QOS} --gpus=1 --time=0:20:0 \
+    --export=USER,HOME,PATH,TERM --pty /bin/bash
 
-Now execute the following commands to install parakeet:
+When the interactive job starts (you may need to wait until the requested computational resources are
+available), execute the following commands to install parakeet:
 
 .. code-block:: bash
    
   # Load required modules
   module purge
   module load baskerville
-  module load bask-apps/test
   module load CUDA/11.4
   module load FFTW
   module load Python/3
    
   # Create a virtual environment
-  python -m venv env
+  python -m venv --system-site-packages env
   source env/bin/activate
   python -m pip install pip --upgrade
 
   # Install parakeet
   python -m pip install python-parakeet
 
-To run parakeet on a baskerville then write a script called run.sh with the
-following contents:
+You can run parakeet on Baskerville non-interactively and interactively.
+
+To run parakeet on Baskerville non-interactively (https://docs.baskerville.ac.uk/jobs/)
+you need write a script called run.sh with the following contents (you will need to know
+your account-project code, qos and how much time do you expect to take for your script to finish):
 
 .. code-block:: bash
 
   #!/bin/bash
   #SBATCH --account=$ACCOUNT
   #SBATCH --qos=$QOS
   #SBATCH --gpus=1
+  #SBATCH --time=$TIME
 
   # Load required modules
   module purge
   module load baskerville
-  module load bask-apps/test
   module load CUDA/11.4
   module load FFTW
   module load Python/3
 
   # Activate environment
   source env/bin/activate
 
   # Parakeet commands
-  parakeet run -c config.yaml
+  parakeet.run -c config.yaml
 
-Then run the simulations as follows:
+To submit the run.sh script and therefore run the parakeet simulations execute the following:
 
 .. code-block:: bash
 
   sbatch run.sh
 
+The benefit of non-interactive job submissions is that your job will be executed automatically,
+when the requested computational resources are available and that you can submit and queue multiple
+jobs.
 
-Install on Baskerville (singularity)
-------------------------------------
-
-In order to install parakeet on the baskerville tier 2 supercomputer with
-singularity, start an interactive job as follows (you will need to know your
-account number and qos to do this):
+To run parakeet interactively (https://docs.baskerville.ac.uk/interactive-jobs/), execute:
 
 .. code-block:: bash
-  
-  salloc --account=${ACCOUNT} --qos=${QOS} --gpus=1 --time=1:0:0
-  srun --pty bash -i
 
-Now run the following commands:
+  srun --account=${ACCOUNT} --qos=${QOS} --gpus=1 --time=${TIME} \
+    --export=USER,HOME,PATH,TERM --pty /bin/bash
+
+When the interactive job starts (you may need to wait until the requested computational resources are
+available), execute the following commands to install parakeet:
 
 .. code-block:: bash
 
   # Load required modules
   module purge
   module load baskerville
-  module load bask-singularity-conf/live
+  module load CUDA/11.4
+  module load FFTW
+  module load Python/3
+
+  # Activate environment
+  source env/bin/activate
 
-  # Install package
-  singularity build parakeet.sif docker://ghcr.io/rosalindfranklininstitute/parakeet:master
+  # Parakeet commands
+  parakeet.run -c config.yaml
+
+Install on Baskerville (apptainer)
+------------------------------------
 
-Once you are happy, log out of the interactive node. To run parakeet on
-baskerville write a script called run.sh with the following contents:
+Alternatively, you may run parakeet on the baskerville tier 2 supercomputer with
+apptainer (https://docs.baskerville.ac.uk/containerisation/).
+
+To run parakeet on Baskerville non-interactively (https://docs.baskerville.ac.uk/jobs/)
+you need write a script called run.sh with the following contents (you will need to know
+your account-project code, qos and how much time do you expect to take for your script to finish):
 
 .. code-block:: bash
 
   #!/bin/bash
   #SBATCH --account=$ACCOUNT
   #SBATCH --qos=$QOS
   #SBATCH --gpus=1
+  #SBATCH --time=$TIME
 
   # Load required modules
   module purge
   module load baskerville
-  module load bask-singularity-conf/live
+  module load CUDA/11.4
+  module load FFTW
+  module load Python/3
+
+  export APPTAINER_CACHEDIR=/path/to/cache/directory/within/your/project/directory
 
-  function parakeet {
-    singularity run --nv parakeet.sif parakeet $@
+  function container {
+    apptainer exec --nv --bind=/path/to/data/directory/within/your/project/directory:/mnt --pwd=/mnt \
+      docker://quay.io/rosalindfranklininstitute/parakeet:latest bash -c "$@"
   }
 
   # Parakeet commands
-  parakeet run -c config.yaml
+  container \
+  "echo Below you can have multiple commands && \
+  parakeet.run -c config.yaml"
 
-Then run the simulations as follows:
+To submit the run.sh script and therefore run the parakeet simulations execute the following:
 
 .. code-block:: bash
 
   sbatch run.sh
 
-.. warning::
-  
-  On Baskerville, you may receive an error like this when using the parakeet sandbox:
+The benefit of non-interactive job submissions is that your job will be executed automatically,
+when the requested computational resources are available and that you can submit and queue multiple
+jobs.
+
+To run parakeet interactively (https://docs.baskerville.ac.uk/interactive-jobs/), execute:
 
 .. code-block:: bash
 
-  WARNING: By using --writable, Singularity can't create /bask destination automatically without overlay or underlay            
-  FATAL:   container creation failed: mount /var/singularity/mnt/session/bask->/bask error: while mounting /var/singularity/mnt/
-  session/bask: destination /bask doesn't exist in container
+  srun --account=${ACCOUNT} --qos=${QOS} --gpus=1 --time=${TIME} \
+    --export=USER,HOME,PATH,TERM --pty /bin/bash
 
-You can fix this by creating the following directory within the sandbox directory:
+When the interactive job starts (you may need to wait until the requested computational resources are
+available), execute the following commands to install parakeet:
 
 .. code-block:: bash
 
-  mkdir -p parakeet_sandbox/bask
+  # Load required modules
+  module purge
+  module load baskerville
+  module load CUDA/11.4
+  module load FFTW
+  module load Python/3
+
+  export APPTAINER_CACHEDIR=/path/to/cache/directory/within/your/project/directory
+
+  function container {
+    apptainer exec --nv --bind=/path/to/data/directory/within/your/project/directory:/mnt --pwd=/mnt \
+      docker://quay.io/rosalindfranklininstitute/parakeet:latest bash -c "$@"
+  }
+
+  # Parakeet commands
+  container \
+  "echo Below you can have multiple commands && \
+  parakeet.run -c config.yaml"
 
 
 Install on STFC Scarf
 ---------------------
 
 In order to install parakeet on the scarf with singularity, start and
 interactive job as follows:
@@ -444,30 +531,33 @@
   
   salloc --time=1:0:0
 
 Now run the following commands:
 
 .. code-block:: bash
 
-  singularity build parakeet.sif docker://ghcr.io/rosalindfranklininstitute/parakeet:master
+  singularity build parakeet.sif docker://quay.io/rosalindfranklininstitute/parakeet:latest
 
 Once you are happy, log out of the interactive node. To run parakeet on scarf
 write a script called run.sh with the following contents:
 
 .. code-block:: bash
 
   #!/bin/bash
   #SBATCH --gpus=1
 
-  function parakeet {
-    singularity run --nv parakeet.sif parakeet $@
+  function container {
+    singularity exec --nv --bind=/path/to/data/directory/within/your/project/directory:/mnt --pwd=/mnt \
+      docker://quay.io/rosalindfranklininstitute/parakeet:latest bash -c "$@"
   }
 
   # Parakeet commands
-  parakeet run -c config.yaml
+  container \
+  "echo Below you can have multiple commands && \
+  parakeet.run -c config.yaml"
 
 Then run the simulations as follows:
 
 .. code-block:: bash
 
   sbatch run.sh
```

### Comparing `python-parakeet-0.4.3/docs/source/tutorial.rst` & `python-parakeet-0.4.4/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/docs/source/usage.rst` & `python-parakeet-0.4.4/docs/source/usage.rst`

 * *Files 5% similar despite different names*

```diff
@@ -173,33 +173,45 @@
 
 .. argparse::
    :module: parakeet.command_line.analyse._refine
    :func: get_parser
    :prog: parakeet.analyse.refine
 
 
+PDB file programs
+------------------
+
+parakeet.pdb.read
+^^^^^^^^^^^^^^^^^
+
+.. argparse::
+   :module: parakeet.command_line.pdb._read
+   :func: get_parser
+   :prog: parakeet.pdb.read
+
+parakeet.pdb.get
+^^^^^^^^^^^^^^^^^
+
+.. argparse::
+   :module: parakeet.command_line.pdb._get
+   :func: get_parser
+   :prog: parakeet.pdb.get
+
+
 Other programs
 --------------
 
 parakeet.export
 ^^^^^^^^^^^^^^^
 
 .. argparse::
    :module: parakeet.command_line._export
    :func: get_parser
    :prog: parakeet.export
 
-parakeet.read_pdb
-^^^^^^^^^^^^^^^^^
-
-.. argparse::
-   :module: parakeet.command_line._read_pdb
-   :func: get_parser
-   :prog: parakeet.read_pdb
-
 parakeet.run
 ^^^^^^^^^^^^
 
 .. argparse::
    :module: parakeet.command_line._run
    :func: get_parser
    :prog: parakeet.run
```

### Comparing `python-parakeet-0.4.3/pybind11/.appveyor.yml` & `python-parakeet-0.4.4/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.clang-format` & `python-parakeet-0.4.4/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.cmake-format.yaml` & `python-parakeet-0.4.4/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/CONTRIBUTING.md` & `python-parakeet-0.4.4/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/bug-report.md` & `python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/feature-request.md` & `python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/ISSUE_TEMPLATE/question.md` & `python-parakeet-0.4.4/pybind11/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/dependabot.yml` & `python-parakeet-0.4.4/pybind11/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/workflows/ci.yml` & `python-parakeet-0.4.4/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/workflows/configure.yml` & `python-parakeet-0.4.4/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/workflows/format.yml` & `python-parakeet-0.4.4/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.github/workflows/pip.yml` & `python-parakeet-0.4.4/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/.pre-commit-config.yaml` & `python-parakeet-0.4.4/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/LICENSE` & `python-parakeet-0.4.4/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/README.rst` & `python-parakeet-0.4.4/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/Doxyfile` & `python-parakeet-0.4.4/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/Makefile` & `python-parakeet-0.4.4/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/chrono.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/custom.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/eigen.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/functional.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/index.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/overview.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/stl.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/cast/strings.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/classes.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/embedding.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/exceptions.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/functions.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/misc.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/numpy.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/object.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/pycpp/utilities.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/advanced/smart_ptrs.rst` & `python-parakeet-0.4.4/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/basics.rst` & `python-parakeet-0.4.4/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/benchmark.py` & `python-parakeet-0.4.4/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/benchmark.rst` & `python-parakeet-0.4.4/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/changelog.rst` & `python-parakeet-0.4.4/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/classes.rst` & `python-parakeet-0.4.4/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/compiling.rst` & `python-parakeet-0.4.4/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/conf.py` & `python-parakeet-0.4.4/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/faq.rst` & `python-parakeet-0.4.4/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/index.rst` & `python-parakeet-0.4.4/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/installing.rst` & `python-parakeet-0.4.4/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/limitations.rst` & `python-parakeet-0.4.4/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/pybind11-logo.png` & `python-parakeet-0.4.4/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python1.png` & `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python1.svg` & `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python2.png` & `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/pybind11_vs_boost_python2.svg` & `python-parakeet-0.4.4/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/reference.rst` & `python-parakeet-0.4.4/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/release.rst` & `python-parakeet-0.4.4/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/docs/upgrade.rst` & `python-parakeet-0.4.4/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/attr.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/buffer_info.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/cast.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/chrono.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/complex.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/detail/class.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/detail/common.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/detail/descr.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/detail/init.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/detail/internals.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/detail/type_caster_base.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/detail/typeid.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/eigen.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/embed.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/eval.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/functional.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/gil.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/iostream.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/numpy.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/operators.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/options.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/pybind11.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/pytypes.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/stl.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/include/pybind11/stl_bind.h` & `python-parakeet-0.4.4/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/pybind11/__main__.py` & `python-parakeet-0.4.4/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/pybind11/commands.py` & `python-parakeet-0.4.4/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/pybind11/setup_helpers.py` & `python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/pybind11/setup_helpers.pyi` & `python-parakeet-0.4.4/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/setup.cfg` & `python-parakeet-0.4.4/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/setup.py` & `python-parakeet-0.4.4/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/conftest.py` & `python-parakeet-0.4.4/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/constructor_stats.h` & `python-parakeet-0.4.4/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/cross_module_gil_utils.cpp` & `python-parakeet-0.4.4/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/env.py` & `python-parakeet-0.4.4/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/extra_python_package/test_files.py` & `python-parakeet-0.4.4/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/extra_setuptools/test_setuphelper.py` & `python-parakeet-0.4.4/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/local_bindings.h` & `python-parakeet-0.4.4/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/object.h` & `python-parakeet-0.4.4/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/pybind11_cross_module_tests.cpp` & `python-parakeet-0.4.4/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/pybind11_tests.cpp` & `python-parakeet-0.4.4/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/pybind11_tests.h` & `python-parakeet-0.4.4/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/pytest.ini` & `python-parakeet-0.4.4/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/requirements.txt` & `python-parakeet-0.4.4/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_async.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_async.py` & `python-parakeet-0.4.4/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_buffers.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_buffers.py` & `python-parakeet-0.4.4/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_builtin_casters.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_builtin_casters.py` & `python-parakeet-0.4.4/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_call_policies.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_call_policies.py` & `python-parakeet-0.4.4/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_callbacks.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_callbacks.py` & `python-parakeet-0.4.4/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_chrono.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_chrono.py` & `python-parakeet-0.4.4/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_class.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_class.py` & `python-parakeet-0.4.4/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/embed.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_constants_and_functions.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_constants_and_functions.py` & `python-parakeet-0.4.4/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_copy_move.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_copy_move.py` & `python-parakeet-0.4.4/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_custom_type_casters.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_custom_type_casters.py` & `python-parakeet-0.4.4/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_docstring_options.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_docstring_options.py` & `python-parakeet-0.4.4/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_eigen.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_eigen.py` & `python-parakeet-0.4.4/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_embed/CMakeLists.txt` & `python-parakeet-0.4.4/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_embed/catch.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_embed/external_module.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_embed/test_interpreter.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_enum.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_enum.py` & `python-parakeet-0.4.4/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_eval.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_eval.py` & `python-parakeet-0.4.4/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_exceptions.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_exceptions.py` & `python-parakeet-0.4.4/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_factory_constructors.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_factory_constructors.py` & `python-parakeet-0.4.4/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_gil_scoped.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_gil_scoped.py` & `python-parakeet-0.4.4/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_iostream.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_iostream.py` & `python-parakeet-0.4.4/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_kwargs_and_defaults.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_kwargs_and_defaults.py` & `python-parakeet-0.4.4/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_local_bindings.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_local_bindings.py` & `python-parakeet-0.4.4/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_methods_and_attributes.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_methods_and_attributes.py` & `python-parakeet-0.4.4/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_modules.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_modules.py` & `python-parakeet-0.4.4/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_multiple_inheritance.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_multiple_inheritance.py` & `python-parakeet-0.4.4/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_numpy_array.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_numpy_array.py` & `python-parakeet-0.4.4/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_numpy_dtypes.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_numpy_dtypes.py` & `python-parakeet-0.4.4/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_numpy_vectorize.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_numpy_vectorize.py` & `python-parakeet-0.4.4/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_opaque_types.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_opaque_types.py` & `python-parakeet-0.4.4/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_operator_overloading.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_operator_overloading.py` & `python-parakeet-0.4.4/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_pickling.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_pickling.py` & `python-parakeet-0.4.4/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_pytypes.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_pytypes.py` & `python-parakeet-0.4.4/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_sequences_and_iterators.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_sequences_and_iterators.py` & `python-parakeet-0.4.4/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_smart_ptr.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_smart_ptr.py` & `python-parakeet-0.4.4/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_stl.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_stl.py` & `python-parakeet-0.4.4/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_stl_binders.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_stl_binders.py` & `python-parakeet-0.4.4/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_tagbased_polymorphic.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_tagbased_polymorphic.py` & `python-parakeet-0.4.4/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_union.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_virtual_functions.cpp` & `python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/test_virtual_functions.py` & `python-parakeet-0.4.4/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/valgrind-numpy-scipy.supp` & `python-parakeet-0.4.4/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tests/valgrind-python.supp` & `python-parakeet-0.4.4/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/FindCatch.cmake` & `python-parakeet-0.4.4/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/FindEigen3.cmake` & `python-parakeet-0.4.4/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/FindPythonLibsNew.cmake` & `python-parakeet-0.4.4/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/check-style.sh` & `python-parakeet-0.4.4/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/cmake_uninstall.cmake.in` & `python-parakeet-0.4.4/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/libsize.py` & `python-parakeet-0.4.4/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/make_changelog.py` & `python-parakeet-0.4.4/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/pybind11Common.cmake` & `python-parakeet-0.4.4/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/pybind11Config.cmake.in` & `python-parakeet-0.4.4/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/pybind11NewTools.cmake` & `python-parakeet-0.4.4/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/pybind11Tools.cmake` & `python-parakeet-0.4.4/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/setup_global.py.in` & `python-parakeet-0.4.4/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/pybind11/tools/setup_main.py.in` & `python-parakeet-0.4.4/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/setup.cfg` & `python-parakeet-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/setup.py` & `python-parakeet-0.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class CMakeBuild(build_ext):
     """
     Build the extensions
 
     """
 
     def build_extensions(self):
-
         # Set the cmake directory
         cmake_lists_dir = os.path.abspath(".")
 
         # Ensure the build directory exists
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
 
@@ -62,15 +61,15 @@
             "distributed",
             "dask_jobqueue",
             "gemmi",
             "guanaco",
             "h5py",
             "maptools",
             "mrcfile",
-            "numpy",
+            "numpy==1.23",  # Until scikit-image updates
             "pandas",
             "pillow",
             "profet",
             "pydantic",
             "python-multem",
             "pyyaml",
             "scipy",
@@ -97,14 +96,15 @@
                 "parakeet.sample.sputter=parakeet.command_line.sample:sputter",
                 "parakeet.sample.show=parakeet.command_line.sample:show",
                 "parakeet.simulate.potential=parakeet.command_line.simulate:potential",
                 "parakeet.simulate.exit_wave=parakeet.command_line.simulate:exit_wave",
                 "parakeet.simulate.optics=parakeet.command_line.simulate:optics",
                 "parakeet.simulate.image=parakeet.command_line.simulate:image",
                 "parakeet.simulate.simple=parakeet.command_line.simulate:simple",
+                "parakeet.simulate.cbed=parakeet.command_line.simulate:cbed",
                 "parakeet.simulate.ctf=parakeet.command_line.simulate:ctf",
                 "parakeet.metadata.export=parakeet.command_line.metadata:export",
                 "parakeet.analyse.reconstruct=parakeet.command_line.analyse:reconstruct",
                 "parakeet.analyse.average_particles=parakeet.command_line.analyse:average_particles",
                 "parakeet.analyse.average_all_particles=parakeet.command_line.analyse:average_all_particles",
                 "parakeet.analyse.extract=parakeet.command_line.analyse:extract",
                 "parakeet.analyse.refine=parakeet.command_line.analyse:refine",
```

### Comparing `python-parakeet-0.4.3/snap/snapcraft.yaml` & `python-parakeet-0.4.4/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/analyse/_average_particles.py` & `python-parakeet-0.4.4/src/parakeet/analyse/_average_particles.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 
 # Set the random seed
 random.seed(0)
 
 
 def _rotate_array(data, rotation, offset):
-
     # Create the pixel indices
     az = np.arange(data.shape[0])
     ay = np.arange(data.shape[1])
     ax = np.arange(data.shape[2])
     x, y, z = np.meshgrid(az, ay, ax, indexing="ij")
 
     # Create a stack of coordinates
@@ -61,15 +60,14 @@
 
     # sample
     result = scipy.ndimage.map_coordinates(data, [x, y, z], order=1)
     return result
 
 
 def _process_sub_tomo(args):
-
     sub_tomo, position, orientation, half_index = args
 
     # Set the data to transform
     data = sub_tomo
     offset = position
 
     # Reorder input vectors
@@ -90,15 +88,14 @@
     centre,
     size,
     half_length,
     half_shape,
     voxel_size,
     tomogram,
 ):
-
     for j in range(len(indices)):
         for i in indices[j]:
             position = positions[i]
             orientation = orientations[i]
 
             # Compute p within the volume
             # start_position = np.array([0, scan["start_pos"], 0])
@@ -190,15 +187,15 @@
         half1_file,
         half2_file,
         particle_size,
         num_particles,
     )
 
 
-@average_particles.register
+@average_particles.register(parakeet.config.Scan)
 def _average_particles_Config(
     config: parakeet.config.Scan,
     sample: parakeet.sample.Sample,
     rec_filename: str,
     half_1_filename: str,
     half_2_filename: str,
     particle_size: int = 0,
@@ -230,15 +227,14 @@
     assert voxel_size[0] == voxel_size[1]
     assert voxel_size[0] == voxel_size[2]
     size = np.array(tomogram.shape)[[2, 0, 1]] * voxel_size
 
     # Loop through the
     assert sample.number_of_molecules == 1
     for name, (atoms, positions, orientations) in sample.iter_molecules():
-
         # Compute the box size based on the size of the particle so that any
         # orientation should fit within the box
         xmin = atoms.data["x"].min()
         xmax = atoms.data["x"].max()
         ymin = atoms.data["y"].min()
         ymax = atoms.data["y"].max()
         zmin = atoms.data["z"].min()
@@ -298,15 +294,14 @@
                     size,
                     half_length,
                     half.shape,
                     voxel_size,
                     tomogram,
                 ),
             ):
-
                 # Add the contribution to the average
                 half[half_index, :, :, :] += data
                 num[half_index] += 1
 
         # Average the sub tomograms
         print("Averaging half 1 with %d particles" % num[0])
         print("Averaging half 2 with %d particles" % num[1])
@@ -361,29 +356,28 @@
 
     # Do the sub tomogram averaging
     _average_all_particles_Config(
         config.scan, sample, rec_file, average_file, particle_size
     )
 
 
-@average_all_particles.register
+@average_all_particles.register(parakeet.config.Scan)
 def _average_all_particles_Config(
     config: parakeet.config.Scan,
     sample: parakeet.sample.Sample,
     rec_filename: str,
     average_filename: str,
     particle_size: int = 0,
 ):
     """
     Average particles to compute averaged reconstruction
 
     """
 
     def rotate_array(data, rotation, offset):
-
         # Create the pixel indices
         az = np.arange(data.shape[0])
         ay = np.arange(data.shape[1])
         ax = np.arange(data.shape[2])
         x, y, z = np.meshgrid(az, ay, ax, indexing="ij")
 
         # Create a stack of coordinates
@@ -436,15 +430,14 @@
     assert voxel_size[0] == voxel_size[1]
     assert voxel_size[0] == voxel_size[2]
     size = np.array(tomogram.shape)[[2, 0, 1]] * voxel_size
 
     # Loop through the
     assert sample.number_of_molecules == 1
     for name, (atoms, positions, orientations) in sample.iter_molecules():
-
         # Compute the box size based on the size of the particle so that any
         # orientation should fit within the box
         xmin = atoms.data["x"].min()
         xmax = atoms.data["x"].max()
         ymin = atoms.data["y"].min()
         ymax = atoms.data["y"].max()
         zmin = atoms.data["z"].min()
@@ -500,15 +493,14 @@
                     size,
                     half_length,
                     average.shape,
                     voxel_size,
                     tomogram,
                 ),
             ):
-
                 # Add the contribution to the average
                 average += data
                 num += 1
 
         # Average the sub tomograms
         print("Averaging map with %d particles" % num)
         if num > 0:
```

### Comparing `python-parakeet-0.4.3/src/parakeet/analyse/_correct.py` & `python-parakeet-0.4.4/src/parakeet/analyse/_correct.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         config,
         image_file,
         corrected_file,
         num_defocus=num_defocus,
     )
 
 
-@correct.register
+@correct.register(parakeet.config.Config)
 def _correct_Config(
     config: parakeet.config.Config,
     image_filename: str,
     corrected_filename: str,
     num_defocus: int = None,
 ):
     """
```

### Comparing `python-parakeet-0.4.3/src/parakeet/analyse/_extract.py` & `python-parakeet-0.4.4/src/parakeet/analyse/_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,29 +56,28 @@
     # Load the sample
     sample = parakeet.sample.load(sample_file)
 
     # Do the sub tomogram averaging
     _extract_Config(config, sample, rec_file, particles_file, particle_size)
 
 
-@extract.register
+@extract.register(parakeet.config.Config)
 def _extract_Config(
     config: parakeet.config.Config,
     sample: parakeet.sample.Sample,
     rec_file: str,
     extract_file: str,
     particle_size: int = 0,
 ):
     """
     Extract particles for post-processing
 
     """
 
     def rotate_array(data, rotation, offset):
-
         # Create the pixel indices
         az = np.arange(data.shape[0])
         ay = np.arange(data.shape[1])
         ax = np.arange(data.shape[2])
         x, y, z = np.meshgrid(az, ay, ax, indexing="ij")
 
         # Create a stack of coordinates
@@ -128,15 +127,14 @@
         )
     )
     size = np.array(tomogram.shape)[[2, 0, 1]] * voxel_size
 
     # Loop through the
     assert sample.number_of_molecules == 1
     for name, (atoms, positions, orientations) in sample.iter_molecules():
-
         # Compute the box size based on the size of the particle so that any
         # orientation should fit within the box
         xmin = atoms.data["x"].min()
         xmax = atoms.data["x"].max()
         ymin = atoms.data["y"].min()
         ymax = atoms.data["y"].max()
         zmin = atoms.data["z"].min()
@@ -167,15 +165,14 @@
         # Sort the positions and orientations by y
         positions, orientations = zip(
             *sorted(zip(positions, orientations), key=lambda x: x[0][1])
         )
 
         # Loop through all the particles
         for i, (position, orientation) in enumerate(zip(positions, orientations)):
-
             # Compute p within the volume
             # start_position = np.array([0, scan["start_pos"], 0])
             p = position - (centre - size / 2.0)  # - start_position
             p[2] = size[2] - p[2]
             print(
                 "Particle %d: position = %s, orientation = %s"
                 % (
@@ -190,15 +187,14 @@
             x1 = np.floor(p).astype("int32") + half_length
             offset = p - np.floor(p).astype("int32")
 
             # Get the sub tomogram
             print("Getting sub tomogram")
             sub_tomo = tomogram[x0[1] : x1[1], x0[2] : x1[2], x0[0] : x1[0]]
             if sub_tomo.shape == particle_instance.shape:
-
                 # Set the data to transform
                 data = sub_tomo
 
                 # Reorder input vectors
                 offset = np.array(data.shape)[::-1] / 2 + offset[[1, 2, 0]]
                 rotation = -np.array(orientation)[[1, 2, 0]]
                 rotation[1] = -rotation[1]
```

### Comparing `python-parakeet-0.4.3/src/parakeet/analyse/_reconstruct.py` & `python-parakeet-0.4.4/src/parakeet/analyse/_reconstruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     _reconstruct_Config(
         config,
         image_file,
         rec_file,
     )
 
 
-@reconstruct.register
+@reconstruct.register(parakeet.config.Config)
 def _reconstruct_Config(
     config: parakeet.config.Config, image_filename: str, rec_filename: str
 ):
     """
     Reconstruct the volume and use 3D CTF correction beforehand if the input image is uncorrected
 
     """
```

### Comparing `python-parakeet-0.4.3/src/parakeet/analyse/_refine.py` & `python-parakeet-0.4.4/src/parakeet/analyse/_refine.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/beam.py` & `python-parakeet-0.4.4/src/parakeet/beam.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __init__(
         self,
         energy: float = 300,
         energy_spread: float = 0,
         acceleration_voltage_spread: float = 0,
         illumination_semiangle: float = 0.1,
-        electrons_per_angstrom: float = 30,
+        electrons_per_angstrom: float = 40,
         theta: float = 0,
         phi: float = 0,
     ):
         """
         Initialise the beam
 
         Args:
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/__init__.py` & `python-parakeet-0.4.4/src/parakeet/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/_export.py` & `python-parakeet-0.4.4/src/parakeet/command_line/_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,59 +4,71 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import logging.config
 import numpy as np
 import random
 import parakeet.io
 import parakeet.config
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["export"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
 
 
-def rebin(data, shape):
+def rebin(data, shape, filter=True):
     """
     Rebin a multidimensional array
 
     Args:
         data (array): The input array
         shape (tuple): The new shape
+        filter: Filter in Fourier space
 
     """
-    f = np.fft.fft2(data)
-    f = np.fft.fftshift(f)
-    yc, xc = data.shape[0] // 2, data.shape[1] // 2
-    yh = shape[0] // 2
-    xh = shape[1] // 2
-    x0 = xc - xh
-    y0 = yc - yh
-    x1 = x0 + shape[1]
-    y1 = y0 + shape[0]
-    y, x = np.mgrid[0 : data.shape[0], 0 : data.shape[1]]
-    r = (y - yc) ** 2 / yh**2 + (x - xc) ** 2 / xh**2
-    mask = r < 1.0
-    f = f * mask
-    f = f[y0:y1, x0:x1]
-    f = np.fft.ifftshift(f)
-    d = np.fft.ifft2(f)
-    return d.real
+    if filter:
+        f = np.fft.fft2(data)
+        f = np.fft.fftshift(f)
+        yc, xc = data.shape[0] // 2, data.shape[1] // 2
+        yh = shape[0] // 2
+        xh = shape[1] // 2
+        x0 = xc - xh
+        y0 = yc - yh
+        x1 = x0 + shape[1]
+        y1 = y0 + shape[0]
+        y, x = np.mgrid[0 : data.shape[0], 0 : data.shape[1]]
+        r = (y - yc) ** 2 / yh**2 + (x - xc) ** 2 / xh**2
+        mask = r < 1.0
+        f = f * mask
+        f = f[y0:y1, x0:x1]
+        f = np.fft.ifftshift(f)
+        d = np.fft.ifft2(f)
+        output = d.real
+    else:
+        shape = (
+            shape[0],
+            data.shape[0] // shape[0],
+            shape[1],
+            data.shape[1] // shape[1],
+        )
+        output = data.reshape(shape).sum(-1).sum(1)
+    return output
 
 
 def filter_image(data, pixel_size, resolution, shape):
     """
     Filter the image
 
     Args:
@@ -318,15 +330,14 @@
     # If converting to images, determine min and max
     if writer.is_image_writer:
         if args.vmin is None or args.vmax is None:
             logger.info("Computing min and max of dataset:")
             min_image = []
             max_image = []
             for i in indices:
-
                 # Transform if necessary
                 image = {
                     "complex": lambda x: x,
                     "real": lambda x: np.real(x),
                     "imaginary": lambda x: np.imag(x),
                     "amplitude": lambda x: np.abs(x),
                     "phase": lambda x: np.real(np.angle(x)),
@@ -382,23 +393,23 @@
             image = filter_image(
                 image, pixel_size, args.filter_resolution, args.filter_shape
             )
 
         # Rebin the array
         if args.rebin != 1:
             new_shape = np.array(image.shape) // args.rebin
-            image = rebin(image, new_shape)
+            image = rebin(image, new_shape, filter=False)
 
         # Write the image info
         writer.data[j, :, :] = image
         writer.header[j] = header
 
     # Update the writer
     writer.update()
 
 
-def export(args: list[str] = None):
+def export(args: List[str] = None):
     """
     Convert the input file type to a different file type
 
     """
     export_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/_main.py` & `python-parakeet-0.4.4/src/parakeet/command_line/_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import parakeet.config
+
 import parakeet.command_line
-import parakeet.command_line.config as config
-import parakeet.command_line.sample as sample
-import parakeet.command_line.simulate as simulate
-import parakeet.command_line.metadata as metadata
-import parakeet.command_line.analyse as analyse
-import parakeet.command_line.pdb as pdb
+from parakeet.command_line import config as config
+from parakeet.command_line import sample as sample
+from parakeet.command_line import simulate as simulate
+from parakeet.command_line import metadata as metadata
+from parakeet.command_line import analyse as analyse
+from parakeet.command_line import pdb as pdb
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["main"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -241,37 +243,45 @@
     )
 
     # Add the "parakeet simulate" command
     add_simulate_command(
         subparsers.add_parser("simulate", help="Commands to simulate the TEM images")
     )
 
-    # Add the "parakeet metadata" command
-    add_metadata_command(
-        subparsers.add_parser("metadata", help="Commands to manipulate metadata")
-    )
-
     # Add the "parakeet analyse" command
     add_analyse_command(
         subparsers.add_parser("analyse", help="Commands to analyse the simulated data")
     )
 
+    # Add the "parakeet metadata" command
+    add_metadata_command(
+        subparsers.add_parser("metadata", help="Commands to manipulate metadata")
+    )
+
     # Add the "parakeet pdb" command
     add_pdb_command(
         subparsers.add_parser("pdb", help="Commands to operate on pdb files")
     )
 
     # Add the parakeet export command
     parakeet.command_line._export.get_parser(
         subparsers.add_parser(
             "export",
             help=parakeet.command_line._export.get_description(),
         )
     )
 
+    # Add the "parakeet run" command
+    parakeet.command_line._run.get_parser(
+        subparsers.add_parser(
+            "run",
+            help=parakeet.command_line._run.get_description(),
+        )
+    )
+
     # Return parser
     return parser
 
 
 def config_main(parser, args):
     """
     Perform the parakeet config action
@@ -316,15 +326,18 @@
 
 
 def metadata_main(parser, args):
     """
     Perform the parakeet metadata action
 
     """
-    {None: lambda x: parser.print_help(), "export": metadata._export.export_impl,}[
+    {
+        None: lambda x: parser.print_help(),
+        "export": metadata._export.export_impl,
+    }[
         args.metadata_command
     ](args)
 
 
 def analyse_main(parser, args):
     """
     Perform the parakeet analyse action
@@ -379,31 +392,36 @@
     for sp in parser._subparsers._group_actions:
         p = sp.choices.get(command, None)
         if p is not None:
             return p
     raise RuntimeError("Parser for %s not found" % command)
 
 
-def main():
+def main_impl(parser, args):
     """
     Parakeet as a single command line program
 
     """
-
-    # Get the parser
-    parser = get_parser()
-
-    # Parse the arguments
-    args = parser.parse_args()
-
-    # Call the top level command
     {
         None: lambda a, b: parser.print_help(),
         "config": config_main,
         "sample": sample_main,
         "simulate": simulate_main,
         "analyse": analyse_main,
         "metadata": metadata_main,
         "pdb": pdb_main,
         "export": export_main,
         "run": run_main,
     }[args.command](get_subparser(parser, args.command), args)
+
+
+def main(args: List[str] = None):
+    """
+    Parakeet as a single command line program
+
+    """
+
+    # Get the parser
+    parser = get_parser()
+
+    # Parse the arguments
+    main_impl(parser, parser.parse_args(args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/_run.py` & `python-parakeet-0.4.4/src/parakeet/command_line/_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["run"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -105,14 +106,32 @@
         "--cluster.method",
         type=str,
         choices=["sge"],
         default=None,
         dest="cluster_method",
         help="The cluster method to use",
     )
+    parser.add_argument(
+        "--steps",
+        type=str,
+        choices=[
+            "all",
+            "sample",
+            "sample.new",
+            "sample.add_molecules",
+            "simulate",
+            "simulate.exit_wave",
+            "simulate.optics",
+            "simulate.image",
+        ],
+        nargs="+",
+        default=None,
+        dest="steps",
+        help="Which simulation steps to run",
+    )
 
     return parser
 
 
 def run_impl(args):
     """
     Run the whole simulation experiment
@@ -131,19 +150,20 @@
         args.sample,
         args.exit_wave,
         args.optics,
         args.image,
         args.device,
         args.cluster_method,
         args.cluster_max_workers,
+        args.steps,
     )
 
     # Print output
     logger.info("Time taken: %.1f seconds" % (time.time() - start_time))
 
 
-def run(args: list[str] = None):
+def run(args: List[str] = None):
     """
     Run the whole simulation experiment
 
     """
     run_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/analyse/_average_all_particles.py` & `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_all_particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.analyse
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["average_all_particles"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -109,13 +110,13 @@
         args.config, args.sample, args.rec, args.average, args.particle_size
     )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def average_all_particles(args: list[str] = None):
+def average_all_particles(args: List[str] = None):
     """
     Perform sub tomogram averaging
 
     """
     average_all_particles_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/analyse/_average_particles.py` & `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_average_particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.analyse
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["average_particles"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -131,13 +132,13 @@
         args.num_particles,
     )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def average_particles(args: list[str] = None):
+def average_particles(args: List[str] = None):
     """
     Perform sub tomogram averaging
 
     """
     average_particles_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/analyse/_correct.py` & `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_correct.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.analyse
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["correct"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -109,13 +110,13 @@
         args.config, args.image, args.corrected, args.num_defocus, args.device
     )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def correct(args: list[str] = None):
+def correct(args: List[str] = None):
     """
     Correct the images using 3D CTF correction
 
     """
     correct_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/analyse/_extract.py` & `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.analyse
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["extract"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -109,13 +110,13 @@
         args.config, args.sample, args.rec, args.particles, args.particle_size
     )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def extract(args: list[str] = None):
+def extract(args: List[str] = None):
     """
     Perform sub tomogram extraction
 
     """
     extract_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/analyse/_reconstruct.py` & `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_reconstruct.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.analyse
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["reconstruct"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -99,13 +100,13 @@
     # Do the reconstruction
     parakeet.analyse.reconstruct(args.config, args.image, args.rec, args.device)
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def reconstruct(args: list[str] = None):
+def reconstruct(args: List[str] = None):
     """
     Reconstruct the volume
 
     """
     reconstruct_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/analyse/_refine.py` & `python-parakeet-0.4.4/src/parakeet/command_line/analyse/_refine.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.analyse
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["refine"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -97,13 +98,13 @@
     # Do the sub tomogram averaging
     parakeet.analyse.refine(args.sample, args.rec)
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def refine(args: list[str] = None):
+def refine(args: List[str] = None):
     """
     Refine against the model
 
     """
     refine_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/config/_edit.py` & `python-parakeet-0.4.4/src/parakeet/command_line/config/_edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import parakeet.config
 import parakeet.command_line
 from argparse import ArgumentParser
+from typing import List
 
 # Get the logger
 logger = logging.getLogger(__name__)
 
 
 __all__ = ["edit"]
 
@@ -85,13 +86,13 @@
     # Call internally
     config = parakeet.config.edit(args.input, args.output, args.config)
 
     # Print the config
     parakeet.config.show(config, full=True)
 
 
-def edit(args: list[str] = None):
+def edit(args: List[str] = None):
     """
     Edit the configuration
 
     """
     edit_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/config/_new.py` & `python-parakeet-0.4.4/src/parakeet/command_line/config/_new.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import parakeet.config
 import parakeet.command_line
 from argparse import ArgumentParser
+from typing import List
 
 # Get the logger
 logger = logging.getLogger(__name__)
 
 
 __all__ = ["new"]
 
@@ -71,13 +72,13 @@
     # Configure some basic logging
     parakeet.command_line.configure_logging()
 
     # Parse the arguments
     parakeet.config.new(filename=args.config, full=args.full)
 
 
-def new(args: list[str] = None):
+def new(args: List[str] = None):
     """
     Create a new configuration
 
     """
     new_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/config/_show.py` & `python-parakeet-0.4.4/src/parakeet/command_line/sample/_sputter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 #
-# parakeet.command_line.config.show.py
+# parakeet.command_line.sample.sputter.py
 #
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
-import parakeet.config
+import time
+import parakeet.io
 import parakeet.command_line
+import parakeet.config
+import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
-# Get the logger
-logger = logging.getLogger(__name__)
 
+__all__ = ["sputter"]
 
-__all__ = ["show"]
+
+# Get the logger
+logger = logging.getLogger(__name__)
 
 
 def get_description():
     """
     Get the program description
 
     """
-    return "Show the configuration"
+    return "Sputter the sample"
 
 
 def get_parser(parser: ArgumentParser = None) -> ArgumentParser:
     """
-    Get the parser for the parakeet.config.show command
+    Get the sputter parser
 
     """
 
     # Initialise the parser
     if parser is None:
         parser = ArgumentParser(description=get_description())
 
@@ -46,30 +51,44 @@
         "--config",
         type=str,
         default=None,
         dest="config",
         required=True,
         help="The yaml file to configure the simulation",
     )
+    parser.add_argument(
+        "-s",
+        "--sample",
+        type=str,
+        default="sample.h5",
+        dest="sample",
+        help="The filename for the sample file",
+    )
 
     return parser
 
 
-def show_impl(args):
+def sputter_impl(args):
     """
-    Show the full configuration
+    Sputter the sample
 
     """
 
-    # Parse the arguments
-    config = parakeet.config.load(args.config)
+    # Get the start time
+    start_time = time.time()
+
+    # Configure some basic logging
+    parakeet.command_line.configure_logging()
+
+    # Do the work
+    parakeet.sample.sputter(args.config, args.sample)
 
-    # Print some options
-    print(parakeet.config.show(config, full=True))
+    # Print output
+    logger.info("Time taken: %.1f seconds" % (time.time() - start_time))
 
 
-def show(args: list[str] = None):
+def sputter(args: List[str] = None):
     """
-    Show the full configuration
+    Sputter the sample
 
     """
-    show_impl(get_parser().parse_args(args=args))
+    sputter_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/metadata/_export.py` & `python-parakeet-0.4.4/src/parakeet/command_line/metadata/_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import parakeet.metadata
 import parakeet.command_line
 from argparse import ArgumentParser
+from typing import List
 
 # Get the logger
 logger = logging.getLogger(__name__)
 
 
 __all__ = ["export"]
 
@@ -87,13 +88,13 @@
     # Configure some basic logging
     parakeet.command_line.configure_logging()
 
     # Parse the arguments
     parakeet.metadata.export(args.config, args.sample, args.directory, args.relion)
 
 
-def export(args: list[str] = None):
+def export(args: List[str] = None):
     """
     Export the metadata
 
     """
     export_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/pdb/_get.py` & `python-parakeet-0.4.4/src/parakeet/command_line/pdb/_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import logging.config
 import os
 import shutil
 from argparse import ArgumentParser
 import parakeet.data
+from typing import List
 
 
 __all__ = ["get"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -73,13 +74,13 @@
     # Get the filename
     filename = parakeet.data.get_pdb(args.id)
 
     # Copy the file to the directory
     shutil.copyfile(filename, os.path.join(args.directory, os.path.basename(filename)))
 
 
-def get(args: list[str] = None):
+def get(args: List[str] = None):
     """
     Read the given PDB file and show the atom positions
 
     """
     return get_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/pdb/_read.py` & `python-parakeet-0.4.4/src/parakeet/command_line/pdb/_read.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import gemmi
 import logging
 import logging.config
 import parakeet.io
 import parakeet.config
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["read"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -92,13 +93,13 @@
                             atom.occ,
                             atom.charge,
                             parakeet.sample.get_atom_sigma(atom),
                         )
                     )
 
 
-def read(args: list[str] = None):
+def read(args: List[str] = None):
     """
     Read the given PDB file and show the atom positions
 
     """
     return read_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/sample/_add_molecules.py` & `python-parakeet-0.4.4/src/parakeet/command_line/sample/_add_molecules.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["add_molecules"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -81,13 +82,13 @@
     # Do the work
     parakeet.sample.add_molecules(args.config, args.sample)
 
     # Print output
     logger.info("Time taken: %.1f seconds" % (time.time() - start_time))
 
 
-def add_molecules(args: list[str] = None):
+def add_molecules(args: List[str] = None):
     """
     Add molecules to the sample
 
     """
     add_molecules_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/sample/_mill.py` & `python-parakeet-0.4.4/src/parakeet/command_line/sample/_mill.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["mill"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -81,13 +82,13 @@
     # Do work
     parakeet.sample.mill(args.config, args.sample)
 
     # Print output
     logger.info("Time taken: %.1f seconds" % (time.time() - start_time))
 
 
-def mill(args: list[str] = None):
+def mill(args: List[str] = None):
     """
     Mill to the shape of the sample
 
     """
     mill_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/sample/_new.py` & `python-parakeet-0.4.4/src/parakeet/command_line/sample/_new.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["new"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -81,13 +82,13 @@
     # Do the work
     parakeet.sample.new(args.config, args.sample)
 
     # Print output
     logger.info("Time taken: %.1f seconds" % (time.time() - start_time))
 
 
-def new(args: list[str] = None):
+def new(args: List[str] = None):
     """
     Create an ice sample and save it
 
     """
     new_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/sample/_show.py` & `python-parakeet-0.4.4/src/parakeet/command_line/sample/_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.sample
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["show"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -66,13 +67,13 @@
     parakeet.command_line.configure_logging()
 
     # Create the sample
     sample = parakeet.sample.load(args.sample)
     logger.info(sample.info())
 
 
-def show(args: list[str] = None):
+def show(args: List[str] = None):
     """
     Show the sample information
 
     """
     show_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/sample/_sputter.py` & `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 #
-# parakeet.command_line.sample.sputter.py
+# parakeet.command_line.simulate.simple.py
 #
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
+import parakeet.microscope
 import parakeet.sample
+import parakeet.scan
+import parakeet.simulate
 from argparse import ArgumentParser
 
 
-__all__ = ["sputter"]
+__all__ = ["simple"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
 
 
 def get_description():
     """
     Get the program description
 
     """
-    return "Sputter the sample"
+    return "Simulate the whole process"
 
 
 def get_parser(parser: ArgumentParser = None) -> ArgumentParser:
     """
-    Get the sputter parser
+    Get the parakeet.simulate.simple parser
 
     """
 
     # Initialise the parser
     if parser is None:
         parser = ArgumentParser(description=get_description())
 
@@ -51,43 +54,50 @@
         type=str,
         default=None,
         dest="config",
         required=True,
         help="The yaml file to configure the simulation",
     )
     parser.add_argument(
-        "-s",
-        "--sample",
+        "-o",
+        "--output",
         type=str,
-        default="sample.h5",
-        dest="sample",
-        help="The filename for the sample file",
+        default="output.h5",
+        dest="output",
+        help="The filename for the output",
+    )
+    parser.add_argument(
+        dest="atoms",
+        type=str,
+        default=None,
+        nargs="?",
+        help="The filename for the input atoms",
     )
 
     return parser
 
 
-def sputter_impl(args):
+def simple_impl(args):
     """
-    Sputter the sample
+    Simulate the image
 
     """
 
     # Get the start time
     start_time = time.time()
 
     # Configure some basic logging
     parakeet.command_line.configure_logging()
 
     # Do the work
-    parakeet.sample.sputter(args.config, args.sample)
+    parakeet.simulate.simple(args.config, args.atoms, args.output)
 
-    # Print output
-    logger.info("Time taken: %.1f seconds" % (time.time() - start_time))
+    # Write some timing stats
+    logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def sputter(args: list[str] = None):
+def simple():
     """
-    Sputter the sample
+    Simulate the image
 
     """
-    sputter_impl(get_parser().parse_args(args=args))
+    simple_impl(get_parser().parse_args())
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/simulate/_ctf.py` & `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_ctf.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 import parakeet.scan
 import parakeet.simulate
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["ctf"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -83,13 +84,13 @@
     # Do the work
     parakeet.simulate.ctf(args.config, args.output)
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def ctf(args: list[str] = None):
+def ctf(args: List[str] = None):
     """
     Simulate the ctf
 
     """
     ctf_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/simulate/_exit_wave.py` & `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_exit_wave.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 import parakeet.scan
 import parakeet.simulate
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["exit_wave"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -122,13 +123,13 @@
         cluster_max_workers=args.cluster_max_workers,
     )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def exit_wave(args: list[str] = None):
+def exit_wave(args: List[str] = None):
     """
     Simulate the exit wave from the sample
 
     """
     exit_wave_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/simulate/_image.py` & `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 import parakeet.scan
 import parakeet.simulate
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["image"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -92,13 +93,13 @@
     # Do the work
     parakeet.simulate.image(args.config, args.optics, args.image)
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def image(args: list[str] = None):
+def image(args: List[str] = None):
     """
     Simulate the image with noise
 
     """
     image_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/simulate/_optics.py` & `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_optics.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 import parakeet.scan
 import parakeet.simulate
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["optics"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -122,13 +123,13 @@
         cluster_max_workers=args.cluster_max_workers,
     )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def optics(args: list[str] = None):
+def optics(args: List[str] = None):
     """
     Simulate the optics
 
     """
     optics_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/simulate/_potential.py` & `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 import parakeet.scan
 import parakeet.simulate
 from argparse import ArgumentParser
+from typing import List
 
 
 __all__ = ["potential"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
@@ -122,13 +123,13 @@
         args.cluster_max_workers,
     )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def potential(args: list[str] = None):
+def potential(args: List[str] = None):
     """
     Simulate the projected potential from the sample
 
     """
     potential_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/command_line/simulate/_simple.py` & `python-parakeet-0.4.4/src/parakeet/command_line/simulate/_cbed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 #
-# parakeet.command_line.simulate.simple.py
+# parakeet.command_line.simulate.cbed.py
 #
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-from __future__ import annotations
+
 
 import logging
 import time
 import parakeet.io
 import parakeet.command_line
 import parakeet.config
 import parakeet.microscope
 import parakeet.sample
 import parakeet.scan
 import parakeet.simulate
 from argparse import ArgumentParser
+from typing import List
 
 
-__all__ = ["simple"]
+__all__ = ["cbed"]
 
 
 # Get the logger
 logger = logging.getLogger(__name__)
 
 
 def get_description():
     """
     Get the program description
 
     """
-    return "Simulate the whole process"
+    return "Simulate the image from the sample"
 
 
 def get_parser(parser: ArgumentParser = None) -> ArgumentParser:
     """
-    Get the parakeet.simulate.simple parser
+    Get the parakeet.simulate.cbed parser
 
     """
 
     # Initialise the parser
     if parser is None:
         parser = ArgumentParser(description=get_description())
 
@@ -54,50 +55,81 @@
         type=str,
         default=None,
         dest="config",
         required=True,
         help="The yaml file to configure the simulation",
     )
     parser.add_argument(
-        "-o",
-        "--output",
+        "-s",
+        "--sample",
         type=str,
-        default="output.h5",
-        dest="output",
-        help="The filename for the output",
+        default="sample.h5",
+        dest="sample",
+        help="The filename for the sample",
     )
     parser.add_argument(
-        dest="atoms",
+        "-i",
+        "--image",
         type=str,
+        default="image.h5",
+        dest="image",
+        help="The filename for the image",
+    )
+    parser.add_argument(
+        "-d",
+        "--device",
+        choices=["cpu", "gpu"],
+        default=None,
+        dest="device",
+        help="Choose the device to use",
+    )
+    parser.add_argument(
+        "--cluster.max_workers",
+        type=int,
         default=None,
-        nargs="?",
-        help="The filename for the input atoms",
+        dest="cluster_max_workers",
+        help="The maximum number of worker processes",
+    )
+    parser.add_argument(
+        "--cluster.method",
+        type=str,
+        choices=["sge"],
+        default=None,
+        dest="cluster_method",
+        help="The cluster method to use",
     )
 
     return parser
 
 
-def simple_impl(args):
+def cbed_impl(args):
     """
-    Simulate the image
+    Simulate the image from the sample
 
     """
 
     # Get the start time
     start_time = time.time()
 
     # Configure some basic logging
     parakeet.command_line.configure_logging()
 
     # Do the work
-    parakeet.simulate.simple(args.config, args.atoms, args.output)
+    parakeet.simulate.cbed(
+        args.config,
+        args.sample,
+        args.image,
+        device=args.device,
+        cluster_method=args.cluster_method,
+        cluster_max_workers=args.cluster_max_workers,
+    )
 
     # Write some timing stats
     logger.info("Time taken: %.2f seconds" % (time.time() - start_time))
 
 
-def simple():
+def cbed(args: List[str] = None):
     """
-    Simulate the image
+    Simulate the image from the sample
 
     """
-    simple_impl(get_parser().parse_args())
+    cbed_impl(get_parser().parse_args(args=args))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/config.py` & `python-parakeet-0.4.4/src/parakeet/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
 import copy
 import logging
+import os
 import yaml
 
 from enum import Enum
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import Field
 from typing import List
 from typing import Optional
@@ -36,15 +37,14 @@
 class BaseModel(PydanticBaseModel):
     """
     Create a custom base to define desired behaviour
 
     """
 
     class Config:
-
         # Ensure that enums use string values
         use_enum_values = True
 
         # Don't allow extra fields
         extra = "forbid"
 
 
@@ -166,17 +166,18 @@
             "position: [] # Assign random position",
             "position: [1, 2, 3] # Assign known position",
         ],
     )
 
     orientation: Optional[Tuple[float, float, float]] = Field(
         description=(
-            "The molecule orientation defined as a rotation vector. Setting "
-            "this to null or an empty list will cause parakeet to give a "
-            "random orientation"
+            "The molecule orientation defined as a rotation vector where "
+            "the direction of the vector gives the rotation axis and the "
+            "magnitude of the vector gives the rotation angle in radians. Setting "
+            "this to null or an empty list will cause parakeet to give a random orientation"
         ),
         examples=[
             "orienation: null # Assign random orienation",
             "orienation: [] # Assign random orienation",
             "orienation: [1, 2, 3] # Assign known orienation",
         ],
     )
@@ -190,14 +191,41 @@
 
     filename: str = Field(
         None, description="The filename of the atomic coordinates to use (*.pdb, *.cif)"
     )
 
     recentre: bool = Field(True, description="Recentre the coordinates")
 
+    scale: float = Field(1, description="Scale the coordinates x' = x * scale")
+
+    position: Optional[Tuple[float, float, float]] = Field(
+        description=(
+            "The model position (A, A, A). "
+            "If recentre if set then the model will be centred on the given position. "
+            "If recentre if not set then the model will be translated by the given position. "
+        ),
+        examples=[
+            "position: null # Assign [0, 0, 0] position",
+            "position: [1, 2, 3] # Assign known position",
+        ],
+    )
+
+    orientation: Optional[Tuple[float, float, float]] = Field(
+        description=(
+            "The model orientation defined as a rotation vector where "
+            "the direction of the vector gives the rotation axis and the "
+            "magnitude of the vector gives the rotation angle in radians. Setting "
+            "this to null or an empty list will cause parakeet to give a zero orientation"
+        ),
+        examples=[
+            "orienation: null # Assign [0, 0, 0] orienation",
+            "orienation: [1, 2, 3] # Assign known orienation",
+        ],
+    )
+
 
 class LocalMolecule(BaseModel):
     """
     A model to describe a local molecule and its instances
 
     """
 
@@ -341,15 +369,16 @@
     energy_spread: float = Field(2.66e-6, description="The energy spread (dE/E)")
 
     acceleration_voltage_spread: float = Field(
         0.8e-6, description="The acceleration voltage spread (dV/V)"
     )
 
     electrons_per_angstrom: float = Field(
-        30, description="The number of electrons per square angstrom"
+        140,
+        description="The number of electrons per square angstrom. This is the dose per image (across all fractions).",
     )
 
     illumination_semiangle: float = Field(
         0.02, description="The illumination semiangle (mrad)."
     )
 
     theta: float = Field(0, description="The beam tilt theta angle (deg)")
@@ -409,14 +438,17 @@
         0, description="The Azimuthal angle of 5th order rosette aberration (rad)"
     )
     c_56: float = Field(0, description="The 6-fold astigmatism (A)")
     phi_56: float = Field(
         0, description="The Azimuthal angle of 6-fold astigmatism (rad)"
     )
 
+    inner_aper_ang: float = Field(0, description="The inner aperture angle")
+    outer_aper_ang: float = Field(0, description="The outer aperture angle")
+
     c_c: float = Field(2.7, description="The chromatic aberration (mm)")
 
     current_spread: float = Field(0.33e-6, description="The current spread (dI/I)")
 
 
 class Detector(BaseModel):
     """
@@ -443,29 +475,44 @@
 
     """
 
     krios = "krios"
     talos = "talos"
 
 
+class PhasePlate(BaseModel):
+    """
+    A model to describe the phase plate
+
+    """
+
+    use: bool = Field(False, description="Use the phase plate")
+
+    phase_shift: float = Field(90, description="The phase shift (degrees)")
+
+    radius: float = Field(0.005, gt=0, description="The spot radius (1/A)")
+
+
 class Microscope(BaseModel):
     """
     A model to describe the microscope
 
     """
 
     model: MicroscopeModel = Field(
         None, description="Use parameters for a given microscope model"
     )
 
     beam: Beam = Field(Beam(), description="The beam model parameters")
 
     lens: Lens = Field(Lens(), description="The lens model parameters")
 
-    phase_plate: bool = Field(False, description="Use a phase plate (True/False)")
+    phase_plate: PhasePlate = Field(
+        PhasePlate(), description="The phase plate parameters"
+    )
 
     detector: Detector = Field(Detector(), description="The detector model parameters")
 
 
 class ScanMode(str, Enum):
     """
     An enumeration to describe the scan mode
@@ -476,25 +523,32 @@
     still = "still"
     tilt_series = "tilt_series"
     dose_symmetric = "dose_symmetric"
     single_particle = "single_particle"
     helical_scan = "helical_scan"
     nhelix = "nhelix"
     beam_tilt = "beam_tilt"
+    grid_scan = "grid_scan"
 
 
 class Drift(BaseModel):
     """
     A model to describe the beam drift
 
     """
 
-    magnitude: float = Field(0, description="The magnitude of the drift (A)")
-
-    kernel_size: int = Field(0, description="How much to smooth the drift")
+    x: Union[float, Tuple[float, float]] = Field(
+        0, description="The model for the x drift a + b*theta**4 (A)"
+    )
+    y: Union[float, Tuple[float, float]] = Field(
+        0, description="The model for the y drift a + b*theta**4 (A)"
+    )
+    z: Union[float, Tuple[float, float]] = Field(
+        0, description="The model for the z drift a + b*theta**4 (A)"
+    )
 
 
 class Scan(BaseModel):
     """
     A model to describe the scan
 
     """
@@ -505,23 +559,40 @@
         (0, 1, 0), description="The scan axis vector"
     )
 
     start_angle: float = Field(0, description="The start angle for the rotation (deg)")
 
     step_angle: float = Field(0, description="The step angle for the rotation (deg)")
 
-    start_pos: float = Field(
+    start_pos: Union[float, Tuple[float, float]] = Field(
         0, description="The start position for a translational scan (A)"
     )
 
-    step_pos: Union[float, Auto] = Field(
+    step_pos: Union[float, Tuple[float, float], Auto] = Field(
         "auto", description="The step distance for a translational scan (A)"
     )
 
-    num_images: int = Field(1, description="The number of images to simulate")
+    num_images: Union[int, Tuple[int, int]] = Field(
+        1,
+        description=(
+            "The number of images to simulate. "
+            "For a tilt series this is the number of tilt steps. "
+            "If num_fractions is also set to something other than 1, "
+            "then there will be num_fractions number of 'movie frames' per 'image'"
+        ),
+    )
+
+    num_fractions: int = Field(
+        1,
+        description=(
+            "The number of movie frames. This refers to the frames of the micrograph 'movies'. "
+            "For a tilt series, all these images will be at the same step and the dose for a 'single image' "
+            "will be fractionated over these image frames"
+        ),
+    )
 
     num_nhelix: int = Field(1, description="The number of scans in an n-helix")
 
     exposure_time: float = Field(1, description="The exposure time per image (s)")
 
     angles: Optional[List[float]] = Field(
         None,
@@ -609,15 +680,21 @@
     mp_loss_width: float = Field(None, description="The MPL energy filter width")
 
     mp_loss_position: MPLPosition = Field(
         "peak", description="The MPL energy filter position"
     )
 
     sensitivity_coefficient: float = Field(
-        0.022, description="The radiation damage model sensitivity coefficient"
+        0.022,
+        description=(
+            "The radiation damage model sensitivity coefficient. "
+            "This value relates the value of an isotropic B factor to the number of "
+            "incident electrons. Typical values for this (calibrated from X-ray and EM data) "
+            "range between 0.02 and 0.08 where a higher value will result in a larger B factor."
+        ),
     )
 
 
 class ClusterMethod(str, Enum):
     """
     An enumeration to describe the cluster method
 
@@ -742,15 +819,19 @@
 
     # Set items to include in output
     if full:
         include = None
     else:
         include = {
             "microscope": {
-                "beam": {"electrons_per_angstrom", "energy", "illumination_semiangle"},
+                "beam": {
+                    "electrons_per_angstrom",
+                    "energy",
+                    "illumination_semiangle",
+                },
                 "detector": {
                     "nx",
                     "ny",
                     "pixel_size",
                 },
                 "lens": {
                     "c_10",
@@ -811,24 +892,47 @@
     # Save the config
     save(config, out_filename, exclude_unset=True)
 
     # Return config
     return config
 
 
-def show(config: Config, full: bool = False):
+def show(config: Config, full: bool = False, schema: str = None):
     """
     Print the command line arguments
 
     Args:
         config: The configuration object
         full: Show the full configuration (True or False)
+        schema: Show the schema
 
     """
-    return yaml.safe_dump(config.dict(exclude_unset=not full), indent=4)
+    if schema:
+        if schema in ["."]:
+            d = config.schema()
+        elif schema.startswith("/definitions/"):
+            schema = os.path.basename(schema)
+            try:
+                d = config.schema()["definitions"][schema]
+            except Exception as e:
+                raise RuntimeError(
+                    "Unable to find definition '%s' in\n%s"
+                    % (
+                        schema,
+                        "\n".join(
+                            " - %s" % v
+                            for v in sorted(config.schema()["definitions"].keys())
+                        ),
+                    )
+                )
+        else:
+            raise RuntimeError("Unknown scheme value '%s' (see help)" % schema)
+    else:
+        d = config.dict(exclude_unset=not full)
+    return yaml.safe_dump(d, indent=4)
 
 
 def deepmerge(a: dict, b: dict) -> dict:
     """
     Perform a deep merge of two dictionaries
 
     Args:
```

### Comparing `python-parakeet-0.4.3/src/parakeet/data/__init__.py` & `python-parakeet-0.4.4/src/parakeet/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 
     """
 
     cache = {}
 
     # Check local and cache directories
     for directory in [get_local_path(), get_cache_path()]:
-
         # Create the directory if not exists
         if not os.path.exists(directory):
             os.mkdir(directory)
 
         # Check all the files in the directory for CIF and PDB files
         for filename in os.listdir(directory):
             if filename.endswith(".cif") or filename.endswith(".pdb"):
```

### Comparing `python-parakeet-0.4.3/src/parakeet/data/files/3jb9.cif` & `python-parakeet-0.4.4/src/parakeet/data/files/3jb9.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/data/files/4v1w.cif` & `python-parakeet-0.4.4/src/parakeet/data/files/4v1w.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/data/files/4v5d.cif` & `python-parakeet-0.4.4/src/parakeet/data/files/4v5d.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/data/files/6qt9.cif` & `python-parakeet-0.4.4/src/parakeet/data/files/6qt9.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/data/files/6z6u.pdb` & `python-parakeet-0.4.4/src/parakeet/data/files/6z6u.pdb`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/data/files/water.cif` & `python-parakeet-0.4.4/src/parakeet/data/files/water.cif`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/detector.py` & `python-parakeet-0.4.4/src/parakeet/detector.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/dqe.py` & `python-parakeet-0.4.4/src/parakeet/dqe.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/error.h` & `python-parakeet-0.4.4/src/parakeet/error.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/freeze/__init__.py` & `python-parakeet-0.4.4/src/parakeet/freeze/__init__.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/freeze/freeze_ext.cc` & `python-parakeet-0.4.4/src/parakeet/freeze/freeze_ext.cc`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/freeze/sphere_packer.h` & `python-parakeet-0.4.4/src/parakeet/freeze/sphere_packer.h`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/futures.py` & `python-parakeet-0.4.4/src/parakeet/futures.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         max_workers (int): The number of worker processes
 
     """
     import dask_jobqueue
     import dask.distributed
 
     if method == "sge":
-
         # Create the SGECluster object
         # For each worker:
         #   - request 1 gpu and 1 core
         #   - use 1 process per worker and 1 thread per process
         # This ensures that only 1 job will be run on each worker at any time
         # which is required to ensure that there is not any competition for
         # gpu resources (by default dask will try to run many jobs at the same
```

### Comparing `python-parakeet-0.4.3/src/parakeet/inelastic.py` & `python-parakeet-0.4.4/src/parakeet/inelastic.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/io.py` & `python-parakeet-0.4.4/src/parakeet/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
-import functools
 import h5py
 import numpy as np
 import mrcfile
 import os
 import PIL.Image
 import parakeet
-from math import pi
 
 try:
     FEI_EXTENDED_HEADER_DTYPE = mrcfile.dtypes.FEI1_EXTENDED_HEADER_DTYPE
 except Exception:
     FEI_EXTENDED_HEADER_DTYPE = mrcfile.dtypes.get_ext_header_dtype(b"FEI1")
 
-
 METADATA_DTYPE = np.dtype(
     [
         #
         # General parameters
         #
         ("application", "S16"),
         ("application_version", "S16"),
         ("timestamp", "f8"),
         #
+        # Scan parameters
+        #
+        ("image_number", "i4"),
+        ("fraction_number", "i4"),
+        #
         # Stage parameters
         #
         ("tilt_alpha", "f8"),
         ("tilt_axis_x", "f8"),
         ("tilt_axis_y", "f8"),
         ("tilt_axis_z", "f8"),
         ("stage_x", "f8"),
@@ -243,47 +245,36 @@
 
 class Header(object):
     """
     An object to represent the header
 
     """
 
-    @functools.singledispatchmethod
     def __getitem__(self, item):
         """
         Get a row or column item
 
         """
-        return Row(self, item)
-
-    @__getitem__.register
-    def _(self, item: str):
-        """
-        Get a row or column item
-
-        """
-        return Column(self, item)
+        if isinstance(item, str):
+            Class = Column
+        else:
+            Class = Row
+        return Class(self, item)
 
-    @functools.singledispatchmethod
     def __setitem__(self, item, value):
         """
         Set a row or column item
 
         """
-        row = Row(self, item)
-        row.assign(value)
-
-    @__setitem__.register
-    def _(self, item: str, value):
-        """
-        Set a row or column item
-
-        """
-        col = Column(self, item)
-        col[:] = value
+        if isinstance(item, str):
+            col = Column(self, item)
+            col[:] = value
+        else:
+            row = Row(self, item)
+            row.assign(value)
 
     def rows(self):
         """
         Get a row iterator
 
         """
         for i in range(self.size):
@@ -369,19 +360,19 @@
 
         """
 
         # Get the metadata
         metadata = np.array(self)
 
         # Construct the orientation
-        orientation = np.stack(
+        axis = np.stack(
             [
-                metadata["tilt_axis_x"] * metadata["tilt_alpha"] * pi / 180.0,
-                metadata["tilt_axis_y"] * metadata["tilt_alpha"] * pi / 180.0,
-                metadata["tilt_axis_z"] * metadata["tilt_alpha"] * pi / 180.0,
+                metadata["tilt_axis_x"],
+                metadata["tilt_axis_y"],
+                metadata["tilt_axis_z"],
             ]
         ).T
 
         # Construct the shift
         shift = np.stack(
             [metadata["shift_x"], metadata["shift_y"], metadata["stage_z"]]
         ).T
@@ -393,15 +384,18 @@
                 metadata["shift_offset_y"],
                 metadata["stage_offset_z"],
             ]
         ).T
 
         # Return a scan object
         return parakeet.scan.Scan(
-            orientation=orientation,
+            image_number=metadata["image_number"],
+            fraction_number=metadata["fraction_number"],
+            axis=axis,
+            angle=metadata["tilt_alpha"],
             shift=shift,
             shift_delta=shift_delta,
             beam_tilt_theta=metadata["theta"],
             beam_tilt_phi=metadata["phi"],
             exposure_time=metadata["exposure_time"],
         )
 
@@ -495,14 +489,19 @@
             #
             # General parameters
             #
             "application": "Application",
             "application_version": "Application version",
             "timestamp": "Timestamp",
             #
+            # Scan parameters
+            #
+            "image_number": "Start frame",
+            "fraction_number": "Fraction number",
+            #
             # Stage parameters
             #
             "tilt_alpha": "Alpha tilt",
             "tilt_axis_angle": "Tilt axis angle",
             "stage_x": "X-Stage",
             "stage_y": "Y-Stage",
             "stage_z": "Z-Stage",
@@ -679,14 +678,56 @@
         """
         Get the size of the header
 
         """
         return self._handle["data"].shape[0]
 
 
+class ImageHeader(Header):
+    """
+    A sub class for an image header
+
+    """
+
+    def __init__(self, handle):
+        self._handle = handle
+
+    def mapping(self, key):
+        """
+        Get the mapping between names
+
+        """
+        assert key in self.dtype.fields
+        return key
+
+    def get(self, index, key):
+        """
+        Get the mapping between names
+
+        """
+        mapping = self.mapping(key)
+        return self._handle[mapping][index]
+
+    def set(self, index, key, value):
+        """
+        Set the value of a property
+
+        """
+        mapping = self.mapping(key)
+        self._handle[mapping][index] = value
+
+    @property
+    def size(self):
+        """
+        Get the size of the header
+
+        """
+        return self._handle.shape[0]
+
+
 class NexusWriter(Writer):
     """
     Write to a nexus file
 
     """
 
     def __init__(self, filename, shape, pixel_size, dtype="float32"):
@@ -766,15 +807,14 @@
         def __init__(self, template, shape=None, vmin=None, vmax=None):
             self.template = template
             self.shape = shape
             self.vmin = vmin
             self.vmax = vmax
 
         def __setitem__(self, item, data):
-
             # Check the input
             assert isinstance(item, tuple)
             assert isinstance(item[1], slice)
             assert isinstance(item[2], slice)
             assert item[1].start is None
             assert item[1].stop is None
             assert item[1].step is None
@@ -818,15 +858,15 @@
 
         """
 
         # Set the proxy data interface
         self._data = ImageWriter.DataProxy(template, shape, vmin, vmax)
 
         # Create dummy arrays for angle and position
-        self._header = np.zeros(shape=shape[0], dtype=METADATA_DTYPE)
+        self._header = ImageHeader(np.zeros(shape=shape[0], dtype=METADATA_DTYPE))
 
     @property
     def vmin(self):
         """
         The vmin property
 
         """
@@ -954,15 +994,15 @@
                 shape=handle.data.shape[0], dtype=FEI_EXTENDED_HEADER_DTYPE
             )
 
         # Set the header
         header = MrcfileHeader(extended_header)
 
         # Get the pixel size
-        pixel_size = handle.voxel_size["x"]
+        pixel_size = float(handle.voxel_size["x"])
 
         # Create the reader
         return Reader(
             handle,
             handle.data,
             header,
             pixel_size,
```

### Comparing `python-parakeet-0.4.3/src/parakeet/landau.py` & `python-parakeet-0.4.4/src/parakeet/landau.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/lens.py` & `python-parakeet-0.4.4/src/parakeet/lens.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/src/parakeet/metadata.py` & `python-parakeet-0.4.4/src/parakeet/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,14 @@
     def write_manual_pick_files(self):
         """
         Write out a star file with picking metadata
 
         """
 
         for i in range(1, self.config.scan.num_images + 1):
-
             # Create the dictionary
             data = {
                 "picking": pd.DataFrame.from_dict(
                     {
                         "rlnCoordinateX": 0,
                         "rlnCoordinateY": 0,
                         "rlnClassNumber": 1,
@@ -233,18 +232,18 @@
     # Load the configuration
     config = parakeet.config.load(config_file)
 
     # Open the sample
     sample = Sample(sample_file, mode="r")
 
     # Export the metadata
-    return _export_Config(config, sample)
+    return _export_Config(config, sample, directory, relion)
 
 
-@export.register
+@export.register(parakeet.config.Config)
 def _export_Config(
     config: parakeet.config.Config,
     sample: Sample,
     directory: str = ".",
     relion: bool = True,
 ):
     """
```

### Comparing `python-parakeet-0.4.3/src/parakeet/microscope.py` & `python-parakeet-0.4.4/src/parakeet/microscope.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,34 +4,52 @@
 # Copyright (C) 2019 Diamond Light Source and Rosalind Franklin Institute
 #
 # Author: James Parkhurst
 #
 # This code is distributed under the GPLv3 license, a copy of
 # which is included in the root directory of this package.
 #
+import numpy as np
 import parakeet.config
 import parakeet.beam
 import parakeet.detector
 import parakeet.lens
 from typing import Optional
+from math import pi
+
+
+class PhasePlate(object):
+    """
+    A class to encapsulate a phase plate
+
+    """
+
+    def __init__(self, use=False, phase_shift=0.5 * pi, radius=0.005):
+        """
+        Init the phase plate
+
+        """
+        self.use = use
+        self.phase_shift = phase_shift
+        self.radius = radius
 
 
 class Microscope(object):
     """
     A class to encapsulate a microscope
 
     """
 
     def __init__(
         self,
         model: parakeet.config.MicroscopeModel = None,
         beam: parakeet.beam.Beam = parakeet.beam.Beam(),
         lens: parakeet.lens.Lens = parakeet.lens.Lens(),
         detector: parakeet.detector.Detector = parakeet.detector.Detector(),
-        phase_plate: bool = False,
+        phase_plate: PhasePlate = PhasePlate(),
     ):
         """
         Initialise the detector
 
         Args:
             model: The microscope model name
             beam: The beam object
@@ -75,15 +93,15 @@
         """
         The detector model
 
         """
         return self._detector
 
     @property
-    def phase_plate(self) -> bool:
+    def phase_plate(self) -> PhasePlate:
         """
         Do we have a phase plate
 
         """
         return self._phase_plate
 
 
@@ -126,9 +144,13 @@
 
     # Return the miroscope object
     return Microscope(
         model=config.model,
         beam=beam,
         lens=lens,
         detector=detector,
-        phase_plate=config.phase_plate,
+        phase_plate=PhasePlate(
+            config.phase_plate.use,
+            np.radians(config.phase_plate.phase_shift),
+            config.phase_plate.radius,
+        ),
     )
```

### Comparing `python-parakeet-0.4.3/src/parakeet/sample/__init__.py` & `python-parakeet-0.4.4/src/parakeet/sample/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from collections import defaultdict
 import h5py
 import gemmi
 import logging
 import numpy as np
 import pandas
 import scipy.constants
+import json
 from math import pi, sqrt, floor, ceil
 from scipy.spatial.transform import Rotation
 
 try:
     import multem
 except ImportError:
     pass
@@ -560,14 +561,17 @@
 
         # Iterate through the atoms
         def iterate_atoms(structure):
             for model_index, model in enumerate(structure):
                 for chain in model:
                     for residue in chain:
                         for atom in residue:
+                            if atom.element.atomic_number <= 0:
+                                print("BAD ELEMENT")
+                                continue
                             assert atom.element.atomic_number > 0
                             yield (
                                 atom.element.atomic_number,
                                 atom.pos.x,
                                 atom.pos.y,
                                 atom.pos.z,
                                 get_atom_sigma(atom),
@@ -1231,15 +1235,14 @@
         z0 = atoms.data["z"].min()
         x1 = atoms.data["x"].max()
         y1 = atoms.data["y"].max()
         z1 = atoms.data["z"].max()
 
         # Check the old bounding box
         if self.number_of_atoms > 0:
-
             # Get the bounding box
             (bx0, by0, bz0), (bx1, by1, bz1) = self.bounding_box
 
             # Get the min/max coords
             x0 = min(x0, bx0)
             y0 = min(y0, by0)
             z0 = min(z0, bz0)
@@ -1321,15 +1324,14 @@
         # Get the reference coords
         reference_coords = atoms.data[["x", "y", "z"]].to_numpy()
 
         # Loop through all the positions and rotations
         for position, rotation, orientation in zip(
             positions, Rotation.from_rotvec(orientations), orientations
         ):
-
             # Make a copy and apply the rotation and translation
             coords = (rotation.apply(reference_coords) + position).astype("float32")
             temp = atoms.data.copy()
             temp["x"] = coords[:, 0]
             temp["y"] = coords[:, 1]
             temp["z"] = coords[:, 2]
 
@@ -1611,14 +1613,42 @@
         """
         Get some sample info
 
         Returns:
             str: Some sample info
 
         """
+
+        class NumpyEncoder(json.JSONEncoder):
+            """Special json encoder for numpy types"""
+
+            def default(self, obj):
+                if isinstance(
+                    obj,
+                    (
+                        np.int_,
+                        np.intc,
+                        np.intp,
+                        np.int8,
+                        np.int16,
+                        np.int32,
+                        np.int64,
+                        np.uint8,
+                        np.uint16,
+                        np.uint32,
+                        np.uint64,
+                    ),
+                ):
+                    return int(obj)
+                elif isinstance(obj, (np.float_, np.float16, np.float32, np.float64)):
+                    return float(obj)
+                elif isinstance(obj, (np.ndarray,)):
+                    return obj.tolist()
+                return json.JSONEncoder.default(self, obj)
+
         lines = [
             "Sample information:",
             "    # Molecules:   %d" % self.number_of_molecules,
             "    # models:      %d" % self.number_of_molecular_models,
             "    # atoms:       %d" % self.number_of_atoms,
             "    Min x:         %.2f" % self.bounding_box[0][0],
             "    Min y:         %.2f" % self.bounding_box[0][1],
@@ -1634,15 +1664,16 @@
             "    Min box z:     %.2f" % self.containing_box[0][2],
             "    Max box x:     %.2f" % self.containing_box[1][0],
             "    Max box y:     %.2f" % self.containing_box[1][1],
             "    Max box z:     %.2f" % self.containing_box[1][2],
             "    Centre x:      %.2f" % self.centre[0],
             "    Centre y:      %.2f" % self.centre[1],
             "    Centre z:      %.2f" % self.centre[2],
-            "    Shape:         %s" % str(self.shape),
+            "    Shape:         %s"
+            % json.dumps(self.shape, cls=NumpyEncoder, indent=2),
         ]
         for name, molecule in self.iter_molecules():
             molecule_lines = [
                 "    Molecule: %s" % name,
                 "        Positions:\n%s"
                 % "\n".join(["%s%s" % (" " * 12, str(p)) for p in molecule[1]]),
                 "        Orientations:\n%s"
@@ -1898,16 +1929,15 @@
         index_z = indices[:, 2]
         assert (indices >= 0).all()
         self.grid[index_x, index_y, index_z] = False
         self.grid = ~self.grid
         # from matplotlib import pylab
         # pylab.imshow(self.grid[:,:,grid_shape[2]//2])
         # pylab.show()
-
-        self.grid = scipy.ndimage.distance_transform_edt(self.grid) < min_distance
+        # self.grid = scipy.ndimage.distance_transform_edt(~self.grid) < min_distance
         return
         # self.grid = scipy.ndimage.morphology.binary_closing(self.grid, iterations=2)
         # self.grid = scipy.ndimage.morphology.binary_fill_holes(self.grid)
         # import mrcfile
 
         # outfile = mrcfile.new("temp.mrc", overwrite=True)
         # outfile.set_data(self.grid.astype("int8"))
```

### Comparing `python-parakeet-0.4.3/src/parakeet/sample/_add_molecules.py` & `python-parakeet-0.4.4/src/parakeet/sample/_add_molecules.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     all_labels = []
     all_radii = []
     all_positions = []
     all_orientations = []
 
     # Generate the orientations and boxes
     for name, value in molecules.items():
-
         # Get the type and instances
         mtype = value["type"]
         items = value["instances"]
 
         # Skip if number is zero
         if len(items) == 0:
             continue
@@ -168,15 +167,14 @@
             shape_volume_object(sample.centre, sample.shape), np.array(all_radii)
         )
 
     # Set the positions and orientations by molecule
     positions = defaultdict(list)
     orientations = defaultdict(list)
     for label, rotation, position in zip(all_labels, all_orientations, all_positions):
-
         # # Get atom data bounds
         # x0 = position - box / 2.0
         # x1 = position + box / 2.0
 
         # # Check the coords
         # assert is_box_inside_shape((x0, x1), sample.centre, sample.shape)
 
@@ -220,15 +218,15 @@
     parakeet.config.show(config)
 
     # Create the sample
     logger.info(f"Writing sample to {sample_file}")
     return _add_molecules_Config(config, sample_file)
 
 
-@add_molecules.register
+@add_molecules.register(parakeet.config.Config)
 def _add_molecules_Config(config: parakeet.config.Config, sample_file: str) -> Sample:
     """
     Take a sample and add a load of molecules
 
     Args:
         config: The sample configuration
         sample_file: The filename of the sample
@@ -240,15 +238,15 @@
     # Open the sample
     sample = Sample(sample_file, mode="r+")
 
     # Do the work
     return _add_molecules_Sample(config.sample, sample)
 
 
-@add_molecules.register
+@add_molecules.register(parakeet.config.Sample)
 def _add_molecules_Sample(config: parakeet.config.Sample, sample: Sample) -> Sample:
     """
     Take a sample and add a load of molecules
 
     Args:
         config: The sample configuration
         sample: The sample object
@@ -264,15 +262,14 @@
 
     # Convert to list of positions/orientations
     temp = {}
     for origin, items in molecules.items():
         if items is None:
             continue
         for item in items:
-
             # Get the key
             if origin == "local":
                 key = item["filename"]
             elif origin == "pdb":
                 key = item["id"]
             else:
                 raise RuntimeError("Unknown origin")
```

### Comparing `python-parakeet-0.4.3/src/parakeet/sample/_mill.py` & `python-parakeet-0.4.4/src/parakeet/sample/_mill.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     parakeet.config.show(config)
 
     # Create the sample
     logger.info(f"Writing sample to {sample_file}")
     return _mill_Config(config, sample_file)
 
 
-@mill.register
+@mill.register(parakeet.config.Config)
 def _mill_Config(config: parakeet.config.Config, sample_file: str) -> Sample:
     """
     Take a sample and add a load of molecules
 
     Args:
         config: The sample configuration
         sample_file: The filename of the sample
@@ -64,15 +64,15 @@
     # Open the sample
     sample = Sample(sample_file, mode="r+")
 
     # Do the work
     return _mill_Sample(config.sample, sample)
 
 
-@mill.register
+@mill.register(parakeet.config.Sample)
 def _mill_Sample(config: parakeet.config.Sample, sample: Sample) -> Sample:
     """
     Mill the sample
 
     Args:
         config: The input config
         sample: The sample model
```

### Comparing `python-parakeet-0.4.3/src/parakeet/sample/_new.py` & `python-parakeet-0.4.4/src/parakeet/sample/_new.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,14 @@
     mass_of_water = (density_of_water * 1000) * (volume * 1e-10**3)  # g
     number_of_waters = int(
         floor((mass_of_water / molar_mass_of_water) * avogadros_number)
     )
 
     # Uniform random or packed
     if not pack:
-
         # The water filename
         filename = parakeet.data.get_path("water.cif")
 
         # Get the water coords
         single_water = parakeet.sample.AtomData.from_ligand_file(filename)
         atoms = single_water.data[0:3]
         water_coords = atoms[["x", "y", "z"]].copy()
@@ -165,15 +164,14 @@
 
         # Rotate the Hydrogens around the Oxygen and translate
         O = rotation.apply(water_coords.iloc[0].copy()) + translation
         H1 = rotation.apply(water_coords.iloc[1].copy()) + translation
         H2 = rotation.apply(water_coords.iloc[2].copy()) + translation
 
         def create_atom_data(atomic_number, coords):
-
             # Create a new array
             def new_array(size, name, value):
                 return (
                     np.zeros(
                         shape=(size,), dtype=parakeet.sample.AtomData.column_data[name]
                     )
                     + value
@@ -203,15 +201,14 @@
         data_buffer.append(create_atom_data(8, O))
         data_buffer.append(create_atom_data(1, H1))
         data_buffer.append(create_atom_data(1, H2))
 
         sample.add_atoms(AtomData(data=pandas.concat(data_buffer, ignore_index=True)))
 
     else:
-
         # Van der Waals radius of water
         van_der_waals_radius = 2.7 / 2.0  # A
 
         # Compute the total volume in the spheres
         volume_of_spheres = (
             (4.0 / 3.0) * pi * van_der_waals_radius**3 * number_of_waters
         )
@@ -252,15 +249,14 @@
 
         # Extract all the data
         logger.info("Generating water positions:")
         start_time = time.time()
         max_buffer = 10_000_000
         data_buffer = []
         for x_index, x_slice in enumerate(packer):
-
             # Read the coordinates. The packer goes along the z axis so we need to
             # flip the coordinates since we want x slices
             coords = []
             for node in x_slice:
                 coords.extend(node)
             coords = np.flip(np.array(coords, dtype="float32"), axis=1) + offset
 
@@ -273,15 +269,14 @@
 
             # Rotate the Hydrogens around the Oxygen and translate
             O = rotation.apply(water_coords.iloc[0].copy()) + coords
             H1 = rotation.apply(water_coords.iloc[1].copy()) + coords
             H2 = rotation.apply(water_coords.iloc[2].copy()) + coords
 
             def create_atom_data(atomic_number, coords):
-
                 # Create a new array
                 def new_array(size, name, value):
                     return (
                         np.zeros(shape=(size,), dtype=AtomData.column_data[name])
                         + value
                     )
 
@@ -362,15 +357,15 @@
     parakeet.config.show(config)
 
     # Create the sample
     logger.info(f"Writing sample to {sample_file}")
     return _new_Config(config, sample_file)
 
 
-@new.register
+@new.register(parakeet.config.Config)
 def _new_Config(config: parakeet.config.Config, filename: str) -> Sample:
     """
     Create the sample
 
     Args:
         config: The sample configuration
         filename: The filename of the sample
@@ -378,15 +373,15 @@
     Returns:
         The sample object
 
     """
     return _new_Sample(config.sample, filename)
 
 
-@new.register
+@new.register(parakeet.config.Sample)
 def _new_Sample(config: parakeet.config.Sample, filename: str) -> Sample:
     """
     Create the sample
 
     Args:
         config: The sample configuration
         filename: The filename of the sample
@@ -418,20 +413,30 @@
 
     # Add atoms from coordinates file
     if coords is not None and coords.filename is not None:
         atoms = AtomData.from_gemmi_file(coords.filename)
         if coords.recentre:
             atoms.data = recentre(atoms.data)
             position = sample.centre
+            orientation = (0, 0, 0)
         else:
             position = (0, 0, 0)
+            orientation = (0, 0, 0)
+        if coords.position:
+            position = coords.position  # type: ignore
+        if coords.orientation:
+            orientation = coords.orientation  # type: ignore
+        if coords.scale != 1.0:
+            atoms.data["x"] = atoms.data["x"] * coords.scale
+            atoms.data["y"] = atoms.data["y"] * coords.scale
+            atoms.data["z"] = atoms.data["z"] * coords.scale
 
         # Add the molecule
         sample.add_molecule(
-            atoms, positions=[position], orientations=[(0, 0, 0)], name=None
+            atoms, positions=[position], orientations=[orientation], name=None
         )
 
     # Print some info
     logger.info(sample.info())
 
     # Get the sample
     return sample
```

### Comparing `python-parakeet-0.4.3/src/parakeet/sample/_sputter.py` & `python-parakeet-0.4.4/src/parakeet/sample/_sputter.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parakeet.config.show(config)
 
     # Create the sample
     logger.info(f"Writing sample to {sample_file}")
     return _sputter_Config(config, sample_file)
 
 
-@sputter.register
+@sputter.register(parakeet.config.Config)
 def _sputter_Config(config: parakeet.config.Config, sample_file: str) -> Sample:
     """
     Take a sample and add a load of molecules
 
     Args:
         config: The sample configuration
         sample_file: The filename of the sample
@@ -70,15 +70,15 @@
     if config.sample.sputter:
         sample = _sputter_Sputter(config.sample.sputter, sample)
     else:
         logger.info("No sputter parameters found in config")
     return sample
 
 
-@sputter.register
+@sputter.register(parakeet.config.Sputter)
 def _sputter_Sputter(config: parakeet.config.Sputter, sample: Sample) -> Sample:
     """
     Add a sputter coating to the sample of the desired thickness
 
     This is very crude and adds atoms at random positions
 
     Params:
@@ -175,15 +175,14 @@
         print("Placed %d atoms" % number_of_atoms)
         print("WARNING - ONLY APPLYING TO TOP OF SAMPLE")
     else:
         raise RuntimeError("Not implemented")
     position = np.array((x, y, z)).T
 
     def create_atom_data(atomic_number, coords):
-
         # Create a new array
         def new_array(size, name, value):
             return (
                 np.zeros(
                     shape=(size,), dtype=parakeet.sample.AtomData.column_data[name]
                 )
                 + value
```

### Comparing `python-parakeet-0.4.3/src/parakeet/sample/distribute.py` & `python-parakeet-0.4.4/src/parakeet/sample/distribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,14 @@
         length_z = cuboid["length_z"]
         length = np.array((length_x, length_y, length_z))
         lower = np.array(centre) - length / 2.0
         upper = lower + length
         return CuboidVolume(lower, upper)
 
     def make_cylinder_volume(centre, cylinder):
-
         # Get the cylinder params
         length = cylinder["length"]
         radius = cylinder["radius"]
         offset_x = cylinder.get("offset_x", None)
         offset_z = cylinder.get("offset_z", None)
         axis = cylinder.get("axis", (0, 1, 0))
         assert np.all(np.equal(axis, (0, 1, 0)))
@@ -291,15 +290,14 @@
 
     Returns:
         list: A list of centre positions
 
     """
 
     def update(volume, position, radius, max_iterations):
-
         assert len(position) == len(radius)
 
         # Get the initial velocities
         size = 3 * np.std(position, axis=0)
         velocity = 0.01 * np.random.uniform(-size / 2, size / 2, size=position.shape)
 
         # Set the box elasticity
@@ -319,15 +317,14 @@
         epsilon = 1e-6
 
         # Set the time step
         dt = 0.1
 
         # Loop through the iterations
         for t in range(max_iterations):
-
             # Update the current position
             position += velocity * dt
 
             # Add some resistance to damp the velocity
             velocity -= velocity * resistance
 
             # Reflect particle if outside box
@@ -346,15 +343,14 @@
             s = j_list > i_list
             i_list = i_list[s]
             j_list = j_list[s]
             print("Step: %d/%d; # overlaps: %d" % (t + 1, max_iterations, len(i_list)))
 
             # Loop through the overlaps and calculate an elastic collision
             for i, j in zip(i_list, j_list):
-
                 # Compute the distance between the position and min separation
                 dp = position[i] - position[j]
                 dr2 = np.sum(dp**2) + epsilon**2
                 dr = np.sqrt(dr2)
                 d = (radius[i] + radius[j]) * 1.01
 
                 # Update the velocity of the particles
```

### Comparing `python-parakeet-0.4.3/src/parakeet/scan.py` & `python-parakeet-0.4.4/src/parakeet/scan.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,67 +20,103 @@
     """
     A scan of angles around a single rotation axis.
 
     """
 
     def __init__(
         self,
-        orientation: np.ndarray = None,
+        image_number: np.ndarray = None,
+        fraction_number: np.ndarray = None,
+        axis: np.ndarray = None,
+        angle: np.ndarray = None,
         shift: np.ndarray = None,
         shift_delta: np.ndarray = None,
         beam_tilt_theta: np.ndarray = None,
         beam_tilt_phi: np.ndarray = None,
+        electrons_per_angstrom: np.ndarray = None,
         exposure_time: float = 1,
         is_uniform_angular_scan: bool = False,
     ):
         """
         Initialise the scan
 
         """
         self.is_uniform_angular_scan = is_uniform_angular_scan
 
-        if orientation is None:
-            orientation = np.array([[0, 0, 0]])
+        if image_number is None:
+            image_number = np.array([0])
+
+        if fraction_number is None:
+            fraction_number = np.zeros(len(image_number))
+
+        if axis is None:
+            axis = np.zeros((len(image_number), 3))
+
+        if angle is None:
+            angle = np.zeros(len(image_number))
 
         if shift is None:
-            shift = np.zeros((len(orientation), 3))
+            shift = np.zeros((len(image_number), 3))
 
         if shift_delta is None:
-            shift_delta = np.zeros((len(orientation), 3))
+            shift_delta = np.zeros((len(image_number), 3))
 
         if beam_tilt_theta is None:
-            beam_tilt_theta = np.zeros(len(orientation))
+            beam_tilt_theta = np.zeros(len(image_number))
 
         if beam_tilt_phi is None:
-            beam_tilt_phi = np.zeros(len(orientation))
+            beam_tilt_phi = np.zeros(len(image_number))
+
+        if electrons_per_angstrom is None:
+            electrons_per_angstrom = np.ones(len(image_number))
 
         self.data = pd.DataFrame(
             data={
-                "orientation_x": orientation[:, 0],
-                "orientation_y": orientation[:, 1],
-                "orientation_z": orientation[:, 2],
+                "image_number": image_number,
+                "fraction_number": fraction_number,
+                "axis_x": axis[:, 0],
+                "axis_y": axis[:, 1],
+                "axis_z": axis[:, 2],
+                "angle": angle * pi / 180,
                 "shift_x": shift[:, 0],
                 "shift_y": shift[:, 1],
                 "shift_z": shift[:, 2],
                 "shift_delta_x": shift_delta[:, 0],
                 "shift_delta_y": shift_delta[:, 1],
                 "shift_delta_z": shift_delta[:, 2],
                 "beam_tilt_theta": beam_tilt_theta,
                 "beam_tilt_phi": beam_tilt_phi,
-                "exposure_time": np.ones(len(orientation)) * exposure_time,
+                "electrons_per_angstrom": electrons_per_angstrom,
+                "exposure_time": np.ones(len(axis)) * exposure_time,
             }
         )
 
     @property
+    def image_number(self) -> np.ndarray:
+        """
+        Get the image number
+
+        """
+        return self.data["image_number"]
+
+    @property
+    def fraction_number(self) -> np.ndarray:
+        """
+        Get the movie fraction number
+
+        """
+        return self.data["fraction_number"]
+
+    @property
     def orientation(self) -> np.ndarray:
         """
         Get the orientations
 
         """
-        return np.array(self.data[["orientation_x", "orientation_y", "orientation_z"]])
+        return self.axes * np.array(self.data["angle"])[:, np.newaxis]
 
     @property
     def shift(self) -> np.ndarray:
         """
         Get the shifts
 
         """
@@ -107,14 +143,22 @@
         """
         Get the beam tilt phi angles
 
         """
         return self.data["beam_tilt_phi"]
 
     @property
+    def electrons_per_angstrom(self) -> np.ndarray:
+        """
+        Get the dose
+
+        """
+        return self.data["electrons_per_angstrom"]
+
+    @property
     def exposure_time(self) -> np.ndarray:
         """
         Get the exposure times
 
         """
         return self.data["exposure_time"]
 
@@ -128,30 +172,23 @@
 
     @property
     def angles(self) -> np.ndarray:
         """
         Get the angles
 
         """
-        n = np.linalg.norm(self.orientation, axis=1)
-        d = np.dot(self.orientation, np.array([0, 1, 0]))
-        return n * np.sign(d) * 180.0 / pi
+        return self.data["angle"] * 180.0 / pi
 
     @property
     def axes(self) -> np.ndarray:
         """
         Get the axes
 
         """
-        n = np.linalg.norm(self.orientation, axis=1)
-        d = np.dot(self.orientation, np.array([0, 1, 0]))
-        s = n > 0
-        n[s] = 1.0 / n[s]
-        n = n * np.sign(d)
-        return self.orientation * n[:, np.newaxis]
+        return np.array(self.data[["axis_x", "axis_y", "axis_z"]])
 
     @property
     def euler_angles(self) -> np.ndarray:
         """
         Euler angle representation of the orientations.
 
         The Euler angles are intrinsic, right handed rotations around ZYZ.
@@ -172,63 +209,94 @@
     """
     A Factory class to generate scans
 
     """
 
     @classmethod
     def _generate_drift(
-        Class, num_images: int, magnitude: float = 0, kernel_size: int = 0
+        Class,
+        angles: np.ndarray,
+        x: Union[float, tuple] = 0,
+        y: Union[float, tuple] = 0,
+        z: Union[float, tuple] = 0,
     ) -> np.ndarray:
         """
         Get the beam drift
 
         """
 
-        # Generate some random noise
-        drift = np.random.normal(0, magnitude, size=(num_images, 3))
+        # Check type
+        if isinstance(x, float):
+            x = tuple([x, 0.0])
+        if isinstance(y, float):
+            y = tuple([y, 0.0])
+        if isinstance(z, float):
+            z = tuple([z, 0.0])
+
+        # Compute the sigma of the normal in x, y, z
+        x_sigma = x[0] + x[1] * (angles * np.pi / 180.0) ** 4
+        y_sigma = y[0] + x[1] * (angles * np.pi / 180.0) ** 4
+        z_sigma = z[0] + x[1] * (angles * np.pi / 180.0) ** 4
 
-        # Optionally smooth the noise
-        if kernel_size > 0:
-            kernel_size = min(kernel_size, num_images)
-            kernel = np.ones(kernel_size) / kernel_size
-            drift = np.apply_along_axis(
-                lambda m: np.convolve(m, kernel, mode="same"), axis=0, arr=drift
-            )
+        # Generate some random noise
+        drift = np.random.normal(0, [x_sigma, y_sigma, z_sigma]).T
 
         # Return the drift
         return drift
 
     @classmethod
     def _rotvec_from_axis_and_angles(
         Class, axis: np.ndarray, angles: np.ndarray
-    ) -> np.ndarray:
+    ) -> tuple:
         """
         Generate the rotvec
 
         """
         axis = axis / np.linalg.norm(axis)
-        angles = angles * pi / 180.0
-        return np.array([axis * a for a in angles])
+        return np.array([axis for a in angles]), angles
+
+    @classmethod
+    def _axis_angle_from_rotvec(Class, orientation) -> tuple:
+        """
+        Get the axis and angle from the rotvec
+
+        """
+        n = np.linalg.norm(orientation, axis=1)
+        d = np.dot(orientation, np.array([0, 1, 0]))
+        angle = n * np.sign(d) * 180 / pi
+        s = n > 0
+        n[s] = 1.0 / n[s]
+        n = n * np.sign(d)
+        axis = orientation * n[:, np.newaxis]
+        return axis, angle
 
     @classmethod
     def _shift_from_axis_and_positions(
         Class, axis: np.ndarray, positions: np.ndarray
     ) -> np.ndarray:
         """
         Generate the shifts
 
         """
-        return np.array([axis * p for p in positions])
+        if len(positions.shape) == 1:
+            positions = axis * positions[:, np.newaxis]
+        else:
+            assert len(positions.shape) == 2
+            z = np.zeros((positions.shape[0], 1))
+            positions = np.append(positions, z, axis=1)
+        return positions
 
     @classmethod
     def single_axis(
         Class,
         axis: Union[np.ndarray, tuple] = (0, 1, 0),
         angles: np.ndarray = None,
         positions: np.ndarray = None,
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a single axis scan
 
@@ -237,41 +305,59 @@
         # Check input
         if angles is None:
             angles = np.array([])
         if positions is None:
             positions = np.array([])
         assert angles is not None
         assert positions is not None
+        assert len(angles) == len(positions)
         num_images = len(angles)
 
         # Create the orientation and shift
-        orientation = Class._rotvec_from_axis_and_angles(np.array(axis), angles)
+        axis, angle = Class._rotvec_from_axis_and_angles(np.array(axis), angles)
         shift = Class._shift_from_axis_and_positions(np.array(axis), positions)
 
+        # Set the image number and frame number
+        image_number = np.arange(num_images)
+        fraction_number = np.arange(num_fractions)
+        fraction_number = np.repeat([fraction_number], num_images, axis=0).flatten()
+
+        # Duplicate for the number of movie frames per step
+        image_number = np.repeat(image_number, num_fractions, axis=0)
+        axis = np.repeat(axis, num_fractions, axis=0)
+        angle = np.repeat(angle, num_fractions, axis=0)
+        shift = np.repeat(shift, num_fractions, axis=0)
+        dose = np.full(angle.shape, electrons_per_angstrom / num_fractions)
+
         # Create the shift delta
         shift_delta = None
         if drift is not None:
-            shift_delta = Class._generate_drift(
-                num_images, drift["magnitude"], drift["kernel_size"]
-            )
+            shift_delta = Class._generate_drift(angles, **drift)
+            shift_delta = np.repeat(shift_delta, num_fractions, axis=0)
 
         # Create the scan object
         return Scan(
-            orientation=orientation,
+            image_number=image_number,
+            fraction_number=fraction_number,
+            axis=np.array(axis),
+            angle=angle,
             shift=shift,
             shift_delta=shift_delta,
+            electrons_per_angstrom=dose,
             exposure_time=exposure_time,
         )
 
     @classmethod
     def manual(
         Class,
         axis: tuple = (0, 1, 0),
         angles: np.ndarray = None,
         positions: np.ndarray = None,
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a manual scan with custom angles and positions
 
@@ -291,50 +377,59 @@
         positions = np.array(positions)
 
         # Create the single axis scan
         return Class.single_axis(
             axis=axis,
             angles=angles,
             positions=positions,
+            num_fractions=num_fractions,
+            electrons_per_angstrom=electrons_per_angstrom,
             exposure_time=exposure_time,
             drift=drift,
         )
 
     @classmethod
     def still(
         Class,
         axis: tuple = (0, 1, 0),
         start_angle: float = 0,
         start_pos: float = 0,
+        num_images: int = 1,
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a still image scan
 
         """
-        angles = np.array([start_angle])
-        positions = np.array([start_pos])
+        angles = np.repeat(start_angle, num_images)
+        positions = np.repeat(start_pos, num_images)
         return Class.single_axis(
             axis=axis,
             angles=angles,
             positions=positions,
+            num_fractions=num_fractions,
+            electrons_per_angstrom=electrons_per_angstrom,
             exposure_time=exposure_time,
             drift=drift,
         )
 
     @classmethod
     def tilt_series(
         Class,
         axis: tuple = (0, 1, 0),
         start_angle: float = 0,
         step_angle: float = 0,
         start_pos: float = 0,
         num_images: int = 1,
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a continuous single axis scan
 
@@ -345,26 +440,30 @@
         positions = np.full(len(angles), start_pos)
 
         # Create the scan
         return Class.single_axis(
             axis=axis,
             angles=angles,
             positions=positions,
+            num_fractions=num_fractions,
+            electrons_per_angstrom=electrons_per_angstrom,
             exposure_time=exposure_time,
             drift=drift,
         )
 
     @classmethod
     def dose_symmetric(
         Class,
         axis: tuple = (0, 1, 0),
         start_angle: float = 0,
         step_angle: float = 0,
         start_pos: float = 0,
         num_images: int = 1,
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a dose symmetric single axis scan
 
@@ -375,27 +474,31 @@
         positions = np.full(len(angles), start_pos)
 
         # Create the scan
         return Class.single_axis(
             axis=axis,
             angles=angles,
             positions=positions,
+            num_fractions=num_fractions,
+            electrons_per_angstrom=electrons_per_angstrom,
             exposure_time=exposure_time,
             drift=drift,
         )
 
     @classmethod
     def helical(
         Class,
         axis: tuple = (0, 1, 0),
         start_angle: float = 0,
         step_angle: float = 0,
         start_pos: float = 0,
         step_pos: float = 0,
         num_images: int = 1,
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a continous helical scan
 
@@ -405,28 +508,32 @@
         positions = start_pos + step_pos * np.arange(num_images)
 
         # Create a single axis scan
         return Class.single_axis(
             axis=axis,
             angles=angles,
             positions=positions,
+            num_fractions=num_fractions,
+            electrons_per_angstrom=electrons_per_angstrom,
             exposure_time=exposure_time,
             drift=drift,
         )
 
     @classmethod
     def nhelix(
         Class,
         axis: tuple = (0, 1, 0),
         start_angle: float = 0,
         step_angle: float = 0,
         start_pos: float = 0,
         step_pos: float = 0,
         num_images: int = 1,
+        num_fractions: int = 1,
         num_nhelix: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a n-helix scan
 
@@ -440,60 +547,83 @@
             positions[j, :] = start_pos + np.full(num_images, j * step_pos)
 
         # Create a single axis scan
         return Class.single_axis(
             axis=axis,
             angles=angles.flatten(),
             positions=positions.flatten(),
+            num_fractions=num_fractions,
+            electrons_per_angstrom=electrons_per_angstrom,
             exposure_time=exposure_time,
             drift=drift,
         )
 
     @classmethod
     def single_particle(
         Class,
         num_images: int = 1,
+        num_fractions: int = 1,
         exposure_time: float = 1,
+        electrons_per_angstrom: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Create a single particle scan. This is a special scan that is actually
         just the particle in different orientations
 
         """
 
         # Get a random list of uniform orientations
         orientation = R.from_matrix(
             special_ortho_group.rvs(dim=3, size=num_images)
         ).as_rotvec()
 
+        # Get the axis and angle
+        axis, angle = Class._axis_angle_from_rotvec(orientation)
+
+        # Set the image number and fraction number
+        image_number = np.arange(len(angle))
+        fraction_number = np.arange(num_fractions)
+        fraction_number = np.repeat([fraction_number], len(angle), axis=0).flatten()
+
+        # Duplicate for the number of movie frames per step
+        image_number = np.repeat(image_number, num_fractions, axis=0)
+        axis = np.repeat(axis, num_fractions, axis=0)
+        angle = np.repeat(angle, num_fractions, axis=0)
+        dose = np.full(angle.shape, electrons_per_angstrom / num_fractions)
+
         # Create the shift delta
         shift_delta = None
         if drift is not None:
-            shift_delta = Class._generate_drift(
-                num_images, drift["magnitude"], drift["kernel_size"]
-            )
+            shift_delta = Class._generate_drift(np.zeros(num_images), **drift)
+            shift_delta = np.repeat(shift_delta, num_fractions, axis=0)
 
         # Create the scan
         return Scan(
-            orientation=orientation,
+            image_number=image_number,
+            fraction_number=fraction_number,
+            axis=axis,
+            angle=angle,
+            electrons_per_angstrom=dose,
             exposure_time=exposure_time,
             shift_delta=shift_delta,
             is_uniform_angular_scan=True,
         )
 
     @classmethod
     def beam_tilt(
         Class,
         axis: Union[np.ndarray, tuple] = (0, 1, 0),
         angles: np.ndarray = None,
         positions: np.ndarray = None,
         theta: np.ndarray = None,
         phi: np.ndarray = None,
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
         exposure_time: float = 1,
         drift: dict = None,
         **kwargs
     ) -> Scan:
         """
         Make a beam tilt scan. For each (angle, position) we scan the beam tilt
 
@@ -530,35 +660,97 @@
         positions = np.stack([positions] * num_beam_tilt).T.flatten()
         beam_tilt_theta = np.stack([theta] * num_stage_tilt).flatten()
         beam_tilt_phi = np.stack([phi] * num_stage_tilt).flatten()
         assert angles is not None
         assert positions is not None
 
         # Create the orientation and shift
-        orientation = Class._rotvec_from_axis_and_angles(np.array(axis), angles)
+        axis, angle = Class._rotvec_from_axis_and_angles(np.array(axis), angles)
         shift = Class._shift_from_axis_and_positions(np.array(axis), positions)
 
+        # Set the image number and fraction number
+        image_number = np.arange(len(angles))
+        fraction_number = np.arange(num_fractions)
+        fraction_number = np.repeat([fraction_number], len(angles), axis=0).flatten()
+
+        # Duplicate for the number of movie frames per step
+        image_number = np.repeat(image_number, num_fractions, axis=0)
+        axis = np.repeat(axis, num_fractions, axis=0)
+        angle = np.repeat(angle, num_fractions, axis=0)
+        shift = np.repeat(shift, num_fractions, axis=0)
+        beam_tilt_theta = np.repeat(beam_tilt_theta, num_fractions, axis=0)
+        beam_tilt_phi = np.repeat(beam_tilt_phi, num_fractions, axis=0)
+        dose = np.full(angle.shape, electrons_per_angstrom / num_fractions)
+
         # Create the shift delta
         shift_delta = None
         if drift is not None:
-            shift_delta = Class._generate_drift(
-                len(angles), drift["magnitude"], drift["kernel_size"]
-            )
+            shift_delta = Class._generate_drift(angles, **drift)
+            shift_delta = np.repeat(shift_delta, num_fractions, axis=0)
 
         # Create the scan object
         return Scan(
-            orientation=orientation,
+            image_number=image_number,
+            fraction_number=fraction_number,
+            axis=np.array(axis),
+            angle=angle,
             shift=shift,
             shift_delta=shift_delta,
             beam_tilt_theta=beam_tilt_theta,
             beam_tilt_phi=beam_tilt_phi,
+            electrons_per_angstrom=dose,
             exposure_time=exposure_time,
         )
 
     @classmethod
+    def grid_scan(
+        Class,
+        axis: Union[np.ndarray, tuple] = (0, 1, 0),
+        angles: np.ndarray = None,
+        start_pos: tuple = (0, 0),
+        step_pos: tuple = (0, 0),
+        num_images: tuple = (1, 1),
+        num_fractions: int = 1,
+        electrons_per_angstrom: float = 1,
+        exposure_time: float = 1,
+        drift: dict = None,
+        **kwargs
+    ) -> Scan:
+        """
+        Make a gridscan. For each angle we perform the grid scan
+
+        """
+
+        # Create the list of angles
+        if angles is None:
+            angles = np.array([0])
+
+        # Create the list of positions
+        x = start_pos[0] + step_pos[0] * np.arange(num_images[0])
+        y = start_pos[1] + step_pos[1] * np.arange(num_images[1])
+        positions = np.array([(xx, yy) for yy in x for xx in y])
+
+        # Get the positions
+        len_angles = len(angles)
+        len_positions = len(positions)
+        angles = np.repeat(angles, len_positions, axis=0)
+        positions = np.concatenate([positions] * len_angles)
+
+        # Create a single axis scan
+        return Class.single_axis(
+            axis=axis,
+            angles=angles,
+            positions=positions,
+            num_fractions=num_fractions,
+            electrons_per_angstrom=electrons_per_angstrom,
+            exposure_time=exposure_time,
+            drift=drift,
+        )
+
+    @classmethod
     def make_scan(Class, mode: str, **kwargs) -> Scan:
         """
         Make a scan from the input arguments
 
         """
 
         # Select the factory function
@@ -568,14 +760,15 @@
             "still": Class.still,
             "tilt_series": Class.tilt_series,
             "dose_symmetric": Class.dose_symmetric,
             "helical_scan": Class.helical,
             "nhelix": Class.nhelix,
             "single_particle": Class.single_particle,
             "beam_tilt": Class.beam_tilt,
+            "grid_scan": Class.grid_scan,
         }[mode]
 
         # Create the scan
         return function(**kwargs)  # type: ignore
 
 
 def new(
@@ -584,19 +777,21 @@
     angles: np.ndarray = None,
     positions: np.ndarray = None,
     start_angle: float = 0,
     step_angle: float = 0,
     start_pos: float = 0,
     step_pos: float = 0,
     num_images: int = 1,
+    num_fractions: int = 1,
     num_nhelix: int = 1,
     exposure_time: float = 1,
     theta: np.ndarray = None,
     phi: np.ndarray = None,
     drift: dict = None,
+    electrons_per_angstrom: float = 40,
 ) -> Scan:
     """
     Create an scan
 
     If angles or positions is None they are generated form the other
     parameters.
 
@@ -606,33 +801,37 @@
         angles: The rotation angles
         positions: The positions
         start_angle: The starting angle (deg)
         step_angle: The angle step (deg)
         start_pos: The starting position (A)
         step_pos: The step in position (A)
         num_images: The number of images
+        num_fractions: The number of movie frames per image
         num_nhelix: The number of scans in an n-helix
         exposure_time: The exposure time (seconds)
         theta: The beam tilt theta angle
         phi: The beam tilt phi angle
         drift: The beam drift model
+        electrons_per_angstrom: The number of electrons per angstrom (per image)
 
     Returns:
         The scan object
 
     """
     kwargs = {
         "axis": axis,
         "angles": angles,
         "positions": positions,
         "start_angle": start_angle,
         "step_angle": step_angle,
         "start_pos": start_pos,
         "step_pos": step_pos,
         "num_images": num_images,
+        "num_fractions": num_fractions,
         "num_nhelix": num_nhelix,
         "exposure_time": exposure_time,
         "theta": theta,
         "phi": phi,
         "drift": drift,
+        "electrons_per_angstrom": electrons_per_angstrom,
     }
     return ScanFactory.make_scan(mode, **kwargs)
```

### Comparing `python-parakeet-0.4.3/src/parakeet/simulate/_ctf.py` & `python-parakeet-0.4.4/src/parakeet/simulate/_ctf.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     # Print some options
     parakeet.config.show(config)
 
     # Do the work
     _ctf_Config(config, output_file)
 
 
-@ctf.register
+@ctf.register(parakeet.config.Config)
 def _ctf_Config(config: parakeet.config.Config, output_file: str):
     """
     Simulate the ctf
 
     Args:
         config: The config object
         output_file: The output ctf filename
```

### Comparing `python-parakeet-0.4.3/src/parakeet/simulate/_exit_wave.py` & `python-parakeet-0.4.4/src/parakeet/simulate/_exit_wave.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,23 +158,26 @@
 
         """
 
         # Get the specimen atoms
         logger.info(f"Simulating image {index+1}")
 
         # Get the rotation angle
+        image_number = self.scan.image_number[index]
+        fraction_number = self.scan.fraction_number[index]
         angle = self.scan.angles[index]
         axis = self.scan.axes[index]
         position = self.scan.position[index]
         orientation = self.scan.orientation[index]
         shift = self.scan.shift[index]
         drift = self.scan.shift_delta[index]
         beam_tilt_theta = self.scan.beam_tilt_theta[index]
         beam_tilt_phi = self.scan.beam_tilt_phi[index]
         exposure_time = self.scan.exposure_time[index]
+        electrons_per_angstrom = self.scan.electrons_per_angstrom[index]
 
         # The field of view
         nx = self.microscope.detector.nx
         ny = self.microscope.detector.ny
         pixel_size = self.microscope.detector.pixel_size
         origin = np.array(self.microscope.detector.origin)
         margin = self.simulation["margin"]
@@ -214,15 +217,15 @@
         # Compute the B factor
         if self.simulation["radiation_damage_model"]:
             input_multislice.static_B_factor = (
                 8
                 * pi**2
                 * (
                     self.simulation["sensitivity_coefficient"]
-                    * self.microscope.beam.electrons_per_angstrom
+                    * electrons_per_angstrom
                     * (index + 1)
                 )
             )
         else:
             input_multislice.static_B_factor = 0
 
         # Set the atoms in the input after translating them for the offset
@@ -270,15 +273,14 @@
             )
             print(
                 "Atoms Z min/max: %.1f, %.1f"
                 % (atoms.data["z"].min(), atoms.data["z"].max())
             )
 
         if self.simulation["ice"] == True:
-
             # Get the masker
             masker = self.get_masker(
                 index,
                 input_multislice,
                 pixel_size,
                 drift,
                 origin,
@@ -287,35 +289,40 @@
                 position,
             )
 
             # Run the simulation
             output_multislice = multem.simulate(system_conf, input_multislice, masker)
 
         else:
-
             # Run the simulation
             logger.info("Simulating")
             output_multislice = multem.simulate(system_conf, input_multislice)
 
         # Get the ideal image data
         # Multem outputs data in column major format. In C++ and Python we
         # generally deal with data in row major format so we must do a
         # transpose here.
         image = np.array(output_multislice.data[0].psi_coh).T
-        image = image[padding:-padding, padding:-padding]
+        x0 = padding
+        y0 = padding
+        x1 = image.shape[1] - padding
+        y1 = image.shape[0] - padding
+        image = image[y0:y1, x0:x1]
 
         # Print some info
         psi_tot = np.abs(image) ** 2
         logger.info("Ideal image min/max: %f/%f" % (np.min(psi_tot), np.max(psi_tot)))
 
         # Get the timestamp
         timestamp = time.time()
 
         # Set the metaadata
         metadata = self.metadata[index]
+        metadata["image_number"] = image_number
+        metadata["fraction_number"] = fraction_number
         metadata["timestamp"] = timestamp
         metadata["tilt_alpha"] = angle
         metadata["tilt_axis_x"] = axis[0]
         metadata["tilt_axis_y"] = axis[1]
         metadata["tilt_axis_z"] = axis[2]
         metadata["shift_x"] = shift[0]
         metadata["shift_y"] = shift[1]
@@ -328,14 +335,15 @@
         metadata["phi"] = self.microscope.beam.phi
         metadata["image_size_x"] = nx
         metadata["image_size_y"] = ny
         metadata["ice"] = self.simulation["ice"]
         metadata["damage_model"] = self.simulation["radiation_damage_model"]
         metadata["sensitivity_coefficient"] = self.simulation["sensitivity_coefficient"]
         metadata["exposure_time"] = exposure_time
+        metadata["dose"] = electrons_per_angstrom
 
         # Compute the image scaled with Poisson noise
         return (index, image, metadata)
 
 
 def simulation_factory(
     microscope: Microscope,
@@ -422,15 +430,15 @@
     logger.info(f"Loading sample from {sample_file}")
     sample = parakeet.sample.load(sample_file)
 
     # The exit wave file
     _exit_wave_Config(config, sample, exit_wave_file)
 
 
-@exit_wave.register
+@exit_wave.register(parakeet.config.Config)
 def _exit_wave_Config(
     config: parakeet.config.Config, sample: parakeet.sample.Sample, exit_wave_file: str
 ):
     """
     Simulate the exit wave from the sample
 
     Args:
@@ -443,15 +451,18 @@
     # Create the microscope
     microscope = parakeet.microscope.new(config.microscope)
 
     # Create the scan
     if config.scan.step_pos == "auto":
         radius = sample.shape_radius
         config.scan.step_pos = config.scan.step_angle * radius * pi / 180.0
-    scan = parakeet.scan.new(**config.scan.dict())
+    scan = parakeet.scan.new(
+        electrons_per_angstrom=microscope.beam.electrons_per_angstrom,
+        **config.scan.dict(),
+    )
 
     # Create the simulation
     simulation = simulation_factory(
         microscope,
         sample,
         scan,
         device=config.device,
```

### Comparing `python-parakeet-0.4.3/src/parakeet/simulate/_image.py` & `python-parakeet-0.4.4/src/parakeet/simulate/_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,27 +65,27 @@
             tuple: (angle, image)
 
         """
 
         # Get the rotation angle
         angle = self.scan.angles[index]
         exposure_time = self.scan.exposure_time[index]
+        electrons_per_angstrom = self.scan.electrons_per_angstrom[index]
         if exposure_time <= 0:
             exposure_time = 1.0
 
         # Check the angle and position
         assert abs(angle - self.optics.header[index]["tilt_alpha"]) < 1e7
 
         # Get the specimen atoms
         logger.info(f"Simulating image {index+1}")
 
         # Compute the number of counts per pixel
         electrons_per_pixel = (
-            self.microscope.beam.electrons_per_angstrom
-            * self.microscope.detector.pixel_size**2
+            electrons_per_angstrom * self.microscope.detector.pixel_size**2
         )
 
         # Compute the electrons per pixel second
         electrons_per_second = electrons_per_pixel / exposure_time
         energy = self.microscope.beam.energy
 
         # Get the image
@@ -113,15 +113,15 @@
         logger.info(
             "    Image min/max/mean: %g/%g/%.2g"
             % (np.min(image), np.max(image), np.mean(image))
         )
 
         # Get the image metadata
         metadata = np.asarray(self.optics.header[index])
-        metadata["dose"] = self.microscope.beam.electrons_per_angstrom
+        metadata["dose"] = electrons_per_angstrom
         metadata["dqe"] = self.microscope.detector.dqe
         metadata["gain"] = 1
         metadata["offset"] = 0
 
         # Compute the image scaled with Poisson noise
         return (index, image.astype("float32"), metadata)
 
@@ -184,15 +184,15 @@
     # Print some options
     parakeet.config.show(config)
 
     # Do the work
     _image_Config(config, optics_file, image_file)
 
 
-@image.register
+@image.register(parakeet.config.Config)
 def _image_Config(config: parakeet.config.Config, optics_file: str, image_file: str):
     """
     Simulate the image with noise
 
     Args:
         config: The config object
         optics_file: The optics image filename
@@ -206,14 +206,21 @@
     # Create the exit wave data
     logger.info(f"Loading sample from {optics_file}")
     optics = parakeet.io.open(optics_file)
 
     # Create the scan
     scan = optics.header.scan
 
+    # Override the dose
+    scan_new = parakeet.scan.new(
+        electrons_per_angstrom=microscope.beam.electrons_per_angstrom,
+        **config.scan.dict(),
+    )
+    scan.data["electrons_per_angstrom"] = scan_new.electrons_per_angstrom
+
     # Create the simulation
     simulation = simulation_factory(
         microscope=microscope,
         optics=optics,
         scan=scan,
         device=config.device,
         simulation=config.simulation.dict(),
```

### Comparing `python-parakeet-0.4.3/src/parakeet/simulate/_optics.py` & `python-parakeet-0.4.4/src/parakeet/simulate/_optics.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,14 @@
 from parakeet.microscope import Microscope
 from parakeet.scan import Scan
 from functools import singledispatch
 from math import sqrt
 from parakeet.simulate.simulation import Simulation
 
 
-Device = parakeet.config.Device
-ClusterMethod = parakeet.config.ClusterMethod
-
-
 __all__ = ["optics"]
 
 
 # Try to input MULTEM
 try:
     import multem
 except ImportError:
@@ -83,15 +79,14 @@
             tuple: (angle, image)
 
         """
 
         def compute_image(
             psi, microscope, simulation, x_fov, y_fov, offset, device, defocus=None
         ):
-
             # Create the multem system configuration
             system_conf = parakeet.simulate.simulation.create_system_configuration(
                 device
             )
 
             # Set the defocus
             if defocus is not None:
@@ -106,14 +101,22 @@
             input_multislice.spec_lx = x_fov + offset * 2
             input_multislice.spec_ly = y_fov + offset * 2
             input_multislice.spec_lz = x_fov  # self.sample.containing_box[1][2]
 
             # Compute and apply the CTF
             ctf = np.array(multem.compute_ctf(system_conf, input_multislice)).T
 
+            # Add the effect of the phase plate
+            if microscope.phase_plate.use:
+                ctf = ctf * parakeet.simulate.phase_plate.compute_phase_shift(
+                    ctf.shape,
+                    microscope.detector.pixel_size,
+                    microscope.phase_plate.phase_shift,
+                    microscope.phase_plate.radius,
+                )
             # Compute the B factor for radiation damage
             # if simulation["radiation_damage_model"]:
             #    sigma_B = sqrt(
             #        simulation["sensitivity_coefficient"]
             #        * microscope.beam.electrons_per_angstrom
             #        * (index + 1)
             #    )
@@ -159,30 +162,28 @@
         defocus = microscope.lens.c_10
 
         # If we do CC correction then set spherical aberration and chromatic
         # aberration to zero
         shape = self.sample["shape"]
         energy_shift = 0
         if self.simulation["inelastic_model"] is None:
-
             # If no inelastic model just calculate image as normal
             image = compute_image(
                 psi,
                 microscope,
                 self.simulation,
                 x_fov,
                 y_fov,
                 offset,
                 self.device,
                 defocus,
             )
             electron_fraction = 1.0
 
         elif self.simulation["inelastic_model"] == "zero_loss":
-
             # Compute the image
             image = compute_image(
                 psi,
                 microscope,
                 self.simulation,
                 x_fov,
                 y_fov,
@@ -194,15 +195,14 @@
             # Calculate the fraction of electrons in the zero loss peak
             electron_fraction = parakeet.inelastic.zero_loss_fraction(shape, angle)
 
             # Scale the image by the fraction of electrons
             image *= electron_fraction
 
         elif self.simulation["inelastic_model"] == "mp_loss":
-
             # Set the filter width
             filter_width = self.simulation["mp_loss_width"]  # eV
 
             # Compute the energy and spread of the plasmon peak
             thickness = parakeet.inelastic.effective_thickness(shape, angle)  # A
             peak, sigma = parakeet.inelastic.most_probable_loss(
                 microscope.beam.energy, shape, angle
@@ -282,15 +282,14 @@
             # Compute the zero loss and mpl image fraction
             electron_fraction = elastic_fraction + inelastic_fraction
 
             # Add the images incoherently and scale the image by the fraction of electrons
             image = elastic_fraction * image1 + inelastic_fraction * image2
 
         elif self.simulation["inelastic_model"] == "unfiltered":
-
             # Compute the energy and spread of the plasmon peak
             peak, sigma = parakeet.inelastic.most_probable_loss(
                 microscope.beam.energy, shape, angle
             )  # eV
             peak = min(peak, 1000 * microscope.beam.energy * 0.1)  # eV
             spread = sigma * sqrt(2) / (microscope.beam.energy * 1000)  # dE / E
 
@@ -331,15 +330,14 @@
             mp_loss_fraction = parakeet.inelastic.mp_loss_fraction(shape, angle)
             electron_fraction = zero_loss_fraction + mp_loss_fraction
 
             # Add the images incoherently and scale the image by the fraction of electrons
             image = zero_loss_fraction * image1 + mp_loss_fraction * image2
 
         elif self.simulation["inelastic_model"] == "cc_corrected":
-
             # Set the Cs and CC to zero
             microscope.lens.c_30 = 0
             microscope.lens.c_c = 0
 
             # Compute the energy and spread of the plasmon peak
             peak, sigma = parakeet.inelastic.most_probable_loss(
                 microscope.beam.energy, shape, angle
@@ -455,15 +453,15 @@
         return (index, image, metadata)
 
 
 def simulation_factory(
     microscope: Microscope,
     exit_wave: object,
     scan: Scan,
-    device: Device = Device.gpu,
+    device: parakeet.config.Device = parakeet.config.Device.gpu,
     simulation: dict = None,
     sample: dict = None,
     cluster: dict = None,
 ) -> Simulation:
     """
     Create the simulation
 
@@ -498,16 +496,16 @@
 
 
 @singledispatch
 def optics(
     config_file,
     exit_wave_file: str,
     optics_file: str,
-    device: Device = Device.gpu,
-    cluster_method: ClusterMethod = None,
+    device: parakeet.config.Device = parakeet.config.Device.gpu,
+    cluster_method: parakeet.config.ClusterMethod = None,
     cluster_max_workers: int = 1,
 ):
     """
     Simulate the optics
 
     Args:
         config_file: The input config filename
@@ -533,15 +531,15 @@
     # Print some options
     parakeet.config.show(config)
 
     # Do the work
     _optics_Config(config, exit_wave_file, optics_file)
 
 
-@optics.register
+@optics.register(parakeet.config.Config)
 def _optics_Config(
     config: parakeet.config.Config, exit_wave_file: str, optics_file: str
 ):
     """
     Simulate the optics
 
     Args:
```

### Comparing `python-parakeet-0.4.3/src/parakeet/simulate/_potential.py` & `python-parakeet-0.4.4/src/parakeet/simulate/_potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     # Print some options
     parakeet.config.show(config)
 
     # Do the work
     _potential_Config(config, sample_file, potential_prefix)
 
 
-@potential.register
+@potential.register(parakeet.config.Config)
 def _potential_Config(
     config: parakeet.config.Config, sample_file: str, potential_prefix: str
 ):
     """
     Simulate the projected potential from the sample
 
     Args:
@@ -295,15 +295,18 @@
     logger.info(f"Loading sample from {sample_file}")
     sample = parakeet.sample.load(sample_file)
 
     # Create the scan
     if config.scan.step_pos == "auto":
         radius = sample.shape_radius
         config.scan.step_pos = config.scan.step_angle * radius * pi / 180.0
-    scan = parakeet.scan.new(**config.scan.dict())
+    scan = parakeet.scan.new(
+        electrons_per_angstrom=microscope.beam.electrons_per_angstrom,
+        **config.scan.dict(),
+    )
 
     # Create the simulation
     simulation = simulation_factory(
         potential_prefix=potential_prefix,
         microscope=microscope,
         sample=sample,
         scan=scan,
```

### Comparing `python-parakeet-0.4.3/src/parakeet/simulate/_simple.py` & `python-parakeet-0.4.4/src/parakeet/simulate/_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     # Print some options
     parakeet.config.show(config)
 
     # Do the work
     _simple_Config(config, atoms_file, output_file)
 
 
-@simple.register
+@simple.register(parakeet.config.Config)
 def _simple_Config(config: parakeet.config.Config, atoms_file: str, output_file: str):
     """
     Simulate the image
 
     Args:
         config: The config object
         atoms_file: The input atoms filename
```

### Comparing `python-parakeet-0.4.3/src/parakeet/util/calibrate_ice_model.py` & `python-parakeet-0.4.4/src/parakeet/util/calibrate_ice_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 def compute_potential():
     """
     Compute the projected potential in slices
 
     """
 
     def compute(atom_data, pixel_size, thickness):
-
         # Get the dimensions
         x_min = atom_data.data["x"].min()
         x_max = atom_data.data["x"].max()
         y_min = atom_data.data["y"].min()
         y_max = atom_data.data["y"].max()
         z_min = atom_data.data["z"].min()
         z_max = atom_data.data["z"].max()
@@ -227,15 +226,14 @@
     input_multislice.spec_ly = ny * pixel_size
     input_multislice.spec_lz = nx * pixel_size
     input_multislice.spec_dz = 1
 
     # For N random placements compute the mean intensity
     means = []
     for j in range(10):
-
         # Compute the position
         x0 = np.random.uniform(0, 1) + nx // 2
         y0 = np.random.uniform(0, 1) + ny // 2
         x0 = pixel_size * x0
         y0 = pixel_size * y0
 
         # Set the atom list
@@ -320,32 +318,32 @@
     # Write out the table to file
     print("Mean0 = %f" % (expected * s**2))
     with open("mean_table.csv", "w") as outfile:
         for x, y in zip(area, mean):
             outfile.write("%.2f, %.7f\n" % (x, y))
 
     # Plot the mean correction
-    ax.plot(area, mean)
-    ax.set_xlabel(r"Pixel area ($Å^2$)" + "\n(b)")
-    ax.set_title("Mean correction factor")
+    ax.plot(area, mean, label="Mean correction")
+    ax.set_xlabel(r"Pixel area ($Å^2$)" + "\n(c)", fontsize=9)
+    ax.set_title("Mean correction factor", fontsize=9)
+    ax.set_xlim(0, 4)
 
 
 def compute_mean_correction2(ax=None):
     """
     Compute the mean correction table
 
     """
 
     X = []
     Y = []
 
     # Loop through the pixel sizes
     thickness = 20
     for pixel_size in np.arange(0.1, 2.1, 0.1):
-
         # Read the projected potential
         handle = np.load("potential_%.1f_%d.npz" % (pixel_size, thickness))
         potential = handle["potential"]
         num_atoms = handle["num_atoms"]
 
         # Select the pixels with potential in
         xsize, ysize = potential.shape
@@ -380,31 +378,31 @@
     print("Mean0 = %f" % Y0)
     with open("mean_table2.csv", "w") as outfile:
         for x, y in zip(X, Y):
             outfile.write("%.2f, %.7f\n" % (x, y))
 
     # Plot
     ax.plot(X, Y)
-    ax.set_xlabel(r"Pixel area ($Å^2$)" + "\n(c)")
-    ax.set_title("Mean correction factor")
+    ax.set_xlabel(r"Pixel area ($Å^2$)" + "\n(d)", fontsize=9)
+    ax.set_title("Mean correction factor", fontsize=9)
+    ax.set_xlim(0, 4)
 
 
 def compute_variance_correction(ax=None):
     """
     Compute the variance correction table
 
     """
 
     X = []
     Y = []
 
     # Loop through the pixel sizes
     thickness = 20
     for pixel_size in np.arange(0.1, 2.1, 0.1):
-
         # Read the projected potential
         handle = np.load("potential_%.1f_%d.npz" % (pixel_size, thickness))
         potential = handle["potential"]
         num_atoms = handle["num_atoms"]
 
         # Select the pixels with potential in
         xsize, ysize = potential.shape
@@ -438,29 +436,29 @@
     # Write out the table to file
     print("Var0 = %f" % Y0)
     with open("variance_table.csv", "w") as outfile:
         for x, y in zip(X, Y):
             outfile.write("%.2f, %.7f\n" % (x, y))
 
     # Plot
-    ax.plot(X, Y)
-    ax.set_xlabel(r"Pixel area ($Å^2$)" + "\n(c)")
-    ax.set_title("Variance correction factor")
+    ax.plot(X, Y, label="Variance correction")
+    ax.set_xlabel(r"Pixel area ($Å^2$)" + "\n(c)", fontsize=9)
+    ax.set_title("Mean and variance correction factors", fontsize=9)
+    ax.set_xlim(0, 4)
 
 
 def compute_power(ax=None):
     """
     Compute the power spectrum
 
     """
 
     # Compute the fit to the power spectrum
     pixel_size = 0.1
     for thickness in [20]:  # , 19, 18, 15, 10, 5]:
-
         # Read the projected potential
         handle = np.load("potential_%.1f_%d.npz" % (pixel_size, thickness))
         potential = handle["potential"]
         num_atoms = handle["num_atoms"]
 
         # Select the pixels with potential in
         xsize, ysize = potential.shape
@@ -550,24 +548,90 @@
 
         # Compute the radial spectrum
         rp = radial_average(np.fft.fftshift(power))
         rm = radial_average(np.fft.fftshift(model))
         d = np.arange(rp.size) / (pixel_size * power.shape[0])
 
         # Plot the power spectrum and best fit
-        ax.plot(d[1:], rp[1:] / C, label="%d" % thickness)
+        ax.plot(d[1:], rp[1:] / C)  # , label="%d" % thickness)
         ax.plot(d[1:], rm[1:] / C, color="black", alpha=0.5, label="Model")
 
     # Set some plot properties
-    ax.set_xlabel("Spatial frequency ($Å$)\n(a)")
-    ax.set_title("Power spectrum")
+    ax.set_xlabel("Spatial frequency ($Å^{-1}$)\n(a)", fontsize=9)
+    ax.set_title("Power spectrum", fontsize=9)
     ax.set_xlim(0, 1)
+    ax.legend(fontsize=9)
     ax.set_yticklabels("")
 
 
+def compute_correlation(ax=None):
+    """
+    Compute the correlation length
+
+    """
+
+    pixel_size = 0.1
+    for thickness in [5]:  # , 19, 18, 15, 10, 5]:
+        # Read the projected potential
+        handle = np.load("potential_%.1f_%d.npz" % (pixel_size, thickness))
+        potential = handle["potential"]
+        num_atoms = handle["num_atoms"]
+
+        # Select the pixels with potential in
+        xsize, ysize = potential.shape
+        x0 = xsize // 8
+        x1 = 7 * xsize // 8
+        y0 = ysize // 8
+        y1 = 7 * ysize // 8
+        potential = potential[x0:x1, y0:y1]
+
+        data = potential
+        data = data - np.mean(data)
+        f = np.fft.fft2(data)
+        power = np.abs(f) ** 2
+        corr = np.abs(np.fft.ifft2(power))
+        corr = np.fft.fftshift(corr)
+        corr = corr / (corr.size * np.var(data))
+
+        rc = radial_average(corr)[0 : data.shape[0] // 2]
+        rd = np.arange(rc.size) * pixel_size
+        rc = rc / np.max(rc)
+
+        corr_length = 0
+        val = rc[0] / np.exp(1)
+        for d, c in zip(rd, rc):
+            if c < val:
+                corr_length = d
+                break
+
+    print("Correlation Length: %f" % corr_length)
+
+    # Plot the correlation
+    if ax is None:
+        width = 0.0393701 * 190
+        height = width * 0.74
+        fig, ax = pylab.subplots(figsize=(width, height), constrained_layout=True)
+    ax.plot(rd, rc)
+    ax.axvline(
+        corr_length,
+        color="black",
+        linestyle="--",
+        label="$𝜉 = %.1f Å$" % corr_length,
+    )
+
+    # Set some plot properties
+    ax.set_xlabel("Distance ($Å$)\n(b)", fontsize=9)
+    ax.set_title("Autocorrelation", fontsize=9)
+    ax.set_xlim(0, 2.5)
+    ax.legend(fontsize=9)
+    if ax is None:
+        fig.savefig("correlation_%.1fA.png" % pixel_size, dpi=300, bbox_inches="tight")
+        pylab.close("all")
+
+
 def calibrate():
     """
     Calibrate ice model
 
     """
     # Get the water atomic model file
     get_water_atomic_model()
@@ -576,17 +640,21 @@
     compute_potential()
 
     # Setup the figure
     width = 0.0393701 * 190
     height = width / 3.0
     fig, ax = pylab.subplots(ncols=3, figsize=(width, height), constrained_layout=True)
     compute_power(ax[0])
-    compute_mean_correction(ax[1])
+    compute_correlation(ax[1])
+    compute_mean_correction(ax[2])
     # compute_mean_correction2(ax[1])
     compute_variance_correction(ax[2])
+    ax[2].legend(fontsize=9)
+    for axx in ax:
+        axx.tick_params(axis="both", labelsize=9)
     fig.savefig("model.png", dpi=300, bbox_inches="tight")
 
 
 def compute_exit_wave(atom_data, pixel_size):
     """
     Compute the exit wave
 
@@ -680,15 +748,14 @@
     # Return the images
     x0 = np.array((x_box_size / 2 - x_size / 2, y_box_size / 2 - y_size / 2))
     x1 = np.array((x_box_size / 2 + x_size / 2, y_box_size / 2 + y_size / 2))
     return physical_image, random_image, x0, x1
 
 
 def load_exit_wave(atom_data, ps):
-
     physical_filename = "exit_wave_physical_%.1f.mrc" % ps
     random_filename = "exit_wave_random_%.1f.mrc" % ps
     metadata_filename = "metadata_%.1f.dat" % ps
 
     if (
         not os.path.exists(physical_filename)
         or not os.path.exists(random_filename)
@@ -711,15 +778,14 @@
             x0 = (x00, x01)
             x1 = (x10, x11)
 
     return physical_image, random_image, x0, x1
 
 
 def plot_mean_and_var(physical_data, random_data, xmin, xmax, ps):
-
     x0 = np.floor(xmin / ps).astype("int32")
     x1 = np.floor(xmax / ps).astype("int32")
     xr = x1 - x0
     x0 = x0 + xr // 3
     x1 = x1 - xr // 3
 
     random_middle = random_data[x0[0] : x1[0], x0[1] : x1[1]]
@@ -812,15 +878,14 @@
         random_middle_mean_imag,
         random_middle_std_real,
         random_middle_std_imag,
     )
 
 
 def plot_power(physical_data, random_data, xmin, xmax, ps):
-
     x0 = np.floor(xmin / ps).astype("int32")
     x1 = np.floor(xmax / ps).astype("int32")
     xr = x1 - x0
     x0 = x0 + xr // 3
     x1 = x1 - xr // 3
 
     random_middle = random_data[x0[0] : x1[0], x0[1] : x1[1]]
@@ -862,15 +927,14 @@
     fig.savefig("power_%.1fA.png" % ps, dpi=300, bbox_inches="tight")
     pylab.close("all")
 
     return physical_d, physical_power, random_d, random_power
 
 
 def plot_edge(physical_data, random_data, xmin, xmax, ps):
-
     x0 = np.floor(xmin / ps).astype("int32")
     x1 = np.floor(xmax / ps).astype("int32")
     xd = x1 - x0
     x0 = x0 - xd // 10
     x1 = x0 + 3 * xd // 10
 
     # x1 = 2 * x0  # + x0 // 2
@@ -1047,26 +1111,24 @@
     ax[1].set_xlim(0, 1.0)
     # pylab.show()
     fig.savefig("mean_and_power.png", dpi=300, bbox_inches="tight")
     pylab.close("all")
 
 
 def plot_all_edge(pixel_size, edge_list):
-
     width = 0.0393701 * 190
     height = 0.5 * width
     fig, ax = pylab.subplots(
         figsize=(width, height), ncols=4, nrows=2, constrained_layout=True
     )
 
     pixel_size = [pixel_size[i] for i in [0, 3, 6, 9]]
     edge_list = [edge_list[i] for i in [0, 3, 6, 9]]
 
     for i, (ps, edge) in enumerate(zip(pixel_size, edge_list)):
-
         vmin = min(np.min(edge[0]), np.min(edge[0]))
         vmax = max(np.max(edge[1]), np.max(edge[1]))
 
         ax[0][i].imshow(edge[0], vmin=vmin, vmax=vmax, cmap="gray_r")
         ax[1][i].imshow(edge[1], vmin=vmin, vmax=vmax, cmap="gray_r")
         # ax[0][i].set_title("Physical model", fontweight="bold")
         # ax[1][i].set_title("Random model", fontweight="bold")
@@ -1099,15 +1161,14 @@
     pixel_size = np.arange(0.1, 1.1, 0.1)  # [0.1]#, 1.0]
 
     stats_list = []
     power_list = []
     edge_list = []
 
     for ps in pixel_size:
-
         # Get the simulated exit wave
         physical_data, random_data, xmin, xmax = load_exit_wave(atom_data, ps)
 
         # Make the plots
         stats = plot_mean_and_var(physical_data, random_data, xmin, xmax, ps)
         power = plot_power(physical_data, random_data, xmin, xmax, ps)
         edge = plot_edge(physical_data, random_data, xmin, xmax, ps)
@@ -1119,15 +1180,14 @@
     # plot_all_mean_and_std(pixel_size, stats_list)
     # plot_all_power(pixel_size, power_list)
     plot_all_mean_and_power(pixel_size, stats_list, power_list)
     plot_all_edge(pixel_size, edge_list)
 
 
 if __name__ == "__main__":
-
     # Create the argument parser
     parser = argparse.ArgumentParser(description="Do the ice model configuration")
 
     # Add arguments
     parser.add_argument(
         "-c",
         "--calibrate",
```

### Comparing `python-parakeet-0.4.3/src/python_parakeet.egg-info/SOURCES.txt` & `python-parakeet-0.4.4/src/python_parakeet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .dockerignore
 .gitignore
 .gitmodules
 .pre-commit-config.yaml
+CHANGES.rst
 CMakeLists.txt
 Dockerfile
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
@@ -29,15 +30,21 @@
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/publications.rst
 docs/source/tutorial.rst
 docs/source/usage.rst
 docs/source/ext/pydantic_settings.py
 docs/source/images/parakeet.png
+docs/source/images/parakeet_logo.png
 docs/source/images/parakeet_small.png
+newsfragments/.gitignore
+newsfragments/39.feature
+newsfragments/44.doc
+newsfragments/50.feature
+newsfragments/51.feature
 pybind11/.appveyor.yml
 pybind11/.clang-format
 pybind11/.clang-tidy
 pybind11/.cmake-format.yaml
 pybind11/.git
 pybind11/.gitignore
 pybind11/.pre-commit-config.yaml
@@ -308,14 +315,15 @@
 src/parakeet/command_line/sample/__init__.py
 src/parakeet/command_line/sample/_add_molecules.py
 src/parakeet/command_line/sample/_mill.py
 src/parakeet/command_line/sample/_new.py
 src/parakeet/command_line/sample/_show.py
 src/parakeet/command_line/sample/_sputter.py
 src/parakeet/command_line/simulate/__init__.py
+src/parakeet/command_line/simulate/_cbed.py
 src/parakeet/command_line/simulate/_ctf.py
 src/parakeet/command_line/simulate/_exit_wave.py
 src/parakeet/command_line/simulate/_image.py
 src/parakeet/command_line/simulate/_optics.py
 src/parakeet/command_line/simulate/_potential.py
 src/parakeet/command_line/simulate/_simple.py
 src/parakeet/data/__init__.py
@@ -331,20 +339,22 @@
 src/parakeet/sample/__init__.py
 src/parakeet/sample/_add_molecules.py
 src/parakeet/sample/_mill.py
 src/parakeet/sample/_new.py
 src/parakeet/sample/_sputter.py
 src/parakeet/sample/distribute.py
 src/parakeet/simulate/__init__.py
+src/parakeet/simulate/_cbed.py
 src/parakeet/simulate/_ctf.py
 src/parakeet/simulate/_exit_wave.py
 src/parakeet/simulate/_image.py
 src/parakeet/simulate/_optics.py
 src/parakeet/simulate/_potential.py
 src/parakeet/simulate/_simple.py
+src/parakeet/simulate/phase_plate.py
 src/parakeet/simulate/simulation.py
 src/parakeet/util/calibrate_ice_model.py
 src/python_parakeet.egg-info/PKG-INFO
 src/python_parakeet.egg-info/SOURCES.txt
 src/python_parakeet.egg-info/dependency_links.txt
 src/python_parakeet.egg-info/entry_points.txt
 src/python_parakeet.egg-info/requires.txt
```

### Comparing `python-parakeet-0.4.3/src/python_parakeet.egg-info/entry_points.txt` & `python-parakeet-0.4.4/src/python_parakeet.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 parakeet.pdb.read = parakeet.command_line.pdb:read
 parakeet.run = parakeet.command_line:run
 parakeet.sample.add_molecules = parakeet.command_line.sample:add_molecules
 parakeet.sample.mill = parakeet.command_line.sample:mill
 parakeet.sample.new = parakeet.command_line.sample:new
 parakeet.sample.show = parakeet.command_line.sample:show
 parakeet.sample.sputter = parakeet.command_line.sample:sputter
+parakeet.simulate.cbed = parakeet.command_line.simulate:cbed
 parakeet.simulate.ctf = parakeet.command_line.simulate:ctf
 parakeet.simulate.exit_wave = parakeet.command_line.simulate:exit_wave
 parakeet.simulate.image = parakeet.command_line.simulate:image
 parakeet.simulate.optics = parakeet.command_line.simulate:optics
 parakeet.simulate.potential = parakeet.command_line.simulate:potential
 parakeet.simulate.simple = parakeet.command_line.simulate:simple
```

### Comparing `python-parakeet-0.4.3/tests/test_command_line.py` & `python-parakeet-0.4.4/tests/test_command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def config_path(tmpdir_factory):
     directory = tmpdir_factory.mktemp("proc")
 
     config_dict = {
         "microscope": {
             "detector": {"nx": 250, "ny": 250, "pixel_size": 2},
             "beam": {
-                "electrons_per_angstrom": 1000,
+                "electrons_per_angstrom": 10000,
             },
         },
         "sample": {
             "molecules": {"pdb": [{"id": "4v1w", "instances": 2}]},
             "shape": {
                 "type": "cube",
                 "cube": {"length": 500},
@@ -39,132 +39,119 @@
     config = parakeet.config.load(config_dict)
     config_path = os.path.abspath(os.path.join(directory, "config.yaml"))
     yaml.safe_dump(config.dict(), open(config_path, "w"))
     return directory
 
 
 def test_config_new(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config-new.yaml"))
     parakeet.command_line.config.new(["-c", config])
     assert os.path.exists(config)
 
 
 def test_config_edit(config_path):
-
     config_in = os.path.abspath(os.path.join(config_path, "config.yaml"))
     config_out = os.path.abspath(os.path.join(config_path, "config-edit.yaml"))
     config_str = "microscope:\n" "  beam:\n" "    energy: 200\n"
     assert os.path.exists(config_in)
     parakeet.command_line.config.edit(
         ["-i", config_in, "-o", config_out, "-s", config_str]
     )
     assert os.path.exists(config_out)
     config = parakeet.config.load(config_out)
     assert config.microscope.beam.energy == 200
 
 
 def test_config_show(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     assert os.path.exists(config)
     parakeet.command_line.config.show(["-c", config])
 
 
 def test_sample_new(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     assert os.path.exists(config)
     parakeet.command_line.sample.new(["-c", config, "-s", sample])
     assert os.path.exists(sample)
 
 
 def test_sample_add_molecules(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     parakeet.command_line.sample.add_molecules(["-c", config, "-s", sample])
 
 
 def test_sample_mill(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     parakeet.command_line.sample.mill(["-c", config, "-s", sample])
 
 
 def test_sample_sputter(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     parakeet.command_line.sample.sputter(["-c", config, "-s", sample])
 
 
 def test_sample_show(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     parakeet.command_line.sample.show(["-s", sample])
 
 
 def test_simulate_exit_wave(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     exit_wave = os.path.abspath(os.path.join(config_path, "exit_wave.h5"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     parakeet.command_line.simulate.exit_wave(
         ["-c", config, "-s", sample, "-e", exit_wave]
     )
     assert os.path.exists(exit_wave)
 
 
 def test_simulate_optics(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     exit_wave = os.path.abspath(os.path.join(config_path, "exit_wave.h5"))
     optics = os.path.abspath(os.path.join(config_path, "optics.h5"))
     assert os.path.exists(config)
     assert os.path.exists(exit_wave)
     parakeet.command_line.simulate.optics(["-c", config, "-e", exit_wave, "-o", optics])
     assert os.path.exists(optics)
 
 
 def test_simulate_image(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     optics = os.path.abspath(os.path.join(config_path, "optics.h5"))
     image = os.path.abspath(os.path.join(config_path, "image.mrc"))
     assert os.path.exists(config)
     assert os.path.exists(optics)
     parakeet.command_line.simulate.image(["-c", config, "-o", optics, "-i", image])
     assert os.path.exists(image)
 
 
 def test_simulate_ctf(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     ctf = os.path.abspath(os.path.join(config_path, "ctf.h5"))
     assert os.path.exists(config)
     parakeet.command_line.simulate.ctf(["-c", config, "-o", ctf])
     assert os.path.exists(ctf)
 
 
 def test_simulate_potential(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     potential = os.path.abspath(os.path.join(config_path, "potential"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     parakeet.command_line.simulate.potential(
         ["-c", config, "-s", sample, "-p", potential]
@@ -174,41 +161,48 @@
 
 
 def test_simulate_simple(config_path):
     pass
 
 
 def test_analyse_correct(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     image = os.path.abspath(os.path.join(config_path, "image.mrc"))
     corrected = os.path.abspath(os.path.join(config_path, "corrected.mrc"))
     assert os.path.exists(config)
     assert os.path.exists(image)
     parakeet.command_line.analyse.correct(
         ["-c", config, "-i", image, "-cr", corrected, "-d", "cpu"]
     )
     assert os.path.exists(corrected)
 
 
 def test_analyse_reconstruct(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     image = os.path.abspath(os.path.join(config_path, "image.mrc"))
-    rec = os.path.abspath(os.path.join(config_path, "rec.mrc"))
+    rec_cpu = os.path.abspath(os.path.join(config_path, "rec.mrc"))
+    # rec_gpu = os.path.abspath(os.path.join(config_path, "rec_gpu.mrc"))
     assert os.path.exists(config)
     assert os.path.exists(image)
     parakeet.command_line.analyse.reconstruct(
-        ["-c", config, "-i", image, "-r", rec, "-d", "cpu"]
+        ["-c", config, "-i", image, "-r", rec_cpu, "-d", "cpu"]
     )
-    assert os.path.exists(rec)
+    # parakeet.command_line.analyse.reconstruct(
+    #     ["-c", config, "-i", image, "-r", rec_gpu, "-d", "gpu"]
+    # )
+    assert os.path.exists(rec_cpu)
+    # assert os.path.exists(rec_gpu)
+
+    # FIXME TEST GIVES THE SAME RESULT
+    # d1 = mrcfile.open(rec_cpu).data
+    # d2 = mrcfile.open(rec_gpu).data
+    # assert np.all(np.isclose(d1, d2))
 
 
 def test_analyse_average_particles(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     rec = os.path.abspath(os.path.join(config_path, "rec.mrc"))
     half1 = os.path.abspath(os.path.join(config_path, "half1.mrc"))
     half2 = os.path.abspath(os.path.join(config_path, "half2.mrc"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
@@ -217,30 +211,28 @@
         ["-c", config, "-s", sample, "-r", rec, "-h1", half1, "-h2", half2]
     )
     assert os.path.exists(half1)
     assert os.path.exists(half2)
 
 
 def test_analyse_average_all_particles(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     rec = os.path.abspath(os.path.join(config_path, "rec.mrc"))
     average = os.path.abspath(os.path.join(config_path, "average.mrc"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     assert os.path.exists(rec)
     parakeet.command_line.analyse.average_all_particles(
         ["-c", config, "-s", sample, "-r", rec, "-avm", average]
     )
     assert os.path.exists(average)
 
 
 def test_analyse_extract(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample.h5"))
     rec = os.path.abspath(os.path.join(config_path, "rec.mrc"))
     particles = os.path.abspath(os.path.join(config_path, "particles.h5"))
     assert os.path.exists(config)
     assert os.path.exists(sample)
     assert os.path.exists(rec)
@@ -251,15 +243,14 @@
 
 
 def test_analyse_refine(config_path):
     pass
 
 
 def test_export(config_path):
-
     exit_wave1 = os.path.abspath(os.path.join(config_path, "exit_wave.h5"))
     exit_wave2 = os.path.abspath(os.path.join(config_path, "exit_wave2.mrc"))
     exit_wave3 = os.path.abspath(os.path.join(config_path, "exit_wave3.h5"))
     optics1 = os.path.abspath(os.path.join(config_path, "optics.h5"))
     optics2 = os.path.abspath(os.path.join(config_path, "optics2.mrc"))
     optics3 = os.path.abspath(os.path.join(config_path, "optics3.h5"))
     image1 = os.path.abspath(os.path.join(config_path, "image.mrc"))
@@ -284,22 +275,20 @@
     assert os.path.exists(optics2)
     assert os.path.exists(optics3)
     assert os.path.exists(image2)
     assert os.path.exists(image3)
 
 
 def test_pdb_read(config_path):
-
     pdb = parakeet.data.get_pdb("4v1w")
     assert os.path.exists(pdb)
     parakeet.command_line.pdb.read([pdb])
 
 
 def test_pdb_get1(config_path):
-
     directory = os.path.abspath(config_path)
     parakeet.command_line.pdb.get(["4v1w", "-d", directory])
     assert os.path.exists(os.path.join(directory, "4v1w.cif"))
 
 
 def test_pdb_get2(config_path):
     if os.getenv("CI"):
@@ -307,21 +296,36 @@
         return
     directory = os.path.abspath(config_path)
     parakeet.command_line.pdb.get(["1uad", "-d", directory])
     assert os.path.exists(os.path.join(directory, "1uad.cif"))
 
 
 def test_run(config_path):
-
     config = os.path.abspath(os.path.join(config_path, "config.yaml"))
     sample = os.path.abspath(os.path.join(config_path, "sample-run.h5"))
     exit_wave = os.path.abspath(os.path.join(config_path, "exit_wave-run.h5"))
     optics = os.path.abspath(os.path.join(config_path, "optics-run.h5"))
     image = os.path.abspath(os.path.join(config_path, "image-run.mrc"))
     assert os.path.exists(config)
     parakeet.command_line.run(
         ["-c", config, "-s", sample, "-e", exit_wave, "-o", optics, "-i", image]
     )
     assert os.path.exists(sample)
     assert os.path.exists(exit_wave)
     assert os.path.exists(optics)
     assert os.path.exists(image)
+
+
+def test_main(config_path):
+    config = os.path.abspath(os.path.join(config_path, "config.yaml"))
+    sample = os.path.abspath(os.path.join(config_path, "sample-main.h5"))
+    exit_wave = os.path.abspath(os.path.join(config_path, "exit_wave-main.h5"))
+    optics = os.path.abspath(os.path.join(config_path, "optics-main.h5"))
+    image = os.path.abspath(os.path.join(config_path, "image-main.mrc"))
+    assert os.path.exists(config)
+    parakeet.command_line.main(
+        ["run", "-c", config, "-s", sample, "-e", exit_wave, "-o", optics, "-i", image]
+    )
+    assert os.path.exists(sample)
+    assert os.path.exists(exit_wave)
+    assert os.path.exists(optics)
+    assert os.path.exists(image)
```

### Comparing `python-parakeet-0.4.3/tests/test_config.py` & `python-parakeet-0.4.4/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,38 +17,33 @@
             print(a, b, a == pytest.approx(b))
             return a == pytest.approx(b)
 
     return walk(a, b)
 
 
 def test_temp_directory():
-
     assert parakeet.config.temp_directory() == "_parakeet"
 
 
 def test_default():
-
     config = parakeet.config.default()
 
 
 def test_save(tmp_path):
-
     filename = os.path.join(tmp_path, "tmp-save.yaml")
     config = parakeet.config.default()
     parakeet.config.save(config, filename)
 
 
 def test_new(tmp_path):
-
     filename = os.path.join(tmp_path, "tmp.yaml")
     config = parakeet.config.new(filename)
 
 
 def test_edit(tmp_path):
-
     filename = os.path.join(tmp_path, "tmp.yaml")
     config = parakeet.config.new(filename)
     config = parakeet.config.edit(
         filename,
         config_obj="""
         sample:
             box:
@@ -68,18 +63,16 @@
     """,
     )
     assert config.sample.molecules.pdb[0].id == "4v1w"
     assert config.sample.box[0] == 2000
 
 
 def test_load(tmp_path):
-
     filename = os.path.join(tmp_path, "tmp.yaml")
     config = parakeet.config.new(filename)
     config = parakeet.config.load(filename)
 
     assert dict_approx_equal(config.dict(), parakeet.config.default().dict())
 
 
 def test_show():
-
     parakeet.config.show(parakeet.config.Config())
```

### Comparing `python-parakeet-0.4.3/tests/test_inelastic.py` & `python-parakeet-0.4.4/tests/test_inelastic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 from math import exp
 from parakeet import inelastic
 
 
 def test_zero_loss_fraction():
-
     cube = {"type": "cube", "cube": {"length": 3150}}
 
     cuboid = {
         "type": "cuboid",
         "cuboid": {"length_x": 1000, "length_y": 1000, "length_z": 3150},
     }
 
@@ -36,15 +35,14 @@
 
     angle = 60
     fraction = inelastic.zero_loss_fraction(cylinder, angle)
     assert fraction == pytest.approx(exp(-1))
 
 
 def test_mp_loss_fraction():
-
     cube = {"type": "cube", "cube": {"length": 3150}}
 
     cuboid = {
         "type": "cuboid",
         "cuboid": {"length_x": 1000, "length_y": 1000, "length_z": 3150},
     }
 
@@ -72,15 +70,14 @@
 
     angle = 60
     fraction = inelastic.mp_loss_fraction(cylinder, angle)
     assert fraction == pytest.approx(1 - exp(-1))
 
 
 def test_fraction_of_electrions():
-
     cube = {"type": "cube", "cube": {"length": 3150}}
 
     fraction = inelastic.fraction_of_electrons(cube, 0, "zero_loss")
     assert fraction == pytest.approx(exp(-1))
     fraction = inelastic.fraction_of_electrons(cube, 60, "zero_loss")
     assert fraction == pytest.approx(exp(-2))
 
@@ -97,13 +94,12 @@
     fraction = inelastic.fraction_of_electrons(cube, 0, "unfiltered")
     assert fraction == pytest.approx(1.0)
     fraction = inelastic.fraction_of_electrons(cube, 60, "unfiltered")
     assert fraction == pytest.approx(1.0)
 
 
 def test_most_probable_loss():
-
     cube = {"type": "cube", "cube": {"length": 3150}}
 
     peak, sigma = inelastic.most_probable_loss(300, cube, 0)
     assert peak == pytest.approx(17.92806966151457)
     assert sigma == pytest.approx(5.300095984425282)
```

### Comparing `python-parakeet-0.4.3/tests/test_io.py` & `python-parakeet-0.4.4/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import pytest
 import parakeet.io
 
 
 @pytest.fixture
 def io_test_data():
-
     # The shape of the data
     shape = (10, 100, 100)
 
     # Generate the data
     data = np.random.randint(low=0, high=100, size=shape[0] * shape[1] * shape[2])
     data.shape = shape
 
@@ -21,15 +20,14 @@
     position = np.array([[x, x, 0] for x in range(0, shape[0])])
 
     # Return the data
     return (data, angle, position)
 
 
 def test_read_write_mrcfile(tmp_path, io_test_data):
-
     filename = os.path.join(tmp_path, "tmp.mrc")
 
     data, angle, position = io_test_data
 
     writer = parakeet.io.new(filename, shape=data.shape)
     for i in range(data.shape[0]):
         writer.data[i, :, :] = data[i, :, :]
@@ -58,15 +56,14 @@
     assert reader.data.shape == (10, 100, 100)
     assert reader.header.size == 10
     assert np.all(np.equal(reader.header["tilt_alpha"], angle))
     assert np.all(np.equal(reader.header.position, position))
 
 
 def test_write_nexus(tmp_path, io_test_data):
-
     filename = os.path.join(tmp_path, "tmp.h5")
 
     data, angle, position = io_test_data
 
     writer = parakeet.io.new(filename, shape=data.shape)
     for i in range(data.shape[0]):
         writer.data[i, :, :] = data[i, :, :]
@@ -95,15 +92,14 @@
     assert reader.data.shape == (10, 100, 100)
     assert reader.header.size == 10
     assert np.all(np.equal(reader.header["tilt_alpha"], angle))
     assert np.all(np.equal(reader.header.position, position))
 
 
 def test_write_images(tmp_path, io_test_data):
-
     filename = os.path.join(tmp_path, "tmp_%03d.png")
 
     data, angle, position = io_test_data
 
     def test(vmin, vmax):
         writer = parakeet.io.new(filename, shape=data.shape, vmin=vmin, vmax=vmax)
         for i in range(data.shape[0]):
@@ -129,15 +125,14 @@
             assert os.path.exists(filename % (i + 1))
 
     test(None, None)
     test(np.min(data), np.max(data))
 
 
 def test_unknown_image(tmp_path):
-
     filename = os.path.join(tmp_path, "tmp.unknown")
 
     with pytest.raises(RuntimeError):
         writer = parakeet.io.new(filename, shape=(1, 10, 10))
 
     with pytest.raises(RuntimeError):
         reader = parakeet.io.open(filename)
```

### Comparing `python-parakeet-0.4.3/tests/test_landau.py` & `python-parakeet-0.4.4/tests/test_landau.py`

 * *Files identical despite different names*

### Comparing `python-parakeet-0.4.3/tests/test_sample.py` & `python-parakeet-0.4.4/tests/test_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import parakeet.sample
 import shutil
 from math import sqrt
 
 
 @pytest.fixture
 def atom_data_4v5d():
-
     # Get the filename of the 4v5d.cif file
     filename = parakeet.data.get_path("4v5d.cif")
 
     # Get the atom data
     atoms = parakeet.sample.AtomData.from_gemmi_file(filename)
     atoms.data = parakeet.sample.recentre(atoms.data)
     return atoms
@@ -51,36 +50,33 @@
 
     # Check dtypes
     for name, dtype in parakeet.sample.AtomData.column_data.items():
         assert data[name].dtype == dtype
 
 
 def test_number_of_water_molecules():
-
     n = parakeet.sample.number_of_water_molecules(1000**3)
     assert n == 31422283
 
 
 def test_random_uniform_rotation():
-
     rotations = parakeet.sample.random_uniform_rotation(size=10)
     assert rotations.shape == (10, 3)
 
 
 # def test_distribute_boxes_uniformly():
 
 #     positions = parakeet.sample.distribute_boxes_uniformly(
 #         ((0, 0, 0), (1000, 1000, 1000)), [(100, 100, 100), (200, 200, 200)]
 #     )
 
 #     assert len(positions) == 2
 
 
 def test_shape_bounding_box():
-
     b1 = parakeet.sample.shape_bounding_box(
         (0, 0, 0), {"type": "cube", "cube": {"length": 1}}
     )
     assert pytest.approx(b1[0]) == (-0.5, -0.5, -0.5)
     assert pytest.approx(b1[1]) == (0.5, 0.5, 0.5)
 
     b2 = parakeet.sample.shape_bounding_box(
@@ -94,15 +90,14 @@
         (0, 0, 0), {"type": "cylinder", "cylinder": {"length": 1, "radius": 2}}
     )
     assert pytest.approx(b3[0]) == (-2.0, -0.5, -2.0)
     assert pytest.approx(b3[1]) == (2.0, 0.5, 2.0)
 
 
 def test_shape_enclosed_box():
-
     b1 = parakeet.sample.shape_enclosed_box(
         (0, 0, 0), {"type": "cube", "cube": {"length": 1}}
     )
     assert pytest.approx(b1[0]) == (-0.5, -0.5, -0.5)
     assert pytest.approx(b1[1]) == (0.5, 0.5, 0.5)
 
     b2 = parakeet.sample.shape_enclosed_box(
@@ -116,15 +111,14 @@
         (0, 0, 0), {"type": "cylinder", "cylinder": {"length": 1, "radius": 2}}
     )
     assert pytest.approx(b3[0]) == (-sqrt(2.0), -0.5, -sqrt(2.0))
     assert pytest.approx(b3[1]) == (sqrt(2.0), 0.5, sqrt(2.0))
 
 
 def test_is_shape_inside_box():
-
     assert (
         parakeet.sample.is_shape_inside_box(
             (10, 10, 10), (0, 0, 0), {"type": "cube", "cube": {"length": 1}}
         )
         == False
     )
 
@@ -133,15 +127,14 @@
             (10, 10, 10), (5, 5, 5), {"type": "cube", "cube": {"length": 1}}
         )
         == True
     )
 
 
 def test_is_box_inside_shape():
-
     assert (
         parakeet.sample.is_box_inside_shape(
             ((0, 0, 0), (0.1, 0.1, 0.1)),
             (0, 0, 0),
             {"type": "cube", "cube": {"length": 1}},
         )
         == True
@@ -190,28 +183,26 @@
             {"type": "cylinder", "cylinder": {"length": 1, "radius": 1}},
         )
         == False
     )
 
 
 def test_AtomData(atom_data_4v5d):
-
     # Check rotate doesn't modify types
     atom_data_4v5d.rotate((0, 0, 1))
     for name, dtype in parakeet.sample.AtomData.column_data.items():
         assert atom_data_4v5d.data[name].dtype == dtype
 
     # Check translate keeps types
     atom_data_4v5d.translate((0, 0, 1))
     for name, dtype in parakeet.sample.AtomData.column_data.items():
         assert atom_data_4v5d.data[name].dtype == dtype
 
 
 def test_SampleHDF5Adapter(tmp_path, atom_data_4v5d):
-
     # Get handle
     handle = parakeet.sample.SampleHDF5Adapter(
         os.path.join(tmp_path, "test_SampleHDF5Adapter.h5"), "w"
     )
 
     # Test sample
     sample = handle.sample
@@ -259,15 +250,14 @@
     assert len(atoms) == 2
     assert atoms.number_of_atoms() == 3 * atom_data_4v5d.data.shape[0]
 
     handle.close()
 
 
 def test_Sample(tmp_path, atom_data_4v5d):
-
     sample = parakeet.sample.Sample(os.path.join(tmp_path, "test_Sample.h5"), mode="w")
 
     assert sample.atoms_dataset_name((1, 2, 3)) == "X=000001; Y=000002; Z=000003"
     a = list(sample.atoms_dataset_range((1, 2, 3), (3, 4, 5)))
     assert (a[0][0] == (0, 0, 0)).all()
     assert (a[0][1] == (sample.step, sample.step, sample.step)).all()
 
@@ -315,15 +305,14 @@
     sample.add_atoms(atom_data_4v5d)
 
     sample.info()
     sample.close()
 
 
 def test_AtomSliceExtractor(tmp_path):
-
     config = {
         "box": (50, 50, 50),
         "centre": (25, 25, 25),
         "shape": {"type": "cube", "cube": {"length": 40}},
         "ice": {"generate": True, "density": 940},
     }
 
@@ -343,15 +332,14 @@
         assert ((coords >= zslice.x_min) & (coords < zslice.x_max)).all(axis=1).all()
         num_atoms += zslice.atoms.data.shape[0]
 
     assert num_atoms == sample.number_of_atoms
 
 
 def test_AtomDeleter(tmp_path):
-
     config = {
         "box": (50, 50, 50),
         "centre": (25, 25, 25),
         "shape": {"type": "cube", "cube": {"length": 40}},
         "ice": {"generate": True, "density": 940},
     }
 
@@ -369,15 +357,14 @@
 
     atoms = deleter(atoms.data)
     coords = atoms[["x", "y", "z"]].to_numpy()
     assert ((coords - (50, 50, 50)) ** 2 >= 20).all()
 
 
 def test_load(tmp_path):
-
     config = {
         "box": (50, 50, 50),
         "centre": (25, 25, 25),
         "shape": {"type": "cylinder", "cylinder": {"length": 40, "radius": 20}},
     }
 
     sample = parakeet.sample.new(
@@ -387,15 +374,14 @@
 
     del sample
 
     sample = parakeet.sample.load(os.path.join(tmp_path, "test_load.h5"))
 
 
 def test_new(tmp_path):
-
     config = {
         "box": (50, 50, 50),
         "centre": (25, 25, 25),
         "shape": {"type": "cylinder", "cylinder": {"length": 40, "radius": 20}},
     }
 
     sample = parakeet.sample.new(
@@ -424,15 +410,14 @@
     margin = 2
     assert len(x) > 0
     assert ((y >= (5 - margin)) & (y < (45 + margin))).all()
     assert (((x - 25) ** 2 + (z - 25) ** 2) <= (20 + margin) ** 2).all()
 
 
 def test_add_molecules(tmp_path):
-
     config = {
         "box": (1000, 1000, 1000),
         "centre": (500, 500, 500),
         "shape": {"type": "cube", "cube": {"length": 1000}},
     }
 
     sample = parakeet.sample.new(
@@ -487,15 +472,14 @@
     )
 
     assert sample.number_of_molecules == 1
     assert sample.number_of_molecular_models == 1
 
 
 def test_sample_new_with_local(tmp_path):
-
     filename = os.path.join(tmp_path, "my.pdb")
 
     src = parakeet.data.get_4v1w()
     shutil.copyfile(src, filename)
 
     config = {
         "box": (50, 50, 50),
```

### Comparing `python-parakeet-0.4.3/tests/test_sample_distribute.py` & `python-parakeet-0.4.4/tests/test_sample_distribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 from parakeet.sample.distribute import CuboidVolume
 from parakeet.sample.distribute import CylindricalVolume
 from parakeet.sample.distribute import distribute_particles_uniformly
 
 
 def test_cube():
-
     radius = np.random.uniform(100, 250, size=1000)
 
     lower = (0, 0, 0)
     upper = (10000, 10000, 10000)
     volume = CuboidVolume(lower, upper)
 
     points = distribute_particles_uniformly(volume, radius)
@@ -22,15 +21,14 @@
             p2 = points[j]
             r1 = radius[i]
             r2 = radius[j]
             assert np.sqrt(np.sum((p1 - p2) ** 2)) > r1 + r2
 
 
 def test_cuboid():
-
     radius = np.random.uniform(100, 250, size=1000)
 
     lower = (0, 0, 0)
     upper = (10000, 1000, 10000)
     volume = CuboidVolume(lower, upper)
 
     points = distribute_particles_uniformly(volume, radius)
@@ -43,15 +41,14 @@
             p2 = points[j]
             r1 = radius[i]
             r2 = radius[j]
             assert np.sqrt(np.sum((p1 - p2) ** 2)) > r1 + r2
 
 
 def test_cylinder_1():
-
     radius = np.random.uniform(100, 250, size=1000)
 
     lower = 0
     upper = 10000
     volume = CylindricalVolume(lower, upper, [(0, 0)], [1500])
 
     points = distribute_particles_uniformly(volume, radius)
@@ -73,15 +70,14 @@
             p2 = points[j]
             r1 = radius[i]
             r2 = radius[j]
             assert np.sqrt(np.sum((p1 - p2) ** 2)) > r1 + r2
 
 
 def test_cylinder_2():
-
     radius = np.random.uniform(100, 250, size=400)
 
     lower = 0
     upper = 10000
     volume = CylindricalVolume(lower, upper, [(0, 0), (0, 0)], [1500, 500])
 
     points = distribute_particles_uniformly(volume, radius)
@@ -103,15 +99,14 @@
             p2 = points[j]
             r1 = radius[i]
             r2 = radius[j]
             assert np.sqrt(np.sum((p1 - p2) ** 2)) > r1 + r2
 
 
 def test_cylinder_3():
-
     radius = np.random.uniform(100, 250, size=900)
 
     lower = 0
     upper = 10000
     volume = CylindricalVolume(
         lower,
         upper,
@@ -149,15 +144,14 @@
             p2 = points[j]
             r1 = radius[i]
             r2 = radius[j]
             assert np.sqrt(np.sum((p1 - p2) ** 2)) > r1 + r2
 
 
 def test_cylinder_4():
-
     radius = np.random.uniform(100, 250, size=900)
 
     lower = 0
     upper = 10000
     volume = CylindricalVolume(
         lower,
         upper,
```

### Comparing `python-parakeet-0.4.3/tests/test_scan.py` & `python-parakeet-0.4.4/tests/test_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pytest
 import parakeet.scan
 
 
 def test_none():
     scan = parakeet.scan.new(mode=None)
-    assert np.all(np.equal(scan.axes, np.array([[0, 0, 0]])))
+    assert np.all(np.equal(scan.axes, np.array([[0, 1, 0]])))
     assert np.all(np.equal(scan.angles, np.array([0])))
     assert np.all(np.equal(scan.position, np.array([(0, 0, 0)])))
 
 
 def test_manual():
     scan = parakeet.scan.new(
         mode="manual", axis=(0, 1, 0), angles=[1, 2, 3], positions=[4, 5, 6]
@@ -17,15 +17,15 @@
     assert np.all(np.equal(scan.axes, np.array([[0, 1, 0]])))
     assert np.allclose(scan.angles, np.array([1, 2, 3]))
     assert np.allclose(scan.position, np.array([(0, i, 0) for i in [4, 5, 6]]))
 
 
 def test_still():
     scan = parakeet.scan.new(mode="still")
-    assert np.all(np.equal(scan.axes, np.array([[0, 0, 0]])))
+    assert np.all(np.equal(scan.axes, np.array([[0, 1, 0]])))
     assert np.all(np.equal(scan.angles, np.array([0])))
     assert np.all(np.equal(scan.position, np.array([(0, 0, 0)])))
 
 
 def test_tilt_series():
     scan = parakeet.scan.new(
         mode="tilt_series", axis=(1, 2, 3), start_angle=1, num_images=8, step_angle=45
@@ -88,22 +88,40 @@
 
     assert np.allclose(scan.axes, np.array([[0, 1, 0]] * 8 * 2))
     assert np.allclose(scan.angles, angles)
     assert np.allclose(scan.position, positions)
 
 
 def test_single_particle():
-
     scan = parakeet.scan.new(
         mode="single_particle",
         num_images=8,
     )
     assert len(scan) == 8
 
 
+def test_grid_scan():
+    scan = parakeet.scan.new(
+        mode="grid_scan",
+        axis=(0, 1, 0),
+        angles=[1, 2, 3, 4],
+        start_pos=(0, 0),
+        step_pos=(10, 10),
+        num_images=(10, 10),
+    )
+    angles = np.array([[1, 2, 3, 4]] * 10 * 10).T.flatten()
+    positions = np.array(
+        [(x * 10, y * 10, 0) for a in range(4) for y in range(10) for x in range(10)]
+    )
+    axis = np.array([[0, 1, 0]] * 10 * 10 * 4)
+    assert np.allclose(scan.axes, axis)
+    assert np.allclose(scan.angles, angles)
+    assert np.allclose(scan.position, positions)
+
+
 def test_beam_tilt():
     scan = parakeet.scan.new(
         mode="beam_tilt",
         axis=(0, 1, 0),
         angles=[1, 2, 3, 4],
         positions=[10, 20, 30, 40],
         theta=[0, 0, 0, 0, 0, 0],
@@ -111,19 +129,17 @@
     )
     angles = np.array([[1, 2, 3, 4]] * 6).T.flatten()
     positions = np.array([[10 * i for i in range(1, 5)]] * 6).T.flatten()
     positions = np.array([np.array((0, 1, 0)) * p for p in positions])
     theta = np.array([[0, 0, 0, 0, 0, 0]] * 4).flatten()
     phi = np.array([[0, 0.1, 0.2, 0.3, 0.4, 0.5]] * 4).flatten()
     axis = np.array([[0, 1, 0]] * 4 * 6)
-    print(scan.angles)
     assert np.allclose(scan.axes, axis)
     assert np.allclose(scan.angles, angles)
     assert np.allclose(scan.position, positions)
     assert np.allclose(scan.beam_tilt_theta, theta)
     assert np.allclose(scan.beam_tilt_phi, phi)
 
 
 def test_unknown():
-
     with pytest.raises(KeyError):
         scan = parakeet.scan.new("unknown")
```

### Comparing `python-parakeet-0.4.3/tests/test_slice.py` & `python-parakeet-0.4.4/tests/test_slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import parakeet.sample
 
 # from matplotlib import pylab
 
 
 def create_input_multislice(n_phonons, single_phonon_conf=False):
-
     # Initialise the input and system configuration
     input_multislice = multem.Input()
 
     # Set simulation experiment
     input_multislice.simulation_type = "EWRS"
 
     # Electron-Specimen interaction model
@@ -52,15 +51,14 @@
     input_multislice.obj_lens_zero_defocus_type = "Last"
     input_multislice.obj_lens_zero_defocus_plane = 0
 
     return input_multislice
 
 
 def test_slice(tmpdir_factory):
-
     directory = tmpdir_factory.mktemp("proc")
     filename = os.path.join(directory, "temp.h5")
     box = (400, 400, 400)
     centre = (200, 200, 200)
     shape = {"type": "cube", "cube": {"length": 400}}
     sample = parakeet.sample.new(
         parakeet.config.Sample(**{"box": box, "centre": centre, "shape": shape}),
```

### Comparing `python-parakeet-0.4.3/tests/test_sphere_packer.py` & `python-parakeet-0.4.4/tests/test_sphere_packer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from math import floor, pi
 import time
 import parakeet.freeze
 
 
 def test_sphere_packer():
-
     # Set the volume size
     length_x = 30  # A
     length_y = 30
     length_z = 30
     volume = length_x * length_y * length_z  # A^3
 
     # Determine the number of waters to place
```

