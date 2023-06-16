# Comparing `tmp/Nuitka-winsvc-1.6.tar.gz` & `tmp/Nuitka-winsvc-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-winsvc-1.6.tar", last modified: Wed May 31 02:06:42 2023, max compression
+gzip compressed data, was "Nuitka-winsvc-1.6.3.tar", last modified: Fri Jun 16 02:38:32 2023, max compression
```

## Comparing `Nuitka-winsvc-1.6.tar` & `Nuitka-winsvc-1.6.3.tar`

### file list

```diff
@@ -1,1798 +1,1798 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.643672 Nuitka-winsvc-1.6/
--rw-rw-rw-   0        0        0   825587 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/Changelog.rst
--rw-rw-rw-   0        0        0   152515 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/Developer_Manual.rst
--rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1751 2023-05-31 02:00:06.000000 Nuitka-winsvc-1.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.061714 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/
--rw-rw-rw-   0        0        0     4624 2023-05-31 02:06:38.000000 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    76624 2023-05-31 02:06:38.000000 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:06:38.000000 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      308 2023-05-31 02:06:38.000000 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-31 02:06:38.000000 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 02:06:38.000000 Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4624 2023-05-31 02:06:42.642693 Nuitka-winsvc-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-05-31 02:00:06.000000 Nuitka-winsvc-1.6/README.md
--rw-rw-rw-   0        0        0    75945 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.076359 Nuitka-winsvc-1.6/bin/
--rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/bin/autoformat-nuitka-source
--rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/bin/check-nuitka-with-pylint
--rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/bin/compare_with_cpython
--rw-rw-rw-   0        0        0     3079 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/bin/compare_with_xml
--rw-rw-rw-   0        0        0     1163 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/bin/measure-construct-performance
--rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/bin/nuitka
--rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/bin/nuitka-run
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.636107 Nuitka-winsvc-1.6/doc/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.134958 Nuitka-winsvc-1.6/doc/Logo/
--rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.169130 Nuitka-winsvc-1.6/doc/images/
--rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/doc/images/Nuitka-Logo-Horizontal.png
--rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/doc/images/Nuitka-Logo-Symbol.png
--rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/doc/images/Nuitka-Logo-Vertical.png
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.171080 Nuitka-winsvc-1.6/lib/
--rw-rw-rw-   0        0        0     4250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/lib/hints.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.173034 Nuitka-winsvc-1.6/misc/
--rwxrwxrwx   0        0        0      901 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/misc/nuitka-run.bat
--rwxrwxrwx   0        0        0     1038 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/misc/nuitka.bat
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.202329 Nuitka-winsvc-1.6/nuitka/
--rw-rw-rw-   0        0        0     7331 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Builtins.py
--rw-rw-rw-   0        0        0     5437 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/BytecodeCaching.py
--rw-rw-rw-   0        0        0     3440 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Bytecodes.py
--rw-rw-rw-   0        0        0     1884 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/CacheCleanup.py
--rw-rw-rw-   0        0        0    11148 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Constants.py
--rw-rw-rw-   0        0        0     2447 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Errors.py
--rw-rw-rw-   0        0        0    37236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/MainControl.py
--rw-rw-rw-   0        0        0     8064 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/ModuleRegistry.py
--rw-rw-rw-   0        0        0    56845 2023-05-31 02:00:06.000000 Nuitka-winsvc-1.6/nuitka/OptionParsing.py
--rw-rw-rw-   0        0        0    65857 2023-05-31 02:00:06.000000 Nuitka-winsvc-1.6/nuitka/Options.py
--rw-rw-rw-   0        0        0     5022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/OutputDirectories.py
--rw-rw-rw-   0        0        0    14550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/PostProcessing.py
--rw-rw-rw-   0        0        0     5770 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Progress.py
--rw-rw-rw-   0        0        0     7472 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/PythonFlavors.py
--rw-rw-rw-   0        0        0     4061 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/PythonOperators.py
--rw-rw-rw-   0        0        0    12179 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/PythonVersions.py
--rw-rw-rw-   0        0        0     8514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Serialization.py
--rw-rw-rw-   0        0        0     4670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/SourceCodeReferences.py
--rw-rw-rw-   0        0        0    11235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Tracing.py
--rw-rw-rw-   0        0        0     3395 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/TreeXML.py
--rw-rw-rw-   0        0        0    15235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Variables.py
--rw-rw-rw-   0        0        0     2053 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/Version.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/__init__.py
--rw-rw-rw-   0        0        0     5615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/__main__.py
--rw-rw-rw-   0        0        0     5295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/__past__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.215026 Nuitka-winsvc-1.6/nuitka/build/
--rw-rw-rw-   0        0        0    33528 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/Backend.scons
--rw-rw-rw-   0        0        0     8314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/CCompilerVersion.scons
--rw-rw-rw-   0        0        0     2433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/DataComposerInterface.py
--rw-rw-rw-   0        0        0    18530 2023-05-31 02:00:58.000000 Nuitka-winsvc-1.6/nuitka/build/Onefile.scons
--rw-rw-rw-   0        0        0    15635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/SconsCaching.py
--rw-rw-rw-   0        0        0    30008 2023-05-31 02:00:58.000000 Nuitka-winsvc-1.6/nuitka/build/SconsCompilerSettings.py
--rw-rw-rw-   0        0        0     5527 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/SconsHacks.py
--rw-rw-rw-   0        0        0    15532 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/SconsInterface.py
--rw-rw-rw-   0        0        0     2361 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/SconsProgress.py
--rw-rw-rw-   0        0        0    11960 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/SconsSpawn.py
--rw-rw-rw-   0        0        0    24287 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/SconsUtils.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.639038 Nuitka-winsvc-1.6/nuitka/build/include/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.256035 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/
--rw-rw-rw-   0        0        0     7972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/allocator.h
--rw-rw-rw-   0        0        0     3423 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/builtins.h
--rw-rw-rw-   0        0        0     4604 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/calling.h
--rw-rw-rw-   0        0        0     1977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/checkers.h
--rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/checksum_tools.h
--rw-rw-rw-   0        0        0     9571 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-rw-rw-   0        0        0     2002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_cell.h
--rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-rw-rw-   0        0        0    16949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_frame.h
--rw-rw-rw-   0        0        0     5972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_function.h
--rw-rw-rw-   0        0        0     9136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_generator.h
--rw-rw-rw-   0        0        0     1838 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_method.h
--rw-rw-rw-   0        0        0     7408 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/constants.h
--rw-rw-rw-   0        0        0     1293 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/constants_blob.h
--rw-rw-rw-   0        0        0    34083 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/exceptions.h
--rw-rw-rw-   0        0        0     3221 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/filesystem_paths.h
--rw-rw-rw-   0        0        0     6253 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/freelists.h
--rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/hedley.h
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.357595 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/
--rw-rw-rw-   0        0        0     3275 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/attributes.h
--rw-rw-rw-   0        0        0     2663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/boolean.h
--rw-rw-rw-   0        0        0     1181 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/bytes.h
--rw-rw-rw-   0        0        0     9335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-rw-rw-   0        0        0    10615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-rw-rw-   0        0        0    13139 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-rw-rw-   0        0        0     1743 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/complex.h
--rw-rw-rw-   0        0        0    13109 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-rw-rw-   0        0        0     1206 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/floats.h
--rw-rw-rw-   0        0        0     3674 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/import_hard.h
--rw-rw-rw-   0        0        0     1798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/indexes.h
--rw-rw-rw-   0        0        0     2941 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/ints.h
--rw-rw-rw-   0        0        0     9992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/iterators.h
--rw-rw-rw-   0        0        0     3411 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/lists.h
--rw-rw-rw-   0        0        0     1633 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-rw-rw-   0        0        0     1328 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/mappings.h
--rw-rw-rw-   0        0        0     4573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations.h
--rw-rw-rw-   0        0        0    12685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-rw-rw-   0        0        0     5641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-rw-rw-   0        0        0     5422 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-rw-rw-   0        0        0     5460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-rw-rw-   0        0        0     2799 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-rw-rw-   0        0        0    15778 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-rw-rw-   0        0        0    13210 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-rw-rw-   0        0        0     5791 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-rw-rw-   0        0        0     4714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-rw-rw-   0        0        0     5824 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-rw-rw-   0        0        0     5438 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-rw-rw-   0        0        0    15100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-rw-rw-   0        0        0     8670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-rw-rw-   0        0        0     3753 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-rw-rw-   0        0        0     4846 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-rw-rw-   0        0        0    10626 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-rw-rw-   0        0        0     9201 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-rw-rw-   0        0        0     5147 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-rw-rw-   0        0        0     4349 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-rw-rw-   0        0        0     4975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-rw-rw-   0        0        0     4826 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-rw-rw-   0        0        0     3297 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/raising.h
--rw-rw-rw-   0        0        0     2178 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-rw-rw-   0        0        0     1146 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-rw-rw-   0        0        0     1112 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/sequences.h
--rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/sets.h
--rw-rw-rw-   0        0        0     8419 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/slices.h
--rw-rw-rw-   0        0        0     1242 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/strings.h
--rw-rw-rw-   0        0        0    17575 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/subscripts.h
--rw-rw-rw-   0        0        0     5720 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/tuples.h
--rw-rw-rw-   0        0        0    14412 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helpers.h
--rw-rw-rw-   0        0        0     5375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/importing.h
--rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/incbin.h
--rw-rw-rw-   0        0        0    14427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/prelude.h
--rw-rw-rw-   0        0        0     2870 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/printing.h
--rw-rw-rw-   0        0        0     1761 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/python_pgo.h
--rw-rw-rw-   0        0        0     2119 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/safe_string_ops.h
--rw-rw-rw-   0        0        0     3840 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/threading.h
--rw-rw-rw-   0        0        0     3144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/tracing.h
--rw-rw-rw-   0        0        0     2936 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/include/nuitka/unfreezing.h
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.909377 Nuitka-winsvc-1.6/nuitka/build/inline_copy/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.379097 Nuitka-winsvc-1.6/nuitka/build/inline_copy/appdirs/
--rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.391790 Nuitka-winsvc-1.6/nuitka/build/inline_copy/atomicwrites/
--rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.392747 Nuitka-winsvc-1.6/nuitka/build/inline_copy/bin/
--rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/bin/scons.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.826374 Nuitka-winsvc-1.6/nuitka/build/inline_copy/clcache/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.406428 Nuitka-winsvc-1.6/nuitka/build/inline_copy/clcache/clcache/
--rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.413266 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/
--rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.422042 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/
--rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.431817 Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/
--rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.437666 Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/
--rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.450367 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.485516 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/
--rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.503102 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/
--rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.539222 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.891801 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.836142 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.575356 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.585122 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.595864 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.615400 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.623201 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.632970 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.755624 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.769295 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.771246 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.781016 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.799568 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.842975 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.839606 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.845464 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.866948 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.875734 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:39.887455 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.001703 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.012444 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.015378 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.017328 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.026116 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.028069 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.892776 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.069081 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.074940 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.094470 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.104236 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.111073 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.219464 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.228253 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.230207 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.236065 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.238992 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.248776 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.253640 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.273169 Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.279029 Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.904496 Nuitka-winsvc-1.6/nuitka/build/inline_copy/pkg_resources/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.284895 Nuitka-winsvc-1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.905470 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.321028 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/
--rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
--rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py
--rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.341468 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.618939 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/
--rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.627734 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.692772 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/
--rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.731543 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:40.781344 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/
--rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.421699 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/
--rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.461735 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/
--rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/debug.h
--rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/fse.h
--rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/huf.h
--rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/mem.h
--rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.476384 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/
--rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/zstd.h
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.609382 Nuitka-winsvc-1.6/nuitka/build/static_src/
--rw-rw-rw-   0        0        0    82114 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-rw-rw-   0        0        0     8250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledCellType.c
--rw-rw-rw-   0        0        0    62733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-rw-rw-   0        0        0    70973 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledCoroutineType.c
--rw-rw-rw-   0        0        0    35861 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledFrameType.c
--rw-rw-rw-   0        0        0   100376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledFunctionType.c
--rw-rw-rw-   0        0        0    60649 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledGeneratorType.c
--rw-rw-rw-   0        0        0    48526 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-rw-rw-   0        0        0    21638 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledMethodType.c
--rw-rw-rw-   0        0        0    18993 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersAllocator.c
--rw-rw-rw-   0        0        0    32849 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersAttributes.c
--rw-rw-rw-   0        0        0    21783 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersBuiltin.c
--rw-rw-rw-   0        0        0   107641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-rw-rw-   0        0        0     3033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersBytes.c
--rw-rw-rw-   0        0        0    13057 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersCalling.c
--rw-rw-rw-   0        0        0   470655 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-rw-rw-   0        0        0     1617 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersChecksumTools.c
--rw-rw-rw-   0        0        0     2991 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersClasses.c
--rw-rw-rw-   0        0        0   317872 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonEq.c
--rw-rw-rw-   0        0        0     4673 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-rw-rw-   0        0        0   313003 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonGe.c
--rw-rw-rw-   0        0        0   312414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonGt.c
--rw-rw-rw-   0        0        0   316217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonLe.c
--rw-rw-rw-   0        0        0   315628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonLt.c
--rw-rw-rw-   0        0        0   314618 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonNe.c
--rw-rw-rw-   0        0        0    36068 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-rw-rw-   0        0        0    19313 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersDeepcopy.c
--rw-rw-rw-   0        0        0    38364 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersDictionaries.c
--rw-rw-rw-   0        0        0    24295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-rw-rw-   0        0        0     7035 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersExceptions.c
--rw-rw-rw-   0        0        0     6668 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersFiles.c
--rw-rw-rw-   0        0        0    11199 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-rw-rw-   0        0        0     2426 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersFloats.c
--rw-rw-rw-   0        0        0     1774 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersHeapStorage.c
--rw-rw-rw-   0        0        0    14585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersImport.c
--rw-rw-rw-   0        0        0    13589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersImportHard.c
--rw-rw-rw-   0        0        0    18433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersLists.c
--rw-rw-rw-   0        0        0    13915 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersListsGenerated.c
--rw-rw-rw-   0        0        0     1640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersMappings.c
--rw-rw-rw-   0        0        0     3513 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersMatching.c
--rw-rw-rw-   0        0        0   181243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-rw-rw-   0        0        0    16700 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-rw-rw-   0        0        0    77782 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-rw-rw-   0        0        0    67487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-rw-rw-   0        0        0    68748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-rw-rw-   0        0        0     6274 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-rw-rw-   0        0        0    83405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-rw-rw-   0        0        0    13776 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-rw-rw-   0        0        0   183202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-rw-rw-   0        0        0   188514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-rw-rw-   0        0        0     3404 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-rw-rw-   0        0        0    66453 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-rw-rw-   0        0        0    78891 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-rw-rw-   0        0        0     1023 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-rw-rw-   0        0        0    77305 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-rw-rw-   0        0        0    70465 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-rw-rw-   0        0        0    68005 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-rw-rw-   0        0        0   149580 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-rw-rw-   0        0        0     4071 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-rw-rw-   0        0        0    53122 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-rw-rw-   0        0        0    76512 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-rw-rw-   0        0        0    47568 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-rw-rw-   0        0        0    17742 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-rw-rw-   0        0        0   136100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-rw-rw-   0        0        0   142211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-rw-rw-   0        0        0    74142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-rw-rw-   0        0        0    82669 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-rw-rw-   0        0        0    45052 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-rw-rw-   0        0        0    82842 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-rw-rw-   0        0        0    76343 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-rw-rw-   0        0        0     3219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersProfiling.c
--rw-rw-rw-   0        0        0     3805 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersPythonPgo.c
--rw-rw-rw-   0        0        0    15369 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersRaising.c
--rw-rw-rw-   0        0        0    11926 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersSafeStrings.c
--rw-rw-rw-   0        0        0     3730 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersSequences.c
--rw-rw-rw-   0        0        0     1946 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersSlices.c
--rw-rw-rw-   0        0        0    26642 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersStrings.c
--rw-rw-rw-   0        0        0     4037 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersTuples.c
--rw-rw-rw-   0        0        0     5578 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersTypes.c
--rw-rw-rw-   0        0        0    11986 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/InspectPatcher.c
--rw-rw-rw-   0        0        0    41670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/MainProgram.c
--rw-rw-rw-   0        0        0    58634 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-rw-rw-   0        0        0     4537 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-rw-rw-   0        0        0     6427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-rw-rw-   0        0        0    17065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-rw-rw-   0        0        0    36509 2023-05-31 02:00:06.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/OnefileBootstrap.c
--rw-rw-rw-   0        0        0     7890 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.687509 Nuitka-winsvc-1.6/nuitka/code_generation/
--rw-rw-rw-   0        0        0     6414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/AsyncgenCodes.py
--rw-rw-rw-   0        0        0    10153 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/AttributeCodes.py
--rw-rw-rw-   0        0        0    21864 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-rw-rw-   0        0        0     2339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/BranchCodes.py
--rw-rw-rw-   0        0        0    16009 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/BuiltinCodes.py
--rw-rw-rw-   0        0        0    35905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/CallCodes.py
--rw-rw-rw-   0        0        0     4896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ClassCodes.py
--rw-rw-rw-   0        0        0    51116 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/CodeGeneration.py
--rw-rw-rw-   0        0        0     2375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/CodeHelperSelection.py
--rw-rw-rw-   0        0        0    14392 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/CodeHelpers.py
--rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/CodeObjectCodes.py
--rw-rw-rw-   0        0        0    17570 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ComparisonCodes.py
--rw-rw-rw-   0        0        0     4446 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-rw-rw-   0        0        0     7335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ConditionalCodes.py
--rw-rw-rw-   0        0        0     6539 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ConstantCodes.py
--rw-rw-rw-   0        0        0    31186 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/Contexts.py
--rw-rw-rw-   0        0        0     8484 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/CoroutineCodes.py
--rw-rw-rw-   0        0        0     1574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/CtypesCodes.py
--rw-rw-rw-   0        0        0    28478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/DictCodes.py
--rw-rw-rw-   0        0        0     2125 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/Emission.py
--rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ErrorCodes.py
--rw-rw-rw-   0        0        0    12304 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/EvalCodes.py
--rw-rw-rw-   0        0        0     8975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ExceptionCodes.py
--rw-rw-rw-   0        0        0     7350 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-rw-rw-   0        0        0     2093 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ExpressionCodes.py
--rw-rw-rw-   0        0        0    17725 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/FrameCodes.py
--rw-rw-rw-   0        0        0    27345 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/FunctionCodes.py
--rw-rw-rw-   0        0        0     7690 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/GeneratorCodes.py
--rw-rw-rw-   0        0        0     5721 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/GlobalConstants.py
--rw-rw-rw-   0        0        0     6911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-rw-rw-   0        0        0     1794 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/IdCodes.py
--rw-rw-rw-   0        0        0    13318 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ImportCodes.py
--rw-rw-rw-   0        0        0     1396 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/Indentation.py
--rw-rw-rw-   0        0        0     1506 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/IndexCodes.py
--rw-rw-rw-   0        0        0     1033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/InjectCCodes.py
--rw-rw-rw-   0        0        0     3432 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/IntegerCodes.py
--rw-rw-rw-   0        0        0    12010 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/IteratorCodes.py
--rw-rw-rw-   0        0        0     2022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/LabelCodes.py
--rw-rw-rw-   0        0        0     2612 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/LineNumberCodes.py
--rw-rw-rw-   0        0        0    15906 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ListCodes.py
--rw-rw-rw-   0        0        0     6375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/LoaderCodes.py
--rw-rw-rw-   0        0        0     9951 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/LocalsDictCodes.py
--rw-rw-rw-   0        0        0     3135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/LoopCodes.py
--rw-rw-rw-   0        0        0     1597 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/MatchCodes.py
--rw-rw-rw-   0        0        0     6291 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ModuleCodes.py
--rw-rw-rw-   0        0        0     8118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/Namify.py
--rw-rw-rw-   0        0        0    12777 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/OperationCodes.py
--rw-rw-rw-   0        0        0    28231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/PackageResourceCodes.py
--rw-rw-rw-   0        0        0     3021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/PrintCodes.py
--rw-rw-rw-   0        0        0     5474 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/PythonAPICodes.py
--rw-rw-rw-   0        0        0    13095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/RaisingCodes.py
--rw-rw-rw-   0        0        0     3443 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/Reports.py
--rw-rw-rw-   0        0        0     5234 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/ReturnCodes.py
--rw-rw-rw-   0        0        0     6517 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/SetCodes.py
--rw-rw-rw-   0        0        0    13949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/SliceCodes.py
--rw-rw-rw-   0        0        0     9809 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/StringCodes.py
--rw-rw-rw-   0        0        0     8188 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/SubscriptCodes.py
--rw-rw-rw-   0        0        0    11176 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/TryCodes.py
--rw-rw-rw-   0        0        0     3786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/TupleCodes.py
--rw-rw-rw-   0        0        0    14717 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/VariableCodes.py
--rw-rw-rw-   0        0        0     9121 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/VariableDeclarations.py
--rw-rw-rw-   0        0        0     8099 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/YieldCodes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.700204 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/
--rw-rw-rw-   0        0        0     6069 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeBases.py
--rw-rw-rw-   0        0        0     3399 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-rw-rw-   0        0        0     1804 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-rw-rw-   0        0        0     1378 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-rw-rw-   0        0        0     3610 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-rw-rw-   0        0        0     5128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-rw-rw-   0        0        0     5211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-rw-rw-   0        0        0     3955 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-rw-rw-   0        0        0    19628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-rw-rw-   0        0        0     2852 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeVoids.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/c_types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.713867 Nuitka-winsvc-1.6/nuitka/code_generation/templates/
--rw-rw-rw-   0        0        0     2845 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-rw-rw-   0        0        0     5865 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-rw-rw-   0        0        0     2921 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-rw-rw-   0        0        0     2290 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-rw-rw-   0        0        0     6339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-rw-rw-   0        0        0     3321 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-rw-rw-   0        0        0     3306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-rw-rw-   0        0        0     2335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-rw-rw-   0        0        0     4217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-rw-rw-   0        0        0    21441 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-rw-rw-   0        0        0     6640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-rw-rw-   0        0        0     2475 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.751537 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/
--rw-rw-rw-   0        0        0    11231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-rw-rw-   0        0        0     5847 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-rw-rw-   0        0        0    23760 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-rw-rw-   0        0        0     5238 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-rw-rw-   0        0        0     1843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-rw-rw-   0        0        0     2817 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-rw-rw-   0        0        0    12819 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-rw-rw-   0        0        0     2044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-rw-rw-   0        0        0     2762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-rw-rw-   0        0        0     1544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-rw-rw-   0        0        0     7197 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-rw-rw-   0        0        0    12850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-rw-rw-   0        0        0     4288 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-rw-rw-   0        0        0     2088 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-rw-rw-   0        0        0     2118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-rw-rw-   0        0        0     3933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-rw-rw-   0        0        0     7407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-rw-rw-   0        0        0     4292 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-rw-rw-   0        0        0     3860 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-rw-rw-   0        0        0     4487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-rw-rw-   0        0        0    11579 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-rw-rw-   0        0        0    19317 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-rw-rw-   0        0        0     2843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-rw-rw-   0        0        0     3635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-rw-rw-   0        0        0    11102 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-rw-rw-   0        0        0    15380 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-rw-rw-   0        0        0     2979 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-rw-rw-   0        0        0    10421 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-rw-rw-   0        0        0     2557 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-rw-rw-   0        0        0     3020 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-rw-rw-   0        0        0     2984 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-rw-rw-   0        0        0     3173 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.757398 Nuitka-winsvc-1.6/nuitka/containers/
--rw-rw-rw-   0        0        0     1435 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/containers/Namedtuples.py
--rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/containers/OrderedDicts.py
--rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/containers/OrderedSets.py
--rw-rw-rw-   0        0        0     4397 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/containers/OrderedSetsFallback.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.760326 Nuitka-winsvc-1.6/nuitka/distutils/
--rw-rw-rw-   0        0        0     1964 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/distutils/Build.py
--rw-rw-rw-   0        0        0    14219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/distutils/DistutilCommands.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/distutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.764233 Nuitka-winsvc-1.6/nuitka/finalizations/
--rw-rw-rw-   0        0        0     1224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/finalizations/Finalization.py
--rw-rw-rw-   0        0        0     6110 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/finalizations/FinalizeMarkups.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/finalizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.776928 Nuitka-winsvc-1.6/nuitka/freezer/
--rw-rw-rw-   0        0        0     7311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/DependsExe.py
--rw-rw-rw-   0        0        0     2584 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesCommon.py
--rw-rw-rw-   0        0        0    10811 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesMacOS.py
--rw-rw-rw-   0        0        0     7211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesPosix.py
--rw-rw-rw-   0        0        0     6620 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesWin32.py
--rw-rw-rw-   0        0        0    17336 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/IncludedDataFiles.py
--rw-rw-rw-   0        0        0     9492 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/IncludedEntryPoints.py
--rw-rw-rw-   0        0        0    10112 2023-05-31 02:00:06.000000 Nuitka-winsvc-1.6/nuitka/freezer/Onefile.py
--rw-rw-rw-   0        0        0    26319 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/Standalone.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/freezer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.787227 Nuitka-winsvc-1.6/nuitka/importing/
--rw-rw-rw-   0        0        0    10934 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/IgnoreListing.py
--rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/ImportCache.py
--rw-rw-rw-   0        0        0     6455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/ImportResolving.py
--rw-rw-rw-   0        0        0    28463 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/Importing.py
--rw-rw-rw-   0        0        0     4738 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/PreloadedPackages.py
--rw-rw-rw-   0        0        0    16375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/Recursion.py
--rw-rw-rw-   0        0        0    10948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/StandardLibrary.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/importing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.925030 Nuitka-winsvc-1.6/nuitka/nodes/
--rw-rw-rw-   0        0        0     3637 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/AsyncgenNodes.py
--rw-rw-rw-   0        0        0     4082 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/AttributeLookupNodes.py
--rw-rw-rw-   0        0        0    12004 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/AttributeNodes.py
--rw-rw-rw-   0        0        0   378745 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/AttributeNodesGenerated.py
--rw-rw-rw-   0        0        0     3823 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinAllNodes.py
--rw-rw-rw-   0        0        0     4098 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinAnyNodes.py
--rw-rw-rw-   0        0        0     2496 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinComplexNodes.py
--rw-rw-rw-   0        0        0     1698 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinDecodingNodes.py
--rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-rw-rw-   0        0        0     4694 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinDictNodes.py
--rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinFormatNodes.py
--rw-rw-rw-   0        0        0     2142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinHashNodes.py
--rw-rw-rw-   0        0        0     5334 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinIntegerNodes.py
--rw-rw-rw-   0        0        0    12723 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinIteratorNodes.py
--rw-rw-rw-   0        0        0     1996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinLenNodes.py
--rw-rw-rw-   0        0        0     3606 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinNextNodes.py
--rw-rw-rw-   0        0        0     3240 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinOpenNodes.py
--rw-rw-rw-   0        0        0   245536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-rw-rw-   0        0        0    18589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinRangeNodes.py
--rw-rw-rw-   0        0        0     9067 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinRefNodes.py
--rw-rw-rw-   0        0        0     3307 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinSumNodes.py
--rw-rw-rw-   0        0        0    13543 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinTypeNodes.py
--rw-rw-rw-   0        0        0     1573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BuiltinVarsNodes.py
--rw-rw-rw-   0        0        0    26113 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/BytesNodes.py
--rw-rw-rw-   0        0        0     6478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/CallNodes.py
--rw-rw-rw-   0        0        0     1550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/Checkers.py
--rw-rw-rw-   0        0        0   605501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ChildrenHavingMixins.py
--rw-rw-rw-   0        0        0     8448 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ClassNodes.py
--rw-rw-rw-   0        0        0     6585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/CodeObjectSpecs.py
--rw-rw-rw-   0        0        0    21683 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ComparisonNodes.py
--rw-rw-rw-   0        0        0    30314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ConditionalNodes.py
--rw-rw-rw-   0        0        0    46536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ConstantRefNodes.py
--rw-rw-rw-   0        0        0    12213 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ContainerMakingNodes.py
--rw-rw-rw-   0        0        0     2834 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ContainerOperationNodes.py
--rw-rw-rw-   0        0        0     4581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/CoroutineNodes.py
--rw-rw-rw-   0        0        0     1714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/CtypesNodes.py
--rw-rw-rw-   0        0        0    51021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/DictionaryNodes.py
--rw-rw-rw-   0        0        0     7856 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ExceptionNodes.py
--rw-rw-rw-   0        0        0     8044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ExecEvalNodes.py
--rw-rw-rw-   0        0        0    44996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ExpressionBases.py
--rw-rw-rw-   0        0        0    45091 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ExpressionBasesGenerated.py
--rw-rw-rw-   0        0        0    21278 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ExpressionShapeMixins.py
--rw-rw-rw-   0        0        0    12156 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/FrameNodes.py
--rw-rw-rw-   0        0        0     3544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/FunctionAttributeNodes.py
--rw-rw-rw-   0        0        0    39803 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/FunctionNodes.py
--rw-rw-rw-   0        0        0     5376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/FutureSpecs.py
--rw-rw-rw-   0        0        0     6256 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/GeneratorNodes.py
--rw-rw-rw-   0        0        0     6850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/GlobalsLocalsNodes.py
--rw-rw-rw-   0        0        0    74177 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/HardImportNodesGenerated.py
--rw-rw-rw-   0        0        0     5511 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ImportHardNodes.py
--rw-rw-rw-   0        0        0    45692 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ImportNodes.py
--rw-rw-rw-   0        0        0     2733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/IndicatorMixins.py
--rw-rw-rw-   0        0        0     1502 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/InjectCNodes.py
--rw-rw-rw-   0        0        0    11228 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/IterationHandles.py
--rw-rw-rw-   0        0        0    11002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/KeyValuePairNodes.py
--rw-rw-rw-   0        0        0    16320 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ListOperationNodes.py
--rw-rw-rw-   0        0        0    23094 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/LocalsDictNodes.py
--rw-rw-rw-   0        0        0    14922 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/LocalsScopes.py
--rw-rw-rw-   0        0        0    15581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/LoopNodes.py
--rw-rw-rw-   0        0        0     1712 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/MatchNodes.py
--rw-rw-rw-   0        0        0     6534 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ModuleAttributeNodes.py
--rw-rw-rw-   0        0        0    30829 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ModuleNodes.py
--rw-rw-rw-   0        0        0    24899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/NodeBases.py
--rw-rw-rw-   0        0        0    15128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/NodeMakingHelpers.py
--rw-rw-rw-   0        0        0     5550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/NodeMetaClasses.py
--rw-rw-rw-   0        0        0    31894 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/OperatorNodes.py
--rw-rw-rw-   0        0        0     9134 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/OperatorNodesUnary.py
--rw-rw-rw-   0        0        0     4202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/OsSysNodes.py
--rw-rw-rw-   0        0        0    12442 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/OutlineNodes.py
--rw-rw-rw-   0        0        0    31330 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/PackageMetadataNodes.py
--rw-rw-rw-   0        0        0     4464 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/PackageResourceNodes.py
--rw-rw-rw-   0        0        0     3407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/PrintNodes.py
--rw-rw-rw-   0        0        0     6772 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/ReturnNodes.py
--rw-rw-rw-   0        0        0     4715 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/SideEffectNodes.py
--rw-rw-rw-   0        0        0    12501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/SliceNodes.py
--rw-rw-rw-   0        0        0    94880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/StatementBasesGenerated.py
--rw-rw-rw-   0        0        0     9430 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/StatementNodes.py
--rw-rw-rw-   0        0        0    28658 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/StrNodes.py
--rw-rw-rw-   0        0        0     3504 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/StringConcatenationNodes.py
--rw-rw-rw-   0        0        0     8640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/SubscriptNodes.py
--rw-rw-rw-   0        0        0    17853 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/TryNodes.py
--rw-rw-rw-   0        0        0     2405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/TypeMatchNodes.py
--rw-rw-rw-   0        0        0    10911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/TypeNodes.py
--rw-rw-rw-   0        0        0    39522 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/VariableAssignNodes.py
--rw-rw-rw-   0        0        0    10746 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/VariableDelNodes.py
--rw-rw-rw-   0        0        0     4574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/VariableNameNodes.py
--rw-rw-rw-   0        0        0    30982 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/VariableRefNodes.py
--rw-rw-rw-   0        0        0     4748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/VariableReleaseNodes.py
--rw-rw-rw-   0        0        0     3902 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/YieldNodes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.930889 Nuitka-winsvc-1.6/nuitka/nodes/shapes/
--rw-rw-rw-   0        0        0   156243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-rw-rw-   0        0        0     4387 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-rw-rw-   0        0        0     4567 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/shapes/ShapeMixins.py
--rw-rw-rw-   0        0        0    42374 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/shapes/StandardShapes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/nodes/shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.944565 Nuitka-winsvc-1.6/nuitka/optimizations/
--rw-rw-rw-   0        0        0     3279 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/BytecodeDemotion.py
--rw-rw-rw-   0        0        0     3920 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/FunctionInlining.py
--rw-rw-rw-   0        0        0     2144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/Graphs.py
--rw-rw-rw-   0        0        0    10762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/Optimization.py
--rw-rw-rw-   0        0        0    52154 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-rw-rw-   0        0        0     2272 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/Tags.py
--rw-rw-rw-   0        0        0    40896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/TraceCollections.py
--rw-rw-rw-   0        0        0    23977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/ValueTraces.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/optimizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.946516 Nuitka-winsvc-1.6/nuitka/pgo/
--rw-rw-rw-   0        0        0     4663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/pgo/PGO.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/pgo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.952371 Nuitka-winsvc-1.6/nuitka/plugins/
--rw-rw-rw-   0        0        0    39924 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/PluginBase.py
--rw-rw-rw-   0        0        0    56200 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/Plugins.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.994362 Nuitka-winsvc-1.6/nuitka/plugins/standard/
--rw-rw-rw-   0        0        0    18638 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-rw-rw-   0        0        0     3460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-rw-rw-   0        0        0     9939 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/DataFilesPlugin.py
--rw-rw-rw-   0        0        0     4051 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/DelvewheelPlugin.py
--rw-rw-rw-   0        0        0     5675 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/DillPlugin.py
--rw-rw-rw-   0        0        0    13757 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/DllFilesPlugin.py
--rw-rw-rw-   0        0        0     2062 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/EnumPlugin.py
--rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/EventletPlugin.py
--rw-rw-rw-   0        0        0     1880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/GeventPlugin.py
--rw-rw-rw-   0        0        0     3482 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/GiPlugin.py
--rw-rw-rw-   0        0        0     5027 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/GlfwPlugin.py
--rw-rw-rw-   0        0        0    18207 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/ImplicitImports.py
--rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/KivyPlugin.py
--rw-rw-rw-   0        0        0     7258 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-rw-rw-   0        0        0     6667 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-rw-rw-   0        0        0     1187 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/NumpyPlugin.py
--rw-rw-rw-   0        0        0     6554 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-rw-rw-   0        0        0     1917 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/PbrPlugin.py
--rw-rw-rw-   0        0        0     4665 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-rw-rw-   0        0        0     6992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/PmwPlugin.py
--rw-rw-rw-   0        0        0    49987 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-rw-rw-   0        0        0     2933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/PywebViewPlugin.py
--rw-rw-rw-   0        0        0     1160 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/TensorflowPlugin.py
--rw-rw-rw-   0        0        0    12180 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/TkinterPlugin.py
--rw-rw-rw-   0        0        0     1140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/TorchPlugin.py
--rw-rw-rw-   0        0        0     9855 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/TransformersPlugin.py
--rw-rw-rw-   0        0        0     3175 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/TrioPlugin.py
--rw-rw-rw-   0        0        0     5640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/UpxPlugin.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/__init__.py
--rw-rw-rw-   0        0        0   135361 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:41.998268 Nuitka-winsvc-1.6/nuitka/reports/
--rw-rw-rw-   0        0        0     2209 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/reports/LicenseReport.rst.j2
--rw-rw-rw-   0        0        0    17538 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/reports/Reports.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.018341 Nuitka-winsvc-1.6/nuitka/specs/
--rw-rw-rw-   0        0        0     5911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-rw-rw-   0        0        0     2786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-rw-rw-   0        0        0     2541 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/BuiltinListOperationSpecs.py
--rw-rw-rw-   0        0        0    26455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/BuiltinParameterSpecs.py
--rw-rw-rw-   0        0        0     6065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-rw-rw-   0        0        0     4802 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-rw-rw-   0        0        0     5133 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/HardImportSpecs.py
--rw-rw-rw-   0        0        0    18740 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/ParameterSpecs.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/specs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.023226 Nuitka-winsvc-1.6/nuitka/tools/
--rw-rw-rw-   0        0        0     1603 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/Basics.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.025172 Nuitka-winsvc-1.6/nuitka/tools/commercial/
--rw-rw-rw-   0        0        0      815 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/commercial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.031032 Nuitka-winsvc-1.6/nuitka/tools/data_composer/
--rw-rw-rw-   0        0        0    14054 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/data_composer/DataComposer.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/data_composer/__init__.py
--rw-rw-rw-   0        0        0     1306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/data_composer/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.036893 Nuitka-winsvc-1.6/nuitka/tools/environments/
--rw-rw-rw-   0        0        0     2449 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/environments/CreateEnvironment.py
--rw-rw-rw-   0        0        0     3735 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/environments/Virtualenv.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.038856 Nuitka-winsvc-1.6/nuitka/tools/general/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/general/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.042750 Nuitka-winsvc-1.6/nuitka/tools/general/dll_report/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/general/dll_report/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/general/dll_report/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.045678 Nuitka-winsvc-1.6/nuitka/tools/general/find_module/
--rw-rw-rw-   0        0        0     3798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/general/find_module/FindModuleCode.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/general/find_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.051676 Nuitka-winsvc-1.6/nuitka/tools/onefile_compressor/
--rw-rw-rw-   0        0        0    10194 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/onefile_compressor/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/onefile_compressor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.056094 Nuitka-winsvc-1.6/nuitka/tools/profiler/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/profiler/__init__.py
--rw-rw-rw-   0        0        0     2529 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/profiler/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.060980 Nuitka-winsvc-1.6/nuitka/tools/scanning/
--rw-rw-rw-   0        0        0     3344 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/scanning/DisplayPackageData.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/scanning/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.068790 Nuitka-winsvc-1.6/nuitka/tools/specialize/
--rw-rw-rw-   0        0        0    51143 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/specialize/CTypeDescriptions.py
--rw-rw-rw-   0        0        0     7685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/specialize/Common.py
--rw-rw-rw-   0        0        0    39625 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/specialize/SpecializeC.py
--rw-rw-rw-   0        0        0    33585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/specialize/SpecializePython.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/specialize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.080509 Nuitka-winsvc-1.6/nuitka/tools/testing/
--rw-rw-rw-   0        0        0    55559 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/Common.py
--rw-rw-rw-   0        0        0     1483 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/Constructs.py
--rw-rw-rw-   0        0        0     8940 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/OutputComparison.py
--rw-rw-rw-   0        0        0     1278 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/Pythons.py
--rw-rw-rw-   0        0        0     7888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/RuntimeTracing.py
--rw-rw-rw-   0        0        0     5371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/SearchModes.py
--rw-rw-rw-   0        0        0     3375 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/Valgrind.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.085390 Nuitka-winsvc-1.6/nuitka/tools/testing/check_reference_counts/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.088321 Nuitka-winsvc-1.6/nuitka/tools/testing/compare_with_cpython/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-rw-rw-   0        0        0    29429 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.091250 Nuitka-winsvc-1.6/nuitka/tools/testing/find_sxs_modules/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.094178 Nuitka-winsvc-1.6/nuitka/tools/testing/measure_construct_performance/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-rw-rw-   0        0        0     8755 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.097108 Nuitka-winsvc-1.6/nuitka/tools/testing/run_nuitka_tests/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-rw-rw-   0        0        0    36321 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.101018 Nuitka-winsvc-1.6/nuitka/tools/watch/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/watch/__init__.py
--rw-rw-rw-   0        0        0     9503 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tools/watch/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.160582 Nuitka-winsvc-1.6/nuitka/tree/
--rw-rw-rw-   0        0        0    47126 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/Building.py
--rw-rw-rw-   0        0        0    74608 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ComplexCallHelperFunctions.py
--rw-rw-rw-   0        0        0     1700 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/Extractions.py
--rw-rw-rw-   0        0        0     2572 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/InternalModule.py
--rw-rw-rw-   0        0        0     1511 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/Operations.py
--rw-rw-rw-   0        0        0     2807 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationAssertStatements.py
--rw-rw-rw-   0        0        0    42768 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationAssignmentStatements.py
--rw-rw-rw-   0        0        0     2948 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationBooleanExpressions.py
--rw-rw-rw-   0        0        0    11693 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationCallExpressions.py
--rw-rw-rw-   0        0        0    15072 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationClasses.py
--rw-rw-rw-   0        0        0    37638 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationClasses3.py
--rw-rw-rw-   0        0        0     6430 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationComparisonExpressions.py
--rw-rw-rw-   0        0        0    22111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationContractionExpressions.py
--rw-rw-rw-   0        0        0    11061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationDictionaryCreation.py
--rw-rw-rw-   0        0        0    14607 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationExecStatements.py
--rw-rw-rw-   0        0        0     7782 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationForLoopStatements.py
--rw-rw-rw-   0        0        0    26211 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationFunctionStatements.py
--rw-rw-rw-   0        0        0    13437 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationImportStatements.py
--rw-rw-rw-   0        0        0     6577 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationLambdaExpressions.py
--rw-rw-rw-   0        0        0    20962 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationMatchStatements.py
--rw-rw-rw-   0        0        0     2409 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationMultidist.py
--rw-rw-rw-   0        0        0     8194 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationNamespacePackages.py
--rw-rw-rw-   0        0        0     4658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationPrintStatements.py
--rw-rw-rw-   0        0        0    15371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationSequenceCreation.py
--rw-rw-rw-   0        0        0     4824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-rw-rw-   0        0        0    14615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationTryExceptStatements.py
--rw-rw-rw-   0        0        0     6982 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-rw-rw-   0        0        0     5674 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-rw-rw-   0        0        0    14341 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationWithStatements.py
--rw-rw-rw-   0        0        0     3088 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/ReformulationYieldExpressions.py
--rw-rw-rw-   0        0        0    12746 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/SourceHandling.py
--rw-rw-rw-   0        0        0     3757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/SyntaxErrors.py
--rw-rw-rw-   0        0        0    22973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/TreeHelpers.py
--rw-rw-rw-   0        0        0    20012 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/VariableClosure.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.210384 Nuitka-winsvc-1.6/nuitka/utils/
--rw-rw-rw-   0        0        0     2655 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/AppDirs.py
--rw-rw-rw-   0        0        0     3248 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/CStrings.py
--rw-rw-rw-   0        0        0     3653 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/CommandLineOptions.py
--rw-rw-rw-   0        0        0     3504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Distributions.py
--rw-rw-rw-   0        0        0     5794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Download.py
--rw-rw-rw-   0        0        0    12376 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Execution.py
--rw-rw-rw-   0        0        0    36129 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/FileOperations.py
--rw-rw-rw-   0        0        0     2885 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Hashing.py
--rw-rw-rw-   0        0        0     2362 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Images.py
--rw-rw-rw-   0        0        0     6816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Importing.py
--rw-rw-rw-   0        0        0     8149 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/InstalledPythons.py
--rw-rw-rw-   0        0        0     2224 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/InstanceCounters.py
--rw-rw-rw-   0        0        0     4336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Jinja2.py
--rw-rw-rw-   0        0        0     1238 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Json.py
--rw-rw-rw-   0        0        0     4173 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/MacOSApp.py
--rw-rw-rw-   0        0        0     5040 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/MemoryUsage.py
--rw-rw-rw-   0        0        0     9057 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/ModuleNames.py
--rw-rw-rw-   0        0        0     4309 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/ReExecute.py
--rw-rw-rw-   0        0        0     3815 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Rest.py
--rw-rw-rw-   0        0        0    22714 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/SharedLibraries.py
--rw-rw-rw-   0        0        0     3664 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Shebang.py
--rw-rw-rw-   0        0        0     2591 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Signing.py
--rw-rw-rw-   0        0        0     6207 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/StaticLibraries.py
--rw-rw-rw-   0        0        0     2602 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/ThreadedExecutor.py
--rw-rw-rw-   0        0        0     2772 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Timing.py
--rw-rw-rw-   0        0        0    10826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Utils.py
--rw-rw-rw-   0        0        0    10574 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/WindowsFileUsage.py
--rw-rw-rw-   0        0        0    19540 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/WindowsResources.py
--rw-rw-rw-   0        0        0     6108 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/Yaml.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/nuitka/utils/__init__.py
--rw-rw-rw-   0        0        0      834 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 02:06:42.644651 Nuitka-winsvc-1.6/setup.cfg
--rw-rw-rw-   0        0        0    15001 2023-05-31 02:00:06.000000 Nuitka-winsvc-1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.211359 Nuitka-winsvc-1.6/tests/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.308715 Nuitka-winsvc-1.6/tests/basics/
--rw-rw-rw-   0        0        0     1766 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/AssertsTest.py
--rw-rw-rw-   0        0        0     5934 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/AssignmentsTest.py
--rw-rw-rw-   0        0        0     5866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/AssignmentsTest32.py
--rw-rw-rw-   0        0        0     4055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/BranchingTest.py
--rw-rw-rw-   0        0        0     1104 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/BuiltinOverload.py
--rw-rw-rw-   0        0        0     3749 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/BuiltinSuperTest.py
--rw-rw-rw-   0        0        0    17080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/BuiltinsTest.py
--rw-rw-rw-   0        0        0      866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ClassMinimalTest.py
--rw-rw-rw-   0        0        0     4764 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ClassesTest.py
--rw-rw-rw-   0        0        0     3414 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ClassesTest32.py
--rw-rw-rw-   0        0        0     1406 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ClassesTest34.py
--rw-rw-rw-   0        0        0     4698 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ComparisonChainsTest.py
--rw-rw-rw-   0        0        0     4639 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ConstantsTest.py
--rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ConstantsTest27.py
--rw-rw-rw-   0        0        0     1628 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/DecoratorsTest.py
--rw-rw-rw-   0        0        0     2317 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/DefaultParametersTest.py
--rw-rw-rw-   0        0        0     1127 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/DoubleDeletionsTest.py
--rw-rw-rw-   0        0        0      806 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/EmptyModuleTest.py
--rw-rw-rw-   0        0        0    14387 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ExceptionRaisingTest.py
--rw-rw-rw-   0        0        0      961 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ExceptionRaisingTest32.py
--rw-rw-rw-   0        0        0     1458 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ExceptionRaisingTest33.py
--rw-rw-rw-   0        0        0     6747 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ExecEvalTest.py
--rw-rw-rw-   0        0        0     1417 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ExtremeClosureTest.py
--rw-rw-rw-   0        0        0     1658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/FunctionObjectsTest.py
--rw-rw-rw-   0        0        0    12335 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/FunctionsTest.py
--rw-rw-rw-   0        0        0     3603 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/FunctionsTest32.py
--rw-rw-rw-   0        0        0     2627 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/FunctionsTest_2.py
--rw-rw-rw-   0        0        0      890 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/FutureTest32.py
--rw-rw-rw-   0        0        0     5809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/GeneratorExpressionsTest.py
--rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/GeneratorExpressionsTest_37.py
--rw-rw-rw-   0        0        0     3824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/GlobalStatementTest.py
--rw-rw-rw-   0        0        0     1286 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/HelloWorldTest_2.py
--rw-rw-rw-   0        0        0     2469 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ImportingTest.py
--rw-rw-rw-   0        0        0     1296 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/InplaceOperationsTest.py
--rw-rw-rw-   0        0        0     4227 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/InspectionTest.py
--rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/InspectionTest_35.py
--rw-rw-rw-   0        0        0     1618 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/InspectionTest_36.py
--rw-rw-rw-   0        0        0     1671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/LambdasTest.py
--rw-rw-rw-   0        0        0     2731 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/LateClosureAssignmentTest.py
--rw-rw-rw-   0        0        0     2923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ListContractionsTest.py
--rw-rw-rw-   0        0        0     3329 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/LoopingTest.py
--rw-rw-rw-   0        0        0     1536 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/MainProgramsTest.py
--rw-rw-rw-   0        0        0     1925 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ModuleAttributesTest.py
--rw-rw-rw-   0        0        0     1988 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/OperatorsTest.py
--rw-rw-rw-   0        0        0    14903 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/OrderChecksTest.py
--rw-rw-rw-   0        0        0     1827 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/OrderChecksTest27.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/OverflowFunctionsTest_2.py
--rw-rw-rw-   0        0        0     5853 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ParameterErrorsTest.py
--rw-rw-rw-   0        0        0     1899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ParameterErrorsTest32.py
--rw-rw-rw-   0        0        0      863 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/PrintFutureTest.py
--rw-rw-rw-   0        0        0     1413 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/PrintingTest_2.py
--rw-rw-rw-   0        0        0      878 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/RecursionTest.py
--rw-rw-rw-   0        0        0    23840 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ReferencingTest.py
--rw-rw-rw-   0        0        0     2076 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ReferencingTest27.py
--rw-rw-rw-   0        0        0     7819 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ReferencingTest33.py
--rw-rw-rw-   0        0        0     4902 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ReferencingTest35.py
--rw-rw-rw-   0        0        0     5092 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ReferencingTest36.py
--rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ReferencingTest_2.py
--rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/SlotsTest.py
--rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/ThreadedGeneratorsTest.py
--rw-rw-rw-   0        0        0    22966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TrickAssignmentsTest32.py
--rw-rw-rw-   0        0        0     1541 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TrickAssignmentsTest35.py
--rw-rw-rw-   0        0        0     1788 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TrickAssignmentsTest_2.py
--rw-rw-rw-   0        0        0     2086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TryContinueFinallyTest.py
--rw-rw-rw-   0        0        0     2212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TryExceptContinueTest.py
--rw-rw-rw-   0        0        0     2275 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TryExceptFinallyTest.py
--rw-rw-rw-   0        0        0     2304 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TryExceptFramesTest.py
--rw-rw-rw-   0        0        0     2842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TryReturnFinallyTest.py
--rw-rw-rw-   0        0        0     2328 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/TryYieldFinallyTest.py
--rw-rw-rw-   0        0        0     1093 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/UnicodeTest.py
--rw-rw-rw-   0        0        0     1877 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/UnpackingTest35.py
--rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/VarargsTest.py
--rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/WithStatementsTest.py
--rw-rw-rw-   0        0        0     3070 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/YieldFromTest33.py
--rw-rw-rw-   0        0        0     3821 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/run_all.py
--rw-rw-rw-   0        0        0     2271 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/basics/run_xml.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.311643 Nuitka-winsvc-1.6/tests/onefile/
--rw-rw-rw-   0        0        0     1213 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/onefile/HelloWorldTest.py
--rw-rw-rw-   0        0        0     1307 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/onefile/KeyboardInterruptTest.py
--rw-rw-rw-   0        0        0     5816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/onefile/run_all.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.329223 Nuitka-winsvc-1.6/tests/optimizations/
--rw-rw-rw-   0        0        0      958 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/ArgumentTypes.py
--rw-rw-rw-   0        0        0     1055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/Attributes.py
--rw-rw-rw-   0        0        0     1021 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/Calls.py
--rw-rw-rw-   0        0        0      921 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/Conditions.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/DecodingOperations.py
--rw-rw-rw-   0        0        0     1212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/FormatStrings36.py
--rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/HardImports.py
--rw-rw-rw-   0        0        0      974 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/HardImports_2.py
--rw-rw-rw-   0        0        0      918 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/Iterations.py
--rw-rw-rw-   0        0        0     1260 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/Len.py
--rw-rw-rw-   0        0        0     2262 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/Operations.py
--rw-rw-rw-   0        0        0     1333 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/Subscripts.py
--rw-rw-rw-   0        0        0     8736 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/optimizations/run_all.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.330199 Nuitka-winsvc-1.6/tests/packages/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.332154 Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/
--rw-rw-rw-   0        0        0     2382 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.336061 Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/variable_package/
--rw-rw-rw-   0        0        0      942 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-rw-rw-   0        0        0     1168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rw-rw-rw-   0        0        0     3671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/run_all.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.938672 Nuitka-winsvc-1.6/tests/packages/sub_package/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.338987 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/
--rw-rw-rw-   0        0        0     1230 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/__init__.py
--rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/bigkitty.py
--rw-rw-rw-   0        0        0      910 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/smallkitty.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.342895 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/
--rw-rw-rw-   0        0        0      929 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/hello.py
--rw-rw-rw-   0        0        0      966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/miau.py
--rw-rw-rw-   0        0        0      968 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/purr.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.939649 Nuitka-winsvc-1.6/tests/packages/top_level_attributes_3/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.344848 Nuitka-winsvc-1.6/tests/packages/top_level_attributes_3/some_package/
--rw-rw-rw-   0        0        0     2336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-rw-rw-   0        0        0      907 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.345825 Nuitka-winsvc-1.6/tests/plugins/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.346801 Nuitka-winsvc-1.6/tests/plugins/code_signing/
--rw-rw-rw-   0        0        0     1170 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/plugins/code_signing/CodeSigningMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.353637 Nuitka-winsvc-1.6/tests/plugins/data_files/
--rw-rw-rw-   0        0        0     1332 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/plugins/data_files/DataFilesMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.356566 Nuitka-winsvc-1.6/tests/plugins/data_files/data_files_package/
--rw-rw-rw-   0        0        0      924 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/plugins/data_files/data_files_package/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/tests/plugins/data_files/data_files_package/lala.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.357542 Nuitka-winsvc-1.6/tests/plugins/data_files/data_files_package/sub_dir/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.360472 Nuitka-winsvc-1.6/tests/plugins/parameters/
--rw-rw-rw-   0        0        0     1019 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/plugins/parameters/ParametersMain.py
--rw-rw-rw-   0        0        0     2168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/plugins/parameters/parameter-using-plugin.py
--rw-rw-rw-   0        0        0     3861 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/plugins/run_all.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.361450 Nuitka-winsvc-1.6/tests/programs/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.362427 Nuitka-winsvc-1.6/tests/programs/absolute_import/
--rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.367314 Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/
--rw-rw-rw-   0        0        0      796 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/foobar.py
--rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/local.py
--rw-rw-rw-   0        0        0      860 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/util.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.368282 Nuitka-winsvc-1.6/tests/programs/case_imports1/
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports1/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.370238 Nuitka-winsvc-1.6/tests/programs/case_imports1/path1/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports1/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.371214 Nuitka-winsvc-1.6/tests/programs/case_imports1/path1/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.372190 Nuitka-winsvc-1.6/tests/programs/case_imports1/path2/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports1/path2/some_module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.372190 Nuitka-winsvc-1.6/tests/programs/case_imports1/path2/some_package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.373167 Nuitka-winsvc-1.6/tests/programs/case_imports2/
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports2/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.374142 Nuitka-winsvc-1.6/tests/programs/case_imports2/path1/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports2/path1/some_module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.375120 Nuitka-winsvc-1.6/tests/programs/case_imports2/path1/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.376096 Nuitka-winsvc-1.6/tests/programs/case_imports2/path2/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports2/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.377072 Nuitka-winsvc-1.6/tests/programs/case_imports2/path2/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.378049 Nuitka-winsvc-1.6/tests/programs/case_imports3/
--rw-rw-rw-   0        0        0     1075 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports3/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.379025 Nuitka-winsvc-1.6/tests/programs/case_imports3/path1/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports3/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.380002 Nuitka-winsvc-1.6/tests/programs/case_imports3/path1/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.380980 Nuitka-winsvc-1.6/tests/programs/case_imports3/path2/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports3/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.382934 Nuitka-winsvc-1.6/tests/programs/case_imports3/path2/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.383914 Nuitka-winsvc-1.6/tests/programs/cyclic_imports/
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.387813 Nuitka-winsvc-1.6/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.390744 Nuitka-winsvc-1.6/tests/programs/dash_import/
--rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/dash_import/DashImportMain.py
--rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/dash_import/dash-module.py
--rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/dash_import/plus+module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.391720 Nuitka-winsvc-1.6/tests/programs/dash_main/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/dash_main/Dash-Main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.392697 Nuitka-winsvc-1.6/tests/programs/deep/
--rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/deep/DeepProgramMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.395628 Nuitka-winsvc-1.6/tests/programs/deep/some_package/
--rw-rw-rw-   0        0        0      980 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/deep/some_package/DeepBrother.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/deep/some_package/DeepChild.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/deep/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.397580 Nuitka-winsvc-1.6/tests/programs/deep/some_package/deep_package/
--rw-rw-rw-   0        0        0      876 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-rw-rw-   0        0        0      952 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/deep/some_package/deep_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.399536 Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/
--rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.401485 Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/package/
--rw-rw-rw-   0        0        0      797 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/package/SubModule.py
--rw-rw-rw-   0        0        0      857 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.402461 Nuitka-winsvc-1.6/tests/programs/import_variants/
--rw-rw-rw-   0        0        0     1005 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/import_variants/ImportVariationsMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.407346 Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/
--rw-rw-rw-   0        0        0      946 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/Child1.py
--rw-rw-rw-   0        0        0     1098 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/Child2.py
--rw-rw-rw-   0        0        0      822 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/Child3.py
--rw-rw-rw-   0        0        0      994 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.409298 Nuitka-winsvc-1.6/tests/programs/main_raises/
--rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/main_raises/ErrorMain.py
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/main_raises/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.411251 Nuitka-winsvc-1.6/tests/programs/main_raises2/
--rw-rw-rw-   0        0        0     1080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/main_raises2/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.412227 Nuitka-winsvc-1.6/tests/programs/module_attributes/
--rw-rw-rw-   0        0        0     1529 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.414246 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.418095 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.421016 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.423946 Nuitka-winsvc-1.6/tests/programs/module_exits/
--rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_exits/ErrorExitingModule.py
--rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_exits/Main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.427852 Nuitka-winsvc-1.6/tests/programs/module_object_replacing/
--rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-rw-rw-   0        0        0     1359 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.428828 Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/
--rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.434702 Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/foo/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/foo/__init__.py
--rw-rw-rw-   0        0        0      836 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/foo/__main__.py
--rw-rw-rw-   0        0        0     1758 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/foo/entry.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.436641 Nuitka-winsvc-1.6/tests/programs/named_imports/
--rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/named_imports/NamedImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.439571 Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.441523 Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/sub_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.442499 Nuitka-winsvc-1.6/tests/programs/package_code/
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_code/PackageInitCodeMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.444450 Nuitka-winsvc-1.6/tests/programs/package_code/some_package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_code/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_code/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.449340 Nuitka-winsvc-1.6/tests/programs/package_contains_main/
--rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_contains_main/PackageContainsMain.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_contains_main/__init__.py
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_contains_main/local.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.451285 Nuitka-winsvc-1.6/tests/programs/package_init_import/
--rw-rw-rw-   0        0        0      823 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_init_import/PackageInitImportMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.455190 Nuitka-winsvc-1.6/tests/programs/package_init_import/some_package/
--rw-rw-rw-   0        0        0     1008 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_init_import/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.456167 Nuitka-winsvc-1.6/tests/programs/package_init_issue/
--rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.458120 Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.461054 Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/child_package/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-rw-rw-   0        0        0      795 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.462027 Nuitka-winsvc-1.6/tests/programs/package_missing_init/
--rw-rw-rw-   0        0        0      926 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.463003 Nuitka-winsvc-1.6/tests/programs/package_missing_init/some_package/
--rw-rw-rw-   0        0        0      965 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_missing_init/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.463980 Nuitka-winsvc-1.6/tests/programs/package_missing_init/some_package/sub_package/
--rw-rw-rw-   0        0        0      977 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.467889 Nuitka-winsvc-1.6/tests/programs/package_module_collision/
--rw-rw-rw-   0        0        0      901 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.468863 Nuitka-winsvc-1.6/tests/programs/package_module_collision/Something/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_module_collision/Something/__init__.py
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_module_collision/something.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.469838 Nuitka-winsvc-1.6/tests/programs/package_overload/
--rw-rw-rw-   0        0        0      852 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_overload/Main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.473747 Nuitka-winsvc-1.6/tests/programs/package_overload/foo/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_overload/foo/__init__.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_overload/foo/bar.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_overload/foo/bar2.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.474720 Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/
--rw-rw-rw-   0        0        0     2972 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.477654 Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/some_package/
--rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:38.997262 Nuitka-winsvc-1.6/tests/programs/package_program/
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.481563 Nuitka-winsvc-1.6/tests/programs/package_program/PackageAsMain/
--rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_program/PackageAsMain/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/package_program/PackageAsMain/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.482538 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/
--rw-rw-rw-   0        0        0     1728 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.484490 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.490346 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.494254 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.495239 Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/
--rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.514759 Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-rw-rw-   0        0        0     1553 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.516712 Nuitka-winsvc-1.6/tests/programs/plugin_import/
--rw-rw-rw-   0        0        0      859 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/plugin_import/PluginImportMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.519642 Nuitka-winsvc-1.6/tests/programs/plugin_import/some_package/
--rw-rw-rw-   0        0        0      771 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/plugin_import/some_package/__init__.py
--rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/plugin_import/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.521596 Nuitka-winsvc-1.6/tests/programs/reimport_main_dynamic/
--rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.522572 Nuitka-winsvc-1.6/tests/programs/reimport_main_static/
--rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.524526 Nuitka-winsvc-1.6/tests/programs/relative_import/
--rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/relative_import/RelativeImportMain.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/relative_import/dircache.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.525502 Nuitka-winsvc-1.6/tests/programs/resource_reader37/
--rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.528434 Nuitka-winsvc-1.6/tests/programs/resource_reader37/some_package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/resource_reader37/some_package/__init__.py
--rw-rw-rw-   0        0        0     6615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/run_all.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.530384 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/
--rw-rw-rw-   0        0        0     1171 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/pyexpat.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.537218 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/__init__.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.540149 Nuitka-winsvc-1.6/tests/programs/syntax_errors/
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/syntax_errors/IndentationErroring.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/syntax_errors/SyntaxErroring.py
--rw-rw-rw-   0        0        0     1079 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.543080 Nuitka-winsvc-1.6/tests/programs/unicode_bom/
--rw-rw-rw-   0        0        0      963 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/unicode_bom/unicode_bom.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.544057 Nuitka-winsvc-1.6/tests/programs/with space/
--rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/programs/with space/Space Main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.545031 Nuitka-winsvc-1.6/tests/reflected/
--rw-rw-rw-   0        0        0    14061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/reflected/compile_itself.py
--rw-rw-rw-   0        0        0     1243 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/run-tests
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.591905 Nuitka-winsvc-1.6/tests/standalone/
--rw-rw-rw-   0        0        0     1058 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/BrotliUsing.py
--rw-rw-rw-   0        0        0     2554 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/CtypesUsing.py
--rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/FlaskUsing.py
--rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/GlfwUsing.py
--rw-rw-rw-   0        0        0     1184 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/GtkUsing.py
--rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/HexEncodingTest_2.py
--rw-rw-rw-   0        0        0     1086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/IdnaUsing.py
--rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/LxmlUsing.py
--rw-rw-rw-   0        0        0     1431 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/MatplotlibUsing.py
--rw-rw-rw-   0        0        0     2538 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/MetadataPackagesUsing.py
--rw-rw-rw-   0        0        0     1727 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/NumpyUsing.py
--rw-rw-rw-   0        0        0      947 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/OpenGLUsing.py
--rw-rw-rw-   0        0        0     1379 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PandasUsing.py
--rw-rw-rw-   0        0        0     1066 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PasslibUsing.py
--rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PendulumUsing.py
--rw-rw-rw-   0        0        0     2074 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PkgResourcesRequiresUsing.py
--rw-rw-rw-   0        0        0     1067 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PmwUsing.py
--rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PyQt5Plugins.py
--rw-rw-rw-   0        0        0     1105 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PyQt5SSLSupport.py
--rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PyQt5Using.py
--rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PyQt6Plugins.py
--rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PyQt6Using.py
--rw-rw-rw-   0        0        0     1091 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PySide6Plugins.py
--rw-rw-rw-   0        0        0     1757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/PySide6Using.py
--rw-rw-rw-   0        0        0     1323 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/RsaUsing.py
--rw-rw-rw-   0        0        0      973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/ShlibUsing.py
--rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/SocketUsing.py
--rw-rw-rw-   0        0        0     1941 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/TkInterUsing.py
--rw-rw-rw-   0        0        0     3228 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/Urllib3Using.py
--rw-rw-rw-   0        0        0     1200 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/Win32ComUsing.py
--rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/run_all.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.592877 Nuitka-winsvc-1.6/tests/standalone/zip_importer/
--rw-rw-rw-   0        0        0     1264 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/standalone/zip_importer/ZipImporterMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 02:06:42.640728 Nuitka-winsvc-1.6/tests/syntax/
--rw-rw-rw-   0        0        0      811 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/AsyncgenReturn36.py
--rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/BreakWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/ClassReturn.py
--rw-rw-rw-   0        0        0      970 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/ClosureDel_2.py
--rw-rw-rw-   0        0        0      849 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/ContinueWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/DuplicateArgument.py
--rw-rw-rw-   0        0        0     1111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/ExecWithNesting_2.py
--rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/FutureBraces.py
--rw-rw-rw-   0        0        0      805 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/FutureUnknown.py
--rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/GeneratorExpressions38.py
--rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/GeneratorReturn_2.py
--rw-rw-rw-   0        0        0      792 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/GlobalForParameter.py
--rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/Importing32.py
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/IndentationError.py
--rw-rw-rw-   0        0        0      915 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/LateFutureImport.py
--rw-rw-rw-   0        0        0      841 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/MisplacedFutureImport.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/ModuleReturn.py
--rw-rw-rw-   0        0        0      883 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/NonlocalForParameter32.py
--rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/NonlocalNotFound32.py
--rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/StarImportExtra.py
--rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/SyntaxError.py
--rw-rw-rw-   0        0        0      874 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/TryExceptAllNotLast.py
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/TryFinallyContinue_37.py
--rw-rw-rw-   0        0        0      776 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/UnpackNoTuple.py
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/UnpackTwoStars32.py
--rw-rw-rw-   0        0        0      793 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/YieldFromInModule.py
--rw-rw-rw-   0        0        0      804 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/YieldInAsync35.py
--rw-rw-rw-   0        0        0      923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/YieldInGenexp38.py
--rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/YieldInModule.py
--rw-rw-rw-   0        0        0     2203 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6/tests/syntax/run_all.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:32.183413 Nuitka-winsvc-1.6.3/
+-rw-rw-rw-   0        0        0   825587 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/Changelog.rst
+-rw-rw-rw-   0        0        0   152515 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/Developer_Manual.rst
+-rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1733 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.126875 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/
+-rw-rw-rw-   0        0        0     4626 2023-06-16 02:38:24.000000 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    76624 2023-06-16 02:38:24.000000 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 02:38:24.000000 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      308 2023-06-16 02:38:24.000000 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-06-16 02:38:24.000000 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-16 02:38:24.000000 Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4626 2023-06-16 02:38:32.182405 Nuitka-winsvc-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2651 2023-06-16 02:32:36.000000 Nuitka-winsvc-1.6.3/README.md
+-rw-rw-rw-   0        0        0    75940 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.233839 Nuitka-winsvc-1.6.3/bin/
+-rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/bin/autoformat-nuitka-source
+-rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/bin/check-nuitka-with-pylint
+-rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/bin/compare_with_cpython
+-rw-rw-rw-   0        0        0     3079 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/bin/compare_with_xml
+-rw-rw-rw-   0        0        0     1163 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/bin/measure-construct-performance
+-rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/bin/nuitka
+-rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/bin/nuitka-run
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.833250 Nuitka-winsvc-1.6.3/doc/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.283866 Nuitka-winsvc-1.6.3/doc/Logo/
+-rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.305873 Nuitka-winsvc-1.6.3/doc/images/
+-rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/doc/images/Nuitka-Logo-Horizontal.png
+-rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/doc/images/Nuitka-Logo-Symbol.png
+-rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/doc/images/Nuitka-Logo-Vertical.png
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.308894 Nuitka-winsvc-1.6.3/lib/
+-rw-rw-rw-   0        0        0     4250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/lib/hints.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.334841 Nuitka-winsvc-1.6.3/misc/
+-rwxrwxrwx   0        0        0      901 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/misc/nuitka-run.bat
+-rwxrwxrwx   0        0        0     1038 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/misc/nuitka.bat
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.379839 Nuitka-winsvc-1.6.3/nuitka/
+-rw-rw-rw-   0        0        0     7331 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Builtins.py
+-rw-rw-rw-   0        0        0     5437 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/BytecodeCaching.py
+-rw-rw-rw-   0        0        0     3440 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Bytecodes.py
+-rw-rw-rw-   0        0        0     1884 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/CacheCleanup.py
+-rw-rw-rw-   0        0        0    11148 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Constants.py
+-rw-rw-rw-   0        0        0     2447 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Errors.py
+-rw-rw-rw-   0        0        0    37236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/MainControl.py
+-rw-rw-rw-   0        0        0     8064 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/ModuleRegistry.py
+-rw-rw-rw-   0        0        0    57087 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/OptionParsing.py
+-rw-rw-rw-   0        0        0    66046 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/Options.py
+-rw-rw-rw-   0        0        0     5022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/OutputDirectories.py
+-rw-rw-rw-   0        0        0    14550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/PostProcessing.py
+-rw-rw-rw-   0        0        0     5770 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Progress.py
+-rw-rw-rw-   0        0        0     7472 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/PythonFlavors.py
+-rw-rw-rw-   0        0        0     4061 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/PythonOperators.py
+-rw-rw-rw-   0        0        0    12179 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/PythonVersions.py
+-rw-rw-rw-   0        0        0     8514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Serialization.py
+-rw-rw-rw-   0        0        0     4670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/SourceCodeReferences.py
+-rw-rw-rw-   0        0        0    11235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Tracing.py
+-rw-rw-rw-   0        0        0     3395 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/TreeXML.py
+-rw-rw-rw-   0        0        0    15235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/Variables.py
+-rw-rw-rw-   0        0        0     2055 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/Version.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/__init__.py
+-rw-rw-rw-   0        0        0     5615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/__main__.py
+-rw-rw-rw-   0        0        0     5295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/__past__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.432841 Nuitka-winsvc-1.6.3/nuitka/build/
+-rw-rw-rw-   0        0        0    33528 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/Backend.scons
+-rw-rw-rw-   0        0        0     8314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/CCompilerVersion.scons
+-rw-rw-rw-   0        0        0     2433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/DataComposerInterface.py
+-rw-rw-rw-   0        0        0    18807 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/build/Onefile.scons
+-rw-rw-rw-   0        0        0    15635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/SconsCaching.py
+-rw-rw-rw-   0        0        0    30984 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/build/SconsCompilerSettings.py
+-rw-rw-rw-   0        0        0     5527 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/SconsHacks.py
+-rw-rw-rw-   0        0        0    15532 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/SconsInterface.py
+-rw-rw-rw-   0        0        0     2361 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/SconsProgress.py
+-rw-rw-rw-   0        0        0    11964 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/build/SconsSpawn.py
+-rw-rw-rw-   0        0        0    24338 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/build/SconsUtils.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.854250 Nuitka-winsvc-1.6.3/nuitka/build/include/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.504412 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/
+-rw-rw-rw-   0        0        0     7972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/allocator.h
+-rw-rw-rw-   0        0        0     3423 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/builtins.h
+-rw-rw-rw-   0        0        0     4604 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/calling.h
+-rw-rw-rw-   0        0        0     1977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/checkers.h
+-rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/checksum_tools.h
+-rw-rw-rw-   0        0        0     9571 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-rw-rw-   0        0        0     2002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_cell.h
+-rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-rw-rw-   0        0        0    16949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_frame.h
+-rw-rw-rw-   0        0        0     5972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_function.h
+-rw-rw-rw-   0        0        0     9136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_generator.h
+-rw-rw-rw-   0        0        0     1838 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_method.h
+-rw-rw-rw-   0        0        0     7408 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/constants.h
+-rw-rw-rw-   0        0        0     1293 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/constants_blob.h
+-rw-rw-rw-   0        0        0    34083 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/exceptions.h
+-rw-rw-rw-   0        0        0     3221 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-rw-rw-   0        0        0     6253 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/freelists.h
+-rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/hedley.h
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.616429 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/
+-rw-rw-rw-   0        0        0     3275 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/attributes.h
+-rw-rw-rw-   0        0        0     2663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/boolean.h
+-rw-rw-rw-   0        0        0     1181 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/bytes.h
+-rw-rw-rw-   0        0        0     9335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-rw-rw-   0        0        0    10615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-rw-rw-   0        0        0    13139 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-rw-rw-   0        0        0     1743 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/complex.h
+-rw-rw-rw-   0        0        0    13109 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-rw-rw-   0        0        0     1206 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/floats.h
+-rw-rw-rw-   0        0        0     3674 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-rw-rw-   0        0        0     1798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/indexes.h
+-rw-rw-rw-   0        0        0     2941 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/ints.h
+-rw-rw-rw-   0        0        0     9992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/iterators.h
+-rw-rw-rw-   0        0        0     3411 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/lists.h
+-rw-rw-rw-   0        0        0     1633 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-rw-rw-   0        0        0     1328 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/mappings.h
+-rw-rw-rw-   0        0        0     4573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations.h
+-rw-rw-rw-   0        0        0    12685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-rw-rw-   0        0        0     5641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-rw-rw-   0        0        0     5422 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-rw-rw-   0        0        0     5460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-rw-rw-   0        0        0     2799 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-rw-rw-   0        0        0    15778 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-rw-rw-   0        0        0    13210 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-rw-rw-   0        0        0     5791 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-rw-rw-   0        0        0     4714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-rw-rw-   0        0        0     5824 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-rw-rw-   0        0        0     5438 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-rw-rw-   0        0        0    15100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-rw-rw-   0        0        0     8670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-rw-rw-   0        0        0     3753 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-rw-rw-   0        0        0     4846 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-rw-rw-   0        0        0    10626 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-rw-rw-   0        0        0     9201 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-rw-rw-   0        0        0     5147 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-rw-rw-   0        0        0     4349 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-rw-rw-   0        0        0     4975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-rw-rw-   0        0        0     4826 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-rw-rw-   0        0        0     3297 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/raising.h
+-rw-rw-rw-   0        0        0     2178 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-rw-rw-   0        0        0     1146 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-rw-rw-   0        0        0     1112 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/sequences.h
+-rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/sets.h
+-rw-rw-rw-   0        0        0     8419 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/slices.h
+-rw-rw-rw-   0        0        0     1242 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/strings.h
+-rw-rw-rw-   0        0        0    17575 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-rw-rw-   0        0        0     5720 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/tuples.h
+-rw-rw-rw-   0        0        0    14412 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helpers.h
+-rw-rw-rw-   0        0        0     5375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/importing.h
+-rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/incbin.h
+-rw-rw-rw-   0        0        0    14427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/prelude.h
+-rw-rw-rw-   0        0        0     2870 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/printing.h
+-rw-rw-rw-   0        0        0     1761 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/python_pgo.h
+-rw-rw-rw-   0        0        0     2119 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-rw-rw-   0        0        0     3840 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/threading.h
+-rw-rw-rw-   0        0        0     3144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/tracing.h
+-rw-rw-rw-   0        0        0     2936 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/unfreezing.h
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.896249 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.627423 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/appdirs/
+-rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.639408 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/atomicwrites/
+-rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.641407 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/bin/
+-rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/bin/scons.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.858250 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/clcache/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.657409 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/clcache/clcache/
+-rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.669408 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/
+-rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.679409 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/
+-rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.696407 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/
+-rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.701412 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/
+-rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.716409 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.763415 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.789409 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/
+-rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.833410 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.881250 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.866249 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.864411 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.872413 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.881411 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.896411 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.902412 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:25.913412 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.047993 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.058993 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.060994 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.067993 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.080994 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.873250 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.111998 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.116996 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.417549 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.424546 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.431549 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.533026 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.545029 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.547026 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.548025 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.555042 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.558028 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.882254 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.585026 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.592027 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.607034 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.612028 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.618026 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.734519 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.745519 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.747521 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.750518 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.753519 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.763520 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.767526 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.780519 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.790523 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.890251 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/pkg_resources/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.794519 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.891256 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.830521 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
+-rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/gui.py
+-rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.848522 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.875355 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/
+-rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.881355 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.903355 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.916355 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.936356 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.946356 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/
+-rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.968357 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/
+-rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:26.978356 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/
+-rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/zstd.h
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.102915 Nuitka-winsvc-1.6.3/nuitka/build/static_src/
+-rw-rw-rw-   0        0        0    82114 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-rw-rw-   0        0        0     8250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledCellType.c
+-rw-rw-rw-   0        0        0    62733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-rw-rw-   0        0        0    70973 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-rw-rw-   0        0        0    35861 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledFrameType.c
+-rw-rw-rw-   0        0        0   100376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledFunctionType.c
+-rw-rw-rw-   0        0        0    60649 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-rw-rw-   0        0        0    48526 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-rw-rw-   0        0        0    21638 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledMethodType.c
+-rw-rw-rw-   0        0        0    18993 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersAllocator.c
+-rw-rw-rw-   0        0        0    32849 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersAttributes.c
+-rw-rw-rw-   0        0        0    21783 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersBuiltin.c
+-rw-rw-rw-   0        0        0   107641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-rw-rw-   0        0        0     3033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersBytes.c
+-rw-rw-rw-   0        0        0    13057 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersCalling.c
+-rw-rw-rw-   0        0        0   470655 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-rw-rw-   0        0        0     1617 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-rw-rw-   0        0        0     2991 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersClasses.c
+-rw-rw-rw-   0        0        0   317872 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-rw-rw-   0        0        0     4673 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-rw-rw-   0        0        0   313003 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-rw-rw-   0        0        0   312414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-rw-rw-   0        0        0   316217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-rw-rw-   0        0        0   315628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-rw-rw-   0        0        0   314618 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-rw-rw-   0        0        0    36068 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-rw-rw-   0        0        0    19313 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-rw-rw-   0        0        0    38364 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersDictionaries.c
+-rw-rw-rw-   0        0        0    24295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-rw-rw-   0        0        0     7035 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersExceptions.c
+-rw-rw-rw-   0        0        0     6668 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersFiles.c
+-rw-rw-rw-   0        0        0    11199 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-rw-rw-   0        0        0     2426 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersFloats.c
+-rw-rw-rw-   0        0        0     1774 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-rw-rw-   0        0        0    14585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersImport.c
+-rw-rw-rw-   0        0        0    13589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersImportHard.c
+-rw-rw-rw-   0        0        0    18433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersLists.c
+-rw-rw-rw-   0        0        0    13915 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-rw-rw-   0        0        0     1640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersMappings.c
+-rw-rw-rw-   0        0        0     3513 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersMatching.c
+-rw-rw-rw-   0        0        0   181243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-rw-rw-   0        0        0    16700 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-rw-rw-   0        0        0    77782 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-rw-rw-   0        0        0    67487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-rw-rw-   0        0        0    68748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-rw-rw-   0        0        0     6274 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-rw-rw-   0        0        0    83405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-rw-rw-   0        0        0    13776 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-rw-rw-   0        0        0   183202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-rw-rw-   0        0        0   188514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-rw-rw-   0        0        0     3404 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-rw-rw-   0        0        0    66453 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-rw-rw-   0        0        0    78891 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-rw-rw-   0        0        0     1023 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-rw-rw-   0        0        0    77305 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-rw-rw-   0        0        0    70465 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-rw-rw-   0        0        0    68005 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-rw-rw-   0        0        0   149580 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-rw-rw-   0        0        0     4071 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-rw-rw-   0        0        0    53122 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-rw-rw-   0        0        0    76512 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-rw-rw-   0        0        0    47568 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-rw-rw-   0        0        0    17742 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-rw-rw-   0        0        0   136100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-rw-rw-   0        0        0   142211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-rw-rw-   0        0        0    74142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-rw-rw-   0        0        0    82669 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-rw-rw-   0        0        0    45052 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-rw-rw-   0        0        0    82842 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-rw-rw-   0        0        0    76343 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-rw-rw-   0        0        0     3219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersProfiling.c
+-rw-rw-rw-   0        0        0     3805 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-rw-rw-   0        0        0    15369 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersRaising.c
+-rw-rw-rw-   0        0        0    11926 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-rw-rw-   0        0        0     3730 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersSequences.c
+-rw-rw-rw-   0        0        0     1946 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersSlices.c
+-rw-rw-rw-   0        0        0    26642 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersStrings.c
+-rw-rw-rw-   0        0        0     4037 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersTuples.c
+-rw-rw-rw-   0        0        0     5578 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersTypes.c
+-rw-rw-rw-   0        0        0    11986 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/InspectPatcher.c
+-rw-rw-rw-   0        0        0    41670 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/MainProgram.c
+-rw-rw-rw-   0        0        0    58634 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-rw-rw-   0        0        0     4537 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-rw-rw-   0        0        0     6427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-rw-rw-   0        0        0    17065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-rw-rw-   0        0        0    36617 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/OnefileBootstrap.c
+-rw-rw-rw-   0        0        0     7984 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.201386 Nuitka-winsvc-1.6.3/nuitka/code_generation/
+-rw-rw-rw-   0        0        0     6414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/AsyncgenCodes.py
+-rw-rw-rw-   0        0        0    10153 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/AttributeCodes.py
+-rw-rw-rw-   0        0        0    21864 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-rw-rw-   0        0        0     2339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/BranchCodes.py
+-rw-rw-rw-   0        0        0    16009 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/BuiltinCodes.py
+-rw-rw-rw-   0        0        0    35905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/CallCodes.py
+-rw-rw-rw-   0        0        0     4896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ClassCodes.py
+-rw-rw-rw-   0        0        0    51116 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeGeneration.py
+-rw-rw-rw-   0        0        0     2375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeHelperSelection.py
+-rw-rw-rw-   0        0        0    14392 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeHelpers.py
+-rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeObjectCodes.py
+-rw-rw-rw-   0        0        0    17570 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ComparisonCodes.py
+-rw-rw-rw-   0        0        0     4446 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-rw-rw-   0        0        0     7335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ConditionalCodes.py
+-rw-rw-rw-   0        0        0     6539 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ConstantCodes.py
+-rw-rw-rw-   0        0        0    31186 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/Contexts.py
+-rw-rw-rw-   0        0        0     8484 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/CoroutineCodes.py
+-rw-rw-rw-   0        0        0     1574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/CtypesCodes.py
+-rw-rw-rw-   0        0        0    28478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/DictCodes.py
+-rw-rw-rw-   0        0        0     2125 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/Emission.py
+-rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ErrorCodes.py
+-rw-rw-rw-   0        0        0    12304 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/EvalCodes.py
+-rw-rw-rw-   0        0        0     8975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ExceptionCodes.py
+-rw-rw-rw-   0        0        0     7350 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-rw-rw-   0        0        0     2093 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ExpressionCodes.py
+-rw-rw-rw-   0        0        0    17725 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/FrameCodes.py
+-rw-rw-rw-   0        0        0    27345 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/FunctionCodes.py
+-rw-rw-rw-   0        0        0     7690 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/GeneratorCodes.py
+-rw-rw-rw-   0        0        0     5721 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/GlobalConstants.py
+-rw-rw-rw-   0        0        0     6911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-rw-rw-   0        0        0     1794 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/IdCodes.py
+-rw-rw-rw-   0        0        0    13318 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ImportCodes.py
+-rw-rw-rw-   0        0        0     1396 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/Indentation.py
+-rw-rw-rw-   0        0        0     1506 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/IndexCodes.py
+-rw-rw-rw-   0        0        0     1033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/InjectCCodes.py
+-rw-rw-rw-   0        0        0     3432 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/IntegerCodes.py
+-rw-rw-rw-   0        0        0    12010 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/IteratorCodes.py
+-rw-rw-rw-   0        0        0     2022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/LabelCodes.py
+-rw-rw-rw-   0        0        0     2612 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/LineNumberCodes.py
+-rw-rw-rw-   0        0        0    15906 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ListCodes.py
+-rw-rw-rw-   0        0        0     6375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/LoaderCodes.py
+-rw-rw-rw-   0        0        0     9951 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/LocalsDictCodes.py
+-rw-rw-rw-   0        0        0     3135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/LoopCodes.py
+-rw-rw-rw-   0        0        0     1597 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/MatchCodes.py
+-rw-rw-rw-   0        0        0     6291 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ModuleCodes.py
+-rw-rw-rw-   0        0        0     8118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/Namify.py
+-rw-rw-rw-   0        0        0    12777 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/OperationCodes.py
+-rw-rw-rw-   0        0        0    28231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/PackageResourceCodes.py
+-rw-rw-rw-   0        0        0     3021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/PrintCodes.py
+-rw-rw-rw-   0        0        0     5474 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/PythonAPICodes.py
+-rw-rw-rw-   0        0        0    13095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/RaisingCodes.py
+-rw-rw-rw-   0        0        0     3443 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/Reports.py
+-rw-rw-rw-   0        0        0     5234 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/ReturnCodes.py
+-rw-rw-rw-   0        0        0     6517 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/SetCodes.py
+-rw-rw-rw-   0        0        0    13949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/SliceCodes.py
+-rw-rw-rw-   0        0        0     9809 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/StringCodes.py
+-rw-rw-rw-   0        0        0     8188 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/SubscriptCodes.py
+-rw-rw-rw-   0        0        0    11176 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/TryCodes.py
+-rw-rw-rw-   0        0        0     3786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/TupleCodes.py
+-rw-rw-rw-   0        0        0    14717 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/VariableCodes.py
+-rw-rw-rw-   0        0        0     9121 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/VariableDeclarations.py
+-rw-rw-rw-   0        0        0     8099 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/YieldCodes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.221400 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/
+-rw-rw-rw-   0        0        0     6069 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeBases.py
+-rw-rw-rw-   0        0        0     3399 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-rw-rw-   0        0        0     1804 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-rw-rw-   0        0        0     1378 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-rw-rw-   0        0        0     3610 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-rw-rw-   0        0        0     5128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-rw-rw-   0        0        0     5211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-rw-rw-   0        0        0     3955 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-rw-rw-   0        0        0    19628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-rw-rw-   0        0        0     2852 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.246386 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/
+-rw-rw-rw-   0        0        0     2845 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-rw-rw-   0        0        0     5865 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-rw-rw-   0        0        0     2921 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-rw-rw-   0        0        0     2290 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-rw-rw-   0        0        0     6339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-rw-rw-   0        0        0     3321 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-rw-rw-   0        0        0     3306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-rw-rw-   0        0        0     2335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-rw-rw-   0        0        0     4217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-rw-rw-   0        0        0    21441 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-rw-rw-   0        0        0     6640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-rw-rw-   0        0        0     2475 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.767711 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/
+-rw-rw-rw-   0        0        0    11231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-rw-rw-   0        0        0     5847 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-rw-rw-   0        0        0    23760 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-rw-rw-   0        0        0     5238 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-rw-rw-   0        0        0     1843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-rw-rw-   0        0        0     2817 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-rw-rw-   0        0        0    12819 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-rw-rw-   0        0        0     2044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-rw-rw-   0        0        0     2762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-rw-rw-   0        0        0     1544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-rw-rw-   0        0        0     7197 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-rw-rw-   0        0        0    12850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-rw-rw-   0        0        0     4288 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-rw-rw-   0        0        0     2088 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-rw-rw-   0        0        0     2118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-rw-rw-   0        0        0     3933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-rw-rw-   0        0        0     7407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-rw-rw-   0        0        0     4292 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-rw-rw-   0        0        0     3860 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-rw-rw-   0        0        0     4487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-rw-rw-   0        0        0    11579 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-rw-rw-   0        0        0    19317 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-rw-rw-   0        0        0     2843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-rw-rw-   0        0        0     3635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-rw-rw-   0        0        0    11102 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-rw-rw-   0        0        0    15380 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-rw-rw-   0        0        0     2979 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-rw-rw-   0        0        0    10421 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-rw-rw-   0        0        0     2557 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-rw-rw-   0        0        0     3020 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-rw-rw-   0        0        0     2984 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-rw-rw-   0        0        0     3173 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.777706 Nuitka-winsvc-1.6.3/nuitka/containers/
+-rw-rw-rw-   0        0        0     1435 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/containers/Namedtuples.py
+-rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/containers/OrderedDicts.py
+-rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/containers/OrderedSets.py
+-rw-rw-rw-   0        0        0     4397 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/containers/OrderedSetsFallback.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.783702 Nuitka-winsvc-1.6.3/nuitka/distutils/
+-rw-rw-rw-   0        0        0     1964 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/distutils/Build.py
+-rw-rw-rw-   0        0        0    14219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/distutils/DistutilCommands.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/distutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.790701 Nuitka-winsvc-1.6.3/nuitka/finalizations/
+-rw-rw-rw-   0        0        0     1224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/finalizations/Finalization.py
+-rw-rw-rw-   0        0        0     6110 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/finalizations/FinalizeMarkups.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/finalizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.807716 Nuitka-winsvc-1.6.3/nuitka/freezer/
+-rw-rw-rw-   0        0        0     7311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/DependsExe.py
+-rw-rw-rw-   0        0        0     2584 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesCommon.py
+-rw-rw-rw-   0        0        0    10811 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesMacOS.py
+-rw-rw-rw-   0        0        0     7211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesPosix.py
+-rw-rw-rw-   0        0        0     6620 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesWin32.py
+-rw-rw-rw-   0        0        0    17336 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/IncludedDataFiles.py
+-rw-rw-rw-   0        0        0     9492 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/IncludedEntryPoints.py
+-rw-rw-rw-   0        0        0    10112 2023-06-16 02:32:36.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/Onefile.py
+-rw-rw-rw-   0        0        0    26319 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/Standalone.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/freezer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.817704 Nuitka-winsvc-1.6.3/nuitka/importing/
+-rw-rw-rw-   0        0        0    10934 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/importing/IgnoreListing.py
+-rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/importing/ImportCache.py
+-rw-rw-rw-   0        0        0     6455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/importing/ImportResolving.py
+-rw-rw-rw-   0        0        0    28463 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/importing/Importing.py
+-rw-rw-rw-   0        0        0     4738 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/importing/PreloadedPackages.py
+-rw-rw-rw-   0        0        0    16375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/importing/Recursion.py
+-rw-rw-rw-   0        0        0    10981 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/importing/StandardLibrary.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/importing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.960704 Nuitka-winsvc-1.6.3/nuitka/nodes/
+-rw-rw-rw-   0        0        0     3637 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/AsyncgenNodes.py
+-rw-rw-rw-   0        0        0     4082 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/AttributeLookupNodes.py
+-rw-rw-rw-   0        0        0    12004 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/AttributeNodes.py
+-rw-rw-rw-   0        0        0   378745 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/AttributeNodesGenerated.py
+-rw-rw-rw-   0        0        0     3823 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinAllNodes.py
+-rw-rw-rw-   0        0        0     4098 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinAnyNodes.py
+-rw-rw-rw-   0        0        0     2496 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinComplexNodes.py
+-rw-rw-rw-   0        0        0     1698 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-rw-rw-   0        0        0     4694 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinDictNodes.py
+-rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinFormatNodes.py
+-rw-rw-rw-   0        0        0     2142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinHashNodes.py
+-rw-rw-rw-   0        0        0     5334 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-rw-rw-   0        0        0    12723 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-rw-rw-   0        0        0     1996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinLenNodes.py
+-rw-rw-rw-   0        0        0     3606 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinNextNodes.py
+-rw-rw-rw-   0        0        0     3240 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinOpenNodes.py
+-rw-rw-rw-   0        0        0   245536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-rw-rw-   0        0        0    18589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinRangeNodes.py
+-rw-rw-rw-   0        0        0     9067 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinRefNodes.py
+-rw-rw-rw-   0        0        0     3307 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinSumNodes.py
+-rw-rw-rw-   0        0        0    13543 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinTypeNodes.py
+-rw-rw-rw-   0        0        0     1573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinVarsNodes.py
+-rw-rw-rw-   0        0        0    26113 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/BytesNodes.py
+-rw-rw-rw-   0        0        0     6478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/CallNodes.py
+-rw-rw-rw-   0        0        0     1550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/Checkers.py
+-rw-rw-rw-   0        0        0   605501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ChildrenHavingMixins.py
+-rw-rw-rw-   0        0        0     8448 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ClassNodes.py
+-rw-rw-rw-   0        0        0     6585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/CodeObjectSpecs.py
+-rw-rw-rw-   0        0        0    21683 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ComparisonNodes.py
+-rw-rw-rw-   0        0        0    30314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ConditionalNodes.py
+-rw-rw-rw-   0        0        0    46536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ConstantRefNodes.py
+-rw-rw-rw-   0        0        0    12213 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ContainerMakingNodes.py
+-rw-rw-rw-   0        0        0     2834 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ContainerOperationNodes.py
+-rw-rw-rw-   0        0        0     4581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/CoroutineNodes.py
+-rw-rw-rw-   0        0        0     1714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/CtypesNodes.py
+-rw-rw-rw-   0        0        0    51021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/DictionaryNodes.py
+-rw-rw-rw-   0        0        0     7856 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ExceptionNodes.py
+-rw-rw-rw-   0        0        0     8044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ExecEvalNodes.py
+-rw-rw-rw-   0        0        0    44996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ExpressionBases.py
+-rw-rw-rw-   0        0        0    45091 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-rw-rw-   0        0        0    21278 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ExpressionShapeMixins.py
+-rw-rw-rw-   0        0        0    12156 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/FrameNodes.py
+-rw-rw-rw-   0        0        0     3544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/FunctionAttributeNodes.py
+-rw-rw-rw-   0        0        0    39803 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/FunctionNodes.py
+-rw-rw-rw-   0        0        0     5376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/FutureSpecs.py
+-rw-rw-rw-   0        0        0     6256 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/GeneratorNodes.py
+-rw-rw-rw-   0        0        0     6850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-rw-rw-   0        0        0    74177 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/HardImportNodesGenerated.py
+-rw-rw-rw-   0        0        0     5511 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ImportHardNodes.py
+-rw-rw-rw-   0        0        0    45692 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ImportNodes.py
+-rw-rw-rw-   0        0        0     2733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/IndicatorMixins.py
+-rw-rw-rw-   0        0        0     1502 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/InjectCNodes.py
+-rw-rw-rw-   0        0        0    11228 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/IterationHandles.py
+-rw-rw-rw-   0        0        0    11002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/KeyValuePairNodes.py
+-rw-rw-rw-   0        0        0    16320 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ListOperationNodes.py
+-rw-rw-rw-   0        0        0    23094 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/LocalsDictNodes.py
+-rw-rw-rw-   0        0        0    14922 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/LocalsScopes.py
+-rw-rw-rw-   0        0        0    15581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/LoopNodes.py
+-rw-rw-rw-   0        0        0     1712 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/MatchNodes.py
+-rw-rw-rw-   0        0        0     6534 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ModuleAttributeNodes.py
+-rw-rw-rw-   0        0        0    30829 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ModuleNodes.py
+-rw-rw-rw-   0        0        0    24899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/NodeBases.py
+-rw-rw-rw-   0        0        0    15128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/NodeMakingHelpers.py
+-rw-rw-rw-   0        0        0     5550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/NodeMetaClasses.py
+-rw-rw-rw-   0        0        0    31894 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/OperatorNodes.py
+-rw-rw-rw-   0        0        0     9134 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/OperatorNodesUnary.py
+-rw-rw-rw-   0        0        0     4202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/OsSysNodes.py
+-rw-rw-rw-   0        0        0    12442 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/OutlineNodes.py
+-rw-rw-rw-   0        0        0    31330 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/PackageMetadataNodes.py
+-rw-rw-rw-   0        0        0     4464 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/PackageResourceNodes.py
+-rw-rw-rw-   0        0        0     3407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/PrintNodes.py
+-rw-rw-rw-   0        0        0     6772 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/ReturnNodes.py
+-rw-rw-rw-   0        0        0     4715 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/SideEffectNodes.py
+-rw-rw-rw-   0        0        0    12501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/SliceNodes.py
+-rw-rw-rw-   0        0        0    94880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/StatementBasesGenerated.py
+-rw-rw-rw-   0        0        0     9430 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/StatementNodes.py
+-rw-rw-rw-   0        0        0    28658 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/StrNodes.py
+-rw-rw-rw-   0        0        0     3504 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/StringConcatenationNodes.py
+-rw-rw-rw-   0        0        0     8640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/SubscriptNodes.py
+-rw-rw-rw-   0        0        0    17853 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/TryNodes.py
+-rw-rw-rw-   0        0        0     2405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/TypeMatchNodes.py
+-rw-rw-rw-   0        0        0    10911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/TypeNodes.py
+-rw-rw-rw-   0        0        0    39522 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/VariableAssignNodes.py
+-rw-rw-rw-   0        0        0    10746 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/VariableDelNodes.py
+-rw-rw-rw-   0        0        0     4574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/VariableNameNodes.py
+-rw-rw-rw-   0        0        0    30982 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/VariableRefNodes.py
+-rw-rw-rw-   0        0        0     4748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/VariableReleaseNodes.py
+-rw-rw-rw-   0        0        0     3902 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/YieldNodes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.966702 Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/
+-rw-rw-rw-   0        0        0   156243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-rw-rw-   0        0        0     4387 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/ShapeMixins.py
+-rw-rw-rw-   0        0        0    42374 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/StandardShapes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.979294 Nuitka-winsvc-1.6.3/nuitka/optimizations/
+-rw-rw-rw-   0        0        0     3279 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/BytecodeDemotion.py
+-rw-rw-rw-   0        0        0     3920 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/FunctionInlining.py
+-rw-rw-rw-   0        0        0     2144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/Graphs.py
+-rw-rw-rw-   0        0        0    10762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/Optimization.py
+-rw-rw-rw-   0        0        0    52154 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-rw-rw-   0        0        0     2272 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/Tags.py
+-rw-rw-rw-   0        0        0    40896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/TraceCollections.py
+-rw-rw-rw-   0        0        0    23977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/ValueTraces.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/optimizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.982295 Nuitka-winsvc-1.6.3/nuitka/pgo/
+-rw-rw-rw-   0        0        0     4663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/pgo/PGO.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/pgo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:27.985293 Nuitka-winsvc-1.6.3/nuitka/plugins/
+-rw-rw-rw-   0        0        0    40054 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/PluginBase.py
+-rw-rw-rw-   0        0        0    56200 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/Plugins.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.034293 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/
+-rw-rw-rw-   0        0        0    19004 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-rw-rw-   0        0        0     3460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-rw-rw-   0        0        0     9939 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-rw-rw-   0        0        0     4404 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DelvewheelPlugin.py
+-rw-rw-rw-   0        0        0     5675 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DillPlugin.py
+-rw-rw-rw-   0        0        0    13757 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-rw-rw-   0        0        0     2062 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/EnumPlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/EventletPlugin.py
+-rw-rw-rw-   0        0        0     1880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/GeventPlugin.py
+-rw-rw-rw-   0        0        0     3482 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/GiPlugin.py
+-rw-rw-rw-   0        0        0     5027 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/GlfwPlugin.py
+-rw-rw-rw-   0        0        0    18335 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/ImplicitImports.py
+-rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/KivyPlugin.py
+-rw-rw-rw-   0        0        0     7258 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-rw-rw-   0        0        0     6667 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-rw-rw-   0        0        0     1187 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/NumpyPlugin.py
+-rw-rw-rw-   0        0        0     6554 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-rw-rw-   0        0        0     1917 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PbrPlugin.py
+-rw-rw-rw-   0        0        0     4665 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-rw-rw-   0        0        0     6992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PmwPlugin.py
+-rw-rw-rw-   0        0        0    50023 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-rw-rw-   0        0        0     2933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-rw-rw-   0        0        0     1160 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-rw-rw-   0        0        0    12180 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TkinterPlugin.py
+-rw-rw-rw-   0        0        0     1140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TorchPlugin.py
+-rw-rw-rw-   0        0        0     9855 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TransformersPlugin.py
+-rw-rw-rw-   0        0        0     3175 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TrioPlugin.py
+-rw-rw-rw-   0        0        0     5640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/UpxPlugin.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/__init__.py
+-rw-rw-rw-   0        0        0   139710 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.052293 Nuitka-winsvc-1.6.3/nuitka/reports/
+-rw-rw-rw-   0        0        0     2209 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/reports/LicenseReport.rst.j2
+-rw-rw-rw-   0        0        0    17538 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/reports/Reports.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.066293 Nuitka-winsvc-1.6.3/nuitka/specs/
+-rw-rw-rw-   0        0        0     5911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-rw-rw-   0        0        0     2786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-rw-rw-   0        0        0     2541 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-rw-rw-   0        0        0    26455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinParameterSpecs.py
+-rw-rw-rw-   0        0        0     6065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-rw-rw-   0        0        0     4802 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-rw-rw-   0        0        0     5133 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/HardImportSpecs.py
+-rw-rw-rw-   0        0        0    18740 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/ParameterSpecs.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/specs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.068293 Nuitka-winsvc-1.6.3/nuitka/tools/
+-rw-rw-rw-   0        0        0     1603 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/Basics.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.069292 Nuitka-winsvc-1.6.3/nuitka/tools/commercial/
+-rw-rw-rw-   0        0        0      815 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/commercial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.073295 Nuitka-winsvc-1.6.3/nuitka/tools/data_composer/
+-rw-rw-rw-   0        0        0    14054 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/data_composer/DataComposer.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/data_composer/__init__.py
+-rw-rw-rw-   0        0        0     1306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/data_composer/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.077294 Nuitka-winsvc-1.6.3/nuitka/tools/environments/
+-rw-rw-rw-   0        0        0     2449 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/environments/CreateEnvironment.py
+-rw-rw-rw-   0        0        0     3735 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/environments/Virtualenv.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.078300 Nuitka-winsvc-1.6.3/nuitka/tools/general/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/general/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.080295 Nuitka-winsvc-1.6.3/nuitka/tools/general/dll_report/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/general/dll_report/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/general/dll_report/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.082294 Nuitka-winsvc-1.6.3/nuitka/tools/general/find_module/
+-rw-rw-rw-   0        0        0     3798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/general/find_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.085301 Nuitka-winsvc-1.6.3/nuitka/tools/onefile_compressor/
+-rw-rw-rw-   0        0        0    10194 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/onefile_compressor/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/onefile_compressor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.087296 Nuitka-winsvc-1.6.3/nuitka/tools/profiler/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/profiler/__init__.py
+-rw-rw-rw-   0        0        0     2529 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/profiler/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.093293 Nuitka-winsvc-1.6.3/nuitka/tools/scanning/
+-rw-rw-rw-   0        0        0     3344 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/scanning/DisplayPackageData.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/scanning/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.098294 Nuitka-winsvc-1.6.3/nuitka/tools/specialize/
+-rw-rw-rw-   0        0        0    51143 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-rw-rw-   0        0        0     7685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/specialize/Common.py
+-rw-rw-rw-   0        0        0    39625 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/specialize/SpecializeC.py
+-rw-rw-rw-   0        0        0    33585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/specialize/SpecializePython.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.6.3/nuitka/tools/specialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.108295 Nuitka-winsvc-1.6.3/nuitka/tools/testing/
+-rw-rw-rw-   0        0        0    55396 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/Common.py
+-rw-rw-rw-   0        0        0     1483 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/Constructs.py
+-rw-rw-rw-   0        0        0     8940 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/OutputComparison.py
+-rw-rw-rw-   0        0        0     1278 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/Pythons.py
+-rw-rw-rw-   0        0        0     7888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/RuntimeTracing.py
+-rw-rw-rw-   0        0        0     5371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/SearchModes.py
+-rw-rw-rw-   0        0        0     3375 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/Valgrind.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.110294 Nuitka-winsvc-1.6.3/nuitka/tools/testing/check_reference_counts/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.112293 Nuitka-winsvc-1.6.3/nuitka/tools/testing/compare_with_cpython/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-rw-rw-   0        0        0    29429 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.114294 Nuitka-winsvc-1.6.3/nuitka/tools/testing/find_sxs_modules/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.116294 Nuitka-winsvc-1.6.3/nuitka/tools/testing/measure_construct_performance/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-rw-rw-   0        0        0     8755 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.117293 Nuitka-winsvc-1.6.3/nuitka/tools/testing/run_nuitka_tests/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-rw-rw-   0        0        0    36321 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.119295 Nuitka-winsvc-1.6.3/nuitka/tools/watch/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/watch/__init__.py
+-rw-rw-rw-   0        0        0     9503 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tools/watch/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.164295 Nuitka-winsvc-1.6.3/nuitka/tree/
+-rw-rw-rw-   0        0        0    47126 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/Building.py
+-rw-rw-rw-   0        0        0    74608 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-rw-rw-   0        0        0     1700 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/Extractions.py
+-rw-rw-rw-   0        0        0     2572 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/InternalModule.py
+-rw-rw-rw-   0        0        0     1511 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/Operations.py
+-rw-rw-rw-   0        0        0     2807 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationAssertStatements.py
+-rw-rw-rw-   0        0        0    42768 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-rw-rw-   0        0        0     2948 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-rw-rw-   0        0        0    11693 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationCallExpressions.py
+-rw-rw-rw-   0        0        0    15072 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationClasses.py
+-rw-rw-rw-   0        0        0    37638 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationClasses3.py
+-rw-rw-rw-   0        0        0     6430 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-rw-rw-   0        0        0    22111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationContractionExpressions.py
+-rw-rw-rw-   0        0        0    11061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-rw-rw-   0        0        0    14607 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationExecStatements.py
+-rw-rw-rw-   0        0        0     7782 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationForLoopStatements.py
+-rw-rw-rw-   0        0        0    26215 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationFunctionStatements.py
+-rw-rw-rw-   0        0        0    13437 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationImportStatements.py
+-rw-rw-rw-   0        0        0     6577 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-rw-rw-   0        0        0    20962 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationMatchStatements.py
+-rw-rw-rw-   0        0        0     2409 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationMultidist.py
+-rw-rw-rw-   0        0        0     8194 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationNamespacePackages.py
+-rw-rw-rw-   0        0        0     4658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationPrintStatements.py
+-rw-rw-rw-   0        0        0    15371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationSequenceCreation.py
+-rw-rw-rw-   0        0        0     4824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-rw-rw-   0        0        0    14615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-rw-rw-   0        0        0     6982 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-rw-rw-   0        0        0     5674 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-rw-rw-   0        0        0    14341 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationWithStatements.py
+-rw-rw-rw-   0        0        0     3088 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationYieldExpressions.py
+-rw-rw-rw-   0        0        0    12746 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/SourceHandling.py
+-rw-rw-rw-   0        0        0     3757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/SyntaxErrors.py
+-rw-rw-rw-   0        0        0    22973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/TreeHelpers.py
+-rw-rw-rw-   0        0        0    20012 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/VariableClosure.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.198295 Nuitka-winsvc-1.6.3/nuitka/utils/
+-rw-rw-rw-   0        0        0     2655 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/AppDirs.py
+-rw-rw-rw-   0        0        0     3248 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/CStrings.py
+-rw-rw-rw-   0        0        0     3653 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/CommandLineOptions.py
+-rw-rw-rw-   0        0        0     4297 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Distributions.py
+-rw-rw-rw-   0        0        0     5794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Download.py
+-rw-rw-rw-   0        0        0    12376 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Execution.py
+-rw-rw-rw-   0        0        0    36129 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/FileOperations.py
+-rw-rw-rw-   0        0        0     2885 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Hashing.py
+-rw-rw-rw-   0        0        0     2362 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Images.py
+-rw-rw-rw-   0        0        0     6816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Importing.py
+-rw-rw-rw-   0        0        0     8149 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/InstalledPythons.py
+-rw-rw-rw-   0        0        0     2224 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/InstanceCounters.py
+-rw-rw-rw-   0        0        0     4336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Jinja2.py
+-rw-rw-rw-   0        0        0     1238 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Json.py
+-rw-rw-rw-   0        0        0     4304 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.6.3/nuitka/utils/MacOSApp.py
+-rw-rw-rw-   0        0        0     5040 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/MemoryUsage.py
+-rw-rw-rw-   0        0        0     9057 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/ModuleNames.py
+-rw-rw-rw-   0        0        0     4309 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/ReExecute.py
+-rw-rw-rw-   0        0        0     3815 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Rest.py
+-rw-rw-rw-   0        0        0    22714 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/SharedLibraries.py
+-rw-rw-rw-   0        0        0     3664 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Shebang.py
+-rw-rw-rw-   0        0        0     2591 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Signing.py
+-rw-rw-rw-   0        0        0     6207 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/StaticLibraries.py
+-rw-rw-rw-   0        0        0     2602 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/ThreadedExecutor.py
+-rw-rw-rw-   0        0        0     2772 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Timing.py
+-rw-rw-rw-   0        0        0    10826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Utils.py
+-rw-rw-rw-   0        0        0    10574 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/WindowsFileUsage.py
+-rw-rw-rw-   0        0        0    19540 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/WindowsResources.py
+-rw-rw-rw-   0        0        0     6108 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/Yaml.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/nuitka/utils/__init__.py
+-rw-rw-rw-   0        0        0      834 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 02:38:32.183413 Nuitka-winsvc-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0    15001 2023-06-16 02:32:36.000000 Nuitka-winsvc-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:28.204298 Nuitka-winsvc-1.6.3/tests/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.363625 Nuitka-winsvc-1.6.3/tests/basics/
+-rw-rw-rw-   0        0        0     1766 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/AssertsTest.py
+-rw-rw-rw-   0        0        0     5934 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/AssignmentsTest.py
+-rw-rw-rw-   0        0        0     5866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/AssignmentsTest32.py
+-rw-rw-rw-   0        0        0     4055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/BranchingTest.py
+-rw-rw-rw-   0        0        0     1104 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/BuiltinOverload.py
+-rw-rw-rw-   0        0        0     3749 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/BuiltinSuperTest.py
+-rw-rw-rw-   0        0        0    17080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/BuiltinsTest.py
+-rw-rw-rw-   0        0        0      866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ClassMinimalTest.py
+-rw-rw-rw-   0        0        0     4764 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ClassesTest.py
+-rw-rw-rw-   0        0        0     3414 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ClassesTest32.py
+-rw-rw-rw-   0        0        0     1406 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ClassesTest34.py
+-rw-rw-rw-   0        0        0     4698 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ComparisonChainsTest.py
+-rw-rw-rw-   0        0        0     4639 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ConstantsTest.py
+-rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ConstantsTest27.py
+-rw-rw-rw-   0        0        0     1628 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/DecoratorsTest.py
+-rw-rw-rw-   0        0        0     2317 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/DefaultParametersTest.py
+-rw-rw-rw-   0        0        0     1127 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/DoubleDeletionsTest.py
+-rw-rw-rw-   0        0        0      806 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/EmptyModuleTest.py
+-rw-rw-rw-   0        0        0    14387 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ExceptionRaisingTest.py
+-rw-rw-rw-   0        0        0      961 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ExceptionRaisingTest32.py
+-rw-rw-rw-   0        0        0     1458 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ExceptionRaisingTest33.py
+-rw-rw-rw-   0        0        0     6747 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ExecEvalTest.py
+-rw-rw-rw-   0        0        0     1417 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ExtremeClosureTest.py
+-rw-rw-rw-   0        0        0     1658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/FunctionObjectsTest.py
+-rw-rw-rw-   0        0        0    12335 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/FunctionsTest.py
+-rw-rw-rw-   0        0        0     3603 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/FunctionsTest32.py
+-rw-rw-rw-   0        0        0     2627 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/FunctionsTest_2.py
+-rw-rw-rw-   0        0        0      890 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/FutureTest32.py
+-rw-rw-rw-   0        0        0     5809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/GeneratorExpressionsTest.py
+-rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/GeneratorExpressionsTest_37.py
+-rw-rw-rw-   0        0        0     3824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/GlobalStatementTest.py
+-rw-rw-rw-   0        0        0     1286 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/HelloWorldTest_2.py
+-rw-rw-rw-   0        0        0     2469 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ImportingTest.py
+-rw-rw-rw-   0        0        0     1296 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/InplaceOperationsTest.py
+-rw-rw-rw-   0        0        0     4227 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/InspectionTest.py
+-rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/InspectionTest_35.py
+-rw-rw-rw-   0        0        0     1618 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/InspectionTest_36.py
+-rw-rw-rw-   0        0        0     1671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/LambdasTest.py
+-rw-rw-rw-   0        0        0     2731 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/LateClosureAssignmentTest.py
+-rw-rw-rw-   0        0        0     2923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ListContractionsTest.py
+-rw-rw-rw-   0        0        0     3329 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/LoopingTest.py
+-rw-rw-rw-   0        0        0     1536 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/MainProgramsTest.py
+-rw-rw-rw-   0        0        0     1925 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ModuleAttributesTest.py
+-rw-rw-rw-   0        0        0     1988 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/OperatorsTest.py
+-rw-rw-rw-   0        0        0    14903 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/OrderChecksTest.py
+-rw-rw-rw-   0        0        0     1827 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/OrderChecksTest27.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/OverflowFunctionsTest_2.py
+-rw-rw-rw-   0        0        0     5853 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ParameterErrorsTest.py
+-rw-rw-rw-   0        0        0     1899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ParameterErrorsTest32.py
+-rw-rw-rw-   0        0        0      863 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/PrintFutureTest.py
+-rw-rw-rw-   0        0        0     1413 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/PrintingTest_2.py
+-rw-rw-rw-   0        0        0      878 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/RecursionTest.py
+-rw-rw-rw-   0        0        0    23840 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest.py
+-rw-rw-rw-   0        0        0     2076 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest27.py
+-rw-rw-rw-   0        0        0     7819 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest33.py
+-rw-rw-rw-   0        0        0     4902 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest35.py
+-rw-rw-rw-   0        0        0     5092 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest36.py
+-rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest_2.py
+-rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/SlotsTest.py
+-rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/ThreadedGeneratorsTest.py
+-rw-rw-rw-   0        0        0    22966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TrickAssignmentsTest32.py
+-rw-rw-rw-   0        0        0     1541 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TrickAssignmentsTest35.py
+-rw-rw-rw-   0        0        0     1788 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TrickAssignmentsTest_2.py
+-rw-rw-rw-   0        0        0     2086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TryContinueFinallyTest.py
+-rw-rw-rw-   0        0        0     2212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TryExceptContinueTest.py
+-rw-rw-rw-   0        0        0     2275 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TryExceptFinallyTest.py
+-rw-rw-rw-   0        0        0     2304 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TryExceptFramesTest.py
+-rw-rw-rw-   0        0        0     2842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TryReturnFinallyTest.py
+-rw-rw-rw-   0        0        0     2328 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/TryYieldFinallyTest.py
+-rw-rw-rw-   0        0        0     1093 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/UnicodeTest.py
+-rw-rw-rw-   0        0        0     1877 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/UnpackingTest35.py
+-rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/VarargsTest.py
+-rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/WithStatementsTest.py
+-rw-rw-rw-   0        0        0     3070 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/YieldFromTest33.py
+-rw-rw-rw-   0        0        0     3821 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/run_all.py
+-rw-rw-rw-   0        0        0     2271 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/basics/run_xml.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.396629 Nuitka-winsvc-1.6.3/tests/onefile/
+-rw-rw-rw-   0        0        0     1213 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/onefile/HelloWorldTest.py
+-rw-rw-rw-   0        0        0     1307 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/onefile/KeyboardInterruptTest.py
+-rw-rw-rw-   0        0        0     5816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/onefile/run_all.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.502246 Nuitka-winsvc-1.6.3/tests/optimizations/
+-rw-rw-rw-   0        0        0      958 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/ArgumentTypes.py
+-rw-rw-rw-   0        0        0     1055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/Attributes.py
+-rw-rw-rw-   0        0        0     1021 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/Calls.py
+-rw-rw-rw-   0        0        0      921 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/Conditions.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/DecodingOperations.py
+-rw-rw-rw-   0        0        0     1212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/FormatStrings36.py
+-rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/HardImports.py
+-rw-rw-rw-   0        0        0      974 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/HardImports_2.py
+-rw-rw-rw-   0        0        0      918 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/Iterations.py
+-rw-rw-rw-   0        0        0     1260 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/Len.py
+-rw-rw-rw-   0        0        0     2262 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/Operations.py
+-rw-rw-rw-   0        0        0     1333 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/Subscripts.py
+-rw-rw-rw-   0        0        0     8736 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/optimizations/run_all.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.512246 Nuitka-winsvc-1.6.3/tests/packages/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.520246 Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/
+-rw-rw-rw-   0        0        0     2382 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.545244 Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/variable_package/
+-rw-rw-rw-   0        0        0      942 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-rw-rw-   0        0        0     1168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rw-rw-rw-   0        0        0     3671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/run_all.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.927253 Nuitka-winsvc-1.6.3/tests/packages/sub_package/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.808716 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/
+-rw-rw-rw-   0        0        0     1230 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/bigkitty.py
+-rw-rw-rw-   0        0        0      910 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/smallkitty.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.905716 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/
+-rw-rw-rw-   0        0        0      929 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/hello.py
+-rw-rw-rw-   0        0        0      966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/miau.py
+-rw-rw-rw-   0        0        0      968 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/purr.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.929250 Nuitka-winsvc-1.6.3/tests/packages/top_level_attributes_3/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.922717 Nuitka-winsvc-1.6.3/tests/packages/top_level_attributes_3/some_package/
+-rw-rw-rw-   0        0        0     2336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.935718 Nuitka-winsvc-1.6.3/tests/plugins/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.937722 Nuitka-winsvc-1.6.3/tests/plugins/code_signing/
+-rw-rw-rw-   0        0        0     1170 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/plugins/code_signing/CodeSigningMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.960739 Nuitka-winsvc-1.6.3/tests/plugins/data_files/
+-rw-rw-rw-   0        0        0     1332 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/plugins/data_files/DataFilesMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.969724 Nuitka-winsvc-1.6.3/tests/plugins/data_files/data_files_package/
+-rw-rw-rw-   0        0        0      924 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/plugins/data_files/data_files_package/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/tests/plugins/data_files/data_files_package/lala.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.970718 Nuitka-winsvc-1.6.3/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:29.987325 Nuitka-winsvc-1.6.3/tests/plugins/parameters/
+-rw-rw-rw-   0        0        0     1019 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/plugins/parameters/ParametersMain.py
+-rw-rw-rw-   0        0        0     2168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/plugins/parameters/parameter-using-plugin.py
+-rw-rw-rw-   0        0        0     3861 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/plugins/run_all.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.018326 Nuitka-winsvc-1.6.3/tests/programs/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.026325 Nuitka-winsvc-1.6.3/tests/programs/absolute_import/
+-rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.059269 Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/
+-rw-rw-rw-   0        0        0      796 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/foobar.py
+-rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/local.py
+-rw-rw-rw-   0        0        0      860 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/util.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.066269 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.074271 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path1/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.081270 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path1/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.088269 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path2/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path2/some_module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.097270 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path2/some_package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.100269 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.106281 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path1/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path1/some_module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.110275 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path1/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.113270 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path2/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.115270 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path2/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.122270 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/
+-rw-rw-rw-   0        0        0     1075 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.130270 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path1/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.137271 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path1/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.148270 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path2/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.156270 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path2/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.164271 Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.187271 Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.210272 Nuitka-winsvc-1.6.3/tests/programs/dash_import/
+-rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/dash_import/DashImportMain.py
+-rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/dash_import/dash-module.py
+-rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/dash_import/plus+module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.218272 Nuitka-winsvc-1.6.3/tests/programs/dash_main/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/dash_main/Dash-Main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.225272 Nuitka-winsvc-1.6.3/tests/programs/deep/
+-rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/deep/DeepProgramMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.245272 Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/
+-rw-rw-rw-   0        0        0      980 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/DeepBrother.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/DeepChild.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.262272 Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/deep_package/
+-rw-rw-rw-   0        0        0      876 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-rw-rw-   0        0        0      952 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/deep_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.269272 Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/
+-rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.285587 Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/package/
+-rw-rw-rw-   0        0        0      797 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-rw-rw-   0        0        0      857 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.294588 Nuitka-winsvc-1.6.3/tests/programs/import_variants/
+-rw-rw-rw-   0        0        0     1005 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/import_variants/ImportVariationsMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.343590 Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/
+-rw-rw-rw-   0        0        0      946 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/Child1.py
+-rw-rw-rw-   0        0        0     1098 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/Child2.py
+-rw-rw-rw-   0        0        0      822 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/Child3.py
+-rw-rw-rw-   0        0        0      994 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.368589 Nuitka-winsvc-1.6.3/tests/programs/main_raises/
+-rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/main_raises/ErrorMain.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/main_raises/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.393590 Nuitka-winsvc-1.6.3/tests/programs/main_raises2/
+-rw-rw-rw-   0        0        0     1080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/main_raises2/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.403600 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/
+-rw-rw-rw-   0        0        0     1529 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.430591 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.453590 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.471591 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.496168 Nuitka-winsvc-1.6.3/tests/programs/module_exits/
+-rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_exits/ErrorExitingModule.py
+-rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_exits/Main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.523167 Nuitka-winsvc-1.6.3/tests/programs/module_object_replacing/
+-rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-rw-rw-   0        0        0     1359 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.537167 Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/
+-rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.574195 Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/foo/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-rw-rw-   0        0        0      836 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-rw-rw-   0        0        0     1758 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/foo/entry.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.595195 Nuitka-winsvc-1.6.3/tests/programs/named_imports/
+-rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/named_imports/NamedImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.612195 Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.616195 Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/sub_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.622195 Nuitka-winsvc-1.6.3/tests/programs/package_code/
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_code/PackageInitCodeMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.638195 Nuitka-winsvc-1.6.3/tests/programs/package_code/some_package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_code/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_code/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.657196 Nuitka-winsvc-1.6.3/tests/programs/package_contains_main/
+-rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_contains_main/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_contains_main/local.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.678196 Nuitka-winsvc-1.6.3/tests/programs/package_init_import/
+-rw-rw-rw-   0        0        0      823 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_init_import/PackageInitImportMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.695196 Nuitka-winsvc-1.6.3/tests/programs/package_init_import/some_package/
+-rw-rw-rw-   0        0        0     1008 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_init_import/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.702196 Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/
+-rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.713196 Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.742197 Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/child_package/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-rw-rw-   0        0        0      795 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.756197 Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/
+-rw-rw-rw-   0        0        0      926 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.774197 Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/some_package/
+-rw-rw-rw-   0        0        0      965 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.783197 Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/some_package/sub_package/
+-rw-rw-rw-   0        0        0      977 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.814198 Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/
+-rw-rw-rw-   0        0        0      901 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.822826 Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/Something/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/Something/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/something.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.838827 Nuitka-winsvc-1.6.3/tests/programs/package_overload/
+-rw-rw-rw-   0        0        0      852 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_overload/Main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.868827 Nuitka-winsvc-1.6.3/tests/programs/package_overload/foo/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_overload/foo/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_overload/foo/bar.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_overload/foo/bar2.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.885828 Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/
+-rw-rw-rw-   0        0        0     2972 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.912830 Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/some_package/
+-rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:24.976253 Nuitka-winsvc-1.6.3/tests/programs/package_program/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.941830 Nuitka-winsvc-1.6.3/tests/programs/package_program/PackageAsMain/
+-rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/package_program/PackageAsMain/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.962832 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/
+-rw-rw-rw-   0        0        0     1728 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:30.973832 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.004601 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.027238 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.037230 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/
+-rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.064983 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-rw-rw-   0        0        0     1553 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.074985 Nuitka-winsvc-1.6.3/tests/programs/plugin_import/
+-rw-rw-rw-   0        0        0      859 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/plugin_import/PluginImportMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.100985 Nuitka-winsvc-1.6.3/tests/programs/plugin_import/some_package/
+-rw-rw-rw-   0        0        0      771 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/plugin_import/some_package/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/plugin_import/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.114985 Nuitka-winsvc-1.6.3/tests/programs/reimport_main_dynamic/
+-rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.128987 Nuitka-winsvc-1.6.3/tests/programs/reimport_main_static/
+-rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.145986 Nuitka-winsvc-1.6.3/tests/programs/relative_import/
+-rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/relative_import/RelativeImportMain.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/relative_import/dircache.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.162983 Nuitka-winsvc-1.6.3/tests/programs/resource_reader37/
+-rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.176986 Nuitka-winsvc-1.6.3/tests/programs/resource_reader37/some_package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.6.3/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/resource_reader37/some_package/__init__.py
+-rw-rw-rw-   0        0        0     6615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/run_all.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.198983 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/
+-rw-rw-rw-   0        0        0     1171 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/pyexpat.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.248984 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.277984 Nuitka-winsvc-1.6.3/tests/programs/syntax_errors/
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/syntax_errors/IndentationErroring.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-rw-rw-   0        0        0     1079 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.300984 Nuitka-winsvc-1.6.3/tests/programs/unicode_bom/
+-rw-rw-rw-   0        0        0      963 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/unicode_bom/unicode_bom.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.309781 Nuitka-winsvc-1.6.3/tests/programs/with space/
+-rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/programs/with space/Space Main.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.341799 Nuitka-winsvc-1.6.3/tests/reflected/
+-rw-rw-rw-   0        0        0    14061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/reflected/compile_itself.py
+-rw-rw-rw-   0        0        0     1243 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/run-tests
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.748987 Nuitka-winsvc-1.6.3/tests/standalone/
+-rw-rw-rw-   0        0        0     1058 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/BrotliUsing.py
+-rw-rw-rw-   0        0        0     2554 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/CtypesUsing.py
+-rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/FlaskUsing.py
+-rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/GlfwUsing.py
+-rw-rw-rw-   0        0        0     1184 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/GtkUsing.py
+-rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/HexEncodingTest_2.py
+-rw-rw-rw-   0        0        0     1086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/IdnaUsing.py
+-rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/LxmlUsing.py
+-rw-rw-rw-   0        0        0     1431 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/MatplotlibUsing.py
+-rw-rw-rw-   0        0        0     2538 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/MetadataPackagesUsing.py
+-rw-rw-rw-   0        0        0     1727 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/NumpyUsing.py
+-rw-rw-rw-   0        0        0      947 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/OpenGLUsing.py
+-rw-rw-rw-   0        0        0     1379 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PandasUsing.py
+-rw-rw-rw-   0        0        0     1066 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PasslibUsing.py
+-rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PendulumUsing.py
+-rw-rw-rw-   0        0        0     2074 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-rw-rw-   0        0        0     1067 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PmwUsing.py
+-rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PyQt5Plugins.py
+-rw-rw-rw-   0        0        0     1105 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PyQt5SSLSupport.py
+-rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PyQt5Using.py
+-rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PyQt6Plugins.py
+-rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PyQt6Using.py
+-rw-rw-rw-   0        0        0     1091 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PySide6Plugins.py
+-rw-rw-rw-   0        0        0     1757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/PySide6Using.py
+-rw-rw-rw-   0        0        0     1323 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/RsaUsing.py
+-rw-rw-rw-   0        0        0      973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/ShlibUsing.py
+-rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/SocketUsing.py
+-rw-rw-rw-   0        0        0     1941 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/TkInterUsing.py
+-rw-rw-rw-   0        0        0     3228 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/Urllib3Using.py
+-rw-rw-rw-   0        0        0     1200 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/Win32ComUsing.py
+-rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/run_all.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:31.762987 Nuitka-winsvc-1.6.3/tests/standalone/zip_importer/
+-rw-rw-rw-   0        0        0     1264 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/standalone/zip_importer/ZipImporterMain.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:38:32.181405 Nuitka-winsvc-1.6.3/tests/syntax/
+-rw-rw-rw-   0        0        0      811 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/AsyncgenReturn36.py
+-rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/BreakWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/ClassReturn.py
+-rw-rw-rw-   0        0        0      970 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/ClosureDel_2.py
+-rw-rw-rw-   0        0        0      849 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/ContinueWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/DuplicateArgument.py
+-rw-rw-rw-   0        0        0     1111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/ExecWithNesting_2.py
+-rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/FutureBraces.py
+-rw-rw-rw-   0        0        0      805 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/FutureUnknown.py
+-rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/GeneratorExpressions38.py
+-rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/GeneratorReturn_2.py
+-rw-rw-rw-   0        0        0      792 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/GlobalForParameter.py
+-rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/Importing32.py
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/IndentationError.py
+-rw-rw-rw-   0        0        0      915 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/LateFutureImport.py
+-rw-rw-rw-   0        0        0      841 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/MisplacedFutureImport.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/ModuleReturn.py
+-rw-rw-rw-   0        0        0      883 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/NonlocalForParameter32.py
+-rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/NonlocalNotFound32.py
+-rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/StarImportExtra.py
+-rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/SyntaxError.py
+-rw-rw-rw-   0        0        0      874 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/TryExceptAllNotLast.py
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/TryFinallyContinue_37.py
+-rw-rw-rw-   0        0        0      776 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/UnpackNoTuple.py
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/UnpackTwoStars32.py
+-rw-rw-rw-   0        0        0      793 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/YieldFromInModule.py
+-rw-rw-rw-   0        0        0      804 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/YieldInAsync35.py
+-rw-rw-rw-   0        0        0      923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/YieldInGenexp38.py
+-rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/YieldInModule.py
+-rw-rw-rw-   0        0        0     2203 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.6.3/tests/syntax/run_all.py
```

### Comparing `Nuitka-winsvc-1.6/Changelog.rst` & `Nuitka-winsvc-1.6.3/Changelog.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/Developer_Manual.rst` & `Nuitka-winsvc-1.6.3/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/LICENSE.txt` & `Nuitka-winsvc-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/MANIFEST.in` & `Nuitka-winsvc-1.6.3/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 include bin/autoformat-nuitka-source
 include bin/measure-construct-performance
 
 # Runners, mainly for source distribution.
 include bin/nuitka
 include bin/nuitka-run
 
