# Comparing `tmp/pyikarus-0.3.3.dev20230616134043.tar.gz` & `tmp/pyikarus-0.3.3.dev20230616134912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.3.dev20230616134043.tar", last modified: Fri Jun 16 13:40:44 2023, max compression
+gzip compressed data, was "pyikarus-0.3.3.dev20230616134912.tar", last modified: Fri Jun 16 13:49:13 2023, max compression
```

## Comparing `pyikarus-0.3.3.dev20230616134043.tar` & `pyikarus-0.3.3.dev20230616134912.tar`

### file list

```diff
@@ -1,333 +1,333 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.324735 pyikarus-0.3.3.dev20230616134043/
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.bettercodehub.yml
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.268735 pyikarus-0.3.3.dev20230616134043/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.280735 pyikarus-0.3.3.dev20230616134043/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.280735 pyikarus-0.3.3.dev20230616134043/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 root         (0) root         (0)     5549 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1834 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2612 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     2042 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/ghpages.yml
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/reuseLint.yml
--rw-r--r--   0 root         (0) root         (0)     3335 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/runExamples.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.280735 pyikarus-0.3.3.dev20230616134043/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.280735 pyikarus-0.3.3.dev20230616134043/.reuse/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5335 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.284735 pyikarus-0.3.3.dev20230616134043/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    18375 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/LICENSES/MIT.txt
--rw-r--r--   0 root         (0) root         (0)    16727 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:40:44.324735 pyikarus-0.3.3.dev20230616134043/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3418 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.284735 pyikarus-0.3.3.dev20230616134043/cmake/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.284735 pyikarus-0.3.3.dev20230616134043/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1807 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.284735 pyikarus-0.3.3.dev20230616134043/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/modules/AddSpectraFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/cmake/tools.cmake
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/codecov.yml
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.288735 pyikarus-0.3.3.dev20230616134043/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.288735 pyikarus-0.3.3.dev20230616134043/docs/BuildLocally/
--rw-r--r--   0 root         (0) root         (0)      439 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.288735 pyikarus-0.3.3.dev20230616134043/docs/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 root         (0) root         (0)     6961 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/literature.bib
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/literature.bib.license
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/mkdocs-macros.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/mkdocs.insiders.yml
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.272735 pyikarus-0.3.3.dev20230616134043/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.288735 pyikarus-0.3.3.dev20230616134043/docs/overrides/partials/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.288735 pyikarus-0.3.3.dev20230616134043/docs/website/
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.288735 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/
--rw-r--r--   0 root         (0) root         (0)     4710 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/assembler.md
--rw-r--r--   0 root         (0) root         (0)     6387 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 root         (0) root         (0)     2024 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 root         (0) root         (0)     3237 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 root         (0) root         (0)    12894 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 root         (0) root         (0)     2745 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/grids.md
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/index.md
--rw-r--r--   0 root         (0) root         (0)     4932 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/localBasis.md
--rw-r--r--   0 root         (0) root         (0)    44213 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 root         (0) root         (0)     3978 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/manifolds.md
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 root         (0) root         (0)     3086 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/observer.md
--rw-r--r--   0 root         (0) root         (0)     5211 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.292735 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/
--rw-r--r--   0 root         (0) root         (0)     6655 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/computePi.md
--rw-r--r--   0 root         (0) root         (0)     5439 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 root         (0) root         (0)     7323 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 root         (0) root         (0)     2164 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/index.md
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 root         (0) root         (0)     6164 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.292735 pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/
--rw-r--r--   0 root         (0) root         (0)     2439 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.292735 pyikarus-0.3.3.dev20230616134043/docs/website/04_blog/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/04_blog/.authors.yml
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.292735 pyikarus-0.3.3.dev20230616134043/docs/website/04_blog/posts/
--rw-r--r--   0 root         (0) root         (0)     7731 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.292735 pyikarus-0.3.3.dev20230616134043/docs/website/05_cppReferences/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.292735 pyikarus-0.3.3.dev20230616134043/docs/website/99_Literature/
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.296735 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/
--rw-r--r--   0 root         (0) root         (0)   280461 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/BigLogo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.296735 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 root         (0) root         (0)    52795 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 root         (0) root         (0)    46250 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 root         (0) root         (0)     2852 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 root         (0) root         (0)    17924 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 root         (0) root         (0)     9455 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.300735 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 root         (0) root         (0)    35234 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 root         (0) root         (0)    62184 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 root         (0) root         (0)     2281 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 root         (0) root         (0)    40033 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 root         (0) root         (0)    25505 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 root         (0) root         (0)   441218 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/logo_blue.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/logo_blue.png.license
--rw-r--r--   0 root         (0) root         (0)   482004 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/logo_white.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/logo_white.png.license
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/download.md
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/gallery.md
--rw-r--r--   0 root         (0) root         (0)     1423 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.300735 pyikarus-0.3.3.dev20230616134043/docs/website/javascripts/
--rw-r--r--   0 root         (0) root         (0)      486 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.300735 pyikarus-0.3.3.dev20230616134043/docs/website/stylesheets/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/docs/website/stylesheets/extra.css
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.300735 pyikarus-0.3.3.dev20230616134043/ikarus/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.300735 pyikarus-0.3.3.dev20230616134043/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12924 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 root         (0) root         (0)    10714 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.300735 pyikarus-0.3.3.dev20230616134043/ikarus/controlRoutines/
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2575 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 root         (0) root         (0)     2970 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.300735 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.304735 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 root         (0) root         (0)     1827 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 root         (0) root         (0)     9346 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 root         (0) root         (0)     1338 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.304735 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    21360 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 root         (0) root         (0)    14203 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.304735 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5699 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)     4635 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 root         (0) root         (0)     5734 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 root         (0) root         (0)     7995 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 root         (0) root         (0)    15991 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 root         (0) root         (0)    12678 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.304735 pyikarus-0.3.3.dev20230616134043/ikarus/io/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/io/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/io/resultEvaluators.hh
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/io/resultFunction.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6735 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 root         (0) root         (0)     7698 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 root         (0) root         (0)    12303 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/assembler/
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6752 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/basis/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/dirichletValues/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4169 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5220 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/materials/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9949 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 root         (0) root         (0)     5207 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/test/
--rw-r--r--   0 root         (0) root         (0)      511 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3830 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)     4340 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/python/utils/
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.308735 pyikarus-0.3.3.dev20230616134043/ikarus/solver/
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.312735 pyikarus-0.3.3.dev20230616134043/ikarus/solver/linearSolver/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8891 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.312735 pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5406 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 root         (0) root         (0)     8297 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 root         (0) root         (0)    18574 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.316735 pyikarus-0.3.3.dev20230616134043/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/algorithms.hh
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/basis.hh
--rw-r--r--   0 root         (0) root         (0)     6930 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.316735 pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 root         (0) root         (0)     2347 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 root         (0) root         (0)     1367 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 root         (0) root         (0)     2171 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 root         (0) root         (0)     6359 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 root         (0) root         (0)     3152 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/init.hh
--rw-r--r--   0 root         (0) root         (0)    15244 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.316735 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 root         (0) root         (0)     5497 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/observer.hh
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/polyfit.cpp
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/polyfit.hh
--rw-r--r--   0 root         (0) root         (0)    10054 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 root         (0) root         (0)    15149 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus/utils/traits.hh
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/ikarus.pc.in
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/iwyu.imp
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.316735 pyikarus-0.3.3.dev20230616134043/python/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/python/ikarus/
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/python/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/assembler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/basis.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/python/ikarus/finite_elements/
--rw-r--r--   0 root         (0) root         (0)      173 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/finite_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/generator.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/python/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:40:44.000000 pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10107 2023-06-16 13:40:44.000000 pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 13:40:44.000000 pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:40:44.000000 pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-16 13:40:44.000000 pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/sandbox/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/sandbox/src/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)   674469 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 13:40:44.324735 pyikarus-0.3.3.dev20230616134043/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-06-16 13:40:43.000000 pyikarus-0.3.3.dev20230616134043/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.320735 pyikarus-0.3.3.dev20230616134043/tests/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.324735 pyikarus-0.3.3.dev20230616134043/tests/src/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3907 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testAssembler.cpp
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 root         (0) root         (0)    14291 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testCommon.hh
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testDependencies.cpp
--rw-r--r--   0 root         (0) root         (0)     6520 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testDirichletValue.cpp
--rw-r--r--   0 root         (0) root         (0)     4795 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testEAS.hh
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testEnhancedAssumedStrains.cpp
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFEElement.hh
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFactories.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:40:44.324735 pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/
--rw-r--r--   0 root         (0) root         (0)     9028 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 root         (0) root         (0)      546 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 root         (0) root         (0)    11431 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testFunctionTraits.cpp
--rw-r--r--   0 root         (0) root         (0)     1114 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testHelpers.hh
--rw-r--r--   0 root         (0) root         (0)     3190 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testLinearElasticity.cpp
--rw-r--r--   0 root         (0) root         (0)     2278 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testManifolds.cpp
--rw-r--r--   0 root         (0) root         (0)     7949 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testMaterial.cpp
--rw-r--r--   0 root         (0) root         (0)    15845 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearElasticityNeoHooke.cpp
--rw-r--r--   0 root         (0) root         (0)     1121 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearElasticitySVK.cpp
--rw-r--r--   0 root         (0) root         (0)     9846 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearOperator.cpp
--rw-r--r--   0 root         (0) root         (0)     6251 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testPathFollowing.cpp
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testPolyFit.cpp
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testPythonConversion.cpp
--rw-r--r--   0 root         (0) root         (0)    17531 2023-06-16 13:40:36.000000 pyikarus-0.3.3.dev20230616134043/tests/src/testTrustRegion.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.629992 pyikarus-0.3.3.dev20230616134912/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.553991 pyikarus-0.3.3.dev20230616134912/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.569991 pyikarus-0.3.3.dev20230616134912/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.569991 pyikarus-0.3.3.dev20230616134912/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.569991 pyikarus-0.3.3.dev20230616134912/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.569991 pyikarus-0.3.3.dev20230616134912/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.573991 pyikarus-0.3.3.dev20230616134912/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:49:13.629992 pyikarus-0.3.3.dev20230616134912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3418 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.573991 pyikarus-0.3.3.dev20230616134912/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.573991 pyikarus-0.3.3.dev20230616134912/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.573991 pyikarus-0.3.3.dev20230616134912/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/modules/AddSpectraFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.577991 pyikarus-0.3.3.dev20230616134912/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.577991 pyikarus-0.3.3.dev20230616134912/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.577991 pyikarus-0.3.3.dev20230616134912/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.553991 pyikarus-0.3.3.dev20230616134912/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.577991 pyikarus-0.3.3.dev20230616134912/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.577991 pyikarus-0.3.3.dev20230616134912/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.581991 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.581991 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6164 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.585991 pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.585991 pyikarus-0.3.3.dev20230616134912/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.585991 pyikarus-0.3.3.dev20230616134912/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.585991 pyikarus-0.3.3.dev20230616134912/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.585991 pyikarus-0.3.3.dev20230616134912/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.585991 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/
+-rw-r--r--   0 root         (0) root         (0)   280461 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/BigLogo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.589991 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.593991 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)   441218 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/logo_blue.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/logo_blue.png.license
+-rw-r--r--   0 root         (0) root         (0)   482004 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/logo_white.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/logo_white.png.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.593991 pyikarus-0.3.3.dev20230616134912/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.593991 pyikarus-0.3.3.dev20230616134912/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.593991 pyikarus-0.3.3.dev20230616134912/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.593991 pyikarus-0.3.3.dev20230616134912/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.593991 pyikarus-0.3.3.dev20230616134912/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.597991 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.597991 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.597991 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    21360 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    14203 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.601991 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     7995 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.601991 pyikarus-0.3.3.dev20230616134912/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.601991 pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7698 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.601991 pyikarus-0.3.3.dev20230616134912/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.601991 pyikarus-0.3.3.dev20230616134912/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.601991 pyikarus-0.3.3.dev20230616134912/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.601991 pyikarus-0.3.3.dev20230616134912/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.605991 pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.605991 pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.605991 pyikarus-0.3.3.dev20230616134912/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.605991 pyikarus-0.3.3.dev20230616134912/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.605991 pyikarus-0.3.3.dev20230616134912/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.605991 pyikarus-0.3.3.dev20230616134912/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.605991 pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.613992 pyikarus-0.3.3.dev20230616134912/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.613992 pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.617992 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10054 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.617992 pyikarus-0.3.3.dev20230616134912/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.617992 pyikarus-0.3.3.dev20230616134912/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.617992 pyikarus-0.3.3.dev20230616134912/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.617992 pyikarus-0.3.3.dev20230616134912/python/ikarus/finite_elements/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.617992 pyikarus-0.3.3.dev20230616134912/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.621992 pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-16 13:49:13.000000 pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10107 2023-06-16 13:49:13.000000 pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 13:49:13.000000 pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-16 13:49:13.000000 pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-16 13:49:13.000000 pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.621992 pyikarus-0.3.3.dev20230616134912/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.621992 pyikarus-0.3.3.dev20230616134912/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.621992 pyikarus-0.3.3.dev20230616134912/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 13:49:13.629992 pyikarus-0.3.3.dev20230616134912/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-16 13:49:12.000000 pyikarus-0.3.3.dev20230616134912/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.621992 pyikarus-0.3.3.dev20230616134912/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.629992 pyikarus-0.3.3.dev20230616134912/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testAssembler.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)    14291 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testCommon.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testDependencies.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testDirichletValue.cpp
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testEAS.hh
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testEnhancedAssumedStrains.cpp
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFEElement.hh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFactories.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:49:13.629992 pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testFunctionTraits.cpp
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testLinearElasticity.cpp
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testManifolds.cpp
+-rw-r--r--   0 root         (0) root         (0)     7949 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testMaterial.cpp
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearElasticityNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearElasticitySVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearOperator.cpp
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testPathFollowing.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testPolyFit.cpp
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testPythonConversion.cpp
+-rw-r--r--   0 root         (0) root         (0)    17531 2023-06-16 13:49:05.000000 pyikarus-0.3.3.dev20230616134912/tests/src/testTrustRegion.cpp
```

### Comparing `pyikarus-0.3.3.dev20230616134043/.clang-format` & `pyikarus-0.3.3.dev20230616134912/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.cmake-format` & `pyikarus-0.3.3.dev20230616134912/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.3.dev20230616134912/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/createRelease.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/createRelease.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
       - uses: actions/checkout@v2
         with:
           path: 'repo'
           token: ${{ secrets.ORGANIZATION_TOKEN }}
       - name: Create tag and push tag
         run: |
           cd repo
