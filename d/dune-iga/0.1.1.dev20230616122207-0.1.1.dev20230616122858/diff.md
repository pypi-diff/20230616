# Comparing `tmp/dune-iga-0.1.1.dev20230616122207.tar.gz` & `tmp/dune-iga-0.1.1.dev20230616122858.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-iga-0.1.1.dev20230616122207.tar", last modified: Fri Jun 16 12:22:08 2023, max compression
+gzip compressed data, was "dune-iga-0.1.1.dev20230616122858.tar", last modified: Fri Jun 16 12:28:59 2023, max compression
```

## Comparing `dune-iga-0.1.1.dev20230616122207.tar` & `dune-iga-0.1.1.dev20230616122858.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.386018 dune-iga-0.1.1.dev20230616122207/
--rw-r--r--   0 root         (0) root         (0)     1025 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.clang-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.350018 dune-iga-0.1.1.dev20230616122207/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.358018 dune-iga-0.1.1.dev20230616122207/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1758 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2245 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.github/workflows/reuseLint.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.358018 dune-iga-0.1.1.dev20230616122207/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3142 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.358018 dune-iga-0.1.1.dev20230616122207/.reuse/
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.358018 dune-iga-0.1.1.dev20230616122207/LICENSES/
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-16 12:22:08.386018 dune-iga-0.1.1.dev20230616122207/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.358018 dune-iga-0.1.1.dev20230616122207/cmake/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.358018 dune-iga-0.1.1.dev20230616122207/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/FormatTarget/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/FormatTarget/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.362018 dune-iga-0.1.1.dev20230616122207/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      753 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      843 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/modules/AddClipperLibFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      826 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/modules/AddEarCutFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      824 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/modules/AddnLohmannJsonFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/cmake/modules/DuneIgaMacros.cmake
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.362018 dune-iga-0.1.1.dev20230616122207/dune/
--rw-r--r--   0 root         (0) root         (0)      219 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.366018 dune-iga-0.1.1.dev20230616122207/dune/iga/
--rw-r--r--   0 root         (0) root         (0)      808 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9152 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/bsplinealgorithms.hh
--rw-r--r--   0 root         (0) root         (0)     2017 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/controlpoint.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.370018 dune-iga-0.1.1.dev20230616122207/dune/iga/geometry/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/geometry/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6122 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/geometry/closestpointprojection.hh
--rw-r--r--   0 root         (0) root         (0)     2825 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/geometry/geohelper.hh
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/gridcapabilities.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.370018 dune-iga-0.1.1.dev20230616122207/dune/iga/io/
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/io/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.370018 dune-iga-0.1.1.dev20230616122207/dune/iga/io/ibra/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/io/ibra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    10369 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/io/ibra/ibrageometry.hh
--rw-r--r--   0 root         (0) root         (0)     7806 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/io/ibra/ibrareader.hh
--rw-r--r--   0 root         (0) root         (0)     8239 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/io/igadatacollector.hh
--rw-r--r--   0 root         (0) root         (0)    30655 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsalgorithms.hh
--rw-r--r--   0 root         (0) root         (0)    29306 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsbasis.hh
--rw-r--r--   0 root         (0) root         (0)    18305 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgeometry.hh
--rw-r--r--   0 root         (0) root         (0)    11629 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgrid.hh
--rw-r--r--   0 root         (0) root         (0)    13111 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridentity.hh
--rw-r--r--   0 root         (0) root         (0)     3063 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridindexsets.hh
--rw-r--r--   0 root         (0) root         (0)     3957 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridleafiterator.hh
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridtraits.hh
--rw-r--r--   0 root         (0) root         (0)     1285 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsidset.hh
--rw-r--r--   0 root         (0) root         (0)     7882 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsintersection.hh
--rw-r--r--   0 root         (0) root         (0)     9302 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsleafgridview.hh
--rw-r--r--   0 root         (0) root         (0)     9447 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbslocalgeometry.hh
--rw-r--r--   0 root         (0) root         (0)    36685 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbspatch.hh
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbspatchdata.hh
--rw-r--r--   0 root         (0) root         (0)     9061 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/nurbspatchgeometry.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.370018 dune-iga-0.1.1.dev20230616122207/dune/iga/test/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.374018 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)     5772 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/element.ibra
--rw-r--r--   0 root         (0) root         (0)     7222 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/element_trim.ibra
--rw-r--r--   0 root         (0) root         (0)     7396 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra
--rw-r--r--   0 root         (0) root         (0)     7665 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/infty_pwh.ibra
--rw-r--r--   0 root         (0) root         (0)     6209 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/nurbs_1.ibra
--rw-r--r--   0 root         (0) root         (0)     6704 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/pipe_trim.ibra
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/plate_quarter.ibra
--rw-r--r--   0 root         (0) root         (0)    10170 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/schale_trim.ibra
--rw-r--r--   0 root         (0) root         (0)    12176 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/shell-hole.ibra
--rw-r--r--   0 root         (0) root         (0)     7146 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/shell.ibra
--rw-r--r--   0 root         (0) root         (0)     7688 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/surface-hole.ibra
--rw-r--r--   0 root         (0) root         (0)    60433 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/surface-multihole.ibra
--rw-r--r--   0 root         (0) root         (0)    45902 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/gridTests.cc
--rw-r--r--   0 root         (0) root         (0)    17532 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/test/trimmedGridTests.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.374018 dune-iga-0.1.1.dev20230616122207/dune/iga/trim/
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/trim/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4636 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/trim/nurbstrimboundary.hh
--rw-r--r--   0 root         (0) root         (0)    37350 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/trim/nurbstrimmer.hh
--rw-r--r--   0 root         (0) root         (0)    14597 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/trim/trimmedelementrepresentation.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.374018 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/
--rw-r--r--   0 root         (0) root         (0)      328 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/fillquadraturerule.hh
--rw-r--r--   0 root         (0) root         (0)     2372 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/igahelpers.hh
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/linearalgebra.hh
--rw-r--r--   0 root         (0) root         (0)    22061 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/mdnet.hh
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/iga/utils/typetraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.378018 dune-iga-0.1.1.dev20230616122207/dune/python/
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.378018 dune-iga-0.1.1.dev20230616122207/dune/python/iga/
--rw-r--r--   0 root         (0) root         (0)      290 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/iga/boundarypatch.hh
--rw-r--r--   0 root         (0) root         (0)     6370 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/iga/grid.hh
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/iga/gridenums.hh
--rw-r--r--   0 root         (0) root         (0)     4441 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/iga/nurbspatchdata.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.378018 dune-iga-0.1.1.dev20230616122207/dune/python/test/
--rw-r--r--   0 root         (0) root         (0)      461 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5187 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/test/poisson.py
--rw-r--r--   0 root         (0) root         (0)     5241 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/test/readGrid.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune/python/test/setpath.py.in
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune-iga.pc.in
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/dune.module
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.378018 dune-iga-0.1.1.dev20230616122207/python/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.378018 dune-iga-0.1.1.dev20230616122207/python/dune/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.382018 dune-iga-0.1.1.dev20230616122207/python/dune/iga/
--rw-r--r--   0 root         (0) root         (0)      675 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/__init__.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/_boundarypatch.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/_iga.cc
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/_igagrids.py
--rw-r--r--   0 root         (0) root         (0)     3110 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/_nurbsAlgorithms.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/_nurbspatchdata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.382018 dune-iga-0.1.1.dev20230616122207/python/dune/iga/basis/
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/python/dune/iga/basis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.382018 dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-16 12:22:08.000000 dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3635 2023-06-16 12:22:08.000000 dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:22:08.000000 dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-16 12:22:08.000000 dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-16 12:22:08.000000 dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:22:08.386018 dune-iga-0.1.1.dev20230616122207/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      889 2023-06-16 12:22:07.000000 dune-iga-0.1.1.dev20230616122207/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.382018 dune-iga-0.1.1.dev20230616122207/src/
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:08.386018 dune-iga-0.1.1.dev20230616122207/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)      228 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/auxiliaryFiles/kirchhoff_plate.parset
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/auxiliaryFiles/linear2dsolid.parset
--rw-r--r--   0 root         (0) root         (0)     7688 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/auxiliaryFiles/surface-hole.ibra
--rw-r--r--   0 root         (0) root         (0)     6609 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/kirchhoff_plate.cc
--rw-r--r--   0 root         (0) root         (0)    13589 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/kirchhoffplate.hh
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/linear2dsolid.cc
--rw-r--r--   0 root         (0) root         (0)    15691 2023-06-16 12:21:57.000000 dune-iga-0.1.1.dev20230616122207/src/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.304460 dune-iga-0.1.1.dev20230616122858/
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.clang-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.244460 dune-iga-0.1.1.dev20230616122858/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.256460 dune-iga-0.1.1.dev20230616122858/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1758 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.github/workflows/reuseLint.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.256460 dune-iga-0.1.1.dev20230616122858/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.260460 dune-iga-0.1.1.dev20230616122858/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.260460 dune-iga-0.1.1.dev20230616122858/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-16 12:28:59.304460 dune-iga-0.1.1.dev20230616122858/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.260460 dune-iga-0.1.1.dev20230616122858/cmake/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.260460 dune-iga-0.1.1.dev20230616122858/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/FormatTarget/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/FormatTarget/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.264460 dune-iga-0.1.1.dev20230616122858/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      843 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/modules/AddClipperLibFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      826 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/modules/AddEarCutFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/modules/AddnLohmannJsonFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/cmake/modules/DuneIgaMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.264460 dune-iga-0.1.1.dev20230616122858/dune/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.272460 dune-iga-0.1.1.dev20230616122858/dune/iga/
+-rw-r--r--   0 root         (0) root         (0)      808 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9152 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/bsplinealgorithms.hh
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/controlpoint.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.272460 dune-iga-0.1.1.dev20230616122858/dune/iga/geometry/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/geometry/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6122 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/geometry/closestpointprojection.hh
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/geometry/geohelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/gridcapabilities.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.272460 dune-iga-0.1.1.dev20230616122858/dune/iga/io/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/io/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.272460 dune-iga-0.1.1.dev20230616122858/dune/iga/io/ibra/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/io/ibra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    10369 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/io/ibra/ibrageometry.hh
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/io/ibra/ibrareader.hh
+-rw-r--r--   0 root         (0) root         (0)     8239 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/io/igadatacollector.hh
+-rw-r--r--   0 root         (0) root         (0)    30655 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsalgorithms.hh
+-rw-r--r--   0 root         (0) root         (0)    29306 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsbasis.hh
+-rw-r--r--   0 root         (0) root         (0)    18305 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgeometry.hh
+-rw-r--r--   0 root         (0) root         (0)    11629 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgrid.hh
+-rw-r--r--   0 root         (0) root         (0)    13111 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridentity.hh
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridindexsets.hh
+-rw-r--r--   0 root         (0) root         (0)     3957 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridleafiterator.hh
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridtraits.hh
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsidset.hh
+-rw-r--r--   0 root         (0) root         (0)     7882 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsintersection.hh
+-rw-r--r--   0 root         (0) root         (0)     9302 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsleafgridview.hh
+-rw-r--r--   0 root         (0) root         (0)     9447 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbslocalgeometry.hh
+-rw-r--r--   0 root         (0) root         (0)    36685 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbspatch.hh
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbspatchdata.hh
+-rw-r--r--   0 root         (0) root         (0)     9061 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/nurbspatchgeometry.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.276460 dune-iga-0.1.1.dev20230616122858/dune/iga/test/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.280460 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)     5772 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/element.ibra
+-rw-r--r--   0 root         (0) root         (0)     7222 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/element_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)     7396 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/infty_pwh.ibra
+-rw-r--r--   0 root         (0) root         (0)     6209 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/nurbs_1.ibra
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/pipe_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/plate_quarter.ibra
+-rw-r--r--   0 root         (0) root         (0)    10170 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/schale_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)    12176 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/shell-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)     7146 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/shell.ibra
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/surface-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)    60433 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/surface-multihole.ibra
+-rw-r--r--   0 root         (0) root         (0)    45902 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/gridTests.cc
+-rw-r--r--   0 root         (0) root         (0)    17532 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/test/trimmedGridTests.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.280460 dune-iga-0.1.1.dev20230616122858/dune/iga/trim/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/trim/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/trim/nurbstrimboundary.hh
+-rw-r--r--   0 root         (0) root         (0)    37350 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/trim/nurbstrimmer.hh
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/trim/trimmedelementrepresentation.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.284460 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/fillquadraturerule.hh
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/igahelpers.hh
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/linearalgebra.hh
+-rw-r--r--   0 root         (0) root         (0)    22061 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/mdnet.hh
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/iga/utils/typetraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.284460 dune-iga-0.1.1.dev20230616122858/dune/python/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.288460 dune-iga-0.1.1.dev20230616122858/dune/python/iga/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/iga/boundarypatch.hh
+-rw-r--r--   0 root         (0) root         (0)     6370 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/iga/grid.hh
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/iga/gridenums.hh
+-rw-r--r--   0 root         (0) root         (0)     4441 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/iga/nurbspatchdata.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.292460 dune-iga-0.1.1.dev20230616122858/dune/python/test/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5187 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/test/poisson.py
+-rw-r--r--   0 root         (0) root         (0)     5241 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/test/readGrid.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune/python/test/setpath.py.in
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune-iga.pc.in
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/dune.module
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.292460 dune-iga-0.1.1.dev20230616122858/python/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.292460 dune-iga-0.1.1.dev20230616122858/python/dune/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.296460 dune-iga-0.1.1.dev20230616122858/python/dune/iga/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/_boundarypatch.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/_iga.cc
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/_igagrids.py
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/_nurbsAlgorithms.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/_nurbspatchdata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.296460 dune-iga-0.1.1.dev20230616122858/python/dune/iga/basis/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/python/dune/iga/basis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.300460 dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-16 12:28:59.000000 dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-06-16 12:28:59.000000 dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:28:59.000000 dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-16 12:28:59.000000 dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-16 12:28:59.000000 dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:28:59.304460 dune-iga-0.1.1.dev20230616122858/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-16 12:28:58.000000 dune-iga-0.1.1.dev20230616122858/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.300460 dune-iga-0.1.1.dev20230616122858/src/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:28:59.304460 dune-iga-0.1.1.dev20230616122858/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/auxiliaryFiles/kirchhoff_plate.parset
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/auxiliaryFiles/linear2dsolid.parset
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/auxiliaryFiles/surface-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)     6609 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/kirchhoff_plate.cc
+-rw-r--r--   0 root         (0) root         (0)    13589 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/kirchhoffplate.hh
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/linear2dsolid.cc
+-rw-r--r--   0 root         (0) root         (0)    15691 2023-06-16 12:28:47.000000 dune-iga-0.1.1.dev20230616122858/src/linearElastic.hh
```

### Comparing `dune-iga-0.1.1.dev20230616122207/.clang-format` & `dune-iga-0.1.1.dev20230616122858/.clang-format`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/.github/workflows/debian-coverage.yml` & `dune-iga-0.1.1.dev20230616122858/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/.github/workflows/debian.yml` & `dune-iga-0.1.1.dev20230616122858/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/.github/workflows/releasePythonPackage.yml` & `dune-iga-0.1.1.dev20230616122858/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/.github/workflows/scripts/release.py` & `dune-iga-0.1.1.dev20230616122858/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/.github/workflows/style.yml` & `dune-iga-0.1.1.dev20230616122858/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/CMakeLists.txt` & `dune-iga-0.1.1.dev20230616122858/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/LICENSES/CC0-1.0.txt` & `dune-iga-0.1.1.dev20230616122858/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/LICENSES/LGPL-3.0-or-later.txt` & `dune-iga-0.1.1.dev20230616122858/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/PKG-INFO` & `dune-iga-0.1.1.dev20230616122858/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-iga
-Version: 0.1.1.dev20230616122207
+Version: 0.1.1.dev20230616122858
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

### Comparing `dune-iga-0.1.1.dev20230616122207/README.md` & `dune-iga-0.1.1.dev20230616122858/README.md`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/cmake/FormatTarget/CMakeLists.txt` & `dune-iga-0.1.1.dev20230616122858/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/cmake/FormatTarget/CPM.cmake` & `dune-iga-0.1.1.dev20230616122858/cmake/FormatTarget/CPM.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/cmake/modules/AddAutoDiffFlags.cmake` & `dune-iga-0.1.1.dev20230616122858/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/cmake/modules/AddClipperLibFlags.cmake` & `dune-iga-0.1.1.dev20230616122858/cmake/modules/AddClipperLibFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/cmake/modules/AddEarCutFlags.cmake` & `dune-iga-0.1.1.dev20230616122858/cmake/modules/AddEarCutFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/cmake/modules/AddEigenFlags.cmake` & `dune-iga-0.1.1.dev20230616122858/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/cmake/modules/AddnLohmannJsonFlags.cmake` & `dune-iga-0.1.1.dev20230616122858/cmake/modules/AddnLohmannJsonFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/config.h.cmake` & `dune-iga-0.1.1.dev20230616122858/config.h.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/CMakeLists.txt` & `dune-iga-0.1.1.dev20230616122858/dune/iga/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/bsplinealgorithms.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/bsplinealgorithms.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/controlpoint.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/controlpoint.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/geometry/closestpointprojection.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/geometry/closestpointprojection.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/geometry/geohelper.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/geometry/geohelper.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/gridcapabilities.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/gridcapabilities.hh`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,15 @@
   class NURBSGrid;
 }
 namespace Dune::Capabilities {
   template <std::integral auto dim, std::integral auto dimworld, int codim, typename ScalarType>
   requires(dim <= 3) struct hasEntity<Dune::IGA::NURBSGrid<dim, dimworld, ScalarType>, codim> {
     static const bool v = true;
   };
-
-  template <typename ScalarType>
-  struct hasEntity<Dune::IGA::NURBSGrid<2, 2, ScalarType>, 1> {
-    static const bool v = false;
-  };
-
-  template <typename ScalarType>
-  struct hasEntity<Dune::IGA::NURBSGrid<2, 2, ScalarType>, 2> {
-    static const bool v = false;
-  };
-
+  
   template <std::integral auto dim, std::integral auto dimworld, int codim, typename ScalarType>
   struct hasEntityIterator<Dune::IGA::NURBSGrid<dim, dimworld, ScalarType>, codim>
       : public hasEntity<Dune::IGA::NURBSGrid<dim, dimworld, ScalarType>, codim> {};
 
   template <std::integral auto dim, std::integral auto dimworld, int codim, typename ScalarType>
   struct canCommunicate<Dune::IGA::NURBSGrid<dim, dimworld, ScalarType>, codim> {
     static const bool v = false;
```

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/io/ibra/ibrageometry.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/io/ibra/ibrageometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/io/ibra/ibrareader.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/io/ibra/ibrareader.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/io/igadatacollector.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/io/igadatacollector.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsalgorithms.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsalgorithms.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsbasis.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsbasis.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgeometry.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgrid.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgrid.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridentity.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridentity.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridindexsets.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridindexsets.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridleafiterator.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridleafiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsgridtraits.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsgridtraits.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsidset.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsidset.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsintersection.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsintersection.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbsleafgridview.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbsleafgridview.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbslocalgeometry.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbslocalgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbspatch.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbspatch.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbspatchdata.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbspatchdata.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/nurbspatchgeometry.h` & `dune-iga-0.1.1.dev20230616122858/dune/iga/nurbspatchgeometry.h`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/CMakeLists.txt` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/element.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/element.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/element_trim.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/element_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/infty_pwh.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/infty_pwh.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/nurbs_1.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/nurbs_1.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/pipe_trim.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/pipe_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/plate_quarter.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/plate_quarter.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/schale_trim.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/schale_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/shell-hole.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/shell-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/shell.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/shell.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/surface-hole.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/surface-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/auxiliaryFiles/surface-multihole.ibra` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/auxiliaryFiles/surface-multihole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/gridTests.cc` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/gridTests.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/test/trimmedGridTests.cc` & `dune-iga-0.1.1.dev20230616122858/dune/iga/test/trimmedGridTests.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/trim/nurbstrimboundary.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/trim/nurbstrimboundary.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/trim/nurbstrimmer.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/trim/nurbstrimmer.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/trim/trimmedelementrepresentation.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/trim/trimmedelementrepresentation.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/utils/concepts.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/utils/fillquadraturerule.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/utils/fillquadraturerule.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/utils/igahelpers.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/utils/igahelpers.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/utils/linearalgebra.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/utils/linearalgebra.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/iga/utils/mdnet.hh` & `dune-iga-0.1.1.dev20230616122858/dune/iga/utils/mdnet.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/python/iga/boundarypatch.hh` & `dune-iga-0.1.1.dev20230616122858/dune/python/iga/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/python/iga/grid.hh` & `dune-iga-0.1.1.dev20230616122858/dune/python/iga/grid.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/python/iga/nurbspatchdata.hh` & `dune-iga-0.1.1.dev20230616122858/dune/python/iga/nurbspatchdata.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/python/test/poisson.py` & `dune-iga-0.1.1.dev20230616122858/dune/python/test/poisson.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/python/test/readGrid.py` & `dune-iga-0.1.1.dev20230616122858/dune/python/test/readGrid.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/dune/python/test/setpath.py.in` & `dune-iga-0.1.1.dev20230616122858/dune/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune/iga/CMakeLists.txt` & `dune-iga-0.1.1.dev20230616122858/python/dune/iga/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune/iga/_boundarypatch.py` & `dune-iga-0.1.1.dev20230616122858/python/dune/iga/_boundarypatch.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune/iga/_igagrids.py` & `dune-iga-0.1.1.dev20230616122858/python/dune/iga/_igagrids.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune/iga/_nurbsAlgorithms.py` & `dune-iga-0.1.1.dev20230616122858/python/dune/iga/_nurbsAlgorithms.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune/iga/_nurbspatchdata.py` & `dune-iga-0.1.1.dev20230616122858/python/dune/iga/_nurbspatchdata.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune/iga/basis/__init__.py` & `dune-iga-0.1.1.dev20230616122858/python/dune/iga/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/PKG-INFO` & `dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-iga
-Version: 0.1.1.dev20230616122207
+Version: 0.1.1.dev20230616122858
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

### Comparing `dune-iga-0.1.1.dev20230616122207/python/dune_iga.egg-info/SOURCES.txt` & `dune-iga-0.1.1.dev20230616122858/python/dune_iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/setup.py` & `dune-iga-0.1.1.dev20230616122858/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 # build _iga
 # cd /tmp/dune-iga
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/dune-iga
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-duneigaVersion = "0.1.1.dev20230616122207"
+duneigaVersion = "0.1.1.dev20230616122858"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = duneigaVersion
 
 setup(**metadata)
```

### Comparing `dune-iga-0.1.1.dev20230616122207/src/CMakeLists.txt` & `dune-iga-0.1.1.dev20230616122858/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/src/auxiliaryFiles/surface-hole.ibra` & `dune-iga-0.1.1.dev20230616122858/src/auxiliaryFiles/surface-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/src/kirchhoff_plate.cc` & `dune-iga-0.1.1.dev20230616122858/src/kirchhoff_plate.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/src/kirchhoffplate.hh` & `dune-iga-0.1.1.dev20230616122858/src/kirchhoffplate.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/src/linear2dsolid.cc` & `dune-iga-0.1.1.dev20230616122858/src/linear2dsolid.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230616122207/src/linearElastic.hh` & `dune-iga-0.1.1.dev20230616122858/src/linearElastic.hh`

 * *Files identical despite different names*