-include misc/*.sh
 include misc/*.bat
 include tests/run-tests
 
 include nuitka/plugins/standard/*.yml
 
 # Logo with source
 include doc/Logo/Nuitka-Logo-Symbol.svg
```

### Comparing `Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/PKG-INFO` & `Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.6
+Version: 1.6.3
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-1.6/Nuitka_winsvc.egg-info/SOURCES.txt` & `Nuitka-winsvc-1.6.3/Nuitka_winsvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/PKG-INFO` & `Nuitka-winsvc-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.6
+Version: 1.6.3
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-1.6/README.md` & `Nuitka-winsvc-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/README.rst` & `Nuitka-winsvc-1.6.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -699,19 +699,19 @@
 
 If you have multiple programs, that each should be executable, in the
 past you had to compile multiple times, and deploy all of these. With
 standalone mode, this of course meant that you were fairly wasteful, as
 sharing the folders could be done, but wasn't really supported by
 Nuitka.
 
-Enter ``Multidist``. There is an option ``--main-path`` that replaces or
-adds to the positional argument given. And it can be given multiple
-times. When given multiple times, Nuitka will create a binary that
-contains the code of all the programs given, but sharing modules used in
-them. They therefore do not have to be distributed multiple times.
+Enter ``Multidist``. There is an option ``--main`` that replaces or adds
+to the positional argument given. And it can be given multiple times.
+When given multiple times, Nuitka will create a binary that contains the
+code of all the programs given, but sharing modules used in them. They
+therefore do not have to be distributed multiple times.
 
 Lets call the basename of the main path, and entry point. The names of
 these must of course be different. Then the created binary can execute
 either entry point, and will react to what ``sys.argv[0]`` appears to
 it. So if executed in the right way (with something like ``subprocess``
 or OS API you can control this name), or by renaming or copying the
 binary, or symlinking to it, you can then achieve the miracle.
```

### Comparing `Nuitka-winsvc-1.6/bin/autoformat-nuitka-source` & `Nuitka-winsvc-1.6.3/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/bin/check-nuitka-with-pylint` & `Nuitka-winsvc-1.6.3/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/bin/compare_with_cpython` & `Nuitka-winsvc-1.6.3/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/bin/compare_with_xml` & `Nuitka-winsvc-1.6.3/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/bin/measure-construct-performance` & `Nuitka-winsvc-1.6.3/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/bin/nuitka` & `Nuitka-winsvc-1.6.3/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/bin/nuitka-run` & `Nuitka-winsvc-1.6.3/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-winsvc-1.6.3/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-winsvc-1.6.3/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-winsvc-1.6.3/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-winsvc-1.6.3/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-winsvc-1.6.3/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-winsvc-1.6.3/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/lib/hints.py` & `Nuitka-winsvc-1.6.3/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/misc/nuitka-run.bat` & `Nuitka-winsvc-1.6.3/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/misc/nuitka.bat` & `Nuitka-winsvc-1.6.3/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Builtins.py` & `Nuitka-winsvc-1.6.3/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/BytecodeCaching.py` & `Nuitka-winsvc-1.6.3/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Bytecodes.py` & `Nuitka-winsvc-1.6.3/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/CacheCleanup.py` & `Nuitka-winsvc-1.6.3/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Constants.py` & `Nuitka-winsvc-1.6.3/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Errors.py` & `Nuitka-winsvc-1.6.3/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/MainControl.py` & `Nuitka-winsvc-1.6.3/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/ModuleRegistry.py` & `Nuitka-winsvc-1.6.3/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/OptionParsing.py` & `Nuitka-winsvc-1.6.3/nuitka/OptionParsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,21 @@
 
 parser.add_option(
     "--main",
     action="append",
     dest="mains",
     metavar="PATH",
     default=[],
-    help=SUPPRESS_HELP,
+    help="""\
+If specified once, this takes the place of the
+positional argument, i.e. the filename to compile.
+When given multiple times, it enables "multidist"
+(see User Manual) it allows you to create binaries
+that depending on file name or invocation name.
+""",
 )
 
 include_group = parser.add_option_group(
     "Control the inclusion of modules and packages in result"
 )
 
 include_group.add_option(
```

### Comparing `Nuitka-winsvc-1.6/nuitka/Options.py` & `Nuitka-winsvc-1.6.3/nuitka/Options.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,15 +649,19 @@
 might be missing required packages. Disable with --static-libpython=no" if you don't \
 want to install it."""
         )
 
     if isApplePython():
         if isStandaloneMode():
             Tracing.options_logger.sysexit(
-                "Error, for standalone mode, Apple Python from macOS is not supported, use e.g. CPython instead."
+                """\
+Error, on macOS, for standalone mode, Apple Python is not supported \
+due to being tied to specific OS releases, use e.g. CPython instead \
+which is available from https://www.python.org/downloads/macos/ for \
+download. With that, your program will work on macOS 10.9 or higher."""
             )
 
         if str is bytes:
             Tracing.options_logger.sysexit(
                 "Error, Apple Python 2.7 from macOS is not usable as per Apple decision, use e.g. CPython 2.7 instead."
             )
```

### Comparing `Nuitka-winsvc-1.6/nuitka/OutputDirectories.py` & `Nuitka-winsvc-1.6.3/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/PostProcessing.py` & `Nuitka-winsvc-1.6.3/nuitka/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Progress.py` & `Nuitka-winsvc-1.6.3/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/PythonFlavors.py` & `Nuitka-winsvc-1.6.3/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/PythonOperators.py` & `Nuitka-winsvc-1.6.3/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/PythonVersions.py` & `Nuitka-winsvc-1.6.3/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Serialization.py` & `Nuitka-winsvc-1.6.3/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/SourceCodeReferences.py` & `Nuitka-winsvc-1.6.3/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Tracing.py` & `Nuitka-winsvc-1.6.3/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/TreeXML.py` & `Nuitka-winsvc-1.6.3/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Variables.py` & `Nuitka-winsvc-1.6.3/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/Version.py` & `Nuitka-winsvc-1.6.3/nuitka/Version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V1.6
+Nuitka V1.6.3
 Copyright (C) 2023 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-winsvc-1.6/nuitka/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/__past__.py` & `Nuitka-winsvc-1.6.3/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/Backend.scons` & `Nuitka-winsvc-1.6.3/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/CCompilerVersion.scons` & `Nuitka-winsvc-1.6.3/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/DataComposerInterface.py` & `Nuitka-winsvc-1.6.3/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/Onefile.scons` & `Nuitka-winsvc-1.6.3/nuitka/build/Onefile.scons`

 * *Files 1% similar despite different names*

```diff
@@ -455,14 +455,24 @@
             sub_path="OnefileBootstrap.c",
             nuitka_src=nuitka_src,
             source_dir=source_dir,
             c11_mode=env.c11_mode,
         )
     )
 
+    if onefile_splash_screen:
+        result.append(
+            provideStaticSourceFile(
+                sub_path="OnefileSplashScreen.cpp",
+                nuitka_src=nuitka_src,
+                source_dir=source_dir,
+                c11_mode=False,
+            )
+        )
+
     return result
 
 
 source_files = discoverSourceFiles()
 
 target = env.Program(result_exe, source_files)
```

### Comparing `Nuitka-winsvc-1.6/nuitka/build/SconsCaching.py` & `Nuitka-winsvc-1.6.3/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/SconsCompilerSettings.py` & `Nuitka-winsvc-1.6.3/nuitka/build/SconsCompilerSettings.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,17 @@
         elif env.msvc_mode:
             env.Append(CCFLAGS=["/std:c11"])
 
     if env.msvc_mode and c11_mode:
         # Windows SDK shows this even in non-debug mode in C11 mode.
         env.Append(CCFLAGS=["/wd5105"])
 
+    if not c11_mode:
+        env.Append(CPPDEFINES=["_NUITKA_NON_C11_MODE"])
+
     scons_details_logger.info("Using C11 mode: %s" % c11_mode)
 
     env.c11_mode = c11_mode
 
 
 def _enableLtoSettings(
     env,
@@ -236,14 +239,17 @@
 
     env.lto_mode = lto_mode
 
     # PGO configuration
     _enablePgoSettings(env, pgo_mode)
 
 
+_python311_min_msvc_version = (14, 3)
+
+
 def checkWindowsCompilerFound(
     env, target_arch, clang_mode, msvc_version, assume_yes_for_downloads
 ):
     """Remove compiler of wrong arch or too old gcc and replace with downloaded winlibs gcc."""
     # Many cases to deal with, pylint: disable=too-many-branches
 
     if os.name == "nt":
@@ -320,14 +326,35 @@
                     % (msvc_version, getMsvcVersionString(env))
                 )
 
                 # This will trigger error exit in branch below.
                 compiler_path = None
                 env["CC"] = None
 
+        # For Python3.11
+        if compiler_path is not None:
+            if (
+                # This is actually OK to use like this, pylint: disable=bad-chained-comparison
+                None is not env.python_version >= (3, 11)
+                and getMsvcVersion(env) < _python311_min_msvc_version
+            ):
+                scons_logger.info(
+                    """\
+For Python version %s MSVC %s or later is required, not %s which is too old."""
+                    % (
+                        ".".join(str(d) for d in env.python_version),
+                        ".".join(str(d) for d in _python311_min_msvc_version),
+                        getMsvcVersionString(env),
+                    )
+                )
+
+                # This will trigger error exit in branch below.
+                compiler_path = None
+                env["CC"] = None
+
         if compiler_path is not None:
             the_cc_name = os.path.basename(compiler_path)
 
             if isGccName(the_cc_name):
                 gcc_version = myDetectVersion(env, compiler_path)
 
                 min_version = (11, 2)
```

### Comparing `Nuitka-winsvc-1.6/nuitka/build/SconsHacks.py` & `Nuitka-winsvc-1.6.3/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/SconsInterface.py` & `Nuitka-winsvc-1.6.3/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/SconsProgress.py` & `Nuitka-winsvc-1.6.3/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/SconsSpawn.py` & `Nuitka-winsvc-1.6.3/nuitka/build/SconsSpawn.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         return self.data, self.err, self.exit_code, self.exception
 
 
 def runProcessMonitored(cmdline, env):
     thread = SubprocessThread(cmdline, env)
     thread.start()
 
-    # Allow a minute before warning for long compile time.
-    thread.join(60)
+    # Allow 5 minutes before warning for long compile time.
+    thread.join(360)
 
     if thread.is_alive():
         reportSlowCompilation(cmdline, thread.timer_report.getTimer().getDelta())
 
     thread.join()
 
     updateSconsProgressBar()
@@ -342,16 +342,16 @@
         return self.result, self.exception
 
 
 def runSpawnMonitored(sh, cmd, args, env):
     thread = SpawnThread(sh, cmd, args, env)
     thread.start()
 
-    # Allow a minute before warning for long compile time.
-    thread.join(60)
+    # Allow 5 minutes before warning for long compile time.
+    thread.join(360)
 
     if thread.is_alive():
         reportSlowCompilation(cmd, thread.timer_report.getTimer().getDelta())
 
     thread.join()
 
     updateSconsProgressBar()
```

### Comparing `Nuitka-winsvc-1.6/nuitka/build/SconsUtils.py` & `Nuitka-winsvc-1.6.3/nuitka/build/SconsUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,16 +595,14 @@
 def getMsvcVersionString(env):
     import SCons.Tool.MSCommon.vc  # pylint: disable=I0021,import-error
 
     return SCons.Tool.MSCommon.vc.get_default_version(env)
 
 
 def getMsvcVersion(env):
-    assert env.msvc_mode
-
     value = getMsvcVersionString(env)
 
     # TODO: Workaround for prompt being used.
     if value is None:
         value = os.environ.get("VCToolsVersion", "14.3").rsplit(".", 1)[0]
 
     value = value.replace("exp", "")
@@ -733,22 +731,22 @@
 
 def raiseNoCompilerFoundErrorExit():
     if os.name == "nt":
         scons_logger.sysexit(
             """\
 Error, cannot locate suitable C compiler. You have the following options:
 
-a) If a suitable Visual Studio version is installed, it will be located
-   automatically via registry. But not if you activate the wrong prompt.
-
-b) Using --mingw64 lets Nuitka download MinGW64 for you.
-
-Note: MinGW64 is the name, it does *not* mean 64 bits, just a gcc with
-better Windows compatibility, it is available for 32 and 64 bits. Cygwin
-based gcc do not work.
+a) If a suitable Visual Studio version is installed (check above trace
+   outputs for rejection messages), it will be located automatically via
+   registry. But not if you activate the wrong prompt.
+
+b) Using "--mingw64" lets Nuitka download MinGW64 for you. Note: MinGW64
+   is the project name, it does *not* mean 64 bits, just a gcc with better
+   Windows compatibility, it is available for 32 and 64 bits. Cygwin based
+   gcc e.g. do not work.
 """
         )
     else:
         scons_logger.sysexit("Error, cannot locate suitable C compiler.")
 
 
 def addBinaryBlobSection(env, blob_filename, section_name):
```

### Comparing `Nuitka-winsvc-1.6/nuitka/build/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/allocator.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/builtins.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/calling.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/checkers.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/constants.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/freelists.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/hedley.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/helpers.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/importing.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/incbin.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/prelude.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/printing.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/threading.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/tracing.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-winsvc-1.6.3/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/gui.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-winsvc-1.6.3/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersImport.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersLists.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/MainProgram.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/MainProgram.c`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 #define environment_char_t wchar_t
 
 static environment_char_t const *getEnvironmentVariable(char const *name) {
     // Max size for environment variables according to docs.
     wchar_t buffer[32768];
     buffer[0] = 0;
 
-    wchar_t name_wide[20];
+    wchar_t name_wide[40];
     name_wide[0] = 0;
     appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
 
     // Size must be in bytes apparently, not in characters. Cannot be larger anyway.
     DWORD res = GetEnvironmentVariableW(name_wide, buffer, 65536);
 
     if (res == 0 || res > sizeof(buffer)) {
@@ -125,26 +125,26 @@
     return wcsdup(buffer);
 }
 
 static void setEnvironmentVariable(char const *name, environment_char_t const *value) {
     assert(name != NULL);
     assert(value != NULL);
 
-    wchar_t name_wide[20];
+    wchar_t name_wide[40];
     name_wide[0] = 0;
     appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
 
     DWORD res = SetEnvironmentVariableW(name_wide, value);
     assert(wcscmp(getEnvironmentVariable(name), value) == 0);
 
     assert(res != 0);
 }
 
 static void unsetEnvironmentVariable(char const *name) {
-    wchar_t name_wide[20];
+    wchar_t name_wide[40];
     name_wide[0] = 0;
     appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
 
     DWORD res = SetEnvironmentVariableW(name_wide, NULL);
 
     assert(res != 0);
 }
```

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files 1% similar despite different names*

```diff
@@ -812,26 +812,33 @@
     }
 }
 
 #else
 void ourConsoleCtrlHandler(int sig) { cleanupChildProcess(false); }
 #endif
 
-#if _NUITKA_ONEFILE_SPLASH_SCREEN
-#include "OnefileSplashScreen.cpp"
-#endif
-
 #if _NUITKA_AUTO_UPDATE_BOOL && !defined(__IDE_ONLY__)
 #include "nuitka_onefile_auto_updater.h"
 #endif
 
 #if _NUITKA_AUTO_UPDATE_BOOL
 extern bool exe_file_updatable;
 #endif
 
+#ifdef _NUITKA_ONEFILE_SPLASH_SCREEN
+#ifdef __cplusplus
+extern "C" {
+#endif
+extern void initSplashScreen(void);
+extern bool checkSplashScreen(void);
+#ifdef __cplusplus
+}
+#endif
+#endif
+
 #ifdef _NUITKA_WINMAIN_ENTRY_POINT
 int __stdcall wWinMain(HINSTANCE hInstance, HINSTANCE hPrevInstance, wchar_t *lpCmdLine, int nCmdShow) {
     int argc = __argc;
     wchar_t **argv = __wargv;
 #else
 #if defined(_WIN32)
 #ifdef _NUITKA_WINSVC_BOOL
```

### Comparing `Nuitka-winsvc-1.6/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-winsvc-1.6.3/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,32 @@
 //     distributed under the License is distributed on an "AS IS" BASIS,
 //     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //     See the License for the specific language governing permissions and
 //     limitations under the License.
 //
 // Creates a stream object initialized with the data from an executable resource.
 
-#ifdef __IDE_ONLY__
-#include "HelpersSafeStrings.c"
-#include "nuitka/tracing.h"
-#include <windows.h>
+#ifdef __MINGW32__
+#error "No support for splash screens with MinGW64 yet, only works with MSVC. Somebody please make it portable."
 #endif
 
-#include <assert.h>
+#include <shlwapi.h>
 #include <wincodec.h>
+#include <windows.h>
 
-#ifdef __MINGW32__
-#error "No support for splash screens with MinGW64 yet, only works with MSVC. Somebody please make it portable."
-#endif
+#include <assert.h>
 
+#ifndef _NUITKA_NON_C11_MODE
+extern "C" {
+#endif
+#include "nuitka/safe_string_ops.h"
+#include "nuitka/tracing.h"
+#ifndef _NUITKA_NON_C11_MODE
+};
+#endif
 IStream *createImageStream(void) {
 
     // Load the resource with image data
     HRSRC res_handle = FindResource(NULL, MAKEINTRESOURCE(28), RT_RCDATA);
     if (res_handle == NULL) {
         return NULL;
     }
@@ -187,15 +192,15 @@
     return splash_window;
 }
 
 HWND splash_window = 0;
 static wchar_t splash_indicator_path[4096] = {0};
 bool splash_active = false;
 
-static void initSplashScreen(void) {
+extern "C" void initSplashScreen(void) {
     CoInitialize(NULL);
     IStream *image_stream = createImageStream();
     if (image_stream == NULL) {
         return;
     }
     IWICBitmapSource *image_source = getBitmapFromImageStream(image_stream);
     image_stream->Release();
@@ -229,15 +234,15 @@
 static void closeSplashScreen(void) {
     if (splash_window) {
         DestroyWindow(splash_window);
         splash_window = 0;
     }
 }
 
-static bool checkSplashScreen(void) {
+extern "C" bool checkSplashScreen(void) {
     if (splash_active) {
         if (!PathFileExistsW(splash_indicator_path)) {
             closeSplashScreen();
             splash_active = false;
         }
     }
```

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/AttributeCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/BranchCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/CallCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ClassCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/CodeGeneration.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/CodeHelpers.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ConstantCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/Contexts.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/CtypesCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/DictCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/Emission.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ErrorCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/EvalCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/FrameCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/FunctionCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/GlobalConstants.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/IdCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ImportCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/Indentation.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/IndexCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/InjectCCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/IntegerCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/IteratorCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/LabelCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ListCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/LoaderCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/LoopCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/MatchCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ModuleCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/Namify.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/OperationCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/PrintCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/RaisingCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/Reports.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/ReturnCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/SetCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/SliceCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/StringCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/TryCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/TupleCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/VariableCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/YieldCodes.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/c_types/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-winsvc-1.6.3/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/containers/Namedtuples.py` & `Nuitka-winsvc-1.6.3/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/containers/OrderedDicts.py` & `Nuitka-winsvc-1.6.3/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/containers/OrderedSets.py` & `Nuitka-winsvc-1.6.3/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-winsvc-1.6.3/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/containers/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/distutils/Build.py` & `Nuitka-winsvc-1.6.3/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/distutils/DistutilCommands.py` & `Nuitka-winsvc-1.6.3/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/distutils/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/finalizations/Finalization.py` & `Nuitka-winsvc-1.6.3/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-winsvc-1.6.3/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/finalizations/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/DependsExe.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/Onefile.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/Standalone.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/freezer/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/IgnoreListing.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/ImportCache.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/ImportResolving.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/Importing.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/PreloadedPackages.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/Recursion.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/StandardLibrary.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/StandardLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,18 +267,20 @@
     "_hashlib",
     "secrets",
     "hmac",
     "fractions",
     "decimal",
     "_pydecimal",
     "_decimal",
+    "statistics",
     "lzma",
     "_lzma",
     "bz2",
     "_bz2",
+    "logging",
     "subprocess",
     "socket",
     "selectors",
     "select",
     "_socket",
     "ssl",
     "_ssl",
```

### Comparing `Nuitka-winsvc-1.6/nuitka/importing/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/AttributeNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/BytesNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/CallNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/Checkers.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ClassNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ComparisonNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ConditionalNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/CoroutineNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/CtypesNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/DictionaryNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ExceptionNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ExpressionBases.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/FrameNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/FunctionNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/FutureSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/GeneratorNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ImportHardNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ImportNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/IndicatorMixins.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/InjectCNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/IterationHandles.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ListOperationNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/LocalsScopes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/LoopNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/MatchNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ModuleNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/NodeBases.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/OperatorNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/OsSysNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/OutlineNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/PrintNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/ReturnNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/SideEffectNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/SliceNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/StatementNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/StrNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/SubscriptNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/TryNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/TypeNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/VariableDelNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/VariableNameNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/VariableRefNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/YieldNodes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/nodes/shapes/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/FunctionInlining.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/Graphs.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/Optimization.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/Tags.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/TraceCollections.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/ValueTraces.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/optimizations/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/pgo/PGO.py` & `Nuitka-winsvc-1.6.3/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/pgo/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/PluginBase.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/PluginBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     shallCreateAppBundle,
     shallMakeModule,
     shallShowExecutedCommands,
 )
 from nuitka.PythonFlavors import isAnacondaPython, isDebianPackagePython
 from nuitka.PythonVersions import getSupportedPythonVersions, python_version
 from nuitka.Tracing import plugins_logger
+from nuitka.utils.Distributions import isDistributionCondaPackage
 from nuitka.utils.Execution import NuitkaCalledProcessError, check_output
 from nuitka.utils.ModuleNames import (
     ModuleName,
     makeTriggerModuleName,
     post_module_load_trigger_name,
     pre_module_load_trigger_name,
 )
@@ -1105,14 +1106,15 @@
 
         context.update(
             {
                 "macos": isMacOS(),
                 "win32": isWin32Windows(),
                 "linux": isLinux(),
                 "anaconda": isAnacondaPython(),
+                "is_conda_package": isDistributionCondaPackage,
                 "debian_python": isDebianPackagePython(),
                 "standalone": isStandaloneMode(),
                 "module_mode": shallMakeModule(),
                 # TODO: Allow to provide this.
                 "deployment": False,
                 # Querying package versions.
                 "version": _getPackageVersion,
```

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/Plugins.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,16 @@
                 self.sysexit(
                     "Error, illegal mode given '%s' in '--noinclude-custom-mode=%s'"
                     % (mode, custom_choice)
                 )
 
             self.handled_modules[ModuleName(module_name)] = mode
 
+        self.warnings_given = set()
+
     def getCacheContributionValues(self, module_name):
         config = self.config.get(module_name, section="anti-bloat")
 
         if config:
             yield str(config)
 
     @classmethod
@@ -467,24 +469,31 @@
                         using_module is None
                         or not using_module.getFullName().hasNamespace(
                             handled_module_name
                         )
                     )
                     and source_ref is not None
                 ):
-
-                    self.warning(
-                        "Undesirable import of '%s' in '%s' (at '%s') encountered. It may slow down compilation."
-                        % (
-                            handled_module_name,
-                            using_module.getFullName(),
-                            source_ref.getAsString(),
-                        ),
-                        mnemonic="unwanted-module",
+                    key = (
+                        handled_module_name,
+                        using_module,
+                        source_ref.getLineNumber(),
                     )
+                    if key not in self.warnings_given:
+                        self.warning(
+                            "Undesirable import of '%s' in '%s' (at '%s') encountered. It may slow down compilation."
+                            % (
+                                handled_module_name,
+                                using_module.getFullName(),
+                                source_ref.getAsString(),
+                            ),
+                            mnemonic="unwanted-module",
+                        )
+
+                        self.warnings_given.add(key)
 
     def onModuleEncounter(self, module_name, module_filename, module_kind):
         for handled_module_name, mode in self.handled_modules.items():
             if module_name.hasNamespace(handled_module_name):
                 # Either issue a warning, or pretend the module doesn't exist for standalone or
                 # at least will not be included.
                 if mode == "nofollow":
```

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
-""" Support for pyzmq, details in below class definitions.
+""" Support for delvewheel, details in below class definitions.
 
 """
 
 import os
 import re
 
 from nuitka import Options
 from nuitka.plugins.PluginBase import NuitkaPluginBase
+from nuitka.PythonFlavors import isAnacondaPython
 from nuitka.utils.FileOperations import getFileList
 
-# spell-checker: ignore delvewheel,pyzmq
+# spell-checker: ignore delvewheel
 
 
 class NuitkaPluginDelvewheel(NuitkaPluginBase):
     """This class represents the main logic of the delvewheel plugin.
 
     This is a plugin to ensure that delvewheel DLLs are loading properly in
     standalone mode. This needed to include the correct DLLs to the correct
@@ -74,41 +75,46 @@
         )
 
         if not match:
             return None
 
         delvewheel_version = match.group(2).replace("_", ".")
 
-        self.info(
-            "Detected usage of 'delvewheel' version '%s' in module '%s'."
-            % (delvewheel_version, module_name.asString())
-        )
-
         code = match.group(1)
 
         code = code.replace("os.add_dll_directory", "add_dll_directory")
         code = code.replace("sys.version_info[:2] >= (3, 8)", "True")
+        code = code.replace("sys.version_info[:2] >= (3, 10)", "True")
 
         self.dll_directory = None
 
         # Fake the "__file__" to the proper value to the exec.
         exec_globals = {
             "__file__": self.locateModule(module_name) + "\\__init__.py",
             "add_dll_directory": self._add_dll_directory,
         }
 
         self.dll_directory = None
 
         # We believe this should be the easiest, pylint: disable=exec-used
         exec(code, exec_globals)
 
-        # Copy it over.
-        assert self.dll_directory is not None, module_name
+        # Copy it over. For Anaconda we allow exceptions, when it's not an
+        # Anaconda package, but a PyPI package, those mixes are acting strange.
+        if not isAnacondaPython():
+            assert self.dll_directory is not None, module_name
+
         self.dll_directories[module_name] = self.dll_directory
 
+        if self.dll_directories[module_name]:
+            self.info(
+                "Detected usage of 'delvewheel' version '%s' in module '%s'."
+                % (delvewheel_version, module_name.asString())
+            )
+
     def getExtraDlls(self, module):
         full_name = module.getFullName()
 
         dll_directory = self.dll_directories.get(full_name)
 
         if dll_directory is not None:
             for dll_filename in getFileList(dll_directory):
```

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/ImplicitImports.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,16 @@
                 yield crypto_module_name + ".Cipher._Salsa20"
 
             elif full_name == crypto_module_name + ".Cipher.ChaCha20":
                 yield crypto_module_name + ".Cipher._chacha20"
 
             elif full_name == crypto_module_name + ".PublicKey.ECC":
                 yield crypto_module_name + ".PublicKey._ec_ws"
+                yield crypto_module_name + ".PublicKey._ed25519"
+                yield crypto_module_name + ".PublicKey._ed448"
 
             elif full_name == crypto_module_name + ".Cipher.ARC4":
                 yield crypto_module_name + ".Cipher._ARC4"
 
             elif full_name == crypto_module_name + ".Cipher.PKCS1_v1_5":
                 yield crypto_module_name + ".Cipher._pkcs1_decode"
```

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
                 "lib/QtWebEngineCore.framework/Resources",
             )
         else:
             return os.path.join(self._getQtInformation().data_path, "resources")
 
     def _getWebEngineExecutablePath(self):
         """Get the path to QtWebEngine binary."""
-        return self._getQtInformation().library_executables_path
+        return os.path.normpath(self._getQtInformation().library_executables_path)
 
     def getQtPluginDirs(self):
         if self.qt_plugins_dirs is not None:
             return self.qt_plugins_dirs
 
         qt_info = self._getQtInformation()
 
@@ -838,16 +838,16 @@
 
         qt_web_engine_dir = self._getWebEngineExecutablePath()
 
         for filename, filename_relative in listDir(qt_web_engine_dir):
             if filename_relative.startswith("QtWebEngineProcess"):
                 yield self.makeExeEntryPoint(
                     source_path=filename,
-                    dest_path=os.path.join(
-                        self._getWebEngineTargetDir(), filename_relative
+                    dest_path=os.path.normpath(
+                        os.path.join(self._getWebEngineTargetDir(), filename_relative)
                     ),
                     package_name=full_name,
                     reason="needed by '%s'" % full_name.asString(),
                 )
 
                 break
         else:
```

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/TransformersPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,20 @@
     - description: 'remove pywin32 reference'
       replacements_plain:
         'import win32com.shell': 'raise ImportError'
       change_function:
         '_get_win_folder_with_pywin32': 'un-callable'
       when: 'not use_pywin32 or not win32'
 
+- module-name: 'apscheduler'
+  implicit-imports:
+    - depends:
+        - 'apscheduler.triggers.*'
+        - 'apscheduler.triggers.*.*'
+
 - module-name: 'apsw'
   implicit-imports:
     - depends:
         - '.shell'
 
 - module-name: 'apt_inst'
   implicit-imports:
@@ -322,14 +328,21 @@
         - 'charset_normalizer.md__mypyc'
 
 - module-name: 'chia.ssl.create_ssl'
   implicit-imports:
     - depends:
         - 'mozilla-ca'
 
+- module-name: 'chromadb'
+  implicit-imports:
+    - depends:
+        - 'chromadb.telemetry.posthog'
+        - 'chromadb.api.local'
+        - 'chromadb.db.duckdb'
+
 - module-name: 'clr'
   dlls:
     - from_filenames:
         prefixes:
           - 'Python.Runtime'
 
 - module-name: 'clr_loader.ffi'
@@ -970,15 +983,15 @@
       when: 'not use_dask'
 
 - module-name: 'jpype'
   data-files:
     dest_path: './jpype'
     patterns:
       - '../org.jpype.jar'
-    when: 'anaconda'
+    when: 'is_conda_package("jpype")'
 
 - module-name: 'jsonrpcserver.main'
   data-files:
     patterns:
       - '*.json'
 
 - module-name: 'jsonschema'
@@ -1197,15 +1210,15 @@
 
 - module-name: 'mkl._mklinit'
   dlls:
     - by_code:
         setup_code: 'import os;import sys'
         filename_code: "os.path.join(sys.prefix, 'lib', 'libmkl_mc3.1.dylib')"
       dest_path: '.'
-      when: 'anaconda and macos'
+      when: 'is_conda_package("mkl") and macos'
 
 - module-name: 'mmcv.utils'
   anti-bloat:
     - description: 'remove mmcv testing framework'
       replacements_plain:
         'from .testing import': 'if False: from .testing import'
       append_plain: '__all__ = [_name for _name in __all__ if _name in globals()]'
@@ -1342,15 +1355,15 @@
           library_path = os.path.join(sys.prefix, library_path)
           library_prefix = "mkl_" if os.name == "nt" else "libmkl_"
         filename_code: |
           [os.path.join(library_path, filename)
            for filename in os.listdir(library_path)
            if filename.startswith(library_prefix)] if os.path.isdir(library_path) else []
       dest_path: '.'
-      when: 'anaconda'
+      when: 'is_conda_package("numpy")'
 
   implicit-imports:
     - depends:
         - 'numpy._mklinit'
         - 'numpy.compat'
         - 'numpy.lib'
         - 'numpy.linalg'
@@ -1583,14 +1596,24 @@
         - 'osgeo._gdal'
         - 'osgeo._gdalconst'
         - 'osgeo._gdal_array'
         - 'osgeo._gnm'
         - 'osgeo._ogr'
         - 'osgeo._osr'
 
+- module-name: 'overrides.enforce'
+  anti-bloat:
+    - description: 'disable overrides function checking'
+      module_code: |
+        from abc import ABCMeta
+        class EnforceOverridesMeta(ABCMeta):
+          pass
+        class EnforceOverrides(metaclass=EnforceOverridesMeta):
+          pass
+
 - module-name: 'overrides.overrides'
   anti-bloat:
     - description: 'disable overrides function checking'
       change_function:
         '_overrides': "'(lambda method, *args, **kwargs: method)'"
 
 - module-name: 'panda3d'
@@ -1915,14 +1938,19 @@
       when: 'not use_dask'
 
 - module-name: 'pint.registry'
   data-files:
     patterns:
       - '*.txt'
 
+- module-name: 'pint.util'
+  anti-bloat:
+    - description: 'workaround __new__ decorator issue'
+      append_plain: 'SharedRegistryObject.__new__ = staticmethod(SharedRegistryObject.__new__)'
+
 - module-name: 'pkg_resources'
   anti-bloat:
     - description: 'avoid using plistlib dependency on non-macOS'
       replacements_plain:
         'import plistlib': ''
       when: 'not macos'
     - description: 'avoid requiring entry points at runtime'
@@ -2005,14 +2033,39 @@
         # Disable lazy loading implicit imports.
         - 'plotly.validators.*'
         - 'plotly.validators.*.*'
         # Maybe misplaced those here. TODO: Also make recursive dependency a thing.
         - 'plotly.graph_objs.layout.*'
         - 'plotly.graph_objs.layout.*.*'
 
+- module-name: 'polars.lazyframe.frame'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'from IPython.display import SVG, display': 'raise ImportError'
+      when: 'not use_ipython'
+
+- module-name: 'polars.series.utils'
+  anti-bloat:
+    - description: 'workaround for compiled method support'
+      append_plain: |
+        _orig_is_empty_method = _is_empty_method
+        def _is_empty_method(func):
+          if hasattr(func, "__compiled_constant__"):
+              return getattr(func, "__compiled_constant__") is None
+
+          return _orig_is_empty_method(func)
+
+- module-name: 'polars.utils.various'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'from IPython import get_ipython': 'raise ImportError'
+      when: 'not use_ipython'
+
 - module-name: 'psutil'
   anti-bloat:
     - description: 'resolve platform specific imports at compile time'
       context:
         - 'import psutil'
       replacements:
         'from ._common import AIX': "'AIX = %r' % psutil.AIX"
@@ -2155,15 +2208,15 @@
   options:
     checks:
       - description: 'PyQt5 is a GUI framework'
         console: 'recommend'
         when: 'plugin("pyqt5")'
       - description: 'PyQt5 cannot be used without bundle'
         macos_bundle: 'yes'
-        when: 'macos and not anaconda and plugin("pyqt5")'
+        when: 'macos and not is_conda_package("pyqt5") and plugin("pyqt5")'
       - description: 'PyQt5 cannot be signed unless onefile'
         macos_bundle_as_onefile: 'yes'
         when: 'macos and plugin("pyqt5")'
 
 - module-name: 'PyQt6'
   options:
     checks:
@@ -2681,14 +2734,36 @@
 
 - module-name: 'scipy.linalg'
   implicit-imports:
     - depends:
         - 'scipy.linalg.cython_blas'
         - 'scipy.linalg.cython_lapack'
 
+- module-name: 'scipy.optimize._cobyla_py'
+  anti-bloat:
+    - replacements_plain:
+        '    info = np.zeros(4, np.float64)': |
+          #
+              info = np.zeros(4, np.float64)
+              def calcfc2(x, con):
+                  f = fun(np.copy(x), *args)
+                  i = 0
+                  for size, c in izip(cons_lengths, constraints):
+                      con[i: i + size] = c['fun'](x, *c['args'])
+                      i += size
+                  return f
+
+              calcfc = eval("lambda x, con: calcfc2(x,con)", locals())
+
+              def wrapped_callback2(x):
+                  if callback is not None:
+                      callback(np.copy(x))
+
+              wrapped_callback = eval("lambda x: wrapped_callback2(x)", locals())
+
 - module-name: 'scipy.sparse.csgraph'
   implicit-imports:
     - depends:
         - 'scipy.sparse.csgraph._validation'
 
 - module-name: 'scipy.sparse.linalg._expm_multiply'
   anti-bloat:
@@ -2891,34 +2966,36 @@
 
 - module-name: 'shapely.geos'
   dlls:
     # PyPI has it contained, but not for Windows.
     - by_code:
         setup_code: 'import shapely.geos'
         filename_code: 'shapely.geos._lgeos._name'
-      when: 'not anaconda and not win32 and version("shapely") < (2,0)'
+      when: 'not is_conda_package("shapely") and not win32 and version("shapely") < (2,0)'
     # Anaconda or Win32 are forced to specific path.
     - by_code:
         setup_code: 'import shapely.geos'
         filename_code: 'shapely.geos._lgeos._name'
       dest_path: 'shapely'
-      when: 'anaconda or win32 and version("shapely") < (1,8,1)'
+      when: 'version("shapely") < (2,0) and (is_conda_package("shapely") or win32 and version("shapely") < (1,8,1))'
   anti-bloat:
     - description: 'change geos DLL location'
       replacements_plain:
         '_lgeos = load_dll("geos_c.dll")': '_lgeos = load_dll("geos_c.dll", fallbacks=[os.path.join(os.path.dirname(__file__), "geos_c.dll")])'
       when: 'win32'
     - description: 'avoid runtime Anaconda environment influence'
       replacements_plain:
         "os.getenv('CONDA_PREFIX', '')": "''"
 
 - module-name: 'shiboken6'
   implicit-imports:
     - depends:
         - 'argparse'
+        - 'enum'
+        - 'logging'
 
 - module-name: 'sip'
   implicit-imports:
     - depends:
         - 'enum'
       when: 'before_python3'
 
@@ -3508,14 +3585,22 @@
       - 'sv.tcl'
 
 - module-name: 'swagger_ui_bundle'
   data-files:
     dirs:
       - 'vendor'
 
+- module-name: 'sympy'
+  anti-bloat:
+    - description: 'remove sympy.testing reference'
+      replacements_plain:
+        "'test', 'doctest',": ''
+        'from .testing import test, doctest': ''
+      when: 'not use_pytest'
+
 - module-name: 'sympy.interactive.printing'
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         'import IPython': 'raise ImportError'
         'from IPython import get_ipython': 'raise ImportError'
         'from IPython.terminal.interactiveshell import TerminalInteractiveShell': 'raise ImportError'
@@ -3528,14 +3613,23 @@
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         'import IPython': 'raise ImportError'
         'from IPython import get_ipython': 'raise ImportError'
       when: 'not use_ipython'
 
+- module-name: 'sympy.utilities.decorator'
+  anti-bloat:
+    - description: 'remove sympy.testing reference'
+      replacements_plain:
+        'from sympy.testing.runtests import DependencyError, SymPyDocTests, PyTestReporter': ''
+      change_function:
+        'skiptests': 'un-callable'
+      when: 'not use_pytest'
+
 - module-name: 'tables'
   anti-bloat:
     - description: 'remove tables.tests usage'
       replacements_plain:
         'from .tests import print_versions, test': ''
 
 - module-name: 'tables.filters'
@@ -4099,18 +4193,34 @@
         # imports to be available.
         - ''
 
 - module-name: 'tls_client.cffi'
   dlls:
     - from_filenames:
         relative_path: 'dependencies'
-        # TODO: We might want to match OS and arches here closely, so we do not pick up
-        # unnecessary arches.
         prefixes:
           - 'tls-client'
+        suffixes:
+          - 'dll'
+      when: 'win32'
+    - from_filenames:
+        relative_path: 'dependencies'
+        prefixes:
+          - 'tls-client'
+        suffixes:
+          - 'so'
+      when: 'linux'
+      # Hopefully this works on MacOS
+    - from_filenames:
+        relative_path: 'dependencies'
+        prefixes:
+          - 'tls-client'
+        suffixes:
+          - 'dylib'
+      when: 'macos'
 
 - module-name: 'tokenizers.tools.visualizer'
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         'from IPython.core.display import HTML, display': 'raise ImportError'
       when: 'not use_ipython'
@@ -4287,14 +4397,21 @@
 
 - module-name: 'tqdm.autonotebook'
   anti-bloat:
     - description: 'remove IPython reference'
       module_code: "from .std import tqdm, trange\n"
       when: 'not use_ipython'
 
+- module-name: 'transformers.integrations'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'from transformers.utils.notebook import NotebookProgressCallback': 'raise ImportError'
+      when: 'not use_ipython'
+
 - module-name: 'transformers.models.deformable_detr.load_custom'
   anti-bloat:
     - description: 'remove setuptools usage'
       change_function:
         'load_cuda_kernels': 'un-callable'
       when: 'not use_setuptools'
 
@@ -4308,14 +4425,35 @@
 - module-name: 'transformers.models.yoso.modeling_yoso'
   anti-bloat:
     - description: 'remove setuptools usage'
       change_function:
         'load_cuda_kernels': "'(lambda : False)'"
       when: 'not use_setuptools'
 
+- module-name: 'transformers.trainer'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'is_in_notebook()': 'False'
+      when: 'not use_ipython'
+
+- module-name: 'transformers.utils.doc'
+  anti-bloat:
+    - description: 'add support for compiled functions'
+      append_plain: |
+        def copy_func(f):
+            try:
+                g = f.clone()
+            except AttributeError:
+                g = types.FunctionType(f.__code__, f.__globals__, name=f.__name__, argdefs=f.__defaults__, closure=f.__closure__)
+                g = functools.update_wrapper(g, f)
+                g.__kwdefaults__ = f.__kwdefaults__
+
+            return g
+
 - module-name: 'transformers.utils.hub'
   implicit-imports:
     - depends:
         - 'huggingface_hub.hf_api'
 
 - module-name: 'transformers.utils.import_utils'
   anti-bloat:
```

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-winsvc-1.6.3/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-winsvc-1.6.3/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/reports/Reports.py` & `Nuitka-winsvc-1.6.3/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/reports/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/HardImportSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/ParameterSpecs.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/specs/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/Basics.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/commercial/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/data_composer/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/data_composer/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/environments/Virtualenv.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/environments/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/general/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/general/find_module/FindModuleCode.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/general/find_module/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/profiler/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/profiler/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/scanning/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/specialize/Common.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/specialize/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/Common.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/Common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1777,17 +1777,15 @@
             continue
 
         if isMacOS():
             ignore = True
             for ignored_dir in (
                 "/System/Library/PrivateFrameworks",
                 "/System/Library/CoreServices",
-                "/System/Library/Frameworks/CoreFoundation.framework",
-                "/System/Library/Frameworks/AppKit.framework",
-                "/System/Library/Frameworks/ApplicationServices.framework",
+                "/System/Library/Frameworks/",
                 "/System/Library/dyld",
                 "/AppleInternal",
                 "/System/Volumes/Preboot",
                 "/usr/lib/system/",
             ):
                 if isFilenameSameAsOrBelowPath(ignored_dir, loaded_filename):
                     ignore = False
```

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/Constructs.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/OutputComparison.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/Pythons.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/SearchModes.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/Valgrind.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/watch/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tools/watch/__main__.py` & `Nuitka-winsvc-1.6.3/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/Building.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/Extractions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/InternalModule.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/Operations.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationClasses.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationClasses3.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         kw_defaults=kw_defaults,
         annotations=annotations,
         source_ref=source_ref,
     )
 
     # Add the "staticmethod" decorator to __new__ methods if not provided.
 
-    # CPython made these optional, but secretly applies them when it does
+    # CPython 2.x made these optional, but secretly applies them when it does
     # "class __new__".  We add them earlier, so our optimization will see it.
     if (
         python_version < 0x300
         and node.name == "__new__"
         and provider.isExpressionClassBodyBase()
     ):
         _injectDecorator(
```

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationMultidist.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/SourceHandling.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/SyntaxErrors.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/TreeHelpers.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/VariableClosure.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/tree/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/AppDirs.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/CStrings.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/CommandLineOptions.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Distributions.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Distributions.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
 """ Tools for accessing distributions and resolving package names for them. """
 
 from nuitka.containers.OrderedSets import OrderedSet
+from nuitka.PythonFlavors import isAnacondaPython
 from nuitka.PythonVersions import python_version
 
 from .ModuleNames import ModuleName, checkModuleName
 
 _package_to_distribution = None
 
 
 def getDistributionTopLevelPackageNames(distribution):
+    """Returns the top level package names for a distribution."""
     top_level_txt = distribution.read_text("top_level.txt")
 
     if top_level_txt:
         result = top_level_txt.split()
         result = [dirname.replace("/", ".") for dirname in result]
     else:
         result = OrderedSet()
@@ -93,14 +95,15 @@
             _package_to_distribution.get(module_name, ()),
             key=lambda dist: dist.metadata["Name"],
         )
     )
 
 
 def getDistribution(distribution_name):
+    """Get a distribution by name."""
     try:
         if python_version >= 0x380:
             from importlib import metadata
         else:
             import importlib_metadata as metadata
     except ImportError:
         return None
@@ -109,10 +112,32 @@
         return metadata.distribution(distribution_name)
     except metadata.PackageNotFoundError:
         # If not found, lets assume package name was given, and resolve to
         # the distribution.
         dists = getDistributionsFromModuleName(distribution_name)
 
         if len(dists) == 1:
-            return dists.values[0]
+            return dists[0]
 
         return None
+
+
+_distribution_to_conda_package = {}
+
+
+def isDistributionCondaPackage(distribution_name):
+    if not isAnacondaPython():
+        return False
+
+    if distribution_name not in _distribution_to_conda_package:
+        distribution = getDistribution(distribution_name)
+
+        if distribution is None:
+            _distribution_to_conda_package[distribution_name] = False
+        else:
+            installer_txt = distribution.read_text("INSTALLER") or ""
+
+            _distribution_to_conda_package[distribution_name] = (
+                installer_txt.upper() == "CONDA"
+            )
+
+    return _distribution_to_conda_package[distribution_name]
```

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Download.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Execution.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/FileOperations.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Hashing.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Images.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Importing.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/InstalledPythons.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/InstanceCounters.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Jinja2.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Json.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/MacOSApp.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/MacOSApp.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,24 +38,28 @@
         bundle_dir = os.path.dirname(
             OutputDirectories.getResultRunFilename(onefile=onefile)
         )
 
     result_filename = OutputDirectories.getResultFullpath(onefile=onefile)
     app_name = Options.getMacOSAppName() or os.path.basename(result_filename)
 
+    executable_name = os.path.basename(
+        OutputDirectories.getResultFullpath(onefile=Options.isOnefileMode())
+    )
+
     signed_app_name = Options.getMacOSSignedAppName() or app_name
     app_version = Options.getMacOSAppVersion() or "1.0"
 
     # TODO: We want an OrderedDict probably for stability.
     infos = OrderedDict(
         [
             ("CFBundleDisplayName", app_name),
             ("CFBundleName", app_name),
             ("CFBundleIdentifier", signed_app_name),
-            ("CFBundleExecutable", app_name),
+            ("CFBundleExecutable", executable_name),
             ("CFBundleInfoDictionaryVersion", "6.0"),
             ("CFBundlePackageType", "APPL"),
             ("CFBundleShortVersionString", app_version),
         ]
     )
 
     icon_paths = Options.getIconPaths()
```

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/MemoryUsage.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/ModuleNames.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/ReExecute.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Rest.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/SharedLibraries.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Shebang.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Signing.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/StaticLibraries.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/ThreadedExecutor.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Timing.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Utils.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/WindowsFileUsage.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/WindowsResources.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/Yaml.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/nuitka/utils/__init__.py` & `Nuitka-winsvc-1.6.3/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/pyproject.toml` & `Nuitka-winsvc-1.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/setup.py` & `Nuitka-winsvc-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/AssertsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/AssignmentsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/AssignmentsTest32.py` & `Nuitka-winsvc-1.6.3/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/BranchingTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/BuiltinOverload.py` & `Nuitka-winsvc-1.6.3/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/BuiltinSuperTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/BuiltinsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ClassMinimalTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ClassesTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ClassesTest32.py` & `Nuitka-winsvc-1.6.3/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ClassesTest34.py` & `Nuitka-winsvc-1.6.3/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ComparisonChainsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ConstantsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ConstantsTest27.py` & `Nuitka-winsvc-1.6.3/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/DecoratorsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/DefaultParametersTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/DoubleDeletionsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/EmptyModuleTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ExceptionRaisingTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-winsvc-1.6.3/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-winsvc-1.6.3/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ExecEvalTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ExtremeClosureTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/FunctionObjectsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/FunctionsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/FunctionsTest32.py` & `Nuitka-winsvc-1.6.3/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/FunctionsTest_2.py` & `Nuitka-winsvc-1.6.3/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/FutureTest32.py` & `Nuitka-winsvc-1.6.3/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-winsvc-1.6.3/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/GlobalStatementTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/HelloWorldTest_2.py` & `Nuitka-winsvc-1.6.3/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ImportingTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/InplaceOperationsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/InspectionTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/InspectionTest_35.py` & `Nuitka-winsvc-1.6.3/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/InspectionTest_36.py` & `Nuitka-winsvc-1.6.3/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/LambdasTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ListContractionsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/LoopingTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/MainProgramsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ModuleAttributesTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/OperatorsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/OrderChecksTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/OrderChecksTest27.py` & `Nuitka-winsvc-1.6.3/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-winsvc-1.6.3/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ParameterErrorsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ParameterErrorsTest32.py` & `Nuitka-winsvc-1.6.3/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/PrintFutureTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/PrintingTest_2.py` & `Nuitka-winsvc-1.6.3/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/RecursionTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ReferencingTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ReferencingTest27.py` & `Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ReferencingTest33.py` & `Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ReferencingTest35.py` & `Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ReferencingTest36.py` & `Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ReferencingTest_2.py` & `Nuitka-winsvc-1.6.3/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/SlotsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-winsvc-1.6.3/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-winsvc-1.6.3/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-winsvc-1.6.3/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TryContinueFinallyTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TryExceptContinueTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TryExceptFinallyTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TryExceptFramesTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TryReturnFinallyTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/TryYieldFinallyTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/UnicodeTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/UnpackingTest35.py` & `Nuitka-winsvc-1.6.3/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/VarargsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/WithStatementsTest.py` & `Nuitka-winsvc-1.6.3/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/YieldFromTest33.py` & `Nuitka-winsvc-1.6.3/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/run_all.py` & `Nuitka-winsvc-1.6.3/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/basics/run_xml.py` & `Nuitka-winsvc-1.6.3/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/onefile/HelloWorldTest.py` & `Nuitka-winsvc-1.6.3/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-winsvc-1.6.3/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/onefile/run_all.py` & `Nuitka-winsvc-1.6.3/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/ArgumentTypes.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/Attributes.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/Calls.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/Conditions.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/DecodingOperations.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/FormatStrings36.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/HardImports.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/HardImports_2.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/Iterations.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/Len.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/Operations.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/Subscripts.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/optimizations/run_all.py` & `Nuitka-winsvc-1.6.3/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/run_all.py` & `Nuitka-winsvc-1.6.3/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-winsvc-1.6.3/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-winsvc-1.6.3/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/plugins/code_signing/CodeSigningMain.py` & `Nuitka-winsvc-1.6.3/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-winsvc-1.6.3/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/plugins/parameters/ParametersMain.py` & `Nuitka-winsvc-1.6.3/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-winsvc-1.6.3/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/plugins/run_all.py` & `Nuitka-winsvc-1.6.3/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/local.py` & `Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/absolute_import/foobar/util.py` & `Nuitka-winsvc-1.6.3/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/dash_import/DashImportMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/dash_import/dash-module.py` & `Nuitka-winsvc-1.6.3/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/dash_import/plus+module.py` & `Nuitka-winsvc-1.6.3/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/dash_main/Dash-Main.py` & `Nuitka-winsvc-1.6.3/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/deep/DeepProgramMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/deep/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/main_raises/ErrorMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-winsvc-1.6.3/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-winsvc-1.6.3/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_exits/Main.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-winsvc-1.6.3/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-winsvc-1.6.3/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-winsvc-1.6.3/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_code/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_contains_main/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_contains_main/local.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_module_collision/something.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_overload/Main.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_overload/foo/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_overload/foo/bar.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_overload/foo/bar2.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-winsvc-1.6.3/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-winsvc-1.6.3/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/relative_import/dircache.py` & `Nuitka-winsvc-1.6.3/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/run_all.py` & `Nuitka-winsvc-1.6.3/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-winsvc-1.6.3/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-winsvc-1.6.3/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-winsvc-1.6.3/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-winsvc-1.6.3/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-winsvc-1.6.3/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/programs/with space/Space Main.py` & `Nuitka-winsvc-1.6.3/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/reflected/compile_itself.py` & `Nuitka-winsvc-1.6.3/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/run-tests` & `Nuitka-winsvc-1.6.3/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/BrotliUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/CtypesUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/FlaskUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/GlfwUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/GtkUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/HexEncodingTest_2.py` & `Nuitka-winsvc-1.6.3/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/IdnaUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/LxmlUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/MatplotlibUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/NumpyUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/OpenGLUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PandasUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PasslibUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PendulumUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PmwUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PyQt5Plugins.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PyQt5Using.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PyQt6Plugins.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PyQt6Using.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PySide6Plugins.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/PySide6Using.py` & `Nuitka-winsvc-1.6.3/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/RsaUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/ShlibUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/SocketUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/TkInterUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/Urllib3Using.py` & `Nuitka-winsvc-1.6.3/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/Win32ComUsing.py` & `Nuitka-winsvc-1.6.3/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/run_all.py` & `Nuitka-winsvc-1.6.3/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-winsvc-1.6.3/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/AsyncgenReturn36.py` & `Nuitka-winsvc-1.6.3/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/BreakWithoutLoop.py` & `Nuitka-winsvc-1.6.3/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/ClassReturn.py` & `Nuitka-winsvc-1.6.3/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/ClosureDel_2.py` & `Nuitka-winsvc-1.6.3/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-winsvc-1.6.3/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/DuplicateArgument.py` & `Nuitka-winsvc-1.6.3/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/ExecWithNesting_2.py` & `Nuitka-winsvc-1.6.3/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/FutureBraces.py` & `Nuitka-winsvc-1.6.3/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/FutureUnknown.py` & `Nuitka-winsvc-1.6.3/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/GeneratorExpressions38.py` & `Nuitka-winsvc-1.6.3/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/GeneratorReturn_2.py` & `Nuitka-winsvc-1.6.3/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/GlobalForParameter.py` & `Nuitka-winsvc-1.6.3/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/Importing32.py` & `Nuitka-winsvc-1.6.3/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/IndentationError.py` & `Nuitka-winsvc-1.6.3/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/LateFutureImport.py` & `Nuitka-winsvc-1.6.3/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/MisplacedFutureImport.py` & `Nuitka-winsvc-1.6.3/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/ModuleReturn.py` & `Nuitka-winsvc-1.6.3/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-winsvc-1.6.3/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/NonlocalForParameter32.py` & `Nuitka-winsvc-1.6.3/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/NonlocalNotFound32.py` & `Nuitka-winsvc-1.6.3/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/StarImportExtra.py` & `Nuitka-winsvc-1.6.3/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/SyntaxError.py` & `Nuitka-winsvc-1.6.3/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-winsvc-1.6.3/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-winsvc-1.6.3/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/UnpackNoTuple.py` & `Nuitka-winsvc-1.6.3/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/UnpackTwoStars32.py` & `Nuitka-winsvc-1.6.3/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/YieldFromInModule.py` & `Nuitka-winsvc-1.6.3/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/YieldInAsync35.py` & `Nuitka-winsvc-1.6.3/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/YieldInGenexp38.py` & `Nuitka-winsvc-1.6.3/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/YieldInModule.py` & `Nuitka-winsvc-1.6.3/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.6/tests/syntax/run_all.py` & `Nuitka-winsvc-1.6.3/tests/syntax/run_all.py`

 * *Files identical despite different names*