+          python .github/workflows/scripts/release.py $NEWVERSION
           git config --local user.email "mueller@ibb.uni-stuttgart.de"
           git config --local user.name "AlexanderMueller"
           git remote set-url origin https://${{ secrets.ORGANIZATION_TOKEN }}@github.com/ikarus-project/ikarus.git
           git add .
           git commit -m "Create release v$NEWVERSION"
           #git tag -a v$NEWVERSION -m "Create release v$NEWVERSION"
```

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/debian.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/ghpages.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/releasePythonPackage.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/runExamples.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/scripts/release.py` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/scripts/release.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,16 +54,18 @@
 
 
 
 
 def update_all_versions(version_override=None):
     """Update all version numbers in local files"""
     old_version_number = read_old_version()
-    if version_override is None or version_override== "dev":
+    if  version_override== "dev":
         new_version_number = bump_patch_number(old_version_number)
+    elif version_override is None:
+        new_version_number = old_version_number
     else:
         new_version_number = version_override
 
     if version_override== "dev":
         new_version_number += '.dev' + datetime.now().strftime('%Y%m%d%H%M%S')
 
     print(f"Bump version from {old_version_number} to {new_version_number}")
```

### Comparing `pyikarus-0.3.3.dev20230616134043/.github/workflows/style.yml` & `pyikarus-0.3.3.dev20230616134912/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/.reuse/dep5` & `pyikarus-0.3.3.dev20230616134912/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/CHANGELOG.md` & `pyikarus-0.3.3.dev20230616134912/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/CMakeLists.txt` & `pyikarus-0.3.3.dev20230616134912/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/CODE_OF_CONDUCT.md` & `pyikarus-0.3.3.dev20230616134912/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/LICENSE.md` & `pyikarus-0.3.3.dev20230616134912/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.3.dev20230616134912/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.3.dev20230616134912/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.3.dev20230616134912/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/LICENSES/MIT.txt` & `pyikarus-0.3.3.dev20230616134912/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.3.dev20230616134912/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/PKG-INFO` & `pyikarus-0.3.3.dev20230616134912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230616134043
+Version: 0.3.3.dev20230616134912
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230616134043 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230616134912 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
 BigLogo.png]
```

### Comparing `pyikarus-0.3.3.dev20230616134043/README.md` & `pyikarus-0.3.3.dev20230616134912/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/CPM.cmake` & `pyikarus-0.3.3.dev20230616134912/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.3.dev20230616134912/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.3.dev20230616134912/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.3.dev20230616134912/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.3.dev20230616134912/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.3.dev20230616134912/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/modules/AddSpectraFlags.cmake` & `pyikarus-0.3.3.dev20230616134912/cmake/modules/AddSpectraFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/cmake/tools.cmake` & `pyikarus-0.3.3.dev20230616134912/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/config.h.cmake` & `pyikarus-0.3.3.dev20230616134912/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.3.dev20230616134912/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/literature.bib` & `pyikarus-0.3.3.dev20230616134912/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/mkdocs-macros.py` & `pyikarus-0.3.3.dev20230616134912/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/mkdocs.yml` & `pyikarus-0.3.3.dev20230616134912/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/overrides/partials/comments.html` & `pyikarus-0.3.3.dev20230616134912/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/assembler.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/grids.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/index.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/observer.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/01_framework/solvers.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/computePi.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/index.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/BigLogo.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/BigLogo.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/logo_blue.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/logo_blue.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/auxiliaryImages/logo_white.png` & `pyikarus-0.3.3.dev20230616134912/docs/website/auxiliaryImages/logo_white.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/download.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/docs/website/index.md` & `pyikarus-0.3.3.dev20230616134912/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/CMakeLists.txt` & `pyikarus-0.3.3.dev20230616134912/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.3.dev20230616134912/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/io/resultEvaluators.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/io/resultEvaluators.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/io/resultFunction.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/io/resultFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/basis/basis.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/algorithms.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/basis.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/concepts.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/init.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/polyfit.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/ikarus/utils/traits.hh` & `pyikarus-0.3.3.dev20230616134912/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/__init__.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/_ikarus.cc` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/basis.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/dirichletValues.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/generator.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/generator.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/materials.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/ikarus/utils/__init__.py` & `pyikarus-0.3.3.dev20230616134912/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230616134043
+Version: 0.3.3.dev20230616134912
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230616134043 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230616134912 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
 BigLogo.png]
```

### Comparing `pyikarus-0.3.3.dev20230616134043/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.3.dev20230616134912/python/pyikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/python/setup.py.in` & `pyikarus-0.3.3.dev20230616134912/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230616134912/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.3.dev20230616134912/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/setup.py` & `pyikarus-0.3.3.dev20230616134912/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # build _ikarus
 # cd /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-ikarusVersion = "0.3.3.dev20230616134043"
+ikarusVersion = "0.3.3.dev20230616134912"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230616134912/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testAssembler.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testAssembler.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testCommon.hh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testCommon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testDependencies.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testDependencies.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testDirichletValue.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testDirichletValue.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testEAS.hh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testEAS.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testEnhancedAssumedStrains.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testEnhancedAssumedStrains.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testFEElement.hh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testFactories.hh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testFactories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testFunctionTraits.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testFunctionTraits.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testHelpers.hh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testLinearElasticity.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testLinearElasticity.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testManifolds.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testManifolds.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testMaterial.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testMaterial.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearElasticity.hh` & `pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearElasticityNeoHooke.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearElasticityNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearElasticitySVK.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearElasticitySVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testNonLinearOperator.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testNonLinearOperator.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testPathFollowing.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testPathFollowing.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testPolyFit.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testPolyFit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testPythonConversion.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testPythonConversion.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230616134043/tests/src/testTrustRegion.cpp` & `pyikarus-0.3.3.dev20230616134912/tests/src/testTrustRegion.cpp`

 * *Files identical despite different names*

