# Comparing `tmp/extrap-4.0.4.tar.gz` & `tmp/extrap-4.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrap-4.0.4.tar", last modified: Fri May  6 08:30:19 2022, max compression
+gzip compressed data, was "extrap-4.1.0a2.tar", last modified: Fri Jun 16 08:36:22 2023, max compression
```

## Comparing `extrap-4.0.4.tar` & `extrap-4.1.0a2.tar`

### file list

```diff
@@ -1,100 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.480677 extrap-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)      840 2022-05-06 08:30:07.000000 extrap-4.0.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (116)     1566 2022-05-06 08:30:07.000000 extrap-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    10454 2022-05-06 08:30:19.480677 extrap-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     9395 2022-05-06 08:30:07.000000 extrap-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.468677 extrap-4.0.4/extrap/
--rw-r--r--   0 runner    (1001) docker     (116)      616 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      370 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.472677 extrap-4.0.4/extrap/entities/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1169 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/callpath.py
--rw-r--r--   0 runner    (1001) docker     (116)     2940 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/calltree.py
--rw-r--r--   0 runner    (1001) docker     (116)     2725 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (116)     7033 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/experiment.py
--rw-r--r--   0 runner    (1001) docker     (116)     4715 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/fraction.py
--rw-r--r--   0 runner    (1001) docker     (116)     4615 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    16612 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/hypotheses.py
--rw-r--r--   0 runner    (1001) docker     (116)     3034 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/measurement.py
--rw-r--r--   0 runner    (1001) docker     (116)     1101 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/metric.py
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/model.py
--rw-r--r--   0 runner    (1001) docker     (116)      985 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)     7761 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/entities/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.472677 extrap-4.0.4/extrap/extrap/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/extrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10635 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/extrap/extrapcmd.py
--rw-r--r--   0 runner    (1001) docker     (116)    10431 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/extrap/extrapgui.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.472677 extrap-4.0.4/extrap/fileio/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9671 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/cube_file_reader2.py
--rw-r--r--   0 runner    (1001) docker     (116)     2017 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/experiment_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    20220 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/extrap3_experiment_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)    12287 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/io_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     6237 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/json_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)     2831 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/jsonlines_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)     2482 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/talpas_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)     6058 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/fileio/text_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.476677 extrap-4.0.4/extrap/gui/
--rw-r--r--   0 runner    (1001) docker     (116)     4157 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/AdvancedPlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     3061 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/ColorWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     9457 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/CubeFileReader.py
--rw-r--r--   0 runner    (1001) docker     (116)    17102 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/DataDisplay.py
--rw-r--r--   0 runner    (1001) docker     (116)     4787 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/ExpanderWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)    35484 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/GraphWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     2036 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/LogWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)    20057 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/MainWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     6915 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/ModelerOptionsWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     5616 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/ModelerWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     2727 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/ParameterValueSlider.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/PlotTypeSelector.py
--rw-r--r--   0 runner    (1001) docker     (116)     2812 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/ProgressWindow.py
--rw-r--r--   0 runner    (1001) docker     (116)    10131 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/SelectorWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)    10887 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/TreeModel.py
--rw-r--r--   0 runner    (1001) docker     (116)     4110 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/TreeView.py
--rw-r--r--   0 runner    (1001) docker     (116)     6352 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/Utils.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.480677 extrap-4.0.4/extrap/gui/plots/
--rw-r--r--   0 runner    (1001) docker     (116)     2982 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     2667 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     6647 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/BaseGraphWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     6745 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     3359 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     8463 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/HeatMapGraphWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     4593 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/InterpolatedContourDisplayWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     4450 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/IsolinesDisplayWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     3227 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)     4586 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/MeasurementPointsPlotWidget.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/gui/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.480677 extrap-4.0.4/extrap/modelers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3405 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/abstract_modeler.py
--rw-r--r--   0 runner    (1001) docker     (116)     3611 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/loader.py
--rw-r--r--   0 runner    (1001) docker     (116)     4778 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/model_generator.py
--rw-r--r--   0 runner    (1001) docker     (116)     5500 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/modeler_options.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.480677 extrap-4.0.4/extrap/modelers/multi_parameter/
--rw-r--r--   0 runner    (1001) docker     (116)      537 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/multi_parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18536 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/multi_parameter/multi_parameter_modeler.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.480677 extrap-4.0.4/extrap/modelers/single_parameter/
--rw-r--r--   0 runner    (1001) docker     (116)      521 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/single_parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7622 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/single_parameter/abstract_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    13494 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/single_parameter/basic.py
--rw-r--r--   0 runner    (1001) docker     (116)     8471 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/modelers/single_parameter/refining.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.480677 extrap-4.0.4/extrap/util/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      808 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/caching.py
--rw-r--r--   0 runner    (1001) docker     (116)      533 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/classproperty.py
--rw-r--r--   0 runner    (1001) docker     (116)     1566 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (116)      899 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     6822 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/options_parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     1695 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (116)     6892 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/serialization_schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     1334 2022-05-06 08:30:07.000000 extrap-4.0.4/extrap/util/unique_list.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-06 08:30:19.468677 extrap-4.0.4/extrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    10454 2022-05-06 08:30:19.000000 extrap-4.0.4/extrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2732 2022-05-06 08:30:19.000000 extrap-4.0.4/extrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-06 08:30:19.000000 extrap-4.0.4/extrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      114 2022-05-06 08:30:19.000000 extrap-4.0.4/extrap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      157 2022-05-06 08:30:19.000000 extrap-4.0.4/extrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-05-06 08:30:19.000000 extrap-4.0.4/extrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-05-06 08:30:19.480677 extrap-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2045 2022-05-06 08:30:07.000000 extrap-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.468173 extrap-4.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-16 08:36:08.000000 extrap-4.1.0a2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:36:08.000000 extrap-4.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-16 08:36:22.468173 extrap-4.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-06-16 08:36:08.000000 extrap-4.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.452173 extrap-4.1.0a2/extrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/entities/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/annotations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/entities/annotations/comment_annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/annotations/comment_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/callpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/calltree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16659 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/hypotheses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/entities/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/extrap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/extrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/extrap/extrapcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/extrap/extrapgui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/experiment_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.460173 extrap-4.1.0a2/extrap/fileio/file_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/abstract_directory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/cube_file_reader2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/extrap3_experiment_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/json_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/jsonlines_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/talpas_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/file_reader/text_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/io_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/fileio/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/AdvancedPlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/ColorWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/CubeFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/DataDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33974 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/GraphWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/LogWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/MainWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/ModelerOptionsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/ModelerWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/PlotTypeSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/SelectorWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/TreeModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/TreeView.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/gui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/ExpanderWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/ParameterValueSlider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/ProgressWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/annotation_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/model_color_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/components/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/gui/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/BaseGraphWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/HeatMapGraphWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/InterpolatedContourDisplayWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/IsolinesDisplayWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/MeasurementPointsPlotWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/gui/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/modelers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/abstract_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/model_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/modeler_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/modelers/multi_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/multi_parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/multi_parameter/multi_parameter_modeler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.464173 extrap-4.1.0a2/extrap/modelers/single_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/abstract_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/modelers/single_parameter/refining.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.468173 extrap-4.1.0a2/extrap/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/extension_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/options_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/serialization_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-16 08:36:08.000000 extrap-4.1.0a2/extrap/util/unique_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:36:22.456173 extrap-4.1.0a2/extrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 08:36:22.000000 extrap-4.1.0a2/extrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:36:22.468173 extrap-4.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-16 08:36:08.000000 extrap-4.1.0a2/setup.py
```

### Comparing `extrap-4.0.4/AUTHORS.md` & `extrap-4.1.0a2/AUTHORS.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 * Alexandru Calotoiu (calotoiu@cs.tu-darmstadt.de)
 * Alexander Geiß (geiss@cs.tu-darmstadt.de)
 * David Giessing (david.giessing93@gmail.com)
 * Marc-Andre Hermanns (m.a.hermanns@fz-juelich.de)
 * Jonas Klesy (jonas.klesy@googlemail.com)
 * Christof Jugel (christof.jugel@stud.tu-darmstadt.de)
+* Samuel Lokadjaja (samuel.lokadjaja@stud.tu-darmstadt.de)
 * Daniel Lorenz (lorenz@cs.tu-darmstadt.de
 * Benedikt Naumann (benedikt.naumann@gmx.de)
 * Nicolas Ollagnier (ncls_olg@yahoo.fr)
 * Marius Poke (m.poke@grs-sim.de)
 * Patrick Reisert (kpreisert@gmail.com)
 * Marcus Ritter (marcus.ritter@tu-darmstadt.de)
 * Niharika Sharma (niharika.sharma1908@gmail.com)
+* Moritz Vanderheyden (moritz.vanderheyden@stud.tu-darmstadt.de)
 * Johannes Wehrstein (johannes.wehrstein@gmx.de)
 * Paul Wiedeking (p.wiedeking@grs-sim.de)
```

### Comparing `extrap-4.0.4/LICENSE` & `extrap-4.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/PKG-INFO` & `extrap-4.1.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: extrap
-Version: 4.0.4
+Version: 4.1.0a2
 Summary: Extra-P, automated performance modeling for HPC applications
 Home-page: https://github.com/extra-p/extrap
 Author: Extra-P project
 Author-email: extra-p@lists.parallel.informatik.tu-darmstadt.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Extra-P
 
 **Automated performance modeling for HPC applications**
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/extrap?style=plastic)](https://badge.fury.io/py/extrap)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/extra-p/extrap?style=plastic)
 [![PyPI version](https://badge.fury.io/py/extrap.png)](https://badge.fury.io/py/extrap)
 [![PyPI - License](https://img.shields.io/pypi/l/extrap?style=plastic)](https://badge.fury.io/py/extrap)
 ![GitHub issues](https://img.shields.io/github/issues/extra-p/extrap?style=plastic)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/extra-p/extrap?style=plastic)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/extra-p/extrap/Test%20extrap%20package?style=plastic)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/extra-p/extrap/python-package.yml?style=plastic)
 
 [<img alt="Screenshot of Extra-P" src="https://github.com/extra-p/extrap/raw/master/docs/images/extra-p-2d.png" height="200" align="right" title="Screenshot of Extra-P"/>](docs/images/extra-p-2d.png)
 Extra-P is an automatic performance-modeling tool that supports the user in the identification of *scalability bugs*. 
 A scalability bug is a part of the program whose scaling behavior is unintentionally poor, 
 that is, much worse than expected. A performance model is a formula that expresses a performance metric of interest 
 such as execution time or energy consumption as a function of one or more execution parameters such as the size of the 
 input problem or the number of processors. 
@@ -70,21 +70,21 @@
 5. [Citation](#Citation)
 6. [Publications](#Publications)
 
 --------------------------------------------------------------------------------------------
 
 ### Requirements
 
-* Python 3.7 or higher
+* Python 3.8 or higher
 * numpy
 * pycubexr
 * marshmallow
 * packaging
 * tqdm
-* PySide2 (for GUI)
+* PySide6 (for GUI)
 * matplotlib (for GUI)
 * pyobjc-framework-Cocoa (only for GUI on macOS)
 
 ### Installation
 
 Use the following command to install Extra-P and all required packages via `pip`.
 
@@ -118,36 +118,38 @@
 * Create model and save it to text file at the given
   path: `extrap --out test.txt --text test/data/text/one_parameter_1.txt`
 
 The Extra-P command line interface has the following options.
 
 | Arguments                                                            |                                              |
 |----------------------------------------------------------------------|----------------------------------------------|
-| **Positional**                                                       |                                              |
-| _FILEPATH_                                                           | Specify a file path for Extra-P to work with |
-| **Optional**                                                         |                                              |
-| `-h`, `--help`                                                       | Show help message and exit                   |
-| `--version`                                                          | Show program's version number and exit       |
-| `--log` {`debug`, `info`, `warning`, `error`, `critical`}            | Set program's log level (default: `warning`) |
-| **Input options**                                                    |                                              |
-| `--cube`                                                             | Load data from CUBE files                    |
-| `--text`                                                             | Load data from text files                    |
-| `--talpas`                                                           | Load data from Talpas data format            |
-| `--json`                                                             | Load data from JSON or JSON Lines file       |
-| `--extra-p-3`                                                        | Load data from Extra-P 3 experiment          |
-| `--scaling` {`weak`, `strong`}                                       | Set weak or strong scaling when loading data from CUBE files (default: `weak`) |
-| **Modeling options**                                                 |                                              |
-| `--median`                                                           | Use median values for computation instead of mean values  |
-| `--modeler` {`default`, `basic`, `refining`, `multi-parameter`}      | Selects the modeler for generating the performance models |
-| `--options` _KEY_=_VALUE_ [_KEY_=_VALUE_ ...]                        | Options for the selected modeler             |
-| `--help-modeler` {`default`, `basic`, `refining`, `multi-parameter`} | Show help for modeler options and exit       |
-| **Output options**                                                   |                                              |
-| `--out` _OUTPUT_PATH_                                                | Specify the output path for Extra-P results  |
-| `--print` {`all`, `callpaths`, `metrics`, `parameters`, `functions`} | Set which information should be displayed after modeling (default: `all`) |
-| `--save-experiment` <i>EXPERIMENT_PATH</i>                           | Saves the experiment including all models as Extra-P experiment (if no extension is specified, “.extra-p” is appended) |
+| **Positional**                                                       |                                              
+| _FILEPATH_                                                           | Specify a file path for Extra-P to work with 
+| **Optional**                                                         |                                              
+| `-h`, `--help`                                                       | Show help message and exit                   
+| `--version`                                                          | Show program's version number and exit       
+| `--log` {`debug`, `info`, `warning`, `error`, `critical`}            | Set program's log level (default: `warning`) 
+| **Input options**                                                    |                                              
+| `--cube`                                                             | Load a set of CUBE files and generate a new experiment
+| `--extra-p-3`                                                        | Load data from Extra-P 3 (legacy) experiment
+| `--json`                                                             | Load data from JSON or JSON Lines input file
+| `--talpas`                                                           | Load data from Talpas data format
+| `--text`                                                             | Load data from text input file
+| `--experiment`                                                       | Load Extra-P experiment and generate new models
+| `--scaling` {`weak`, `strong`}                                       | Set weak or strong scaling when loading data from CUBE files (default: `weak`) 
+| **Modeling options**                                                 |                                              
+| `--median`                                                           | Use median values for computation instead of mean values  
+| `--modeler` {`default`, `basic`, `refining`, `multi-parameter`}      | Selects the modeler for generating the performance models 
+| `--options` _KEY_=_VALUE_ [_KEY_=_VALUE_ ...]                        | Options for the selected modeler             
+| `--help-modeler` {`default`, `basic`, `refining`, `multi-parameter`} | Show help for modeler options and exit       
+| **Output options**                                                   |                                              
+| `--out` _OUTPUT_PATH_                                                | Specify the output path for Extra-P results  
+| `--print` {`all`, `callpaths`, `metrics`, `parameters`, `functions`, _FORMAT_STRING_} | Set which information should be displayed after modeling. Use one of the predefined values or specify a formatting string using placeholders (see [docs/output-formatting.md](docs/output-formatting.md)) (default: `all`).
+| `--save-experiment` <i>EXPERIMENT_PATH</i>                           | Saves the experiment including all models as Extra-P experiment (if no extension is specified, “.extra-p” is appended) 
+| `--model-set-name` _NAME_                                            | Set the name of the generated set of models when outputting an experiment (default: “New model”)
 
 ### License
 
 [BSD 3-Clause "New" or "Revised" License](LICENSE)
 
 ### Citation
 
@@ -168,9 +170,7 @@
 ### Publications
 
 1. Alexandru Calotoiu, David Beckingsale, Christopher W. Earl, Torsten Hoefler, Ian Karlin, Martin Schulz, Felix Wolf: Fast Multi-Parameter Performance Modeling. In Proc. of the 2016 IEEE International Conference on Cluster Computing (CLUSTER), Taipei, Taiwan, pages 172–181, IEEE, September 2016. [PDF](https://apps.fz-juelich.de/jsc-pubsystem/aigaion/attachments/fastmultiparam.pdf-f839eba376c6d61a8c4cab9860b6b3bf.pdf)
 
 2. Marcus Ritter, Alexandru Calotoiu, Sebastian Rinke, Thorsten Reimann, Torsten Hoefler, Felix Wolf: *Learning Cost-Effective Sampling Strategies for Empirical Performance Modeling.* In Proc. of the 34th IEEE International Parallel and Distributed Processing Symposium (IPDPS), New Orleans, LA, USA, pages 884–895, IEEE, May 2020. [PDF](https://apps.fz-juelich.de/jsc-pubsystem/aigaion/attachments/ritter_ea_2020_ipdps.pdf-01cbe96f7a170aba7c7ef941f966d292.pdf)
 
 3. Marcus Ritter, Alexander Geiß, Johannes Wehrstein, Alexandru Calotoiu, Thorsten Reimann, Torsten Hoefler, Felix Wolf: *Noise-Resilient Empirical Performance Modeling with Deep Neural Networks.* In Proc. of the 35th IEEE International Parallel and Distributed Processing Symposium (IPDPS), Portland, Oregon, USA, pages 23–34, IEEE, May 2021. [PDF](http://htor.inf.ethz.ch/publications/img/noiseresilientmodeling.pdf)
-
-
```

### Comparing `extrap-4.0.4/README.md` & `extrap-4.1.0a2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/extrap?style=plastic)](https://badge.fury.io/py/extrap)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/extra-p/extrap?style=plastic)
 [![PyPI version](https://badge.fury.io/py/extrap.png)](https://badge.fury.io/py/extrap)
 [![PyPI - License](https://img.shields.io/pypi/l/extrap?style=plastic)](https://badge.fury.io/py/extrap)
 ![GitHub issues](https://img.shields.io/github/issues/extra-p/extrap?style=plastic)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/extra-p/extrap?style=plastic)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/extra-p/extrap/Test%20extrap%20package?style=plastic)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/extra-p/extrap/python-package.yml?style=plastic)
 
 [<img alt="Screenshot of Extra-P" src="https://github.com/extra-p/extrap/raw/master/docs/images/extra-p-2d.png" height="200" align="right" title="Screenshot of Extra-P"/>](docs/images/extra-p-2d.png)
 Extra-P is an automatic performance-modeling tool that supports the user in the identification of *scalability bugs*. 
 A scalability bug is a part of the program whose scaling behavior is unintentionally poor, 
 that is, much worse than expected. A performance model is a formula that expresses a performance metric of interest 
 such as execution time or energy consumption as a function of one or more execution parameters such as the size of the 
 input problem or the number of processors. 
@@ -43,21 +43,21 @@
 5. [Citation](#Citation)
 6. [Publications](#Publications)
 
 --------------------------------------------------------------------------------------------
 
 ### Requirements
 
-* Python 3.7 or higher
+* Python 3.8 or higher
 * numpy
 * pycubexr
 * marshmallow
 * packaging
 * tqdm
-* PySide2 (for GUI)
+* PySide6 (for GUI)
 * matplotlib (for GUI)
 * pyobjc-framework-Cocoa (only for GUI on macOS)
 
 ### Installation
 
 Use the following command to install Extra-P and all required packages via `pip`.
 
@@ -91,36 +91,38 @@
 * Create model and save it to text file at the given
   path: `extrap --out test.txt --text test/data/text/one_parameter_1.txt`
 
 The Extra-P command line interface has the following options.
 
 | Arguments                                                            |                                              |
 |----------------------------------------------------------------------|----------------------------------------------|
-| **Positional**                                                       |                                              |
-| _FILEPATH_                                                           | Specify a file path for Extra-P to work with |
-| **Optional**                                                         |                                              |
-| `-h`, `--help`                                                       | Show help message and exit                   |
-| `--version`                                                          | Show program's version number and exit       |
-| `--log` {`debug`, `info`, `warning`, `error`, `critical`}            | Set program's log level (default: `warning`) |
-| **Input options**                                                    |                                              |
-| `--cube`                                                             | Load data from CUBE files                    |
-| `--text`                                                             | Load data from text files                    |
-| `--talpas`                                                           | Load data from Talpas data format            |
-| `--json`                                                             | Load data from JSON or JSON Lines file       |
-| `--extra-p-3`                                                        | Load data from Extra-P 3 experiment          |
-| `--scaling` {`weak`, `strong`}                                       | Set weak or strong scaling when loading data from CUBE files (default: `weak`) |
-| **Modeling options**                                                 |                                              |
-| `--median`                                                           | Use median values for computation instead of mean values  |
-| `--modeler` {`default`, `basic`, `refining`, `multi-parameter`}      | Selects the modeler for generating the performance models |
-| `--options` _KEY_=_VALUE_ [_KEY_=_VALUE_ ...]                        | Options for the selected modeler             |
-| `--help-modeler` {`default`, `basic`, `refining`, `multi-parameter`} | Show help for modeler options and exit       |
-| **Output options**                                                   |                                              |
-| `--out` _OUTPUT_PATH_                                                | Specify the output path for Extra-P results  |
-| `--print` {`all`, `callpaths`, `metrics`, `parameters`, `functions`} | Set which information should be displayed after modeling (default: `all`) |
-| `--save-experiment` <i>EXPERIMENT_PATH</i>                           | Saves the experiment including all models as Extra-P experiment (if no extension is specified, “.extra-p” is appended) |
+| **Positional**                                                       |                                              
+| _FILEPATH_                                                           | Specify a file path for Extra-P to work with 
+| **Optional**                                                         |                                              
+| `-h`, `--help`                                                       | Show help message and exit                   
+| `--version`                                                          | Show program's version number and exit       
+| `--log` {`debug`, `info`, `warning`, `error`, `critical`}            | Set program's log level (default: `warning`) 
+| **Input options**                                                    |                                              
+| `--cube`                                                             | Load a set of CUBE files and generate a new experiment
+| `--extra-p-3`                                                        | Load data from Extra-P 3 (legacy) experiment
+| `--json`                                                             | Load data from JSON or JSON Lines input file
+| `--talpas`                                                           | Load data from Talpas data format
+| `--text`                                                             | Load data from text input file
+| `--experiment`                                                       | Load Extra-P experiment and generate new models
+| `--scaling` {`weak`, `strong`}                                       | Set weak or strong scaling when loading data from CUBE files (default: `weak`) 
+| **Modeling options**                                                 |                                              
+| `--median`                                                           | Use median values for computation instead of mean values  
+| `--modeler` {`default`, `basic`, `refining`, `multi-parameter`}      | Selects the modeler for generating the performance models 
+| `--options` _KEY_=_VALUE_ [_KEY_=_VALUE_ ...]                        | Options for the selected modeler             
+| `--help-modeler` {`default`, `basic`, `refining`, `multi-parameter`} | Show help for modeler options and exit       
+| **Output options**                                                   |                                              
+| `--out` _OUTPUT_PATH_                                                | Specify the output path for Extra-P results  
+| `--print` {`all`, `callpaths`, `metrics`, `parameters`, `functions`, _FORMAT_STRING_} | Set which information should be displayed after modeling. Use one of the predefined values or specify a formatting string using placeholders (see [docs/output-formatting.md](docs/output-formatting.md)) (default: `all`).
+| `--save-experiment` <i>EXPERIMENT_PATH</i>                           | Saves the experiment including all models as Extra-P experiment (if no extension is specified, “.extra-p” is appended) 
+| `--model-set-name` _NAME_                                            | Set the name of the generated set of models when outputting an experiment (default: “New model”)
 
 ### License
 
 [BSD 3-Clause "New" or "Revised" License](LICENSE)
 
 ### Citation
```

### Comparing `extrap-4.0.4/extrap/__init__.py` & `extrap-4.1.0a2/extrap/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 __title__ = "Extra-P"
-__version__ = "4.0.4"
+__version__ = "4.1.0-alpha2"
 __description__ = "Extra-P, automated performance modeling for HPC applications"
-__copyright__ = "Copyright (c) 2020-2021 Technical University of Darmstadt, Darmstadt, Germany"
+__copyright__ = "Copyright (c) 2020-2022 Technical University of Darmstadt, Darmstadt, Germany"
 __documentation_link__ = f"https://github.com/extra-p/extrap/tree/v{__version__}/docs"
```

### Comparing `extrap-4.0.4/extrap/entities/calltree.py` & `extrap-4.1.0a2/extrap/entities/calltree.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/entities/coordinate.py` & `extrap-4.1.0a2/extrap/entities/coordinate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import itertools
 from typing import Union, Iterable
 
@@ -44,14 +44,15 @@
         """
         return str(self._values)
 
     def __getitem__(self, param: int):
         """
         Returns the value for a parameter.
         """
+        assert param >= 0
         return self._values[param]
 
     def __repr__(self):
         """
         Returns a string representation of the coordinate.
         """
         return f'Coordinate{str(self._values)}'
```

### Comparing `extrap-4.0.4/extrap/entities/experiment.py` & `extrap-4.1.0a2/extrap/entities/experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import logging
 import warnings
 from itertools import chain
 from typing import List, Dict, Tuple
 
-from marshmallow import fields, validate, pre_load
+from marshmallow import fields, validate, pre_load, post_dump
 from packaging.version import Version
 
 import extrap
 from extrap.entities.callpath import Callpath, CallpathSchema
 from extrap.entities.calltree import CallTree
 from extrap.entities.coordinate import Coordinate
 from extrap.entities.measurement import Measurement, MeasurementSchema
 from extrap.entities.metric import Metric, MetricSchema
 from extrap.entities.parameter import Parameter, ParameterSchema
 from extrap.fileio import io_helper
 from extrap.modelers.model_generator import ModelGenerator, ModelGeneratorSchema
 from extrap.util.deprecation import deprecated
 from extrap.util.progress_bar import DUMMY_PROGRESS
-from extrap.util.serialization_schema import Schema, TupleKeyDict
+from extrap.util.serialization_schema import TupleKeyDict, BaseSchema, ListToMappingField
 from extrap.util.unique_list import UniqueList
 
 
 class Experiment:
 
     def __init__(self):
         self.callpaths: List[Callpath] = UniqueList()
@@ -102,19 +102,22 @@
             coordinate = measurement.coordinate
             value_mean = measurement.mean
             value_median = measurement.median
             logging.debug(
                 f"Measurement {i}: {metric}, {callpath}, {coordinate}: {value_mean} (mean), {value_median} (median)")
 
 
-class ExperimentSchema(Schema):
+class ExperimentSchema(BaseSchema):
     _version_ = fields.Constant(extrap.__version__, data_key=extrap.__title__)
     scaling = fields.Str(required=False, allow_none=True, validate=validate.OneOf(['strong', 'weak']))
-    parameters = fields.List(fields.Nested(ParameterSchema))
-    measurements = TupleKeyDict(keys=(fields.Nested(CallpathSchema), fields.Nested(MetricSchema)),
+    parameters = fields.List(fields.Pluck(ParameterSchema, 'name'))
+    callpaths = ListToMappingField(CallpathSchema, 'name', list_type=UniqueList, dump_condition=lambda x: bool(x.tags))
+    metrics = ListToMappingField(MetricSchema, 'name', list_type=UniqueList, dump_condition=lambda x: bool(x.tags))
+
+    measurements = TupleKeyDict(keys=(fields.Pluck(CallpathSchema, 'name'), fields.Pluck(MetricSchema, 'name')),
                                 values=fields.List(fields.Nested(MeasurementSchema, exclude=('callpath', 'metric'))))
 
     modelers = fields.List(fields.Nested(ModelGeneratorSchema), missing=[], required=False)
 
     def set_progress_bar(self, pbar):
         self.context['progress_bar'] = pbar
 
@@ -145,14 +148,19 @@
             ms = data.get('modelers')
             if ms:
                 pbar.total += len(ms)
                 pbar.total += len(ms) * models
             pbar.update(0)
         return data
 
+    @post_dump
+    def remove_empty_fields(self, val, **kwargs):
+        val = {k: v for k, v in val.items() if v is not None and not (hasattr(v, '__len__') and len(v) == 0)}
+        return val
+
     def create_object(self):
         return Experiment()
 
     def postprocess_object(self, obj: Experiment):
         if 'progress_bar' in self.context:
             pbar = self.context['progress_bar']
         else:
```

### Comparing `extrap-4.0.4/extrap/entities/fraction.py` & `extrap-4.1.0a2/extrap/entities/fraction.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/entities/functions.py` & `extrap-4.1.0a2/extrap/entities/functions.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/entities/hypotheses.py` & `extrap-4.1.0a2/extrap/entities/hypotheses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
 # Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-import abc
 from typing import Sequence
 
 import numpy
 from marshmallow import fields
 
 from extrap.entities.functions import Function, MultiParameterFunction, FunctionSchema
 from extrap.entities.measurement import Measurement
@@ -172,14 +171,15 @@
         else:
             self.function.constant_coefficient = numpy.mean([m.mean for m in measurements])
 
     def compute_cost(self, measurements: Sequence[Measurement]):
         """
         Computes the cost of the constant hypothesis using all data points.
         """
+        self._AR2 = 1  # TODO: should this be calculated?
         smape = 0
         for measurement in measurements:
             predicted = self.function.constant_coefficient
             if self._use_median:
                 actual = measurement.median
             else:
                 actual = measurement.mean
```

### Comparing `extrap-4.0.4/extrap/entities/measurement.py` & `extrap-4.1.0a2/extrap/entities/measurement.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/entities/model.py` & `extrap-4.1.0a2/extrap/entities/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
+from __future__ import annotations
+
 from typing import Optional, List
 
 import numpy
-from marshmallow import fields, post_load
+from marshmallow import fields, post_load, pre_dump
 
+from extrap.entities.annotations import Annotation, AnnotationSchema
 from extrap.entities.callpath import CallpathSchema
 from extrap.entities.hypotheses import Hypothesis, HypothesisSchema
 from extrap.entities.measurement import Measurement
 from extrap.entities.metric import MetricSchema
 from extrap.util.caching import cached_property
 from extrap.util.serialization_schema import Schema
 
@@ -21,14 +24,15 @@
 class Model:
 
     def __init__(self, hypothesis, callpath=None, metric=None):
         self.hypothesis: Hypothesis = hypothesis
         self.callpath = callpath
         self.metric = metric
         self.measurements: Optional[List[Measurement]] = None
+        self.annotations: list[Annotation] = []
 
     @cached_property
     def predictions(self):
         coordinates = numpy.array([m.coordinate for m in self.measurements])
         return self.hypothesis.function.evaluate(coordinates.transpose())
 
     def __eq__(self, other):
@@ -49,10 +53,17 @@
 
     @post_load
     def report_progress(self, data, **kwargs):
         if 'progress_bar' in self.context:
             self.context['progress_bar'].update()
         return data
 
+    @pre_dump
+    def report_progress(self, data, **kwargs):
+        if 'progress_bar' in self.context:
+            self.context['progress_bar'].update()
+        return data
+
     hypothesis = fields.Nested(HypothesisSchema)
     callpath = fields.Nested(CallpathSchema)
     metric = fields.Nested(MetricSchema)
+    annotations = fields.List(fields.Nested(AnnotationSchema))
```

### Comparing `extrap-4.0.4/extrap/entities/parameter.py` & `extrap-4.1.0a2/extrap/util/caching.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
 # Copyright (c) 2020, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-import itertools
+import sys
 
-from extrap.util.serialization_schema import make_value_schema
+if sys.version_info >= (3, 8):
+    import functools
 
-
-class Parameter:
-    """
-    Counter for global parameter ids
-    """
-    ID_COUNTER = itertools.count()
-
-    def __init__(self, name):
-        self.name = name
-        self.id = next(Parameter.ID_COUNTER)
-
-    def __hash__(self):
-        return hash(self.name)
-
-    def __eq__(self, other):
-        if not isinstance(other, Parameter):
-            return NotImplemented
-        return self is other or self.name == other.name
-
-    def __str__(self):
-        return self.name
-
-    def __repr__(self):
-        return f"Parameter({self.name})"
-
-
-ParameterSchema = make_value_schema(Parameter, 'name')
+    cached_property = functools.cached_property
+else:
+    class cached_property(object):
+        """
+        A property that is cached for later retrieval.
+        """
+
+        def __init__(self, func):
+            self.func = func
+
+        def __get__(self, obj, cls):
+            if obj is None:
+                return self
+
+            value = self.func(obj)
+            obj.__dict__[self.func.__name__] = value
+            return value
```

### Comparing `extrap-4.0.4/extrap/entities/terms.py` & `extrap-4.1.0a2/extrap/entities/terms.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 from marshmallow import fields, validate
 
 from extrap.entities.coordinate import Coordinate
 from extrap.entities.fraction import Fraction
 from extrap.entities.parameter import Parameter
 from extrap.util.serialization_schema import Schema, NumberField
 
+DEFAULT_PARAM_NAMES = (
+    'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l',
+    'm', 'n', 'o')
+
 
 class Term(ABC):
 
     def __init__(self):
         self.coefficient = 1
 
     @abstractmethod
@@ -185,15 +189,15 @@
         for param, term in self.parameter_term_pairs:
             parameter_value = parameter_values[param]
             function_value *= term.evaluate(parameter_value)
         return function_value
 
     def to_string(self, *parameters: Union[Parameter, str, Mapping[int, Union[Parameter, str]]]):
         if len(parameters) == 0:
-            parameters = ('p', 'q', 'r', 's', 't')
+            parameters = DEFAULT_PARAM_NAMES
         elif len(parameters) == 1 and not isinstance(parameters[0], str):
             parameters = parameters[0]
         function_string = str(self.coefficient)
         for param, term in self.parameter_term_pairs:
             function_string += ' * '
             function_string += term.to_string(parameters[param])
         return function_string
```

### Comparing `extrap-4.0.4/extrap/extrap/extrapcmd.py` & `extrap-4.1.0a2/extrap/extrap/extrapcmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,61 +5,58 @@
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import argparse
 import logging
 import os
 import sys
+import warnings
 from itertools import chain
 
 import extrap
 from extrap.fileio import experiment_io
-from extrap.fileio.cube_file_reader2 import read_cube_file
-from extrap.fileio.extrap3_experiment_reader import read_extrap3_experiment
-from extrap.fileio.io_helper import format_output
+from extrap.fileio.experiment_io import ExperimentReader
+from extrap.fileio.file_reader import all_readers
+from extrap.fileio.file_reader.cube_file_reader2 import CubeFileReader2
 from extrap.fileio.io_helper import save_output
-from extrap.fileio.json_file_reader import read_json_file
-from extrap.fileio.talpas_file_reader import read_talpas_file
-from extrap.fileio.text_file_reader import read_text_file
+from extrap.fileio.output import format_output
 from extrap.modelers import multi_parameter
 from extrap.modelers import single_parameter
 from extrap.modelers.abstract_modeler import MultiParameterModeler
 from extrap.modelers.model_generator import ModelGenerator
 from extrap.util.exceptions import RecoverableError
 from extrap.util.options_parser import ModelerOptionsAction, ModelerHelpAction
 from extrap.util.options_parser import SINGLE_PARAMETER_MODELER_KEY, SINGLE_PARAMETER_OPTIONS_KEY
 from extrap.util.progress_bar import ProgressBar
 
 
 def main(args=None, prog=None):
     # argparse
     modelers_list = list(set(k.lower() for k in
                              chain(single_parameter.all_modelers.keys(), multi_parameter.all_modelers.keys())))
-    parser = argparse.ArgumentParser(prog=prog, description=extrap.__description__, add_help=False)
+    parser = argparse.ArgumentParser(prog=prog, description=extrap.__description__, add_help=False,
+                                     formatter_class=WideHelpFormatter)
     positional_arguments = parser.add_argument_group("Positional arguments")
     basic_arguments = parser.add_argument_group("Optional arguments")
     basic_arguments.add_argument('-h', '--help', action='help', default=argparse.SUPPRESS,
                                  help='Show this help message and exit')
 
     basic_arguments.add_argument("--version", action="version", version=extrap.__title__ + " " + extrap.__version__,
                                  help="Show program's version number and exit")
     basic_arguments.add_argument("--log", action="store", dest="log_level", type=str.lower, default='warning',
                                  choices=['debug', 'info', 'warning', 'error', 'critical'],
                                  help="Set program's log level (default: warning)")
 
     input_options = parser.add_argument_group("Input options")
     group = input_options.add_mutually_exclusive_group(required=True)
-    group.add_argument("--cube", action="store_true", default=False, dest="cube", help="Load data from CUBE files")
-    group.add_argument("--text", action="store_true", default=False, dest="text", help="Load data from text files")
-    group.add_argument("--talpas", action="store_true", default=False, dest="talpas",
-                       help="Load data from Talpas data format")
-    group.add_argument("--json", action="store_true", default=False, dest="json",
-                       help="Load data from JSON or JSON Lines file")
-    group.add_argument("--extra-p-3", action="store_true", default=False, dest="extrap3",
-                       help="Load data from Extra-P 3 experiment")
+    for reader in all_readers.values():
+        group.add_argument(reader.CMD_ARGUMENT, action="store_true", default=False, dest=reader.NAME,
+                           help=reader.DESCRIPTION)
+    group.add_argument(ExperimentReader.CMD_ARGUMENT, action="store_true", default=False, dest=ExperimentReader.NAME,
+                       help='Load Extra-P experiment and generate new models')
     input_options.add_argument("--scaling", action="store", dest="scaling_type", default="weak", type=str.lower,
                                choices=["weak", "strong"],
                                help="Set weak or strong scaling when loading data from CUBE files (default: weak)")
 
     modeling_options = parser.add_argument_group("Modeling options")
     modeling_options.add_argument("--median", action="store_true", dest="median",
                                   help="Use median values for computation instead of mean values")
@@ -73,29 +70,35 @@
                                   help="Show help for modeler options and exit",
                                   action=ModelerHelpAction)
 
     output_options = parser.add_argument_group("Output options")
     output_options.add_argument("--out", action="store", metavar="OUTPUT_PATH", dest="out",
                                 help="Specify the output path for Extra-P results")
     output_options.add_argument("--print", action="store", dest="print_type", default="all",
-                                choices=["all", "callpaths", "metrics", "parameters", "functions"],
-                                help="Set which information should be displayed after modeling "
-                                     "(default: all)")
+                                metavar='{all,callpaths,metrics,parameters,functions,FORMAT_STRING}',
+                                help="Set which information should be displayed after modeling. Use one of "
+                                     "{all, callpaths, metrics, parameters, functions} or specify a "
+                                     "formatting string using placeholders "
+                                     f"(see {extrap.__documentation_link__}/output-formatting.md).")
     output_options.add_argument("--save-experiment", action="store", metavar="EXPERIMENT_PATH", dest="save_experiment",
                                 help="Saves the experiment including all models as Extra-P experiment "
                                      "(if no extension is specified, '.extra-p' is appended)")
+    output_options.add_argument("--model-set-name", action="store", metavar="NAME", default='New model',
+                                dest="model_name", type=str,
+                                help="Sets the name of the generated set of models when outputting an "
+                                     "experiment (default: 'New model')")
 
     positional_arguments.add_argument("path", metavar="FILEPATH", type=str, action="store",
                                       help="Specify a file path for Extra-P to work with")
     arguments = parser.parse_args(args)
 
     # set log level
     loglevel = logging.getLevelName(arguments.log_level.upper())
     # set output print type
-    printtype = arguments.print_type.upper()
+    printtype = arguments.print_type
 
     # set log format location etc.
     if loglevel == logging.DEBUG:
         # import warnings
         # warnings.simplefilter('always', DeprecationWarning)
         # check if log file exists and create it if necessary
         # if not os.path.exists("../temp/extrap.log"):
@@ -122,46 +125,36 @@
         print_output = True
         print_path = arguments.out
     else:
         print_output = False
 
     if arguments.path is not None:
         with ProgressBar(desc='Loading file') as pbar:
-            if arguments.cube:
-                # load data from cube files
-                if os.path.isdir(arguments.path):
-                    experiment = read_cube_file(arguments.path, scaling_type)
-                else:
-                    logging.error("The given path is not valid. It must point to a directory.")
-                    sys.exit(1)
-            elif os.path.isfile(arguments.path):
-                if arguments.text:
-                    # load data from text files
-                    experiment = read_text_file(arguments.path, pbar)
-                elif arguments.talpas:
-                    # load data from talpas format
-                    experiment = read_talpas_file(arguments.path, pbar)
-                elif arguments.json:
-                    # load data from json file
-                    experiment = read_json_file(arguments.path, pbar)
-                elif arguments.extrap3:
-                    # load data from Extra-P 3 file
-                    experiment = read_extrap3_experiment(arguments.path, pbar)
-                else:
-                    logging.error("The file format specifier is missing.")
-                    sys.exit(1)
-            else:
-                logging.error("The given file path is not valid.")
-                sys.exit(1)
+            for reader in chain(all_readers.values(), [ExperimentReader]):
+                if getattr(arguments, reader.NAME):
+                    file_reader = reader()
+                    if reader.LOADS_FROM_DIRECTORY:
+                        if os.path.isdir(arguments.path):
+                            if reader is CubeFileReader2:
+                                file_reader.scaling_type = arguments.scaling_type
+                            experiment = file_reader.read_experiment(arguments.path, pbar)
+                        else:
+                            logging.error("The given path is not valid. It must point to a directory.")
+                            sys.exit(1)
+                    elif os.path.isfile(arguments.path):
+                        experiment = file_reader.read_experiment(arguments.path, pbar)
+                    else:
+                        logging.error("The given file path is not valid.")
+                        sys.exit(1)
 
         experiment.debug()
 
         # initialize model generator
         model_generator = ModelGenerator(
-            experiment, modeler=arguments.modeler, use_median=use_median)
+            experiment, modeler=arguments.modeler, name=arguments.model_name, use_median=use_median)
 
         # apply modeler options
         modeler = model_generator.modeler
         if isinstance(modeler, MultiParameterModeler) and arguments.modeler_options:
             # set single-parameter modeler of multi-parameter modeler
             single_modeler = arguments.modeler_options[SINGLE_PARAMETER_MODELER_KEY]
             if single_modeler is not None:
@@ -201,9 +194,21 @@
             save_output(text, print_path)
 
     else:
         logging.error("No file path given to load files.")
         sys.exit(1)
 
 
+class WideHelpFormatter(argparse.ArgumentDefaultsHelpFormatter):
+
+    def __init__(self, *args, **kwargs):
+        try:
+            kwargs['width'] = 100
+            super().__init__(*args, **kwargs)
+        except TypeError:
+            warnings.warn("Wide argparse help formatter failed, falling back.")
+            del kwargs['width']
+            super().__init__(*args, **kwargs)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `extrap-4.0.4/extrap/extrap/extrapgui.py` & `extrap-4.1.0a2/extrap/extrap/extrapgui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import argparse
 import logging
 import sys
 import threading
 import traceback
 import warnings
 
-from PySide2.QtCore import Qt
-from PySide2.QtGui import QPalette, QColor
-from PySide2.QtWidgets import QApplication, QMessageBox, QToolTip
+from PySide6.QtCore import Qt
+from PySide6.QtGui import QPalette, QColor
+from PySide6.QtWidgets import QApplication, QMessageBox, QToolTip
 from matplotlib import font_manager
 
 import extrap
-from extrap.fileio.cube_file_reader2 import read_cube_file
 from extrap.fileio.experiment_io import read_experiment
-from extrap.fileio.extrap3_experiment_reader import read_extrap3_experiment
-from extrap.fileio.json_file_reader import read_json_file
-from extrap.fileio.talpas_file_reader import read_talpas_file
-from extrap.fileio.text_file_reader import read_text_file
+from extrap.fileio.file_reader import all_readers
+from extrap.fileio.file_reader.cube_file_reader2 import CubeFileReader2
 from extrap.gui.MainWidget import MainWidget
 from extrap.util.exceptions import RecoverableError, CancelProcessError
 
 TRACEBACK = logging.DEBUG - 1
 logging.addLevelName(TRACEBACK, 'TRACEBACK')
 
 
@@ -57,15 +54,15 @@
 
     try:
         load_from_command(arguments, window)
     except CancelProcessError:
         pass
 
     if not test:
-        app.exec_()
+        app.exec()
         font_preloader.join()
     else:
         font_preloader.join()
         return window, app
 
 
 def parse_arguments(args=None):
@@ -74,46 +71,39 @@
                         choices=['traceback', 'debug', 'info', 'warning', 'error', 'critical'],
                         help="set program's log level (default: critical)")
     parser.add_argument("--logfile", action="store", dest="log_file",
                         help="set path of log file")
     parser.add_argument("--version", action="version", version=extrap.__title__ + " " + extrap.__version__)
 
     group = parser.add_mutually_exclusive_group(required=False)
-    group.add_argument("--cube", action="store_true", default=False, dest="cube", help="load data from cube files")
-    group.add_argument("--text", action="store_true", default=False, dest="text", help="load data from text files")
-    group.add_argument("--talpas", action="store_true", default=False, dest="talpas",
-                       help="load data from talpas data format")
-    group.add_argument("--json", action="store_true", default=False, dest="json",
-                       help="load data from json or jsonlines file")
-    group.add_argument("--extra-p-3", action="store_true", default=False, dest="extrap3",
-                       help="load data from Extra-P 3 experiment")
+    for reader in all_readers.values():
+        group.add_argument(reader.CMD_ARGUMENT, action="store_true", default=False, dest=reader.NAME,
+                           help=reader.DESCRIPTION)
+
     parser.add_argument("path", metavar="FILEPATH", type=str, action="store", nargs='?',
                         help="specify a file path for Extra-P to work with")
 
     parser.add_argument("--scaling", action="store", dest="scaling_type", default="weak", type=str.lower,
                         choices=["weak", "strong"],
                         help="set weak or strong scaling when loading data from cube files [weak (default), strong]")
     arguments = parser.parse_args(args)
     return arguments
 
 
 def load_from_command(arguments, window):
     if arguments.path:
-        if arguments.text:
-            window.import_file(read_text_file, file_name=arguments.path)
-        elif arguments.json:
-            window.import_file(read_json_file, file_name=arguments.path)
-        elif arguments.talpas:
-            window.import_file(read_talpas_file, file_name=arguments.path)
-        elif arguments.cube:
-            window.import_file(lambda x, y: read_cube_file(x, arguments.scaling_type, y), file_name=arguments.path)
-        elif arguments.extrap3:
-            window.import_file(read_extrap3_experiment, model=False, file_name=arguments.path)
-        else:
-            window.import_file(read_experiment, model=False, file_name=arguments.path)
+        for reader in all_readers.values():
+            if getattr(arguments, reader.NAME):
+                file_reader = reader()
+                if file_reader is CubeFileReader2:
+                    file_reader.scaling_type = arguments.scaling_type
+                window.import_file(file_reader.read_experiment, file_name=arguments.path,
+                                   model=file_reader.GENERATE_MODELS_AFTER_LOAD)
+                return
+        window.import_file(read_experiment, file_name=arguments.path, model=False)
 
 
 def _init_warning_system(window, test=False):
     open_message_boxes = []
     current_warnings = set()
 
     # save old handlers
```

### Comparing `extrap-4.0.4/extrap/fileio/experiment_io.py` & `extrap-4.1.0a2/extrap/fileio/experiment_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import zipfile
+from pathlib import Path
+from typing import Union
 from zipfile import ZipFile
 
 from marshmallow import ValidationError
 
-from extrap.entities.experiment import ExperimentSchema
+from extrap.entities.experiment import ExperimentSchema, Experiment
+from extrap.fileio.file_reader import FileReader
 from extrap.util.exceptions import FileFormatError, RecoverableError
-from extrap.util.progress_bar import DUMMY_PROGRESS
+from extrap.util.progress_bar import DUMMY_PROGRESS, ProgressBar
 
 EXPERIMENT_DATA_FILE = 'experiment.json'
 
 
-def read_experiment(path, progress_bar=DUMMY_PROGRESS):
+def read_experiment(path, progress_bar=DUMMY_PROGRESS) -> Experiment:
     progress_bar.total += 3
     schema = ExperimentSchema()
     schema.set_progress_bar(progress_bar)
     try:
         with ZipFile(path, 'r', allowZip64=True) as file:
             progress_bar.update()
             data = file.read(EXPERIMENT_DATA_FILE).decode("utf-8")
@@ -32,17 +35,33 @@
                 return experiment
             except ValidationError as v_err:
                 raise FileFormatError(str(v_err)) from v_err
     except (IOError, zipfile.BadZipFile) as err:
         raise RecoverableError(str(err)) from err
 
 
+class ExperimentReader(FileReader):
+    NAME = 'experiment'
+    CMD_ARGUMENT = '--experiment'
+    GUI_ACTION = '&Open experiment'
+    DESCRIPTION = 'Load Extra-P experiment'
+    FILTER = 'Experiments (*.extra-p)'
+    GENERATE_MODELS_AFTER_LOAD = False
+
+    def read_experiment(self, path: Union[Path, str], progress_bar: ProgressBar = DUMMY_PROGRESS) -> Experiment:
+        return read_experiment(path, progress_bar)
+
+
 def write_experiment(experiment, path, progress_bar=DUMMY_PROGRESS):
-    progress_bar.total += 3
+    progress_bar.update(0)
+    progress_bar.total += 4
     schema = ExperimentSchema()
+    progress_bar.total += sum((len(m.models) for m in experiment.modelers), 0)
+    schema.set_progress_bar(progress_bar)
+    progress_bar.update()
     try:
         with ZipFile(path, 'w', compression=zipfile.ZIP_DEFLATED, compresslevel=1, allowZip64=True) as file:
             progress_bar.update()
             try:
                 data = schema.dumps(experiment)
                 progress_bar.update()
                 file.writestr(EXPERIMENT_DATA_FILE, data)
```

### Comparing `extrap-4.0.4/extrap/fileio/extrap3_experiment_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/extrap3_experiment_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import copy
 import logging
 import os
 import struct
-from typing import Optional
+from pathlib import Path
+from typing import Optional, Union
 
 from extrap.entities.callpath import Callpath
 from extrap.entities.coordinate import Coordinate
 from extrap.entities.experiment import Experiment
 from extrap.entities.functions import Function, SingleParameterFunction, MultiParameterFunction
 from extrap.entities.hypotheses import Hypothesis
 from extrap.entities.measurement import Measurement
 from extrap.entities.metric import Metric
 from extrap.entities.model import Model
 from extrap.entities.parameter import Parameter
 from extrap.entities.terms import CompoundTerm, SimpleTerm, MultiParameterTerm
 from extrap.fileio import io_helper
+from extrap.fileio.file_reader import FileReader
 from extrap.modelers.model_generator import ModelGenerator
 from extrap.modelers.multi_parameter.multi_parameter_modeler import MultiParameterModeler
 from extrap.modelers.single_parameter.basic import SingleParameterModeler
 from extrap.util.exceptions import FileFormatError
-from extrap.util.progress_bar import DUMMY_PROGRESS
+from extrap.util.progress_bar import DUMMY_PROGRESS, ProgressBar
 
 
 class IoTransaction:
     def __init__(self, m_input_stream):
         self._input_stream = m_input_stream
         self._position = m_input_stream.tell()
         self.__commited = False
@@ -480,130 +482,137 @@
 
 
 def SAFE_RETURN_None(x):
     if x is None:
         raise FileFormatError()
 
 
-class __Ref:
-    def __init__(self, _):
-        self.__ = _
-
-
 class _Mappings:
-    region_mapping = {}
-    region_set = {}
-    callpath_mapping = {}
-    parameter_mapping = {}
-    coordinate_mapping = {}
-
-
-def read_extrap3_experiment(path, progress_bar=DUMMY_PROGRESS):
-    progress_bar.total += os.path.getsize(path)
-    with open(path, "rb") as file:
-        ioHelper = IoHelper(file)
-
-        try:
-            qualifier = ioHelper.readString()
-
-            if qualifier != "EXTRAP_EXPERIMENT":
-                raise FileFormatError("This is not an Extra-P 3 Experiment File. Qualifier was " + str(qualifier))
-        except struct.error as err:
-            raise FileFormatError("This is not an Extra-P 3 Experiment File.") from err
-
-        try:
-            exp = Experiment()
-            id_mappings = _Mappings()
-            versionNumber = ioHelper.readString()
-            prefix = ioHelper.readString()
-            progress_bar.step('Load Extra-P 3 experiment')
-            last_pos = 0
-
-            is_sparse = __Ref(False)
-            while prefix:
-                pos = file.tell()
-                progress_bar.update(pos - last_pos)
-                last_pos = pos
-                # logging.debug("Deserialize " + str(prefix))
-                # noinspection PyNoneFunctionAssignment
-                if prefix == 'Parameter':
-                    p = deserialize_parameter(id_mappings, ioHelper)
-                    exp.add_parameter(p)
-
-                elif prefix == 'Metric':
-                    m = deserialize_metric(ioHelper)
-                    SAFE_RETURN_None(m)
-                    exp.add_metric(m)
-
-                elif prefix == 'Region':
-                    deserialize_region(id_mappings, ioHelper)
-
-                elif prefix == 'Callpath':
-                    c = deserialize_callpath(id_mappings, ioHelper)
-                    SAFE_RETURN_None(c)
-                    exp.add_callpath(c)
-                    progress_bar.total += 100
-
-                elif prefix == 'Coordinate':
-                    c = deserialize_coordinate(exp, id_mappings, ioHelper)
-                    SAFE_RETURN_None(c)
-                    exp.add_coordinate(c)
-
-                elif prefix == 'ModelComment':
-                    deserialize_modelcomment(ioHelper)
-                    # SAFE_RETURN_None(comment)
-                    # exp.addModelComment(comment)
-
-                elif prefix == 'SingleParameterSimpleModelGenerator':
-                    generator = deserialize_SingleParameterSimpleModelGenerator(exp, is_sparse, ioHelper)
-                    SAFE_RETURN_None(generator)
-                    exp.add_modeler(generator)
-
-                elif prefix == 'SingleParameterRefiningModelGenerator':
-                    generator = deserialize_SingleParameterModelGenerator(exp, is_sparse, ioHelper)
-                    SAFE_RETURN_None(generator)
-                    exp.add_modeler(generator)
-
-                elif prefix == 'MultiParameterSimpleModelGenerator':
-                    generator = deserialize_MultiParameterModelGenerator(exp, is_sparse, ioHelper)
-                    SAFE_RETURN_None(generator)
-                    exp.add_modeler(generator)
-
-                elif prefix == 'MultiParameterSparseModelGenerator':
-                    generator = deserialize_MultiParameterModelGenerator(exp, is_sparse, ioHelper)
-                    SAFE_RETURN_None(generator)
-                    exp.add_modeler(generator)
-
-                elif prefix == 'ExperimentPoint':
-                    point = deserialize_ExperimentPoint(exp, id_mappings, ioHelper)
-                    SAFE_RETURN_None(point)
-                    exp.add_measurement(point)
-
-                elif prefix == 'Model':
-                    model, generator_id = deserialize_Model(exp, id_mappings, is_sparse, ioHelper)
-                    SAFE_RETURN_None(model)
-                    exp.modelers[generator_id].models[(model.callpath, model.metric)] = model
-
-                else:
-                    raise FileFormatError("Unknown object: " + prefix + ". Can not load experiment.")
-
+    def __init__(self):
+        self.region_mapping = {}
+        self.region_set = {}
+        self.callpath_mapping = {}
+        self.parameter_mapping = {}
+        self.coordinate_mapping = {}
+
+
+class Extrap3ExperimentFileReader(FileReader):
+    NAME = "extrap3"
+    GUI_ACTION = "Open Extra-P &3 experiment"
+    DESCRIPTION = "Load data from Extra-P 3 (legacy) experiment"
+    CMD_ARGUMENT = "--extra-p-3"
+    GENERATE_MODELS_AFTER_LOAD = False
+
+    class __Ref:
+        def __init__(self, _):
+            self.__ = _
+
+    def read_experiment(self, path: Union[Path, str], progress_bar: ProgressBar = DUMMY_PROGRESS) -> Experiment:
+        progress_bar.total += os.path.getsize(path)
+        with open(path, "rb") as file:
+            ioHelper = IoHelper(file)
+
+            try:
+                qualifier = ioHelper.readString()
+
+                if qualifier != "EXTRAP_EXPERIMENT":
+                    raise FileFormatError("This is not an Extra-P 3 Experiment File. Qualifier was " + str(qualifier))
+            except struct.error as err:
+                raise FileFormatError("This is not an Extra-P 3 Experiment File.") from err
+
+            try:
+                exp = Experiment()
+                id_mappings = _Mappings()
+                versionNumber = ioHelper.readString()
                 prefix = ioHelper.readString()
-        except struct.error as err:
-            raise FileFormatError(str(err)) from err
-
-        pos = file.tell()
-        progress_bar.update(pos - last_pos)
+                progress_bar.step('Load Extra-P 3 experiment')
+                last_pos = 0
 
-        # remove empty modelers
-        exp.modelers = [m for m in exp.modelers if len(m.models) > 0]
-        # add measurements to model
-        for modeler in exp.modelers:
-            for key, model in modeler.models.items():
-                model.measurements = exp.measurements.get(key)
-
-        callpaths = exp.callpaths
-        call_tree = io_helper.create_call_tree(callpaths, progress_bar, True, progress_scale=100)
-        exp.call_tree = call_tree
-
-        io_helper.validate_experiment(exp, progress_bar)
-        # new code
-        return exp
+                is_sparse = Extrap3ExperimentFileReader.__Ref(False)
+                while prefix:
+                    pos = file.tell()
+                    progress_bar.update(pos - last_pos)
+                    last_pos = pos
+                    # logging.debug("Deserialize " + str(prefix))
+                    # noinspection PyNoneFunctionAssignment
+                    if prefix == 'Parameter':
+                        p = deserialize_parameter(id_mappings, ioHelper)
+                        exp.add_parameter(p)
+
+                    elif prefix == 'Metric':
+                        m = deserialize_metric(ioHelper)
+                        SAFE_RETURN_None(m)
+                        exp.add_metric(m)
+
+                    elif prefix == 'Region':
+                        deserialize_region(id_mappings, ioHelper)
+
+                    elif prefix == 'Callpath':
+                        c = deserialize_callpath(id_mappings, ioHelper)
+                        SAFE_RETURN_None(c)
+                        exp.add_callpath(c)
+                        progress_bar.total += 100
+
+                    elif prefix == 'Coordinate':
+                        c = deserialize_coordinate(exp, id_mappings, ioHelper)
+                        SAFE_RETURN_None(c)
+                        exp.add_coordinate(c)
+
+                    elif prefix == 'ModelComment':
+                        deserialize_modelcomment(ioHelper)
+                        # SAFE_RETURN_None(comment)
+                        # exp.addModelComment(comment)
+
+                    elif prefix == 'SingleParameterSimpleModelGenerator':
+                        generator = deserialize_SingleParameterSimpleModelGenerator(exp, is_sparse, ioHelper)
+                        SAFE_RETURN_None(generator)
+                        exp.add_modeler(generator)
+
+                    elif prefix == 'SingleParameterRefiningModelGenerator':
+                        generator = deserialize_SingleParameterModelGenerator(exp, is_sparse, ioHelper)
+                        SAFE_RETURN_None(generator)
+                        exp.add_modeler(generator)
+
+                    elif prefix == 'MultiParameterSimpleModelGenerator':
+                        generator = deserialize_MultiParameterModelGenerator(exp, is_sparse, ioHelper)
+                        SAFE_RETURN_None(generator)
+                        exp.add_modeler(generator)
+
+                    elif prefix == 'MultiParameterSparseModelGenerator':
+                        generator = deserialize_MultiParameterModelGenerator(exp, is_sparse, ioHelper)
+                        SAFE_RETURN_None(generator)
+                        exp.add_modeler(generator)
+
+                    elif prefix == 'ExperimentPoint':
+                        point = deserialize_ExperimentPoint(exp, id_mappings, ioHelper)
+                        SAFE_RETURN_None(point)
+                        exp.add_measurement(point)
+
+                    elif prefix == 'Model':
+                        model, generator_id = deserialize_Model(exp, id_mappings, is_sparse, ioHelper)
+                        SAFE_RETURN_None(model)
+                        exp.modelers[generator_id].models[(model.callpath, model.metric)] = model
+
+                    else:
+                        raise FileFormatError("Unknown object: " + prefix + ". Can not load experiment.")
+
+                    prefix = ioHelper.readString()
+            except struct.error as err:
+                raise FileFormatError(str(err)) from err
+
+            pos = file.tell()
+            progress_bar.update(pos - last_pos)
+
+            # remove empty modelers
+            exp.modelers = [m for m in exp.modelers if len(m.models) > 0]
+            # add measurements to model
+            for modeler in exp.modelers:
+                for key, model in modeler.models.items():
+                    model.measurements = exp.measurements.get(key)
+
+            callpaths = exp.callpaths
+            call_tree = io_helper.create_call_tree(callpaths, progress_bar, True, progress_scale=100)
+            exp.call_tree = call_tree
+
+            io_helper.validate_experiment(exp, progress_bar)
+            # new code
+            return exp
```

### Comparing `extrap-4.0.4/extrap/fileio/io_helper.py` & `extrap-4.1.0a2/extrap/fileio/io_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,69 +19,69 @@
 
 if TYPE_CHECKING:
     from extrap.entities.experiment import Experiment
 
 
 def format_callpaths(experiment):
     """
-    This method formats the ouput so that only the callpaths are shown.
+    This method formats the output so that only the callpaths are shown.
     """
     callpaths = experiment.callpaths
     text = ""
     for callpath_id in range(len(callpaths)):
         callpath = callpaths[callpath_id]
         callpath_string = callpath.name
         text += callpath_string + "\n"
     return text
 
 
 def format_metrics(experiment):
     """
-    This method formats the ouput so that only the metrics are shown.
+    This method formats the output so that only the metrics are shown.
     """
     metrics = experiment.metrics
     text = ""
     for metric_id in range(len(metrics)):
         metric = metrics[metric_id]
         metric_string = metric.name
         text += metric_string + "\n"
     return text
 
 
 def format_parameters(experiment):
     """
-    This method formats the ouput so that only the parameters are shown.
+    This method formats the output so that only the parameters are shown.
     """
     parameters = experiment.parameters
     text = ""
     for parameters_id in range(len(parameters)):
         parameter = parameters[parameters_id]
         parameter_string = parameter.name
         text += parameter_string + "\n"
     return text
 
 
 def format_functions(experiment):
     """
-    This method formats the ouput so that only the functions are shown.
+    This method formats the output so that only the functions are shown.
     """
     modeler = experiment.modelers[0]
     models = modeler.models
     text = ""
     for model in models.values():
         hypothesis = model.hypothesis
         function = hypothesis.function
         function_string = function.to_string(*experiment.parameters)
         text += function_string + "\n"
     return text
 
 
 def format_all(experiment):
     """
-    This method formats the ouput so that all information is shown.
+    This method formats the output so that all information is shown.
     """
     coordinates = experiment.coordinates
     callpaths = experiment.callpaths
     metrics = experiment.metrics
     modeler = experiment.modelers[0]
     text = ""
     for callpath_id in range(len(callpaths)):
@@ -128,15 +128,15 @@
             text += "\t\tRSS: {:.2E}\n".format(rss)
             text += "\t\tAdjusted R^2: {:.2E}\n".format(ar2)
     return text
 
 
 def format_output(experiment, printtype):
     """
-    This method formats the ouput of the modeler to a string that can be printed in the console
+    This method formats the output of the modeler to a string that can be printed in the console
     or to a file. Depending on the given options only parts of the modelers output get printed.
     """
     if printtype == "ALL":
         text = format_all(experiment)
     elif printtype == "CALLPATHS":
         text = format_callpaths(experiment)
     elif printtype == "METRICS":
```

### Comparing `extrap-4.0.4/extrap/fileio/json_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/json_file_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,142 +1,152 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import json
 import logging
 from json.decoder import JSONDecodeError
+from pathlib import Path
+from typing import Union
 
 from extrap.entities.callpath import Callpath
 from extrap.entities.coordinate import Coordinate
 from extrap.entities.experiment import Experiment
 from extrap.entities.measurement import Measurement
 from extrap.entities.metric import Metric
 from extrap.entities.parameter import Parameter
 from extrap.fileio import io_helper
+from extrap.fileio.file_reader import FileReader
+from extrap.fileio.file_reader.jsonlines_file_reader import read_jsonlines_file
 from extrap.fileio.io_helper import create_call_tree
-from extrap.fileio.jsonlines_file_reader import read_jsonlines_file
 from extrap.util.exceptions import FileFormatError
-from extrap.util.progress_bar import DUMMY_PROGRESS
+from extrap.util.progress_bar import DUMMY_PROGRESS, ProgressBar
 
 SCHEMA_URI = ""
 
 
-def read_json_file(path, progress_bar=DUMMY_PROGRESS):
-    # read lines from json file
-    with open(path, "r") as inputfile:
-        try:
-            json_data = json.load(inputfile)
-        except JSONDecodeError as error:
-            inputfile.seek(0)
-            is_jsonlines = any(line.strip().startswith('{') for line in inputfile) and \
-                           all(line.strip().startswith('{') or line.strip() == "" for line in inputfile)
-            if is_jsonlines:
-                return read_jsonlines_file(path, progress_bar=DUMMY_PROGRESS)
-            else:
-                raise FileFormatError(str(error)) from error
-
-    # create an experiment object to save the date loaded from the text file
-    experiment = Experiment()
-
-    if "callpaths" not in json_data:
-        try:
-            _read_new_json_file(experiment, json_data, progress_bar)
-        except KeyError as err:
-            raise FileFormatError(str(err)) from err
-    else:
-        try:
-            _read_legacy_json_file(experiment, json_data, progress_bar)
-        except KeyError as err:
-            raise FileFormatError(str(err)) from err
-
-    call_tree = create_call_tree(experiment.callpaths, progress_bar)
-    experiment.call_tree = call_tree
-
-    io_helper.validate_experiment(experiment, progress_bar)
-
-    return experiment
-
-
-def _read_new_json_file(experiment, json_data, progress_bar):
-    parameter_data = json_data["parameters"]
-    for p in parameter_data:
-        parameter = Parameter(p)
-        experiment.add_parameter(parameter)
-
-    measurements_data = json_data["measurements"]
-    for callpath_name, data in progress_bar(measurements_data.items()):
-        for metric_name, measurements in data.items():
-            for measurement in measurements:
-                coordinate = Coordinate(measurement['point'])
-                experiment.add_coordinate(coordinate)
-                callpath = Callpath(callpath_name)
-                experiment.add_callpath(callpath)
-                metric = Metric(metric_name)
-                experiment.add_metric(metric)
-                measurement = Measurement(coordinate, callpath, metric, measurement['values'])
-                experiment.add_measurement(measurement)
-
-
-def _read_legacy_json_file(experiment, json_data, progress_bar):
-    # read parameters
-    parameter_data = json_data["parameters"]
-    parameter_data = sorted(parameter_data, key=lambda x: x["id"])
-    logging.debug("Number of parameters: " + str(len(parameter_data)))
-    for i, p_data in enumerate(progress_bar(parameter_data)):
-        parameter_name = p_data["name"]
-        parameter = Parameter(parameter_name)
-        experiment.add_parameter(parameter)
-        logging.debug("Parameter " + str(i + 1) + ": " + parameter_name)
-    # read callpaths
-    callpath_data = json_data["callpaths"]
-    callpath_data = sorted(callpath_data, key=lambda x: x["id"])
-    logging.debug("Number of callpaths: " + str(len(callpath_data)))
-    for i, c_data in enumerate(progress_bar(callpath_data)):
-        callpath_name = c_data["name"]
-        callpath = Callpath(callpath_name)
-        experiment.add_callpath(callpath)
-        logging.debug("Callpath " + str(i + 1) + ": " + callpath_name)
-    # read metrics
-    metric_data = json_data["metrics"]
-    metric_data = sorted(metric_data, key=lambda x: x["id"])
-    logging.debug("Number of metrics: " + str(len(metric_data)))
-    for i, m_data in enumerate(progress_bar(metric_data)):
-        metric_name = m_data["name"]
-        metric = Metric(metric_name)
-        experiment.add_metric(metric)
-        logging.debug("Metric " + str(i + 1) + ": " + metric_name)
-    # read coordinates
-    coordinate_data = json_data["coordinates"]
-    coordinate_data = sorted(coordinate_data, key=lambda x: x["id"])
-    logging.debug("Number of coordinates: " + str(len(coordinate_data)))
-    for i, c_data in enumerate(progress_bar(coordinate_data)):
-        parameter_value_pairs = c_data["parameter_value_pairs"]
-        parameter_value_pairs = sorted(parameter_value_pairs, key=lambda x: x["parameter_id"])
-        coordinate = Coordinate(float(p["parameter_value"]) for p in parameter_value_pairs)
-        experiment.add_coordinate(coordinate)
-        logging.debug(f"Coordinate {i + 1}: {coordinate}")
-    aggregate_data = {}
-    # read measurements
-    measurements_data = json_data["measurements"]
-    logging.debug("Number of measurements: " + str(len(measurements_data)))
-    for i, m_data in enumerate(progress_bar(measurements_data)):
-        coordinate_id = int(m_data["coordinate_id"]) - 1
-        callpath_id = int(m_data["callpath_id"]) - 1
-        metric_id = int(m_data["metric_id"]) - 1
-        value = float(m_data["value"])
-        key = coordinate_id, callpath_id, metric_id
-        if key in aggregate_data:
-            aggregate_data[key].append(value)
+class JsonFileReader(FileReader):
+    NAME = "json"
+    GUI_ACTION = "Open &JSON input"
+    DESCRIPTION = "Load data from JSON or JSON Lines input file"
+    FILTER = "JSON (Lines) Files (*.json *.jsonl);;All Files (*)"
+    CMD_ARGUMENT = "--json"
+
+    def read_experiment(self, path: Union[Path, str], progress_bar: ProgressBar = DUMMY_PROGRESS) -> Experiment:
+        # read lines from json file
+        with open(path, "r") as inputfile:
+            try:
+                json_data = json.load(inputfile)
+            except JSONDecodeError as error:
+                inputfile.seek(0)
+                is_jsonlines = any(line.strip().startswith('{') for line in inputfile) and \
+                               all(line.strip().startswith('{') or line.strip() == "" for line in inputfile)
+                if is_jsonlines:
+                    return read_jsonlines_file(path, progress_bar=DUMMY_PROGRESS)
+                else:
+                    raise FileFormatError(str(error)) from error
+
+        # create an experiment object to save the date loaded from the text file
+        experiment = Experiment()
+
+        if "callpaths" not in json_data:
+            try:
+                self._read_new_json_file(experiment, json_data, progress_bar)
+            except KeyError as err:
+                raise FileFormatError(str(err)) from err
         else:
-            aggregate_data[key] = [value]
-    for key in progress_bar(aggregate_data):
-        coordinate_id, callpath_id, metric_id = key
-        coordinate = experiment.coordinates[coordinate_id]
-        callpath = experiment.callpaths[callpath_id]
-        metric = experiment.metrics[metric_id]
-        values = aggregate_data[key]
-        measurement = Measurement(coordinate, callpath, metric, values)
-        experiment.add_measurement(measurement)
+            try:
+                self._read_legacy_json_file(experiment, json_data, progress_bar)
+            except KeyError as err:
+                raise FileFormatError(str(err)) from err
+
+        call_tree = create_call_tree(experiment.callpaths, progress_bar)
+        experiment.call_tree = call_tree
+
+        io_helper.validate_experiment(experiment, progress_bar)
+
+        return experiment
+
+    @staticmethod
+    def _read_new_json_file(experiment, json_data, progress_bar):
+        parameter_data = json_data["parameters"]
+        for p in parameter_data:
+            parameter = Parameter(p)
+            experiment.add_parameter(parameter)
+
+        measurements_data = json_data["measurements"]
+        for callpath_name, data in progress_bar(measurements_data.items()):
+            for metric_name, measurements in data.items():
+                for measurement in measurements:
+                    coordinate = Coordinate(measurement['point'])
+                    experiment.add_coordinate(coordinate)
+                    callpath = Callpath(callpath_name)
+                    experiment.add_callpath(callpath)
+                    metric = Metric(metric_name)
+                    experiment.add_metric(metric)
+                    measurement = Measurement(coordinate, callpath, metric, measurement['values'])
+                    experiment.add_measurement(measurement)
+
+    @staticmethod
+    def _read_legacy_json_file(experiment, json_data, progress_bar):
+        # read parameters
+        parameter_data = json_data["parameters"]
+        parameter_data = sorted(parameter_data, key=lambda x: x["id"])
+        logging.debug("Number of parameters: " + str(len(parameter_data)))
+        for i, p_data in enumerate(progress_bar(parameter_data)):
+            parameter_name = p_data["name"]
+            parameter = Parameter(parameter_name)
+            experiment.add_parameter(parameter)
+            logging.debug("Parameter " + str(i + 1) + ": " + parameter_name)
+        # read callpaths
+        callpath_data = json_data["callpaths"]
+        callpath_data = sorted(callpath_data, key=lambda x: x["id"])
+        logging.debug("Number of callpaths: " + str(len(callpath_data)))
+        for i, c_data in enumerate(progress_bar(callpath_data)):
+            callpath_name = c_data["name"]
+            callpath = Callpath(callpath_name)
+            experiment.add_callpath(callpath)
+            logging.debug("Callpath " + str(i + 1) + ": " + callpath_name)
+        # read metrics
+        metric_data = json_data["metrics"]
+        metric_data = sorted(metric_data, key=lambda x: x["id"])
+        logging.debug("Number of metrics: " + str(len(metric_data)))
+        for i, m_data in enumerate(progress_bar(metric_data)):
+            metric_name = m_data["name"]
+            metric = Metric(metric_name)
+            experiment.add_metric(metric)
+            logging.debug("Metric " + str(i + 1) + ": " + metric_name)
+        # read coordinates
+        coordinate_data = json_data["coordinates"]
+        coordinate_data = sorted(coordinate_data, key=lambda x: x["id"])
+        logging.debug("Number of coordinates: " + str(len(coordinate_data)))
+        for i, c_data in enumerate(progress_bar(coordinate_data)):
+            parameter_value_pairs = c_data["parameter_value_pairs"]
+            parameter_value_pairs = sorted(parameter_value_pairs, key=lambda x: x["parameter_id"])
+            coordinate = Coordinate(float(p["parameter_value"]) for p in parameter_value_pairs)
+            experiment.add_coordinate(coordinate)
+            logging.debug(f"Coordinate {i + 1}: {coordinate}")
+        aggregate_data = {}
+        # read measurements
+        measurements_data = json_data["measurements"]
+        logging.debug("Number of measurements: " + str(len(measurements_data)))
+        for i, m_data in enumerate(progress_bar(measurements_data)):
+            coordinate_id = int(m_data["coordinate_id"]) - 1
+            callpath_id = int(m_data["callpath_id"]) - 1
+            metric_id = int(m_data["metric_id"]) - 1
+            value = float(m_data["value"])
+            key = coordinate_id, callpath_id, metric_id
+            if key in aggregate_data:
+                aggregate_data[key].append(value)
+            else:
+                aggregate_data[key] = [value]
+        for key in progress_bar(aggregate_data):
+            coordinate_id, callpath_id, metric_id = key
+            coordinate = experiment.coordinates[coordinate_id]
+            callpath = experiment.callpaths[callpath_id]
+            metric = experiment.metrics[metric_id]
+            values = aggregate_data[key]
+            measurement = Measurement(coordinate, callpath, metric, values)
+            experiment.add_measurement(measurement)
```

### Comparing `extrap-4.0.4/extrap/fileio/jsonlines_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/jsonlines_file_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import json
 import os
 from json import JSONDecodeError
```

### Comparing `extrap-4.0.4/extrap/fileio/talpas_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/talpas_file_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import json
 import os
 from json import JSONDecodeError
+from pathlib import Path
+from typing import Union
 
 from extrap.entities.callpath import Callpath
 from extrap.entities.coordinate import Coordinate
 from extrap.entities.experiment import Experiment
 from extrap.entities.metric import Metric
 from extrap.entities.parameter import Parameter
 from extrap.fileio import io_helper
+from extrap.fileio.file_reader import FileReader
 from extrap.fileio.io_helper import create_call_tree
 from extrap.util.exceptions import FileFormatError
-from extrap.util.progress_bar import DUMMY_PROGRESS
+from extrap.util.progress_bar import DUMMY_PROGRESS, ProgressBar
 
 
-def read_talpas_file(path, progress_bar=DUMMY_PROGRESS):
-    # create an experiment object to save the date loaded from the text file
-    experiment = Experiment()
-
-    complete_data = {}
-    parameters = None
-
-    progress_bar.total += os.path.getsize(path)
-    # read talpas file into complete_data
-    with open(path) as file:
-
-        progress_bar.step('Reading file')
-        for ln, line in enumerate(file):
-            progress_bar.update(len(line))
-            if line.isspace():
-                continue
-            line = line.replace(';', ',')
-
-            try:
-                data = json.loads(line)
-            except JSONDecodeError as error:
-                raise FileFormatError(f'Decoding of line {ln} failed: {str(error).replace(",", ";")}. Line: "{line}"')
-            try:
-                key = Callpath(data['callpath']), Metric(data['metric'])
-                if parameters is None:
-                    parameters = [Parameter(p) for p in data['parameters'].keys()]
-                coordinate = Coordinate(data['parameters'][p.name] for p in parameters)
-                io_helper.append_to_repetition_dict(complete_data, key, coordinate, data['value'], progress_bar)
-            except KeyError as error:
-                raise FileFormatError(f'Missing property in line {ln}: {str(error)}. Line: "{line}"')
-
-    # create experiment
-    io_helper.repetition_dict_to_experiment(complete_data, experiment, progress_bar)
-
-    for p in parameters:
-        experiment.add_parameter(p)
+class TalpasFileReader(FileReader):
+    NAME = "talpas"
+    GUI_ACTION = "Open Tal&pas input"
+    DESCRIPTION = "Load data from Talpas data format"
+    FILTER = "Talpas Files (*.txt);;All Files (*)"
+    CMD_ARGUMENT = "--talpas"
+
+    def read_experiment(self, path: Union[Path, str], progress_bar: ProgressBar = DUMMY_PROGRESS) -> Experiment:
+        # create an experiment object to save the date loaded from the text file
+        experiment = Experiment()
+
+        complete_data = {}
+        parameters = None
+
+        progress_bar.total += os.path.getsize(path)
+        # read talpas file into complete_data
+        with open(path) as file:
+
+            progress_bar.step('Reading file')
+            for ln, line in enumerate(file):
+                progress_bar.update(len(line))
+                if line.isspace():
+                    continue
+                line = line.replace(';', ',')
+
+                try:
+                    data = json.loads(line)
+                except JSONDecodeError as error:
+                    raise FileFormatError(
+                        f'Decoding of line {ln} failed: {str(error).replace(",", ";")}. Line: "{line}"')
+                try:
+                    key = Callpath(data['callpath']), Metric(data['metric'])
+                    if parameters is None:
+                        parameters = [Parameter(p) for p in data['parameters'].keys()]
+                    coordinate = Coordinate(data['parameters'][p.name] for p in parameters)
+                    io_helper.append_to_repetition_dict(complete_data, key, coordinate, data['value'], progress_bar)
+                except KeyError as error:
+                    raise FileFormatError(f'Missing property in line {ln}: {str(error)}. Line: "{line}"')
+
+        # create experiment
+        io_helper.repetition_dict_to_experiment(complete_data, experiment, progress_bar)
+
+        for p in parameters:
+            experiment.add_parameter(p)
 
-    call_tree = create_call_tree(experiment.callpaths, progress_bar)
-    experiment.call_tree = call_tree
+        call_tree = create_call_tree(experiment.callpaths, progress_bar)
+        experiment.call_tree = call_tree
 
-    io_helper.validate_experiment(experiment, progress_bar)
+        io_helper.validate_experiment(experiment, progress_bar)
 
-    return experiment
+        return experiment
```

### Comparing `extrap-4.0.4/extrap/fileio/text_file_reader.py` & `extrap-4.1.0a2/extrap/fileio/file_reader/text_file_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,149 +1,159 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import re
+from pathlib import Path
+from typing import Union
 
 from extrap.entities.callpath import Callpath
 from extrap.entities.coordinate import Coordinate
 from extrap.entities.experiment import Experiment
 from extrap.entities.measurement import Measurement
 from extrap.entities.metric import Metric
 from extrap.entities.parameter import Parameter
 from extrap.fileio import io_helper
+from extrap.fileio.file_reader import FileReader
 from extrap.fileio.io_helper import create_call_tree
 from extrap.util.exceptions import FileFormatError
-from extrap.util.progress_bar import DUMMY_PROGRESS
+from extrap.util.progress_bar import DUMMY_PROGRESS, ProgressBar
 
 re_whitespace = re.compile(r'\s+')
 
 
-def read_text_file(path, progress_bar=DUMMY_PROGRESS):
-    # read text file into list
-    with open(path) as file:
-        lines = file.readlines()
-
-    # remove empty lines
-    lines_no_space = [l for l in lines if not l.isspace()]
-
-    # remove line breaks
-    lines_no_space = [l.replace("\n", "") for l in lines_no_space]
-
-    # create an experiment object to save the date loaded from the text file
-    experiment = Experiment()
-
-    # variables for parsing
-    number_parameters = 0
-    last_metric = None
-    last_callpath = Callpath("")
-    coordinate_id = 0
-
-    if len(lines_no_space) == 0:
-        raise FileFormatError(f'File contains no data: "{path}"')
-
-    # parse text to extrap objects
-    for i, line in enumerate(progress_bar(lines)):
-        if line.isspace() or line.startswith('#'):
-            continue  # allow comments
-        line = re_whitespace.sub(' ', line)
-        # get field name
-        field_separator_idx = line.find(" ")
-        field_name = line[:field_separator_idx]
-        field_value = line[field_separator_idx + 1:].strip()
-
-        if field_name == "METRIC":
-            # create a new metric if not already exists
-            metric_name = field_value
-            test_metric = Metric(metric_name)
-            if test_metric not in experiment.metrics:
-                metric = test_metric
-                experiment.add_metric(metric)
-                last_metric = metric
+class TextFileReader(FileReader):
+    NAME = "text"
+    GUI_ACTION = "Open &text input"
+    DESCRIPTION = "Load data from text input file"
+    FILTER = "Text Files (*.txt);;All Files (*)"
+    CMD_ARGUMENT = "--text"
+
+    def read_experiment(self, path: Union[Path, str], progress_bar: ProgressBar = DUMMY_PROGRESS) -> Experiment:
+        # read text file into list
+        with open(path) as file:
+            lines = file.readlines()
+
+        # remove empty lines
+        lines_no_space = [l for l in lines if not l.isspace()]
+
+        # remove line breaks
+        lines_no_space = [l.replace("\n", "") for l in lines_no_space]
+
+        # create an experiment object to save the date loaded from the text file
+        experiment = Experiment()
+
+        # variables for parsing
+        number_parameters = 0
+        last_metric = None
+        last_callpath = Callpath("")
+        coordinate_id = 0
+
+        if len(lines_no_space) == 0:
+            raise FileFormatError(f'File contains no data: "{path}"')
+
+        # parse text to extrap objects
+        for i, line in enumerate(progress_bar(lines)):
+            if line.isspace() or line.startswith('#'):
+                continue  # allow comments
+            line = re_whitespace.sub(' ', line)
+            # get field name
+            field_separator_idx = line.find(" ")
+            field_name = line[:field_separator_idx]
+            field_value = line[field_separator_idx + 1:].strip()
+
+            if field_name == "METRIC":
+                # create a new metric if not already exists
+                metric_name = field_value
+                test_metric = Metric(metric_name)
+                if test_metric not in experiment.metrics:
+                    metric = test_metric
+                    experiment.add_metric(metric)
+                    last_metric = metric
+                else:
+                    for metric in experiment.metrics:
+                        if metric == test_metric:
+                            last_metric = metric
+                            break
+                # reset the coordinate id, since moving to a new region
+                coordinate_id = 0
+
+            elif field_name == "REGION":
+                # create a new region if not already exists
+                callpath_name = field_value
+
+                callpath = Callpath(callpath_name)
+                experiment.add_callpath(callpath)
+                last_callpath = callpath
+
+                # reset the coordinate id, since moving to a new region
+                coordinate_id = 0
+
+            elif field_name == "DATA":
+                if last_metric is None:
+                    last_metric = Metric("")
+                # create a new data set
+                data_string = field_value
+                data_list = data_string.split(" ")
+                values = [float(d) for d in data_list]
+                if 1 <= number_parameters <= 4:
+                    # create one measurement per repetition
+
+                    if coordinate_id >= len(experiment.coordinates):
+                        raise FileFormatError(
+                            f'To many DATA lines ({coordinate_id}) for the number of POINTS '
+                            f'({len(experiment.coordinates)}) in line {i}.')
+                    measurement = Measurement(
+                        experiment.coordinates[coordinate_id], last_callpath, last_metric, values)
+                    experiment.add_measurement(measurement)
+                    coordinate_id += 1
+                elif number_parameters >= 5:
+                    raise FileFormatError("This input format supports a maximum of 4 parameters.")
+                else:
+                    raise FileFormatError("This file has no parameters.")
+
+            elif field_name == "PARAMETER":
+                # create a new parameter
+                parameters = field_value.split(' ')
+                experiment.parameters += [Parameter(p) for p in parameters]
+                number_parameters = len(experiment.parameters)
+
+            elif field_name == "POINTS":
+                coordinate_string = field_value.strip()
+                if '(' in coordinate_string:
+                    coordinate_string = coordinate_string.replace(") (", ")(")
+                    coordinate_string = coordinate_string[1:-1]
+                    coordinate_strings = coordinate_string.split(')(')
+                else:
+                    coordinate_strings = coordinate_string.split(' ')
+                # create a new point
+                if number_parameters == 1:
+                    coordinates = [Coordinate(float(c))
+                                   for c in coordinate_strings]
+                    experiment.coordinates.extend(coordinates)
+                elif 1 < number_parameters < 5:
+                    for coordinate_string in coordinate_strings:
+                        coordinate_string = coordinate_string.strip()
+                        values = coordinate_string.split(" ")
+                        coordinate = Coordinate(float(v) for v in values)
+                        experiment.coordinates.append(coordinate)
+                elif number_parameters >= 5:
+                    raise FileFormatError("This input format supports a maximum of 4 parameters.")
+                else:
+                    raise FileFormatError("This file has no parameters.")
             else:
-                for metric in experiment.metrics:
-                    if metric == test_metric:
-                        last_metric = metric
-                        break
-            # reset the coordinate id, since moving to a new region
-            coordinate_id = 0
-
-        elif field_name == "REGION":
-            # create a new region if not already exists
-            callpath_name = field_value
-
-            callpath = Callpath(callpath_name)
-            experiment.add_callpath(callpath)
-            last_callpath = callpath
-
-            # reset the coordinate id, since moving to a new region
-            coordinate_id = 0
-
-        elif field_name == "DATA":
-            if last_metric is None:
-                last_metric = Metric("")
-            # create a new data set
-            data_string = field_value
-            data_list = data_string.split(" ")
-            values = [float(d) for d in data_list]
-            if 1 <= number_parameters <= 4:
-                # create one measurement per repetition
-
-                if coordinate_id >= len(experiment.coordinates):
-                    raise FileFormatError(
-                        f'To many DATA lines ({coordinate_id}) for the number of POINTS '
-                        f'({len(experiment.coordinates)}) in line {i}.')
-                measurement = Measurement(
-                    experiment.coordinates[coordinate_id], last_callpath, last_metric, values)
-                experiment.add_measurement(measurement)
-                coordinate_id += 1
-            elif number_parameters >= 5:
-                raise FileFormatError("This input format supports a maximum of 4 parameters.")
-            else:
-                raise FileFormatError("This file has no parameters.")
+                raise FileFormatError(f'Encountered wrong field: "{field_name}" in line {i}: {line}')
 
-        elif field_name == "PARAMETER":
-            # create a new parameter
-            parameters = field_value.split(' ')
-            experiment.parameters += [Parameter(p) for p in parameters]
-            number_parameters = len(experiment.parameters)
-
-        elif field_name == "POINTS":
-            coordinate_string = field_value.strip()
-            if '(' in coordinate_string:
-                coordinate_string = coordinate_string.replace(") (", ")(")
-                coordinate_string = coordinate_string[1:-1]
-                coordinate_strings = coordinate_string.split(')(')
-            else:
-                coordinate_strings = coordinate_string.split(' ')
-            # create a new point
-            if number_parameters == 1:
-                coordinates = [Coordinate(float(c))
-                               for c in coordinate_strings]
-                experiment.coordinates.extend(coordinates)
-            elif 1 < number_parameters < 5:
-                for coordinate_string in coordinate_strings:
-                    coordinate_string = coordinate_string.strip()
-                    values = coordinate_string.split(" ")
-                    coordinate = Coordinate(float(v) for v in values)
-                    experiment.coordinates.append(coordinate)
-            elif number_parameters >= 5:
-                raise FileFormatError("This input format supports a maximum of 4 parameters.")
-            else:
-                raise FileFormatError("This file has no parameters.")
-        else:
-            raise FileFormatError(f'Encountered wrong field: "{field_name}" in line {i}: {line}')
-
-    if last_metric == Metric(''):
-        experiment.metrics.append(last_metric)
-    if last_metric == Callpath(''):
-        experiment.callpaths.append(last_callpath)
-    # create the call tree and add it to the experiment
-    call_tree = create_call_tree(experiment.callpaths, progress_bar, progress_scale=10)
-    experiment.call_tree = call_tree
+        if last_metric == Metric(''):
+            experiment.metrics.append(last_metric)
+        if last_metric == Callpath(''):
+            experiment.callpaths.append(last_callpath)
+        # create the call tree and add it to the experiment
+        call_tree = create_call_tree(experiment.callpaths, progress_bar, progress_scale=10)
+        experiment.call_tree = call_tree
 
-    io_helper.validate_experiment(experiment, progress_bar)
+        io_helper.validate_experiment(experiment, progress_bar)
 
-    return experiment
+        return experiment
```

### Comparing `extrap-4.0.4/extrap/gui/AdvancedPlotWidget.py` & `extrap-4.1.0a2/extrap/gui/AdvancedPlotWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
 
 #####################################################################
 
 
 class AdvancedPlotWidget(QWidget):
@@ -116,8 +116,8 @@
 
 
 class MyCustomToolbar(NavigationToolbar):
     """This class represents a Toolbar that is used to show the x,y, z value
        and save the figure.
     """
     toolitems = [toolitem for toolitem in NavigationToolbar.toolitems if
-                 toolitem[0] in ('Home1', 'Save')]
+                 toolitem[0] in ('Home', 'Save')]
```

### Comparing `extrap-4.0.4/extrap/gui/ColorWidget.py` & `extrap-4.1.0a2/extrap/gui/ColorWidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-from PySide2.QtCore import *
-from PySide2.QtGui import *  # @UnusedWildImport
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtCore import *
+from PySide6.QtGui import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
 from extrap.gui.Utils import formatNumber
 
 
 class ColorWidget(QWidget):
 
     def __init__(self):
@@ -67,15 +67,17 @@
             interpolate = (value - 0.75) * 4
             return QColor(255, int(255 - interpolate * 255), 0)
 
     def drawColors(self, paint):
 
         rect_width = self.frameGeometry().width()
         rect_height = self.frameGeometry().height()
-        (mleft, mtop, mright, mbottom) = self.getContentsMargins()
+
+        cm = self.contentsMargins()
+        mleft, mtop, mright, mbottom = cm.left(), cm.top(), cm.right(), cm.bottom()
 
         for position in range(mleft, rect_width - mright):
             ratio = float(position) / rect_width
             color = self.getColor(ratio)
             paint.setPen(color)
             paint.setBrush(color)
             paint.drawRect(position, mtop, 1, rect_height - mbottom - mtop)
```

### Comparing `extrap-4.0.4/extrap/gui/CubeFileReader.py` & `extrap-4.1.0a2/extrap/gui/CubeFileReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from functools import partial
 from threading import Event
 
-from PySide2.QtCore import *  # @UnusedWildImport
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtCore import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
-from extrap.fileio.cube_file_reader2 import read_cube_file
+from extrap.fileio.file_reader.cube_file_reader2 import CubeFileReader2
 from extrap.util.exceptions import CancelProcessError
 from extrap.util.progress_bar import ProgressBar
 
 
 class ParameterWidget(QWidget):
 
     def __init__(self, parent):
@@ -229,15 +229,15 @@
         with ProgressBar(total=0, gui=True) as pbar:
             self._show_progressbar()
             pbar.display = partial(self._display_progress, pbar)
             pbar.sp = None
 
             # read the cube files
             try:
-                self.experiment = read_cube_file(self.dir_name, self.scaling_type, pbar)
+                self.experiment = CubeFileReader2().read_cube_file(self.dir_name, self.scaling_type, pbar)
             except Exception as err:
                 self.close()
                 raise err
 
             if not self.experiment:
                 QMessageBox.critical(self,
                                      "Error",
```

### Comparing `extrap-4.0.4/extrap/gui/DataDisplay.py` & `extrap-4.1.0a2/extrap/gui/DataDisplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from collections import defaultdict
 
-from PySide2.QtCore import *  # @UnusedWildImport
-from PySide2.QtGui import *  # @UnusedWildImport
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtCore import *  # @UnusedWildImport
+from PySide6.QtGui import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
 from extrap.entities.parameter import Parameter
 from extrap.gui.AdvancedPlotWidget import AdvancedPlotWidget
 from extrap.gui.GraphWidget import GraphWidget
 from extrap.gui.plots.AllFunctionsAsDifferentSurfacePlotWidget import AllFunctionsAsDifferentSurfacePlot
 from extrap.gui.plots.AllFunctionsAsOneSurfacePlotWidget import AllFunctionsAsOneSurfacePlot
 from extrap.gui.plots.DominatingFunctionsAsSingleScatterPlotWidget import DominatingFunctionsAsSingleScatterPlot
 from extrap.gui.plots.HeatMapGraphWidget import HeatMapGraph
 from extrap.gui.plots.InterpolatedContourDisplayWidget import InterpolatedContourDisplay
 from extrap.gui.plots.IsolinesDisplayWidget import IsolinesDisplay
 from extrap.gui.plots.MaxZAsSingleSurfacePlotWidget import MaxZAsSingleSurfacePlot
 from extrap.gui.plots.MeasurementPointsPlotWidget import MeasurementPointsPlot
-
 #####################################################################
 MIN_PARAM_VALUE = 0.01
 MAX_PARAM_VALUE = 2000000000
 
 
 class AxisSelection(QWidget):
-    ''' This class is a helper class for the class DataDisplay.
+    """ This class is a helper class for the class DataDisplay.
         It represents one parameter in the data display which
         shown on one of the graph axis. It allows to set the maximum
         value for the axis in the graph.
-    '''
+    """
     #####################################################################
 
     max_values = [10, 10, 10]
 
     def __init__(self, manager, parent, index: int, parameters):
         super(AxisSelection, self).__init__(parent)
         self.manager = manager
@@ -62,14 +61,15 @@
             label1 = QLabel("Axis " + str(self.index))
         label1.setMinimumWidth(75)
         self.combo_box = QComboBox(self)
         # self.combo_box.setMinimumWidth( 75 )
         self.combo_box.setMinimumHeight(20)
         for i in range(0, len(parameters)):
             self.combo_box.addItem(parameters[i].name)
+        self.combo_box.setEnabled(self.index < len(parameters))
         self.combo_box.setCurrentIndex(self.index)
 
         self.combo_box.currentIndexChanged.connect(self.parameter_selected)
 
         label2 = QLabel("max.")
         label2.setMinimumWidth(40)
         label2.setAlignment(Qt.AlignRight | Qt.AlignVCenter)
@@ -96,32 +96,32 @@
         self.show()
 
     def updateDisplay(self):
         display = self.manager.display_widget.currentWidget()
         display.setMax(self.index, self.max_edit.value())
 
     def max_changed(self):
-        ''' This function should only be called from the connected event
+        """ This function should only be called from the connected event
             when the user has entered a new value.
             Otherwise use maxChanged() which does not update the graph drawing.
             This is to avoid multiple updates of the graph.
-        '''
+        """
         self.maxChanged()
         display = self.manager.display_widget.currentWidget()
         if isinstance(display, GraphWidget):
             display.update()
         else:
             display.drawGraph()
             display.update()
 
     def maxChanged(self):
-        ''' This function updates the max value without redrawing the graph.
+        """ This function updates the max value without redrawing the graph.
             Use this function from external calls to avoid multiple redraws
             of the graph.
-        '''
+        """
         if self.max_edit.value() == 0:
             self.max_edit.setValue(self.max_edit.minimum())
             return
         display = self.manager.display_widget.currentWidget()
 
         if self.index <= 2:
             AxisSelection.max_values[self.index] = self.max_edit.value()
@@ -195,15 +195,15 @@
         label2 = QLabel("Value:")
         label2.setMinimumWidth(40)
         label2.setAlignment(Qt.AlignRight | Qt.AlignVCenter)
 
         self.value_edit = QDoubleSpinBox()
         self.value_edit.setMinimum(MIN_PARAM_VALUE)
         self.value_edit.setMaximum(MAX_PARAM_VALUE)
-        self.value_edit.setValue(self.default_values[self.parameter])
+        self.value_edit.setValue(float(self.default_values[self.parameter]))
         self.value_edit.setMinimumHeight(25)
         self.value_edit.valueChanged.connect(self._value_changed)
 
         self.grid.addWidget(label0, 0, 0)
         self.grid.addWidget(self.parameter_label, 0, 1)
         self.grid.addWidget(label2, 0, 2, Qt.AlignRight)
         self.grid.addWidget(self.value_edit, 0, 3)
@@ -289,15 +289,15 @@
         self.display_widget.tabsClosable()
         self.display_widget.currentChanged.connect(self.experimentChange)
         self.show()
 
     def closeTab(self, currentIndex):
         self.display_widget.removeTab(currentIndex)
 
-    def ifTabAlreadyOpened(self, text):
+    def is_tab_already_opened(self, text):
         tabStatus = False
         tabCount = self.display_widget.count()
         for index in range(0, tabCount):
             if text == self.display_widget.tabText(index):
                 tabStatus = True
 
         return tabStatus
@@ -310,15 +310,15 @@
         # 4: MaxZAsSingleSurfacePlotWidget
         # 5: HeatMapGraphWidget,
         # 6: IsolinesDisplayWidget
         # 7: InterpolatedContourDisplayWidget
         # 8: Measurement Points
         if 0 in selectedCheckBoxesIndex:
             labelText = "Line graph"
-            tabStatus = self.ifTabAlreadyOpened(labelText)
+            tabStatus = self.is_tab_already_opened(labelText)
             if tabStatus is False:
                 graph = GraphWidget(self.main_widget, self)
                 self.display_widget.addTab(graph, labelText)
 
         graph_widgets = {
             1: ('Single surface plot', AllFunctionsAsOneSurfacePlot),
             2: ('Surface plots', AllFunctionsAsDifferentSurfacePlot),
@@ -330,15 +330,15 @@
             8: ("Measurement points", MeasurementPointsPlot)
         }
 
         for i in selectedCheckBoxesIndex:
             if i == 0:
                 continue
             labelText, plot = graph_widgets[i]
-            if not self.ifTabAlreadyOpened(labelText):
+            if not self.is_tab_already_opened(labelText):
                 advance_plot_widget = AdvancedPlotWidget(
                     self.main_widget, self, plot)
                 self.display_widget.addTab(
                     advance_plot_widget, labelText)
 
     def experimentChange(self):
         experiment = self.main_widget.getExperiment()
```

### Comparing `extrap-4.0.4/extrap/gui/ExpanderWidget.py` & `extrap-4.1.0a2/extrap/gui/components/ExpanderWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import sys
 
-from PySide2.QtCore import Qt, Slot
-from PySide2.QtWidgets import QToolButton, QSizePolicy, QWidget, QGroupBox, QVBoxLayout, QApplication
+from PySide6.QtCore import Qt, Slot
+from PySide6.QtWidgets import QToolButton, QSizePolicy, QWidget, QGroupBox, QVBoxLayout, QApplication
 
 
 class ExpanderWidget(QGroupBox):
     def __init__(self, parent, title, content=None):
         super(ExpanderWidget, self).__init__(parent)
         self._title = title
         self._toggle = QToolButton(self)
```

### Comparing `extrap-4.0.4/extrap/gui/GraphWidget.py` & `extrap-4.1.0a2/extrap/gui/GraphWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from __future__ import annotations
 
 import math
 import typing
 
 import numpy
-from PySide2.QtCore import *  # @UnusedWildImport
-from PySide2.QtGui import *  # @UnusedWildImport
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtCore import *  # @UnusedWildImport
+from PySide6.QtGui import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
 from extrap.gui.Utils import formatFormula
 from extrap.gui.Utils import formatNumber
 
 if typing.TYPE_CHECKING:
     from extrap.gui.MainWidget import MainWidget
 
@@ -111,46 +111,46 @@
         self.clicked_x_pos = None
         self.clicked_y_pos = None
 
         # colors
         self.BACKGROUND_COLOR = QColor("white")
         self.TEXT_COLOR = QColor("black")
         self.AXES_COLOR = QColor("black")
-        self.AGGREGATE_MODEL_COLOR = QColor(self.main_widget.graph_color_list[0])
-        self.DATA_POINT_COLOR = QColor(self.main_widget.graph_color_list[0]).darker(200)
-        self.DATA_RANGE_COLOR = QColor(self.main_widget.graph_color_list[0]).darker(150)
+        self.AGGREGATE_MODEL_COLOR = QColor(self.main_widget.model_color_map.default_color)
+        self.DATA_POINT_COLOR = QColor(self.main_widget.model_color_map.default_color).darker(200)
+        self.DATA_RANGE_COLOR = QColor(self.main_widget.model_color_map.default_color).darker(150)
 
         self.minimum_number_points_marked = 2
         self.aggregate_callpath = False
         self.datapoints_type = ""
 
         self.datapointType_Int_Map = {
             'min': 1, 'mean': 2, 'max': 3, 'median': 4, 'standardDeviation': 5, 'outlier': 6}
 
     @property
     def show_datapoints(self):
         return not self.combine_all_callpath and self.datapoints_type != ''
 
     @property
     def combine_all_callpath(self):
-        return self.aggregate_callpath and len(self.main_widget.getSelectedCallpath()) > 1
+        return self.aggregate_callpath and len(self.main_widget.get_selected_call_tree_nodes()) > 1
 
     @Slot(QPoint)
     def showContextMenu(self, point):
         """
           This function takes care of different options and their visibility in the context menu.
         """
 
-        # selected_metric = self.main_widget.getSelectedMetric()
-        selected_callpaths = self.main_widget.getSelectedCallpath()
+        # selected_metric = self.main_widget.get_selected_metric()
+        selected_callpaths = self.main_widget.get_selected_call_tree_nodes()
 
         if not selected_callpaths:
             return
 
-        menu = QMenu()
+        menu = QMenu(self)
         points_group = QActionGroup(self)
         points_group.setEnabled(not self.combine_all_callpath)
 
         data_point_selection = [
             # To show data points for mean values
             ("Show Mean Points", 'mean'),
             # To show data points for min values
@@ -223,16 +223,16 @@
           This function shows all callpaths.
         """
         self.aggregate_callpath = False
         self.update()
 
     @Slot()
     def screenshot(self):
-        selected_callpaths = self.main_widget.getSelectedCallpath()
-        selected_metric = self.main_widget.getSelectedMetric()
+        selected_callpaths = self.main_widget.get_selected_call_tree_nodes()
+        selected_metric = self.main_widget.get_selected_metric()
 
         name_addition = "-"
         if selected_metric:
             name_addition = f"-{selected_metric}-"
         if selected_callpaths:
             name_addition += ','.join((c.name for c in selected_callpaths))
 
@@ -240,51 +240,32 @@
 
     @Slot()
     def exportData(self):
         """
           This function allows to export the currently shown points and functions in a text format
         """
 
-        selected_metric = self.main_widget.getSelectedMetric()
-        selected_callpaths = self.main_widget.getSelectedCallpath()
-
-        if not selected_callpaths:
-            return
-
-        # model_list = list()
-
         text = ''
-
-        model_set = self.main_widget.getCurrentModel()
-        if model_set is None:
+        models, _ = self.main_widget.get_selected_models()
+        if models is None:
             return
-        model_set_models = model_set.models
-        if not model_set_models:
-            return
-
-        for selected_callpath in selected_callpaths:
-            model = model_set_models[selected_callpath.path, selected_metric]
-            if model is None:
-                return
-            model_function = model.hypothesis.function
-            data_points = [p for (_, p) in self.calculateDataPoints(
-                selected_metric, selected_callpath, True)]
-            callpath_name = selected_callpath.name
 
-            parameters = self.main_widget.experiment.parameters
+        for model in models:
+            callpath_name = model.callpath.name
+            data_points = [p for (_, p) in self.calculateDataPoints(model, True)]
+            parameters = self.main_widget.getExperiment().parameters
             model_function_text = 'Model: ' + \
                                   formatFormula(
-                                      model_function.to_string(*parameters))
+                                      model.hypothesis.function.to_string(*parameters))
 
             data_points_text = '\n'.join(
                 ('(' + str(x) + ', ' + str(y) + ')') for (x, y) in data_points)
-            text += callpath_name + '\n' + data_points_text + \
-                    '\n' + model_function_text + '\n\n'
+            text += callpath_name + '\n' + data_points_text + '\n' + model_function_text + '\n\n'
 
-        msg = QMessageBox()
+        msg = QMessageBox(self)
         msg.setIcon(QMessageBox.Information)
         msg.setText(
             "Exported data (text can be copied to the clipboard using the context menu):")
         msg.setInformativeText(text)
         msg.setWindowTitle("Export Data")
         # msg.setDetailedText("The details are as follows:")
         msg.setStandardButtons(QMessageBox.Ok)
@@ -292,82 +273,63 @@
 
     def drawGraph(self, paint):
         """
             This function is being called by paintEvent to draw the graph
         """
 
         # Get data
-        model_set = self.main_widget.getCurrentModel()
-        selected_metric = self.main_widget.getSelectedMetric()
-        selected_callpaths = self.main_widget.getSelectedCallpath()
-        if not selected_callpaths or model_set is None:
-            return
-
-        model_set_models = model_set.models
-        if not model_set_models:
+        model_list, selected_call_nodes = self.main_widget.get_selected_models()
+        if not model_list:
             return
 
-        model_list = list()
-        selected_callpaths_checked=[]
-        for selected_callpath in selected_callpaths:
-            key = (selected_callpath.path, selected_metric)
-            if key in model_set_models:
-                model = model_set_models[key]
-                model_list.append(model)
-                selected_callpaths_checked.append(selected_callpath)
-
-
         # Calculate geometry constraints
         self.graph_width = self.frameGeometry().width() - self.left_margin - self.right_margin
         self.graph_height = self.frameGeometry().height() - self.top_margin - self.bottom_margin
         y = self.calculateMaxY(model_list) * 1.2
         self.max_y = y
 
         # Draw coordinate system
-        self.drawAxis(paint, selected_metric)
+        self.drawAxis(paint, self.main_widget.get_selected_metric())
 
         # Draw functionss
         index_indicator = 0
         if not self.combine_all_callpath:
-            for model in model_list:
-                color = self.main_widget.getColorForCallPath(
-                    selected_callpaths_checked[index_indicator])
+            for model, call_node in zip(model_list, selected_call_nodes):
+                color = self.main_widget.model_color_map[call_node]
                 self.drawModel(paint, model, color)
-                index_indicator = index_indicator + 1
         else:
-            color = self.main_widget.getColorForCallPath(selected_callpaths_checked[0])
+            # main_widget = self.main_widget
+            # color = main_widget.model_color_map[selected_call_nodes[0]]
             self.drawAggregratedModel(paint, model_list)
 
         # Draw data points
-        self.drawDataPoints(paint, selected_metric, selected_callpaths_checked)
+        self.drawDataPoints(paint, model_list)
 
         # Draw legend
         self.drawLegend(paint)
 
-    def drawDataPoints(self, paint, selectedMetric, selectedCallpaths):
+    def drawDataPoints(self, paint, selected_models):
         if self.show_datapoints is True:
             pen = QPen(self.DATA_POINT_COLOR)
             pen.setWidth(4)
             paint.setPen(pen)
             # data_points_list = list()
-            for selected_callpath in selectedCallpaths:
+            for selected_model in selected_models:
                 if self.datapoints_type == "outlier":
-                    self.showOutlierPoints(
-                        paint, selectedMetric, selected_callpath)
+                    self.showOutlierPoints(paint, selected_model)
 
                 else:
-                    data_points = self.calculateDataPoints(
-                        selectedMetric, selected_callpath)
-                    self.plotPointsOnGraph(
-                        paint, data_points)
+                    data_points = self.calculateDataPoints(selected_model)
+                    self.plotPointsOnGraph(paint, data_points)
 
     def drawLegend(self, paint):
         # drawing the graph legend
         px_between = 15
-        callpath_color_dict = self.main_widget.get_callpath_color_map()
+        widget = self.main_widget
+        callpath_color_dict = widget.model_color_map
         dict_size = len(callpath_color_dict)
         font_size = int(self.main_widget.getFontSize())
         paint.setFont(QFont('Decorative', font_size))
         paint.setBrush(self.BACKGROUND_COLOR)
         pen = QPen(self.TEXT_COLOR)
         pen.setWidth(1)
         paint.setPen(pen)
@@ -607,15 +569,15 @@
                      for x, y in cord_list_before_filtering
                      if not math.isnan(y) and 0 <= y)
         return cord_list
 
     def _calculate_evaluation_points(self, length_x_axis):
         number_of_x_points = int(length_x_axis / 2)
         x_values = numpy.linspace(0, self.max_x, number_of_x_points)
-        x_list = numpy.ndarray((len(self.main_widget.experiment.parameters), number_of_x_points))
+        x_list = numpy.ndarray((len(self.main_widget.getExperiment().parameters), number_of_x_points))
         param = self.main_widget.data_display.getAxisParameter(0).id
         parameter_value_list = self.main_widget.data_display.getValues()
         for i, val in parameter_value_list.items():
             x_list[i] = numpy.repeat(val, number_of_x_points)
         x_list[param] = x_values
         return number_of_x_points, x_list, x_values
 
@@ -675,19 +637,19 @@
         """ This function formats and beautify the number to be shown on the graph.
         """
         splitted_value = value.split('e')
         first_part = float(splitted_value[0])
         first_part = round(first_part, 2)
         return '{:g}'.format(float(first_part)) + "e" + ''.join(splitted_value[1])
 
-    def calculateDataPoints(self, selectedMetric, selectedCallpath, ignore_limit=False):
+    def calculateDataPoints(self, model, ignore_limit=False):
         """ This function calculates datapoints to be marked on the graph
         """
 
-        datapoints = self.main_widget.getCurrentModel().models[(selectedCallpath.path, selectedMetric)].measurements
+        datapoints = model.measurements
         parameter_datapoint = self.main_widget.data_display.getAxisParameter(0).id
         datapoint_x_absolute_pos_list = list()
         datapoint_y_absolute_pos_list = list()
         datapoint_x_list = list()
         datapoint_y_list = list()
 
         if self.datapoints_type == "min":
@@ -782,17 +744,16 @@
         numpy.seterr(**previous)
         # Ensure that the maximum value is never too small
         if y_max < 0.000001:
             y_max = 1
 
         return y_max
 
-    def showOutlierPoints(self, paint, selectedMetric, selectedCallpath):
-        model_set = self.main_widget.getCurrentModel()
-        datapoints = model_set.models[(selectedCallpath.path, selectedMetric)].measurements
+    def showOutlierPoints(self, paint, selected_model):
+        datapoints = selected_model.measurements
         parameter_datapoint = self.main_widget.data_display.getAxisParameter(0).id
         for datapoint in datapoints:
             x_value = datapoint.coordinate[parameter_datapoint]
             if x_value <= self.max_x:
                 y_min_value = datapoint.minimum
                 y_max_value = datapoint.maximum
                 y_mean_value = datapoint.mean
```

### Comparing `extrap-4.0.4/extrap/gui/LogWidget.py` & `extrap-4.1.0a2/extrap/gui/LogWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import logging
 
-import PySide2
-from PySide2.QtGui import QPaintEvent
-from PySide2.QtWidgets import QWidget, QGridLayout, QTextEdit
+import PySide6
+from PySide6.QtGui import QPaintEvent
+from PySide6.QtWidgets import QWidget, QGridLayout, QTextEdit
 
 
 class LogWidget(QWidget):
     def __init__(self, parent):
         super(LogWidget, self).__init__(parent)
         self.log_box = QTextEdit(self)
         self.initUI()
@@ -22,25 +22,25 @@
         handler.setLevel(logging.INFO)
         handler.setFormatter(logging.Formatter("%(levelname)s: %(message)s"))
         logging.getLogger().addHandler(handler)
 
     def initUI(self):
         layout = QGridLayout(self)
         # layout.setContentsMargins(10, 5, 10, 5)
-        layout.setMargin(0)
+        #layout.setMargin(0, 0, 0, 0)
         self.setLayout(layout)
         layout.addWidget(self.log_box)
         self.log_box.setAcceptRichText(True)
         self.log_box.setReadOnly(True)
         self.log_box.setLineWrapMode(QTextEdit.LineWrapMode.NoWrap)
         self.log_box.setStyleSheet("QTextEdit{"
                                    "background-color:white;"
                                    "}")
 
-    def showEvent(self, event: PySide2.QtGui.QShowEvent):
+    def showEvent(self, event: PySide6.QtGui.QShowEvent):
         self._reset_scrollbars()
         super().showEvent(event)
 
     def write(self, text):
         if text.startswith('WARNING:'):
             text = '<span style="color:#DF6F0F">' + text + '</span>'
         elif text.startswith('ERROR:'):
```

### Comparing `extrap-4.0.4/extrap/gui/MainWidget.py` & `extrap-4.1.0a2/extrap/gui/MainWidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import signal
+import sys
 from enum import Enum
 from functools import partial
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Sequence, Tuple
 
-from PySide2.QtCore import *  # @UnusedWildImport
-from PySide2.QtGui import *  # @UnusedWildImport
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtCore import *  # @UnusedWildImport
+from PySide6.QtGui import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
 import extrap
+from extrap.entities.calltree import Node
+from extrap.entities.experiment import Experiment
+from extrap.entities.model import Model
 from extrap.fileio.experiment_io import read_experiment, write_experiment
-from extrap.fileio.extrap3_experiment_reader import read_extrap3_experiment
-from extrap.fileio.json_file_reader import read_json_file
-from extrap.fileio.talpas_file_reader import read_talpas_file
-from extrap.fileio.text_file_reader import read_text_file
+from extrap.fileio.file_reader import all_readers
+from extrap.fileio.file_reader.cube_file_reader2 import CubeFileReader2
 from extrap.gui.ColorWidget import ColorWidget
 from extrap.gui.CubeFileReader import CubeFileReader
 from extrap.gui.DataDisplay import DataDisplayManager, GraphLimitsWidget
 from extrap.gui.LogWidget import LogWidget
 from extrap.gui.ModelerWidget import ModelerWidget
 from extrap.gui.PlotTypeSelector import PlotTypeSelector
-from extrap.gui.ProgressWindow import ProgressWindow
+from extrap.gui.components.ProgressWindow import ProgressWindow
 from extrap.gui.SelectorWidget import SelectorWidget
+from extrap.gui.components import file_dialog
+from extrap.gui.components.model_color_map import ModelColorMap
 from extrap.modelers.model_generator import ModelGenerator
 
+DEFAULT_MODEL_NAME = "Default Model"
+
 
 class CallPathEnum(Enum):
     constant = "constant"
     logarithmic = "logarithmic"
     polynomial = "polynomial"
     exponential = "exponential"
 
@@ -42,37 +48,37 @@
 class MainWidget(QMainWindow):
 
     def __init__(self, *args, **kwargs):
         """
         Initializes the extrap application widget.
         """
         super(MainWidget, self).__init__(*args, **kwargs)
-        self.max_value = 1
-        self.min_value = 1
+        self.max_value = 0
+        self.min_value = 0
         self.old_x_pos = 0
-        self.experiment = None
-        self.graph_color_list = ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728',
-                                 '#9467bd', '#8c564b', '#e377c2', '#7f7f7f',
-                                 '#bcbd22', '#17becf']
-        # ['#8B0000', '#00008B', '#006400', '#2F4F4F', '#8B4513', '#556B2F',
-        #  '#808000', '#008080', '#FF00FF', '#800000', '#FF0000', '#000080', '#008000', '#00FFFF', '#800080']
+        self._experiment = None
+        self.model_color_map = ModelColorMap()
         self.font_size = 6
         self.experiment_change = True
         self.initUI()
         signal.signal(signal.SIGINT, signal.SIG_DFL)
 
         # switch for using mean or median measurement values for modeling
         # is used when loading the data from a file and then modeling directly
         self.median = False
 
+        if sys.platform.startswith('darwin'):
+            self._macos_update_title_bar()
+
     # noinspection PyAttributeOutsideInit
     def initUI(self):
         """
         Initializes the User Interface of the extrap widget. E.g. the menus.
         """
+
         self.setWindowTitle(extrap.__title__)
         # Status bar
         # self.statusBar()
 
         # Main splitter
         self.setCorner(Qt.BottomRightCorner, Qt.RightDockWidgetArea)
         self.setCorner(Qt.BottomLeftCorner, Qt.LeftDockWidgetArea)
@@ -94,15 +100,14 @@
         self.modeler_widget = ModelerWidget(self, dock)
         dock.setWidget(self.modeler_widget)
         self.addDockWidget(Qt.RightDockWidgetArea, dock)
 
         # bottom widget
         dock = QDockWidget("Color Info", self)
         self.color_widget = ColorWidget()
-        self.color_widget.update_min_max(self.min_value, self.max_value)
         dock.setWidget(self.color_widget)
         self.addDockWidget(Qt.LeftDockWidgetArea, dock)
 
         dock = QDockWidget("Graph Limits", self)
         self.graph_limits_widget = GraphLimitsWidget(self, self.data_display)
         dock.setWidget(self.graph_limits_widget)
         self.addDockWidget(Qt.BottomDockWidgetArea, dock, Qt.Horizontal)
@@ -121,29 +126,24 @@
         screenshot_action.triggered.connect(self.screenshot)
 
         exit_action = QAction('E&xit', self)
         exit_action.setShortcut(QKeySequence.Quit)
         exit_action.setStatusTip('Exit application')
         exit_action.triggered.connect(self.close)
 
-        file_imports = [
-            ('Open set of &CUBE files', 'Open a set of CUBE files for single-parameter models and generate data points '
-                                        'for a new experiment from them', self.open_cube_file),
-            ('Open &text input', 'Open text input file',
-             self._make_import_func('Open a Text Input File', read_text_file,
-                                    filter="Text Files (*.txt);;All Files (*)")),
-            ('Open &JSON input', 'Open JSON or JSON Lines input file',
-             self._make_import_func('Open a JSON or JSON Lines Input File', read_json_file,
-                                    filter="JSON (Lines) Files (*.json *.jsonl);;All Files (*)")),
-            ('Open Tal&pas input', 'Open Talpas input file',
-             self._make_import_func('Open a Talpas Input File', read_talpas_file,
-                                    filter="Talpas Files (*.txt);;All Files (*)")),
-            ('Open Extra-P &3 experiment', 'Opens legacy experiment file',
-             self._make_import_func('Open an Extra-P 3 Experiment', read_extrap3_experiment, model=False))
-        ]
+        file_imports = []
+        for reader in all_readers.values():
+            if reader is CubeFileReader2:
+                file_imports.append((reader.GUI_ACTION, reader.DESCRIPTION, self.open_cube_file))
+            else:
+                file_mode = QFileDialog.FileMode.Directory if reader.LOADS_FROM_DIRECTORY else None
+                file_imports.append((reader.GUI_ACTION, reader.DESCRIPTION,
+                                     self._make_import_func(reader.DESCRIPTION, reader().read_experiment,
+                                                            filter=reader.FILTER, file_mode=file_mode,
+                                                            model=reader.GENERATE_MODELS_AFTER_LOAD)))
 
         open_experiment_action = QAction('&Open experiment', self)
         open_experiment_action.setStatusTip('Opens experiment file')
         open_experiment_action.setShortcut(QKeySequence.Open)
         open_experiment_action.triggered.connect(self.open_experiment)
 
         save_experiment_action = QAction('&Save experiment', self)
@@ -180,14 +180,22 @@
         model_delete_action.triggered.connect(self.selector_widget.model_delete)
 
         model_rename_action = QAction('&Rename model', self)
         model_rename_action.setShortcut('Ctrl+R')
         model_rename_action.setStatusTip('Rename the current model')
         model_rename_action.triggered.connect(self.selector_widget.model_rename)
 
+        metric_delete_action = QAction('Dele&te metrics', self)
+        metric_delete_action.triggered.connect(self.selector_widget.delete_metric)
+
+        # compare menu
+        compare_action = QAction('&Compare with experiment', self)
+        compare_action.setStatusTip('Compare the current models with ')
+        compare_action.triggered.connect(self.selector_widget.model_delete)
+
         # Filter menu
         # filter_callpath_action = QAction('Filter Callpaths', self)
         # filter_callpath_action.setShortcut('Ctrl+F')
         # filter_callpath_action.setStatusTip('Select the callpath you want to hide')
         # filter_callpath_action.triggered.connect(self.hide_callpath_dialog_box)
 
         # Main menu bar
@@ -219,14 +227,16 @@
         plots_menu = menubar.addMenu('&Plots')
         for g in graph_actions:
             plots_menu.addAction(g)
 
         model_menu = menubar.addMenu('&Model')
         model_menu.addAction(model_delete_action)
         model_menu.addAction(model_rename_action)
+        model_menu.addSeparator()
+        model_menu.addAction(metric_delete_action)
 
         # filter_menu = menubar.addMenu('Filter')
         # filter_menu.addAction(filter_callpath_action)
 
         # Help menue
         help_menu = menubar.addMenu('&Help')
 
@@ -240,35 +250,29 @@
 
         # Main window
         self.resize(1200, 800)
         self.setCentralWidget(central_widget)
         self.experiment_change = False
         self.show()
 
-    def setExperiment(self, experiment):
+    def set_experiment(self, experiment, file_name="", *, compared=False):
+        if experiment is None:
+            raise ValueError("Experiment cannot be none.")
         self.experiment_change = True
-        self.experiment = experiment
-        self.selector_widget.updateModelList()
-        self.selector_widget.fillMetricList()
-        self.selector_widget.createParameterSliders()
-        self.selector_widget.fillCalltree()
-
-        self.selector_widget.tree_model.valuesChanged()
+        self._experiment = experiment
+        self._set_opened_file_name(file_name, compared=compared)
+        self.save_experiment_action.setEnabled(True)
+        self.selector_widget.on_experiment_changed()
         self.data_display.experimentChange()
         self.modeler_widget.experimentChanged()
         self.experiment_change = False
         self.updateMinMaxValue()
         self.update()
 
-    def updateAllWidget(self):
-        if not self.experiment_change:
-            self.data_display.updateWidget()
-            self.update()
-
-    def metricIndexChanged(self):
+    def on_selection_changed(self):
         if not self.experiment_change:
             self.data_display.updateWidget()
             self.update()
             self.updateMinMaxValue()
 
     def keyPressEvent(self, e):
         if e.key() == Qt.Key_Escape:
@@ -283,26 +287,29 @@
         msg_box.setDefaultButton(QMessageBox.No)
 
         if msg_box.exec_() == QMessageBox.Yes:
             event.accept()
         else:
             event.ignore()
 
-    def getExperiment(self):
-        return self.experiment
+    def getExperiment(self) -> Experiment:
+        return self._experiment
 
-    def getSelectedMetric(self):
+    def get_selected_metric(self):
         return self.selector_widget.getSelectedMetric()
 
-    def getSelectedCallpath(self):
-        return self.selector_widget.getSelectedCallpath()
+    def get_selected_call_tree_nodes(self) -> Sequence[Node]:
+        return self.selector_widget.get_selected_call_tree_nodes()
 
-    def getCurrentModel(self) -> Optional[ModelGenerator]:
+    def get_current_model_gen(self) -> Optional[ModelGenerator]:
         return self.selector_widget.getCurrentModel()
 
+    def get_selected_models(self) -> Tuple[Optional[Sequence[Model]], Optional[Sequence[Node]]]:
+        return self.selector_widget.get_selected_models()
+
     def open_font_dialog_box(self):
         fontSizeItems = list()
         for i in range(4, 9, +1):
             fontSizeItems.append(str(i))
 
         fontSize, ok = QInputDialog.getItem(
             self, "Font Size", "Select the font size:", fontSizeItems, 0, False, Qt.Sheet)
@@ -341,147 +348,107 @@
             with ProgressWindow(self, "Saving Screenshot"):
                 image.save(file_name)
 
         initial_path = Path(self.windowFilePath()).stem + name_addition
         file_filter = ';;'.join(
             [f"{str(f, 'utf-8').upper()} image (*.{str(f, 'utf-8')})" for f in QImageWriter.supportedImageFormats() if
              str(f, 'utf-8') not in ['icns', 'cur', 'ico']])
-        dialog = self._file_dialog(_save, "Save Screenshot", initial_path,
-                                   file_filter, accept_mode=QFileDialog.AcceptSave)
+        dialog = file_dialog.showSave(self, _save, "Save Screenshot", initial_path, file_filter)
         dialog.selectNameFilter("PNG image (*.png)")
 
-    def model_experiment(self, experiment):
+    def model_experiment(self, experiment, file_name=""):
         # initialize model generator
-        model_generator = ModelGenerator(experiment, use_median=self.median, name="Default Model")
+        model_generator = ModelGenerator(experiment, use_median=self.median, name=DEFAULT_MODEL_NAME)
         with ProgressWindow(self, 'Modeling') as pbar:
             # create models from data
             model_generator.model_all(pbar)
-        self.setExperiment(experiment)
+        self.set_experiment(experiment, file_name)
 
     def _make_import_func(self, title, reader_func, **kwargs):
         return partial(self.import_file, reader_func, title, **kwargs)
 
     def import_file(self, reader_func, title='Open File', filter='', model=True, progress_text="Loading File",
-                    file_name=None):
+                    file_name=None, file_mode=None):
         def _import_file(file_name):
             with ProgressWindow(self, progress_text) as pw:
                 experiment = reader_func(file_name, pw)
-                self._set_opened_file_name(file_name)
                 # call the modeler and create a function model
                 if model:
-                    self.model_experiment(experiment)
+                    self.model_experiment(experiment, file_name)
                 else:
-                    self.setExperiment(experiment)
+                    self.set_experiment(experiment, file_name)
 
         if file_name:
             _import_file(file_name)
         else:
-            self._file_dialog(_import_file, title, filter=filter)
-
-    def _file_dialog(self, on_accept, caption='', directory='', filter='', file_mode=None,
-                     accept_mode=QFileDialog.AcceptOpen):
-        if file_mode is None:
-            file_mode = QFileDialog.ExistingFile if accept_mode == QFileDialog.AcceptOpen else QFileDialog.AnyFile
-        f_dialog = QFileDialog(self, caption, directory, filter)
-        f_dialog.setAcceptMode(accept_mode)
-        f_dialog.setFileMode(file_mode)
-
-        def _on_accept():
-            file_list = f_dialog.selectedFiles()
-            if file_list:
-                if len(file_list) > 1:
-                    on_accept(file_list)
-                else:
-                    on_accept(file_list[0])
-
-        f_dialog.accepted.connect(_on_accept)
-        f_dialog.open()
-        return f_dialog
+            file_dialog.show(self, _import_file, title, filter=filter, file_mode=file_mode)
 
-    def _set_opened_file_name(self, file_name):
+    def _set_opened_file_name(self, file_name, *, compared=False):
         if file_name:
-            self.save_experiment_action.setEnabled(True)
-            self.setWindowFilePath(file_name)
+            self.setWindowFilePath(file_name if not compared else "")
             self.setWindowTitle(Path(file_name).name + " – " + extrap.__title__)
-
         else:
-            self.save_experiment_action.setEnabled(False)
             self.setWindowFilePath("")
             self.setWindowTitle(extrap.__title__)
 
-    def open_experiment(self):
+    def open_experiment(self, file_name=None):
         self.import_file(read_experiment, 'Open Experiment',
                          filter='Experiments (*.extra-p)',
                          model=False,
-                         progress_text="Loading experiment")
+                         progress_text="Loading experiment",
+                         file_name=file_name)
 
     def save_experiment(self):
         def _save(file_name):
             with ProgressWindow(self, "Saving Experiment") as pw:
                 write_experiment(self.getExperiment(), file_name, pw)
                 self._set_opened_file_name(file_name)
 
-        self._file_dialog(_save,
-                          'Save Experiment', filter='Experiments (*.extra-p)', accept_mode=QFileDialog.AcceptSave)
+        file_dialog.showSave(self, _save, 'Save Experiment', filter='Experiments (*.extra-p)')
 
     def open_cube_file(self):
         def _process_cube(dir_name):
             dialog = CubeFileReader(self, dir_name)
             dialog.setWindowFlag(Qt.Sheet, True)
             dialog.setModal(True)
             dialog.exec_()  # do not use open, wait for loading to finish
             if dialog.valid:
-                self._set_opened_file_name(dir_name)
-                self.model_experiment(dialog.experiment)
+                self.model_experiment(dialog.experiment, dir_name)
 
-        self._file_dialog(_process_cube,
-                          'Select a Directory with a Set of CUBE Files', "", file_mode=QFileDialog.Directory)
+        file_dialog.showOpenDirectory(self, _process_cube, 'Select a Directory with a Set of CUBE Files')
 
     def updateMinMaxValue(self):
         if not self.experiment_change:
-            updated_value_list = self.selector_widget.getMinMaxValue()
-            # don't allow values < 0
-            updated_max_value = max(0.0, max(updated_value_list))
-            updated_min_value = max(0.0, min(updated_value_list))
-            self.min_value = updated_min_value
-            self.max_value = updated_max_value
-            self.color_widget.update_min_max(self.min_value, self.max_value)
-
-    def populateCallPathColorMap(self, call_tree_nodes):
-        metric = self.selector_widget.getSelectedMetric()
-        call_tree_nodes = [c for c in set(call_tree_nodes) if (c.path, metric) in self.selector_widget.getCurrentModel().models]
-        current_index = 0
-        size_of_color_list = len(self.graph_color_list)
-        self.dict_callpath_color = {}
-        for callpath in call_tree_nodes:
-            if current_index < size_of_color_list:
-                self.dict_callpath_color[callpath] = self.graph_color_list[current_index]
-            else:
-                offset = (current_index - size_of_color_list) % size_of_color_list
-                multiple = int(current_index / size_of_color_list)
-                color = self.graph_color_list[offset]
-                newcolor = color[:-1] + str(multiple)
-                self.dict_callpath_color[callpath] = newcolor
-            current_index = current_index + 1
+            self.color_widget.update_min_max(*self.selector_widget.update_min_max_value())
 
     def show_about_dialog(self):
         QMessageBox.about(self, "About " + extrap.__title__,
                           f"""<h1>{extrap.__title__}</h1>
 <p>Version {extrap.__version__}</p>
 <p>{extrap.__description__}</p>
 <p>{extrap.__copyright__}</p>
-"""
-                          )
-
-    def getColorForCallPath(self, callpath):
-        return self.dict_callpath_color[callpath]
-
-    def get_callpath_color_map(self):
-        return self.dict_callpath_color
+""")
 
     activate_event_handlers = []
 
     def event(self, e: QEvent) -> bool:
-        if e.type() == QEvent.WindowActivate:
+        if e.type() == QEvent.Type.WindowActivate:
             for h in self.activate_event_handlers:
                 h(e)
+        elif e.type() == QEvent.Type.LayoutRequest or e.type() == QEvent.Type.WinIdChange:
+            if sys.platform.startswith('darwin'):
+                self._macos_update_title_bar()
         return super().event(e)
+
+    def _macos_update_title_bar(self):
+        try:
+            import objc
+            from AppKit import NSWindow, NSView, NSColor, NSColorSpace
+            ns_view = objc.objc_object(c_void_p=int(self.winId()))
+            ns_window = ns_view.window()
+            ns_window.setTitlebarAppearsTransparent_(True)
+            ns_window.setColorSpace_(NSColorSpace.sRGBColorSpace())
+            c = self.palette().window().color()
+            ns_window_color = NSColor.colorWithDeviceRed_green_blue_alpha_(c.redF(), c.greenF(), c.blueF(), c.alphaF())
+            ns_window.setBackgroundColor_(ns_window_color)
+        except ImportError:
+            pass
```

### Comparing `extrap-4.0.4/extrap/gui/ModelerOptionsWidget.py` & `extrap-4.1.0a2/extrap/gui/ModelerOptionsWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from typing import Mapping, Collection, cast
 
-from PySide2.QtCore import Qt
-from PySide2.QtWidgets import QWidget, QFormLayout, QLineEdit, QCheckBox, QSpinBox, QDoubleSpinBox, QGroupBox, \
+from PySide6.QtCore import Qt
+from PySide6.QtWidgets import QWidget, QFormLayout, QLineEdit, QCheckBox, QSpinBox, QDoubleSpinBox, QGroupBox, \
     QComboBox, QVBoxLayout, QLabel, QPushButton
 
 from extrap.modelers import single_parameter
 from extrap.modelers.abstract_modeler import AbstractModeler, MultiParameterModeler
 from extrap.modelers.modeler_options import ModelerOption, ModelerOptionsGroup, modeler_options
```

### Comparing `extrap-4.0.4/extrap/gui/ModelerWidget.py` & `extrap-4.1.0a2/extrap/gui/ModelerWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-from PySide2.QtCore import Slot, Qt
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtCore import Slot, Qt
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
-from extrap.gui.ExpanderWidget import ExpanderWidget
+from extrap.gui.components.ExpanderWidget import ExpanderWidget
 from extrap.gui.ModelerOptionsWidget import ModelerOptionsWidget
-from extrap.gui.ProgressWindow import ProgressWindow
+from extrap.gui.components.ProgressWindow import ProgressWindow
 from extrap.modelers import multi_parameter
 from extrap.modelers import single_parameter
 from extrap.modelers.abstract_modeler import AbstractModeler
 from extrap.modelers.model_generator import ModelGenerator
 
 
 class ModelerWidget(QWidget):
```

### Comparing `extrap-4.0.4/extrap/gui/ParameterValueSlider.py` & `extrap-4.1.0a2/extrap/gui/components/ParameterValueSlider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import math
 
-from PySide2.QtCore import *  # @UnusedWildImport
-from PySide2.QtGui import *  # @UnusedWildImport
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtCore import *  # @UnusedWildImport
+from PySide6.QtGui import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
 
 class ParameterValueSlider(QWidget):
     def __init__(self, selectorWidget, parameter, parent):
         super(ParameterValueSlider, self).__init__(parent)
         self.selector_widget = selectorWidget
         self.parameter = parameter
```

### Comparing `extrap-4.0.4/extrap/gui/PlotTypeSelector.py` & `extrap-4.1.0a2/extrap/gui/PlotTypeSelector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
 
 class PlotTypeSelector(QDialog):
 
     def __init__(self, parent, dataDisplay):
         super(PlotTypeSelector, self).__init__(parent)
         self.valid = False
```

### Comparing `extrap-4.0.4/extrap/gui/ProgressWindow.py` & `extrap-4.1.0a2/extrap/gui/components/ProgressWindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from threading import Event
 
-from PySide2.QtCore import Qt, QCoreApplication, Slot
-from PySide2.QtWidgets import QProgressDialog, QLabel
+from PySide6.QtCore import Qt, QCoreApplication, Slot
+from PySide6.QtWidgets import QProgressDialog, QLabel
 
 from extrap.util.exceptions import CancelProcessError
 from extrap.util.progress_bar import ProgressBar
 
 
 class ProgressWindow(ProgressBar):
     def __init__(self, parent, title, **kwargs):
```

### Comparing `extrap-4.0.4/extrap/gui/SelectorWidget.py` & `extrap-4.1.0a2/extrap/gui/SelectorWidget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
+from __future__ import annotations
+
 import math
-from typing import Optional, Sequence
+from typing import Optional, Sequence, TYPE_CHECKING, Tuple
 
 import numpy
-from PySide2.QtCore import *  # @UnusedWildImport
-from PySide2.QtGui import *  # @UnusedWildImport
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 
 from extrap.entities.calltree import Node
 from extrap.entities.metric import Metric
-from extrap.gui.ParameterValueSlider import ParameterValueSlider
-from extrap.gui.TreeModel import TreeModel
+from extrap.entities.model import Model
+from extrap.gui.TreeModel import TreeModel, TreeItemFilterProvider
 from extrap.gui.TreeView import TreeView
+from extrap.gui.components.ParameterValueSlider import ParameterValueSlider
 from extrap.modelers.model_generator import ModelGenerator
 
+if TYPE_CHECKING:
+    from extrap.gui.MainWidget import MainWidget
+
 
 class SelectorWidget(QWidget):
-    def __init__(self, mainWidget, parent):
+    def __init__(self, main_widget: MainWidget, parent):
         super(SelectorWidget, self).__init__(parent)
-        self.main_widget = mainWidget
+        self.main_widget = main_widget
         self.tree_model = TreeModel(self)
         self.parameter_sliders = list()
         self.initUI()
         self._sections_switched = False
+        self.min_value = 0
+        self.max_value = 0
 
     # noinspection PyAttributeOutsideInit
     def initUI(self):
         self.grid = QGridLayout(self)
         self.setLayout(self.grid)
 
         # Model selection
@@ -45,30 +51,68 @@
 
         # Metric selection
         metric_label = QLabel("Metric:", self)
         self.metric_selector = QComboBox(self)
         self.metric_selector.currentIndexChanged.connect(
             self.metric_index_changed)
 
-        # Callpath selection
-        self.tree_view = TreeView(self)
+        group = QFrame(self)
+        group.setObjectName("TreeViewContainer")
+        group.setStyleSheet("QFrame#TreeViewContainer{border:1px solid #939393}")
+        group_layout = QVBoxLayout(group)
+        group.setLayout(group_layout)
+        group.setContentsMargins(0, 0, 0, 0)
+        group_layout.setContentsMargins(0, 0, 0, 0)
+        group_layout.setSpacing(0)
 
+        # group.setAutoFillBackground(True)
+        # Callpath selection
+        self.tree_view = TreeView(group)
+        group_layout.addWidget(self.tree_view)
         # Input variable values
-        self.asymptoticCheckBox = QCheckBox('Show model', self)
+
+        self.toolbar = QToolBar(group)
+        self.toolbar.layout().setContentsMargins(2, 3, 2, 2)
+        self.toolbar.layout().setSpacing(5)
+        group_layout.addWidget(self.toolbar)
+
+        self.tree_display_select = QComboBox(self.toolbar)
+        self.tree_display_select.addItem('All', TreeItemFilterProvider.DisplayType.INCLUDE)
+        self.tree_display_select.addItem('Compact', TreeItemFilterProvider.DisplayType.COMPACT)
+        self.tree_display_select.addItem('Flat', TreeItemFilterProvider.DisplayType.FLAT)
+
+        def select_view_type(x):
+            self.tree_model.item_filter.display_type = self.tree_display_select.currentData()
+
+        self.tree_display_select.currentIndexChanged.connect(select_view_type)
+        self.toolbar.addWidget(self.tree_display_select)
+        spacer = QWidget()
+        spacer.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+        self.toolbar.addWidget(spacer)
+
+        self.asymptoticCheckBox = QCheckBox('Show model', self.toolbar)
         self.asymptoticCheckBox.toggle()
         self.asymptoticCheckBox.stateChanged.connect(
             self.changeAsymptoticBehavior)
+        self.toolbar.addWidget(self.asymptoticCheckBox)
+
+        self.show_parameters = QCheckBox('Show parameters', self.toolbar)
+        # self.show_parameters.toggle()
+        self.show_parameters.stateChanged.connect(
+            self.changeAsymptoticBehavior)
+        self.toolbar.addWidget(self.show_parameters)
 
         # Positioning
         self.grid.addWidget(model_label, 0, 0)
         self.grid.addWidget(self.model_selector, 0, 1)
         self.grid.addWidget(metric_label, 1, 0)
         self.grid.addWidget(self.metric_selector, 1, 1)
-        self.grid.addWidget(self.tree_view, 2, 0, 1, 2)
-        self.grid.addWidget(self.asymptoticCheckBox, 3, 1, Qt.AlignRight)
+        self.grid.addWidget(group, 2, 0, 1, 2)
+        # self.grid.addWidget(self.toolbar, 3, 0, 1, 2)
+
         self.grid.setColumnStretch(1, 1)
 
     def createParameterSliders(self):
         for param in self.parameter_sliders:
             param.clearRowLayout()
             self.grid.removeWidget(param)
         del self.parameter_sliders[:]
@@ -93,36 +137,45 @@
         self.tree_view.header().resizeSection(1, 23)
         self.tree_view.header().resizeSection(2, 23)
         selectionModel = self.tree_view.selectionModel()
         selectionModel.selectionChanged.connect(
             self.callpath_selection_changed)
 
     def callpath_selection_changed(self):
-        callpath_list = self.getSelectedCallpath()
-        # self.dict_callpath_color = {}
-        self.main_widget.populateCallPathColorMap(callpath_list)
-        self.main_widget.updateAllWidget()
+        call_tree_nodes = self.get_selected_call_tree_nodes()
+        metric = self.getSelectedMetric()
+        call_tree_nodes = [c for c in call_tree_nodes if
+                           (c.path, metric) in self.getCurrentModel().models]
+        self.main_widget.model_color_map.update(call_tree_nodes)
+        self.main_widget.on_selection_changed()
 
     def fillMetricList(self):
         self.metric_selector.clear()
         experiment = self.main_widget.getExperiment()
         if experiment is None:
             return
         metrics = experiment.metrics
         for metric in metrics:
             name = metric.name if metric.name != '' else '<default>'
             self.metric_selector.addItem(name, metric)
 
+    def on_experiment_changed(self):
+        self.updateModelList()
+        self.fillMetricList()
+        self.createParameterSliders()
+        self.fillCalltree()
+        self.tree_model.valuesChanged()
+
     def changeAsymptoticBehavior(self):
         self.tree_model.valuesChanged()
 
     def getSelectedMetric(self) -> Metric:
         return self.metric_selector.currentData()
 
-    def getSelectedCallpath(self) -> Sequence[Node]:
+    def get_selected_call_tree_nodes(self) -> Sequence[Node]:
         indexes = self.tree_view.selectedIndexes()
         callpath_list = list()
 
         for index in indexes:
             # We only care for the first column, otherwise we would get the same callpath repeatedly for each column
             if index.column() != 0:
                 continue
@@ -130,14 +183,31 @@
             callpath_list.append(callpath)
         return callpath_list
 
     def getCurrentModel(self) -> Optional[ModelGenerator]:
         model = self.model_selector.currentData()
         return model
 
+    def get_selected_models(self) -> Tuple[Optional[Sequence[Model]], Optional[Sequence[Node]]]:
+        selected_metric = self.getSelectedMetric()
+        selected_call_tree_nodes = self.get_selected_call_tree_nodes()
+        model_set = self.getCurrentModel()
+        if not selected_call_tree_nodes or model_set is None:
+            return None, None
+        model_set_models = model_set.models
+        if not model_set_models:
+            return None, None
+        model_list = list()
+        for node in selected_call_tree_nodes:
+            key = (node.path, selected_metric)
+            if key in model_set_models:
+                model = model_set_models[key]
+                model_list.append(model)
+        return model_list, selected_call_tree_nodes
+
     def renameCurrentModel(self, newName):
         index = self.model_selector.currentIndex()
         self.getCurrentModel().name = newName
         self.model_selector.setItemText(index, newName)
 
     def getModelIndex(self):
         return self.model_selector.currentIndex()
@@ -162,15 +232,15 @@
 
         # Introduced " and text != "No models to load" " as a second guard since always when the text would be
         # "No models to load" the gui would crash.
         # if model != None and text != "No models to load":
         #     generator = model._modeler
         self.main_widget.selector_widget.tree_model.valuesChanged()
 
-        self.main_widget.updateAllWidget()
+        self.main_widget.on_selection_changed()
         self.update()
 
     def model_rename(self):
         index = self.getModelIndex()
         if index < 0:
             return
         result = QInputDialog.getText(self,
@@ -179,87 +249,104 @@
         new_name = result[0]
         if result[1] and new_name:
             self.renameCurrentModel(new_name)
 
     def model_delete(self):
         reply = QMessageBox.question(self,
                                      'Delete Current Model',
-                                     "Are you sure to delete the model?",
+                                     "Are you sure to delete the current model?",
                                      QMessageBox.Yes | QMessageBox.No,
                                      QMessageBox.No)
         if reply == QMessageBox.Yes:
             index = self.getModelIndex()
             experiment = self.main_widget.getExperiment()
             if index < 0:
                 return
 
             self.model_selector.removeItem(index)
             del experiment.modelers[index]
 
+    def delete_metric(self):
+        reply = QMessageBox.question(self,
+                                     'Delete Current Metric',
+                                     "Are you sure to delete the current metric?",
+                                     QMessageBox.Yes | QMessageBox.No,
+                                     QMessageBox.No)
+        if reply == QMessageBox.Yes:
+            index = self.metric_selector.currentIndex()
+            metric = self.getSelectedMetric()
+            if index < 0:
+                return
+            experiment = self.main_widget.getExperiment()
+            self.metric_selector.removeItem(index)
+            experiment.metrics.remove(metric)
+            for callpath in experiment.callpaths:
+                key = (callpath, metric)
+                if key in experiment.measurements:
+                    del experiment.measurements[key]
+            for model_set in experiment.modelers:
+                for callpath in experiment.callpaths:
+                    key = (callpath, metric)
+                    if key in model_set.models:
+                        del model_set.models[key]
+
     @staticmethod
     def get_all_models(experiment):
         if experiment is None:
             return None
         models = experiment.modelers
         if len(models) == 0:
             return None
         return models
 
     def metric_index_changed(self):
-        self.main_widget.metricIndexChanged()
+        self.main_widget.on_selection_changed()
         self.tree_model.on_metric_changed()
 
     def getParameterValues(self):
-        ''' This functions returns the parameter value list with the
+        """ This functions returns the parameter value list with the
             parameter values from the bottom of the calltree selection.
             This information is necessary for the evaluation of the model
-            functions, e.g. to colot the severity boxes.
-        '''
+            functions, e.g. to color the severity boxes.
+        """
         value_list = []
         for param in self.parameter_sliders:
             value_list.append(param.getValue())
         return value_list
 
-    def iterate_children(self, paramValueList, callpaths, metric):
-        ''' This is a helper function for getMinMaxValue.
+    def iterate_children(self, models, param_value_list, callpaths, metric):
+        """ This is a helper function for update_min_max_value.
             It iterates the calltree recursively.
-        '''
+        """
         value_list = list()
         for callpath in callpaths:
-            model = self.getCurrentModel().models.get((callpath.path, metric))
-            if model is None:
-                continue
-
-            formula = model.hypothesis.function
-            value = formula.evaluate(paramValueList)
-            if not math.isinf(value):
-                value_list.append(value)
+            model = models.get((callpath.path, metric))
+            if model is not None:
+                formula = model.hypothesis.function
+                value = formula.evaluate(param_value_list)
+                if not math.isinf(value) and not math.isnan(value):
+                    value_list.append(value)
             children = callpath.childs
-            value_list += self.iterate_children(paramValueList,
-                                                children, metric)
+            value_list += self.iterate_children(models, param_value_list, children, metric)
         return value_list
 
-    def getMinMaxValue(self):
-        ''' This function calculated the minimum and the maximum values that
+    def update_min_max_value(self):
+        """ This function calculated the minimum and the maximum values that
             appear in the call tree. This information is e.g. used to scale
             legends ot the color line at the bottom of the extrap window.
-        '''
-        value_list = list()
+        """
+        min_max_value = (0, 0)
         experiment = self.main_widget.getExperiment()
-        if experiment is None:
-            value_list.append(1)
-            return value_list
-        selectedMetric = self.getSelectedMetric()
-        if selectedMetric is None:
-            value_list.append(1)
-            return value_list
-        param_value_list = self.getParameterValues()
-        call_tree = experiment.call_tree
-        nodes = call_tree.get_nodes()
-        previous = numpy.seterr(divide='ignore', invalid='ignore')
-        value_list.extend(self.iterate_children(param_value_list,
-                                                nodes,
-                                                selectedMetric))
-        numpy.seterr(**previous)
-        if len(value_list) == 0:
-            value_list.append(1)
-        return value_list
+        if experiment:
+            selected_metric = self.getSelectedMetric()
+            model_set = self.getCurrentModel()
+            if selected_metric and model_set:
+                param_value_list = self.getParameterValues()
+                call_tree = experiment.call_tree
+                nodes = call_tree.get_nodes()
+                previous = numpy.seterr(divide='ignore', invalid='ignore')
+                value_list = self.iterate_children(model_set.models, param_value_list, nodes, selected_metric)
+                numpy.seterr(**previous)
+                if len(value_list) > 0:
+                    min_max_value = max(0.0, min(value_list)), max(0.0, max(value_list))
+        self.min_value, self.max_value = min_max_value
+        return min_max_value
```

### Comparing `extrap-4.0.4/extrap/gui/Utils.py` & `extrap-4.1.0a2/extrap/gui/Utils.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from extrap.gui.plots.BaseGraphWidget import GraphDisplayWindow
 
 
@@ -17,25 +17,26 @@
 
     def draw_figure(self):
         """ 
           This function draws the graph
         """
 
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_List, z_List = self.calculate_z_models(maxX, maxY, model_list)
 
         # Get the callpath color map
-        dict_callpath_color = self.main_widget.get_callpath_color_map()
+        widget = self.main_widget
+        dict_callpath_color = widget.model_color_map
 
         # Create subplots based on the number of functions
         number_of_subplots = len(Z_List)
 
         # Adjusting subplots in order to avoid overlapping of labels
         # Reference : https://stackoverflow.com/questions/2418125/matplotlib-subplots-adjust-hspace-so-titles-and-xlabels-dont-overlap
 
@@ -66,13 +67,13 @@
             ax.yaxis.major.formatter._useMathText = True
             ax.zaxis.major.formatter._useMathText = True
             ax.plot_surface(
                 X, Y, Z_List[i], color=dict_callpath_color[selected_callpaths[i]])
             ax.set_xlabel('\n' + x_label)
             ax.set_ylabel('\n' + y_label, linespacing=3.1)
             ax.set_zlabel(
-                '\n' + self.main_widget.getSelectedMetric().name, linespacing=3.1)
+                '\n' + self.main_widget.get_selected_metric().name, linespacing=3.1)
 
         # draw legend
         self.draw_legend(ax, dict_callpath_color)
 
         self.fig.tight_layout()
```

### Comparing `extrap-4.0.4/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from extrap.gui.plots.BaseGraphWidget import GraphDisplayWindow
 
 
@@ -18,25 +18,26 @@
 
     def draw_figure(self):
         """ 
           This function draws the graph
         """
 
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_List, z_List = self.calculate_z_models(maxX, maxY, model_list)
 
         # Get the callpath color map
-        dict_callpath_color = self.main_widget.get_callpath_color_map()
+        widget = self.main_widget
+        dict_callpath_color = widget.model_color_map
 
         # colors = ['r','g','b','c','m','y']
         # colors = ["#1f77b4", "#ff7f0e", "#2ca02c", "#d62728", "#9467bd", "#8c564b", "#e377c2", "#7f7f7f", "#bcbd22", "#17becf"]
 
         # Set the x_label and y_label based on parameter selected.
         x_label = self.main_widget.data_display.getAxisParameter(0).name
         if x_label.startswith("_"):
@@ -55,14 +56,14 @@
         ax_all.get_xaxis().get_major_formatter().set_scientific(True)
         ax_all.xaxis.major.formatter._useMathText = True
         ax_all.yaxis.major.formatter._useMathText = True
         ax_all.zaxis.major.formatter._useMathText = True
         ax_all.set_xlabel('\n' + x_label)
         ax_all.set_ylabel('\n' + y_label, linespacing=3.1)
         ax_all.set_zlabel(
-            '\n' + self.main_widget.getSelectedMetric().name, linespacing=3.1)
+            '\n' + self.main_widget.get_selected_metric().name, linespacing=3.1)
         for i in range(len(Z_List)):
             ax_all.plot_surface(
                 X, Y, Z_List[i], color=dict_callpath_color[selected_callpaths[i]])
 
         # draw legend
         self.draw_legend(ax_all, dict_callpath_color)
```

### Comparing `extrap-4.0.4/extrap/gui/plots/BaseGraphWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/BaseGraphWidget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from __future__ import annotations
 
 import warnings
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
 import numpy as np
-from PySide2.QtWidgets import QSizePolicy
+from PySide6.QtWidgets import QSizePolicy
 from matplotlib import patches as mpatches
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.figure import Figure
 from mpl_toolkits.mplot3d import Axes3D
 
 if TYPE_CHECKING:
     from extrap.gui.MainWidget import MainWidget
@@ -83,16 +83,18 @@
         points = np.ndarray((len(self.main_widget.data_display.parameters), len(xs)))
 
         parameter_value_list = self.main_widget.data_display.getValues()
         for p, v in parameter_value_list.items():
             points[p] = v
         param1 = self.main_widget.data_display.getAxisParameter(0).id
         param2 = self.main_widget.data_display.getAxisParameter(1).id
-        points[param1] = xs
-        points[param2] = ys
+        if param1 >= 0:
+            points[param1] = xs
+        if param2 >= 0:
+            points[param2] = ys
 
         z_value = function.evaluate(points)
         return z_value
 
     def calculate_z_models(self, maxX, maxY, model_list, max_z=0):
         # define grid parameters based on max x and max y value
         pixelGap_x, pixelGap_y = self._calculate_grid_parameters(maxX, maxY)
@@ -113,31 +115,14 @@
             max_z = max(max_z, np.max(zs[np.logical_not(np.isinf(zs))]))
         np.seterr(**previous)
         for z, Z in zip(z_List, Z_List):
             z[np.isinf(z)] = max_z
             Z[np.isinf(Z)] = max_z
         return X, Y, Z_List, z_List
 
-    def get_selected_models(self):
-        selected_metric = self.main_widget.getSelectedMetric()
-        selected_callpaths = self.main_widget.getSelectedCallpath()
-        model_set = self.main_widget.getCurrentModel()
-        if not selected_callpaths or model_set is None:
-            return None, None
-        model_set_models = model_set.models
-        if not model_set_models:
-            return None, None
-        model_list = list()
-        for selected_callpath in selected_callpaths:
-            key = (selected_callpath.path, selected_metric)
-            if key in model_set_models:
-                model = model_set_models[key]
-                model_list.append(model)
-        return model_list, selected_callpaths
-
     def draw_legend(self, ax_all, dict_callpath_color):
         fontSize = self.graphWidget.getFontSize()
         # draw legend
         patches = list()
         for key, value in dict_callpath_color.items():
             labelName = str(key.name)
             if labelName.startswith("_"):
```

### Comparing `extrap-4.0.4/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import sys
 
 import matplotlib.patches as mpatches
 import numpy as np
-from PySide2.QtWidgets import *  # @UnusedWildImport
+from PySide6.QtWidgets import *  # @UnusedWildImport
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.figure import Figure
 
 from extrap.gui.plots.BaseGraphWidget import GraphDisplayWindow
 
 
 #####################################################################
@@ -160,17 +160,14 @@
         dict_callpath_color = {}
         current_index = 0
         for callpath in callpaths:
             dict_callpath_color[callpath] = colors[current_index]
             current_index = current_index + 1
         return dict_callpath_color
 
-    def getColorForCallPath(self, callpath):
-        return self.dict_callpath_color[callpath]
-
     @staticmethod
     def getColorMap():
         colors = [(0, 0, 1), (0, 1, 0), (1, 0, 0)]
         n_bin = 100
         cmap_name = 'my_list'
         colorMap = LinearSegmentedColormap.from_list(
             cmap_name, colors, N=n_bin)
```

### Comparing `extrap-4.0.4/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import numpy as np
 
 from extrap.gui.plots.BaseGraphWidget import GraphDisplayWindow
@@ -25,25 +25,26 @@
         super().__init__(graphWidget, main_widget, width, height, dpi)
 
     def draw_figure(self):
         """ 
           This function draws the graph
         """
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_list, z_List = self.calculate_z_models(maxX, maxY, model_list)
 
         # Get the callpath color map
-        dict_callpath_color = self.main_widget.get_callpath_color_map()
+        widget = self.main_widget
+        dict_callpath_color = widget.model_color_map
 
         # calculate max_z value
         color_for_max_z = dict_callpath_color[selected_callpaths[0]]
         max_z_list = list()
         max_color_list = list()
 
         for i in range(len(z_List[0])):
@@ -76,11 +77,11 @@
         ax.zaxis.major.formatter._useMathText = True
         ax.get_xaxis().get_major_formatter().set_scientific(True)
         for (x, y, z, colour) in zip(X, Y, max_Z_List, max_Color_List):
             ax.scatter(x, y, z, c=colour)
         ax.set_xlabel('\n' + x_label)
         ax.set_ylabel('\n' + y_label, linespacing=3.1)
         ax.set_zlabel(
-            '\n' + self.main_widget.getSelectedMetric().name, linespacing=3.1)
+            '\n' + self.main_widget.get_selected_metric().name, linespacing=3.1)
         ax.set_title(r'Dominating Functions')
 
         self.draw_legend(ax, dict_callpath_color)
```

### Comparing `extrap-4.0.4/extrap/gui/plots/HeatMapGraphWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/HeatMapGraphWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import random
 import sys
 
@@ -34,25 +34,26 @@
         super().__init__(graphWidget, main_widget, width, height, dpi)
 
     def draw_figure(self):
         """ 
           This function draws the graph
         """
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_List, z_List = self.calculate_z_models(maxX, maxY, model_list)
 
         # Get the callpath color map
-        dict_callpath_color = self.main_widget.get_callpath_color_map()
+        widget = self.main_widget
+        dict_callpath_color = widget.model_color_map
 
         # for each x,y value , calculate max z for all function and
         # get the associated model functions for which z is highest.
         # Also store the the associated z value.
 
         color_for_max_z = dict_callpath_color[selected_callpaths[0]]
         max_z_list = list()
```

### Comparing `extrap-4.0.4/extrap/gui/plots/InterpolatedContourDisplayWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/InterpolatedContourDisplayWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import warnings
 
 import matplotlib.ticker as ticker
@@ -27,15 +27,15 @@
 
     def draw_figure(self):
         """ 
           This function draws the graph
         """
 
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get font size for legend
         fontSize = self.graphWidget.getFontSize()
 
         # Get max x and max y value as a initial default value or a value provided by user
```

### Comparing `extrap-4.0.4/extrap/gui/plots/IsolinesDisplayWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/IsolinesDisplayWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import warnings
 
 from extrap.gui.plots.BaseGraphWidget import BaseContourGraph
@@ -19,25 +19,26 @@
 
     def draw_figure(self):
         """ 
           This function draws the graph
         """
 
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_List, z_List = self.calculate_z_models(maxX, maxY, model_list)
 
         # Get the callpath color map
-        dict_callpath_color = self.main_widget.get_callpath_color_map()
+        widget = self.main_widget
+        dict_callpath_color = widget.model_color_map
         number_of_subplots = 1
         if len(Z_List) > 1:
             number_of_subplots = len(Z_List) + 1
 
         # Adjusting subplots in order to avoid overlapping of labels
         # Reference : https://stackoverflow.com/questions/2418125/matplotlib-subplots-adjust-hspace-so-titles-and-xlabels-dont-overlap
         left = 0.1
```

### Comparing `extrap-4.0.4/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/MaxZAsSingleSurfacePlotWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import matplotlib.ticker as ticker
 import numpy as np
 from matplotlib import cm
@@ -26,15 +26,15 @@
 
     def draw_figure(self):
         """ 
           This function draws the graph
         """
 
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
             # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         X, Y, Z_List, z_List = self.calculate_z_models(maxX, maxY, model_list)
@@ -74,12 +74,12 @@
         ax.yaxis.major.formatter._useMathText = True
         ax.zaxis.major.formatter._useMathText = True
         im = ax.plot_surface(X, Y, max_Z_List, cmap=self.colormap)
 
         ax.set_xlabel('\n' + x_label, linespacing=3.2)
         ax.set_ylabel('\n' + y_label, linespacing=3.1)
         ax.set_zlabel(
-            '\n' + self.main_widget.getSelectedMetric().name, linespacing=3.1)
+            '\n' + self.main_widget.get_selected_metric().name, linespacing=3.1)
         ax.set_title('Max. Z Value')
         self.fig.colorbar(im, ax=ax, orientation="horizontal",
                           pad=0.2, format=ticker.ScalarFormatter(useMathText=True))
         # self.fig.tight_layout()
```

### Comparing `extrap-4.0.4/extrap/gui/plots/MeasurementPointsPlotWidget.py` & `extrap-4.1.0a2/extrap/gui/plots/MeasurementPointsPlotWidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import numpy as np
 
 from extrap.gui.plots.BaseGraphWidget import GraphDisplayWindow
@@ -19,52 +19,60 @@
 
     def draw_figure(self):
         """
           This function draws the graph
         """
 
         # Get data
-        model_list, selected_callpaths = self.get_selected_models()
+        model_list, selected_callpaths = self.main_widget.get_selected_models()
         if model_list is None:
             return
 
         # Get max x and max y value as a initial default value or a value provided by user
         maxX, maxY = self.get_max()
 
         if len(model_list) < 1:
             return
 
         # Get the callpath color map
-        dict_callpath_color = self.main_widget.get_callpath_color_map()
+        widget = self.main_widget
+        dict_callpath_color = widget.model_color_map
+
+        # Get base data for drawing points
+        parameter_x = self.main_widget.data_display.getAxisParameter(0)
+        parameter_y = self.main_widget.data_display.getAxisParameter(1)
 
         # Set the x_label and y_label based on parameter selected.
-        x_label = self.main_widget.data_display.getAxisParameter(0).name
+        x_label = parameter_x.name
         if x_label.startswith("_"):
             x_label = x_label[1:]
-        y_label = self.main_widget.data_display.getAxisParameter(1).name
+        y_label = parameter_y.name
         if y_label.startswith("_"):
             y_label = y_label[1:]
 
         # 1 because we are going to show all the models in same plot
         number_of_subplots = 1
 
         # Draw all the selected models as surface plots and measuremnet point around them
         ax_all = self.fig.add_subplot(
             1, number_of_subplots, number_of_subplots, projection='3d')
 
-        # Gat base data for drawing points
-        parameter_x = self.main_widget.data_display.getAxisParameter(0)
-        parameter_y = self.main_widget.data_display.getAxisParameter(1)
         max_z = 0
 
         for model, callpath in zip(model_list, selected_callpaths):
             callpath_color = dict_callpath_color[callpath]
             points = model.measurements
-            xs = np.array([m.coordinate[parameter_x.id] for m in points])
-            ys = np.array([m.coordinate[parameter_y.id] for m in points])
+            if parameter_x.id >= 0:
+                xs = np.array([m.coordinate[parameter_x.id] for m in points])
+            else:
+                xs = np.zeros(len(points))
+            if parameter_y.id >= 0:
+                ys = np.array([m.coordinate[parameter_y.id] for m in points])
+            else:
+                ys = np.full(len(points), max(min(np.min(xs), 0), 0))
             in_range = (xs <= maxX) & (ys <= maxY)
             xs, ys = xs[in_range], ys[in_range]
 
             mean = np.array([m.mean for m in points])[in_range]
             median = np.array([m.median for m in points])[in_range]
             minimum = np.array([m.minimum for m in points])[in_range]
             maximum = np.array([m.maximum for m in points])[in_range]
@@ -91,15 +99,15 @@
         ax_all.mouse_init()
         ax_all.xaxis.major.formatter._useMathText = True
         ax_all.yaxis.major.formatter._useMathText = True
         ax_all.zaxis.major.formatter._useMathText = True
         ax_all.set_xlabel('\n' + x_label)
         ax_all.set_ylabel('\n' + y_label, linespacing=3.1)
         ax_all.set_zlabel(
-            '\n' + self.main_widget.getSelectedMetric().name, linespacing=3.1)
+            '\n' + self.main_widget.get_selected_metric().name, linespacing=3.1)
         ax_all.set_title("Measurement Points")
         # ax_all.zaxis.set_major_locator(LinearLocator(10))
         # ax_all.zaxis.set_major_formatter(FormatStrFormatter('%.02f'))
         for i in range(len(Z_List)):
             ax_all.plot_surface(X, Y, Z_List[i], color=dict_callpath_color[selected_callpaths[i]],
                                 rstride=1, cstride=1, antialiased=False, alpha=0.1)
```

### Comparing `extrap-4.0.4/extrap/modelers/abstract_modeler.py` & `extrap-4.1.0a2/extrap/modelers/abstract_modeler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import copy
+import logging
+import warnings
 from abc import ABC, abstractmethod
 from typing import Sequence, Optional
 
-from marshmallow import fields
+from marshmallow import fields, post_load
 
 from extrap.entities.measurement import Measurement
 from extrap.entities.model import Model
 from extrap.util.classproperty import classproperty
 from extrap.util.progress_bar import DUMMY_PROGRESS
 from extrap.util.serialization_schema import BaseSchema
 
 
 class AbstractModeler(ABC):
     def __init__(self, use_median: bool):
-        # use mean or median measurement values to calculate models
+        """Creates a new modeler object, that uses either the median or the mean when modeling.
+
+           :param use_median: use mean or median measurement values to calculate models
+        """
         self._use_median = use_median
 
     @property
     def use_median(self) -> bool:
         return self._use_median
 
     @use_median.setter
@@ -84,9 +89,39 @@
         self._use_median = value
         self.single_parameter_modeler.use_median = value
 
 
 class ModelerSchema(BaseSchema):
     use_median = fields.Bool()
 
+    def on_missing_sub_schema(self, type_, data, **kwargs):
+        warnings.warn(f"Loaded unknown modeler of type {type_}")
+        data['type_'] = type_
+        return super(BaseSchema, self).load(data, **kwargs)
+
     def create_object(self):
+        logging.debug(f"Created placeholder for unknown modeler")
+        return _EmptyModeler(False)
+
+
+class _EmptyModeler(AbstractModeler):
+    NAME = "<Empty>"
+
+    def model(self, measurements: Sequence[Sequence[Measurement]], progress_bar=DUMMY_PROGRESS) -> Sequence[Model]:
         raise NotImplementedError()
+
+    def __eq__(self, o: object) -> bool:
+        return o is self or isinstance(o, _EmptyModeler)
+
+
+EMPTY_MODELER = _EmptyModeler(False)
+
+
+class _EmptyModelerSchema(ModelerSchema):
+    use_median = fields.Constant(False, load_only=True, dump_only=True)
+
+    @post_load
+    def unpack_to_object(self, data, **kwargs):
+        return EMPTY_MODELER
+
+    def create_object(self):
+        return EMPTY_MODELER
```

### Comparing `extrap-4.0.4/extrap/modelers/loader.py` & `extrap-4.1.0a2/extrap/modelers/loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,26 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
 # Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-import inspect
-import pkgutil
-from typing import Mapping, Type, MutableMapping, TypeVar, Iterator
+from typing import Mapping, Type, MutableMapping
 
 from marshmallow import fields, validate
 
+from extrap.util.extension_loader import load_extensions
 from extrap.util.serialization_schema import NumberField
 from .abstract_modeler import AbstractModeler, ModelerSchema
 from .modeler_options import ModelerOption, modeler_options
 
-_VT = TypeVar("_VT")
-
-
-class CaseInsensitiveStringDict(MutableMapping[str, _VT]):
-    def __init__(self):
-        self.case_mapping = {}
-        self.data = {}
-
-    def __delitem__(self, v: str) -> None:
-        v = self.resolve_key(v)
-        del self.data[v]
-        del self.case_mapping[v.lower()]
-
-    def resolve_key(self, k):
-        if k not in self.data:
-            return self.case_mapping[k.lower()]
-        return k
-
-    def __len__(self) -> int:
-        return len(self.data)
-
-    def __iter__(self) -> Iterator:
-        return iter(self.data)
-
-    def __getitem__(self, k: str) -> _VT:
-        k = self.resolve_key(k)
-        return self.data[k]
-
-    def __setitem__(self, k: str, value: _VT):
-        self.case_mapping[k.lower()] = k
-        self.data[k] = value
-
 
 def load_modelers(path, pkg_name) -> MutableMapping[str, Type[AbstractModeler]]:
-    def is_modeler(x):
-        return inspect.isclass(x) \
-               and issubclass(x, AbstractModeler) \
-               and not inspect.isabstract(x)
-
-    modelers = CaseInsensitiveStringDict()
-    for importer, modname, is_pkg in pkgutil.walk_packages(path=path,
-                                                           prefix=pkg_name + '.',
-                                                           onerror=lambda x: None):
-        module = importer.find_module(modname).load_module(modname)
-        for name, clazz in inspect.getmembers(module, is_modeler):
-            clazz: Type[AbstractModeler]
-            name = clazz.NAME
-            modelers[name] = clazz
-            create_schema(clazz)
-    return modelers
+    return load_extensions(path, pkg_name, AbstractModeler, create_schema)
 
 
 def _determine_field(option: ModelerOption):
     if option.range:
         if isinstance(option.range, range):
             if range.step == 1:
                 validation = validate.Range(option.range.start, option.range.stop, max_inclusive=False)
```

### Comparing `extrap-4.0.4/extrap/modelers/model_generator.py` & `extrap-4.1.0a2/extrap/modelers/model_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from __future__ import annotations
 
 import itertools
@@ -15,14 +15,15 @@
 from extrap.entities.callpath import Callpath, CallpathSchema
 from extrap.entities.metric import Metric, MetricSchema
 from extrap.entities.model import Model, ModelSchema
 from extrap.modelers import multi_parameter
 from extrap.modelers import single_parameter
 from extrap.modelers.abstract_modeler import AbstractModeler, MultiParameterModeler, ModelerSchema
 from extrap.modelers.modeler_options import modeler_options
+from extrap.util.exceptions import RecoverableError
 from extrap.util.progress_bar import DUMMY_PROGRESS
 from extrap.util.serialization_schema import Schema, TupleKeyDict
 
 if TYPE_CHECKING:
     from extrap.entities.experiment import Experiment
 
 
@@ -58,15 +59,15 @@
                     # multi-parameter model generator init here...
                     result_modeler = multi_parameter.all_modelers[modeler]()
                 result_modeler.use_median = use_median
             except KeyError:
                 raise ValueError(
                     f'Modeler with name "{modeler}" does not exist.')
         elif modeler is NotImplemented:
-            return NotImplemented
+            result_modeler = NotImplemented
         else:
             if (len(self.experiment.parameters) > 1) == isinstance(modeler, MultiParameterModeler):
                 # single-parameter model generator init here...
                 result_modeler = modeler
                 if use_median is not None:
                     result_modeler.use_median = use_median
             elif len(self.experiment.parameters) > 1:
@@ -98,15 +99,15 @@
                    self._modeler.use_median == other._modeler.use_median and \
                    modeler_options.equal(self._modeler, other._modeler)
 
 
 class ModelGeneratorSchema(Schema):
     name = fields.Str()
     _modeler = fields.Nested(ModelerSchema, data_key='modeler')
-    models = TupleKeyDict(keys=(fields.Nested(CallpathSchema), fields.Nested(MetricSchema)),
+    models = TupleKeyDict(keys=(fields.Pluck(CallpathSchema, 'name'), fields.Pluck(MetricSchema, 'name')),
                           values=fields.Nested(ModelSchema, exclude=('callpath', 'metric')))
 
     def create_object(self):
         return ModelGenerator(None, NotImplemented)
 
     def postprocess_object(self, obj: ModelGenerator):
         for (callpath, metric), m in obj.models.items():
```

### Comparing `extrap-4.0.4/extrap/modelers/modeler_options.py` & `extrap-4.1.0a2/extrap/modelers/modeler_options.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/modelers/multi_parameter/__init__.py` & `extrap-4.1.0a2/extrap/modelers/multi_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/modelers/multi_parameter/multi_parameter_modeler.py` & `extrap-4.1.0a2/extrap/modelers/multi_parameter/multi_parameter_modeler.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/modelers/single_parameter/__init__.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/modelers/single_parameter/abstract_base.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/abstract_base.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/modelers/single_parameter/basic.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import copy
 import itertools
 import logging
```

### Comparing `extrap-4.0.4/extrap/modelers/single_parameter/refining.py` & `extrap-4.1.0a2/extrap/modelers/single_parameter/refining.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/util/caching.py` & `extrap-4.1.0a2/extrap/entities/metric.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
-import sys
+import itertools
 
-if sys.version_info >= (3, 8):
-    import functools
+from extrap.entities.named_entity import NamedEntityWithTags, NamedEntityWithTagsSchema
 
-    cached_property = functools.cached_property
-else:
-    class cached_property(object):
-        """
-        A property that is cached for later retrieval.
-        """
-
-        def __init__(self, func):
-            self.func = func
-
-        def __get__(self, obj, cls):
-            if obj is None:
-                return self
-
-            value = self.func(obj)
-            obj.__dict__[self.func.__name__] = value
-            return value
+
+class Metric(NamedEntityWithTags):
+    """
+    This class represents a metric such as time or FLOPS.
+    """
+    TYPENAME = "Metric"
+
+    ID_COUNTER = itertools.count()
+    """
+    Counter for global metric ids
+    """
+
+
+class MetricSchema(NamedEntityWithTagsSchema):
+    def create_object(self):
+        return Metric('')
```

### Comparing `extrap-4.0.4/extrap/util/classproperty.py` & `extrap-4.1.0a2/extrap/util/classproperty.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/util/deprecation.py` & `extrap-4.1.0a2/extrap/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/util/exceptions.py` & `extrap-4.1.0a2/extrap/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/util/options_parser.py` & `extrap-4.1.0a2/extrap/util/options_parser.py`

 * *Files identical despite different names*

### Comparing `extrap-4.0.4/extrap/util/progress_bar.py` & `extrap-4.1.0a2/extrap/util/progress_bar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
+from numbers import Number
+
 from tqdm import tqdm
 
 
 class ProgressBar(tqdm):
     def __init__(self, **kwargs):
         if 'iterable' not in kwargs:
             kwargs['total'] = 0
         if 'bar_format' not in kwargs:
             kwargs['bar_format'] = '{l_bar}{bar}| [{elapsed}<{remaining}{postfix}]'
         super().__init__(**kwargs)
 
     def step(self, s='', refresh=True):
         super().set_postfix_str(s, refresh)
 
+    def create_target(self, target: Number):
+        self.total += target
+        return self.total
+
+    def reach_target(self, target):
+        if self.n < target:
+            self.update(target - self.n)
+            self.refresh()
+
     def __call__(self, iterable, length=None, scale=1):
         if length:
             self.total += length * scale
         else:
             try:
                 self.total += len(iterable) * scale
             except (TypeError, AttributeError):
@@ -62,8 +73,8 @@
     def display(self, msg=None, pos=None):
         return True
 
     def close(self):
         pass
 
 
-DUMMY_PROGRESS = DummyProgressBar()
+DUMMY_PROGRESS: ProgressBar = DummyProgressBar()
```

### Comparing `extrap-4.0.4/extrap/util/serialization_schema.py` & `extrap-4.1.0a2/extrap/util/serialization_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2022, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 import collections
 import math
+import typing
 from abc import abstractmethod, ABC
 from collections.abc import Mapping
-from typing import Union, Sequence
+from typing import Union, Sequence, Tuple, Type
 
 from marshmallow import post_load, fields, ValidationError, EXCLUDE
+from marshmallow.base import SchemaABC
 from marshmallow.fields import Field
 from marshmallow.schema import Schema as _Schema
 
 from extrap.entities.fraction import Fraction
 
 
 class SchemaMeta(type(_Schema), type(ABC)):
@@ -24,18 +26,18 @@
 
 class Schema(_Schema, ABC, metaclass=SchemaMeta):
     class Meta:
         ordered = True
         unknown = EXCLUDE
 
     @abstractmethod
-    def create_object(self):
+    def create_object(self) -> Union[object, Tuple[type(NotImplemented), Type]]:
         raise NotImplementedError()
 
-    def postprocess_object(self, obj):
+    def postprocess_object(self, obj: object) -> object:
         return obj
 
     @post_load
     def unpack_to_object(self, data, **kwargs):
         obj = self.create_object()
         try:
             for k, v in data.items():
@@ -46,45 +48,54 @@
 
 
 class BaseSchema(Schema):
     _subclasses = None
     type_field = '$type'
 
     def create_object(self):
-        raise NotImplementedError()
+        raise NotImplementedError(f"{type(self)} has no create object method.")
 
     def __init_subclass__(cls, **kwargs):
         if not cls.__is_direct_subclass(cls, BaseSchema):
-            cls._subclasses[type(cls().create_object()).__name__] = cls
+            obj = cls().create_object()
+            if isinstance(obj, tuple) and obj[0] == NotImplemented:
+                cls._subclasses[obj[1].__name__] = cls
+            else:
+                cls._subclasses[type(cls().create_object()).__name__] = cls
         else:
             cls._subclasses = {}
         super().__init_subclass__(**kwargs)
 
     @staticmethod
     def __is_direct_subclass(subclass, classs_):
         return subclass.mro()[1] == classs_
 
+    def on_missing_sub_schema(self, type_, data, **kwargs):
+        """Handles missing subschema. May return a parsed object to fail gracefully."""
+        raise ValidationError(f'No subschema found for {type_} in {type(self).__name__}')
+
     def load(self, data, **kwargs):
-        if self.__is_direct_subclass(type(self), BaseSchema):
+        if self.__is_direct_subclass(type(self), BaseSchema) and self.type_field in data:
             type_ = data[self.type_field]
             del data[self.type_field]
             try:
                 schema = self._subclasses[type_]()
             except KeyError:
-                raise ValidationError(f'No subschema found for {type_} in {type(self).__name__}')
+                return self.on_missing_sub_schema(type, data, **kwargs)
             return schema.load(data, **kwargs)
         else:
             return super(BaseSchema, self).load(data, **kwargs)
 
     def dump(self, obj, **kwargs):
-        if self.__is_direct_subclass(type(self), BaseSchema):
+        if self.__is_direct_subclass(type(self), BaseSchema) and type(obj).__name__ in self._subclasses:
             return self._subclasses[type(obj).__name__]().dump(obj, **kwargs)
         else:
             result = super(BaseSchema, self).dump(obj, **kwargs)
-            result[self.type_field] = type(obj).__name__
+            if type(obj).__name__ in self._subclasses:
+                result[self.type_field] = type(obj).__name__
             return result
 
 
 def make_value_schema(class_, value):
     class Schema(_Schema):
         def dump(self, obj, *, many: bool = None):
             return getattr(obj, value)
@@ -201,7 +212,50 @@
         elif isinstance(value, Fraction):
             return self._to_string(value)
         elif math.isnan(value) or math.isinf(value):
             return self._to_string(value)
         else:
             ret = super()._format_num(value)
         return self._to_string(ret) if self.as_string else ret
+
+
+class ListToMappingField(fields.List):
+    def __init__(self, nested: typing.Union[SchemaABC, type, str, typing.Callable[[], SchemaABC]], key_field: str, *,
+                 list_type=list, dump_condition=None, **kwargs):
+        super().__init__(fields.Nested(nested), **kwargs)
+        self.dump_condition = dump_condition
+        self.list_type = list_type
+        only_field = self.inner.schema.fields[key_field]
+        self.key_field_name = only_field.data_key or key_field
+        self.inner: fields.Nested
+
+    def _serialize(self, value: typing.Any, attr: str, obj: typing.Any, **kwargs):
+        if value is None:
+            return None
+        if self.dump_condition:
+            value = [v for v in value if self.dump_condition(v)]
+        value = super()._serialize(value, attr, obj, **kwargs)
+        result = {}
+        for each in value:
+            key = each[self.key_field_name]
+            del each[self.key_field_name]
+            result[key] = each
+        return result
+
+    def _deserialize(self, value: typing.Any, attr: str, data: typing.Optional[typing.Mapping[str, typing.Any]],
+                     **kwargs) -> typing.List[typing.Any]:
+        if not isinstance(value, Mapping):
+            raise self.make_error("invalid")
+
+        value_list = []
+        for k, v in value.items():
+            if not isinstance(v, typing.MutableMapping):
+                raise self.make_error("invalid")
+            v[self.key_field_name] = k
+            value_list.append(v)
+
+        result = super()._deserialize(value_list, attr, data, **kwargs)
+
+        if self.list_type != list:
+            return self.list_type(result)
+        else:
+            return result
```

### Comparing `extrap-4.0.4/extrap.egg-info/PKG-INFO` & `extrap-4.1.0a2/extrap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: extrap
-Version: 4.0.4
+Version: 4.1.0a2
 Summary: Extra-P, automated performance modeling for HPC applications
 Home-page: https://github.com/extra-p/extrap
 Author: Extra-P project
 Author-email: extra-p@lists.parallel.informatik.tu-darmstadt.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Extra-P
 
 **Automated performance modeling for HPC applications**
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/extrap?style=plastic)](https://badge.fury.io/py/extrap)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/extra-p/extrap?style=plastic)
 [![PyPI version](https://badge.fury.io/py/extrap.png)](https://badge.fury.io/py/extrap)
 [![PyPI - License](https://img.shields.io/pypi/l/extrap?style=plastic)](https://badge.fury.io/py/extrap)
 ![GitHub issues](https://img.shields.io/github/issues/extra-p/extrap?style=plastic)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/extra-p/extrap?style=plastic)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/extra-p/extrap/Test%20extrap%20package?style=plastic)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/extra-p/extrap/python-package.yml?style=plastic)
 
 [<img alt="Screenshot of Extra-P" src="https://github.com/extra-p/extrap/raw/master/docs/images/extra-p-2d.png" height="200" align="right" title="Screenshot of Extra-P"/>](docs/images/extra-p-2d.png)
 Extra-P is an automatic performance-modeling tool that supports the user in the identification of *scalability bugs*. 
 A scalability bug is a part of the program whose scaling behavior is unintentionally poor, 
 that is, much worse than expected. A performance model is a formula that expresses a performance metric of interest 
 such as execution time or energy consumption as a function of one or more execution parameters such as the size of the 
 input problem or the number of processors. 
@@ -70,21 +70,21 @@
 5. [Citation](#Citation)
 6. [Publications](#Publications)
 
 --------------------------------------------------------------------------------------------
 
 ### Requirements
 
-* Python 3.7 or higher
+* Python 3.8 or higher
 * numpy
 * pycubexr
 * marshmallow
 * packaging
 * tqdm
-* PySide2 (for GUI)
+* PySide6 (for GUI)
 * matplotlib (for GUI)
 * pyobjc-framework-Cocoa (only for GUI on macOS)
 
 ### Installation
 
 Use the following command to install Extra-P and all required packages via `pip`.
 
@@ -118,36 +118,38 @@
 * Create model and save it to text file at the given
   path: `extrap --out test.txt --text test/data/text/one_parameter_1.txt`
 
 The Extra-P command line interface has the following options.
 
 | Arguments                                                            |                                              |
 |----------------------------------------------------------------------|----------------------------------------------|
-| **Positional**                                                       |                                              |
-| _FILEPATH_                                                           | Specify a file path for Extra-P to work with |
-| **Optional**                                                         |                                              |
-| `-h`, `--help`                                                       | Show help message and exit                   |
-| `--version`                                                          | Show program's version number and exit       |
-| `--log` {`debug`, `info`, `warning`, `error`, `critical`}            | Set program's log level (default: `warning`) |
-| **Input options**                                                    |                                              |
-| `--cube`                                                             | Load data from CUBE files                    |
-| `--text`                                                             | Load data from text files                    |
-| `--talpas`                                                           | Load data from Talpas data format            |
-| `--json`                                                             | Load data from JSON or JSON Lines file       |
-| `--extra-p-3`                                                        | Load data from Extra-P 3 experiment          |
-| `--scaling` {`weak`, `strong`}                                       | Set weak or strong scaling when loading data from CUBE files (default: `weak`) |
-| **Modeling options**                                                 |                                              |
-| `--median`                                                           | Use median values for computation instead of mean values  |
-| `--modeler` {`default`, `basic`, `refining`, `multi-parameter`}      | Selects the modeler for generating the performance models |
-| `--options` _KEY_=_VALUE_ [_KEY_=_VALUE_ ...]                        | Options for the selected modeler             |
-| `--help-modeler` {`default`, `basic`, `refining`, `multi-parameter`} | Show help for modeler options and exit       |
-| **Output options**                                                   |                                              |
-| `--out` _OUTPUT_PATH_                                                | Specify the output path for Extra-P results  |
-| `--print` {`all`, `callpaths`, `metrics`, `parameters`, `functions`} | Set which information should be displayed after modeling (default: `all`) |
-| `--save-experiment` <i>EXPERIMENT_PATH</i>                           | Saves the experiment including all models as Extra-P experiment (if no extension is specified, “.extra-p” is appended) |
+| **Positional**                                                       |                                              
+| _FILEPATH_                                                           | Specify a file path for Extra-P to work with 
+| **Optional**                                                         |                                              
+| `-h`, `--help`                                                       | Show help message and exit                   
+| `--version`                                                          | Show program's version number and exit       
+| `--log` {`debug`, `info`, `warning`, `error`, `critical`}            | Set program's log level (default: `warning`) 
+| **Input options**                                                    |                                              
+| `--cube`                                                             | Load a set of CUBE files and generate a new experiment
+| `--extra-p-3`                                                        | Load data from Extra-P 3 (legacy) experiment
+| `--json`                                                             | Load data from JSON or JSON Lines input file
+| `--talpas`                                                           | Load data from Talpas data format
+| `--text`                                                             | Load data from text input file
+| `--experiment`                                                       | Load Extra-P experiment and generate new models
+| `--scaling` {`weak`, `strong`}                                       | Set weak or strong scaling when loading data from CUBE files (default: `weak`) 
+| **Modeling options**                                                 |                                              
+| `--median`                                                           | Use median values for computation instead of mean values  
+| `--modeler` {`default`, `basic`, `refining`, `multi-parameter`}      | Selects the modeler for generating the performance models 
+| `--options` _KEY_=_VALUE_ [_KEY_=_VALUE_ ...]                        | Options for the selected modeler             
+| `--help-modeler` {`default`, `basic`, `refining`, `multi-parameter`} | Show help for modeler options and exit       
+| **Output options**                                                   |                                              
+| `--out` _OUTPUT_PATH_                                                | Specify the output path for Extra-P results  
+| `--print` {`all`, `callpaths`, `metrics`, `parameters`, `functions`, _FORMAT_STRING_} | Set which information should be displayed after modeling. Use one of the predefined values or specify a formatting string using placeholders (see [docs/output-formatting.md](docs/output-formatting.md)) (default: `all`).
+| `--save-experiment` <i>EXPERIMENT_PATH</i>                           | Saves the experiment including all models as Extra-P experiment (if no extension is specified, “.extra-p” is appended) 
+| `--model-set-name` _NAME_                                            | Set the name of the generated set of models when outputting an experiment (default: “New model”)
 
 ### License
 
 [BSD 3-Clause "New" or "Revised" License](LICENSE)
 
 ### Citation
 
@@ -168,9 +170,7 @@
 ### Publications
 
 1. Alexandru Calotoiu, David Beckingsale, Christopher W. Earl, Torsten Hoefler, Ian Karlin, Martin Schulz, Felix Wolf: Fast Multi-Parameter Performance Modeling. In Proc. of the 2016 IEEE International Conference on Cluster Computing (CLUSTER), Taipei, Taiwan, pages 172–181, IEEE, September 2016. [PDF](https://apps.fz-juelich.de/jsc-pubsystem/aigaion/attachments/fastmultiparam.pdf-f839eba376c6d61a8c4cab9860b6b3bf.pdf)
 
 2. Marcus Ritter, Alexandru Calotoiu, Sebastian Rinke, Thorsten Reimann, Torsten Hoefler, Felix Wolf: *Learning Cost-Effective Sampling Strategies for Empirical Performance Modeling.* In Proc. of the 34th IEEE International Parallel and Distributed Processing Symposium (IPDPS), New Orleans, LA, USA, pages 884–895, IEEE, May 2020. [PDF](https://apps.fz-juelich.de/jsc-pubsystem/aigaion/attachments/ritter_ea_2020_ipdps.pdf-01cbe96f7a170aba7c7ef941f966d292.pdf)
 
 3. Marcus Ritter, Alexander Geiß, Johannes Wehrstein, Alexandru Calotoiu, Thorsten Reimann, Torsten Hoefler, Felix Wolf: *Noise-Resilient Empirical Performance Modeling with Deep Neural Networks.* In Proc. of the 35th IEEE International Parallel and Distributed Processing Symposium (IPDPS), Portland, Oregon, USA, pages 23–34, IEEE, May 2021. [PDF](http://htor.inf.ethz.ch/publications/img/noiseresilientmodeling.pdf)
-
-
```

### Comparing `extrap-4.0.4/extrap.egg-info/SOURCES.txt` & `extrap-4.1.0a2/extrap.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -17,46 +17,57 @@
 extrap/entities/experiment.py
 extrap/entities/fraction.py
 extrap/entities/functions.py
 extrap/entities/hypotheses.py
 extrap/entities/measurement.py
 extrap/entities/metric.py
 extrap/entities/model.py
+extrap/entities/named_entity.py
 extrap/entities/parameter.py
 extrap/entities/terms.py
+extrap/entities/annotations/__init__.py
+extrap/entities/annotations/comment_annotation/__init__.py
 extrap/extrap/__init__.py
 extrap/extrap/extrapcmd.py
 extrap/extrap/extrapgui.py
 extrap/fileio/__init__.py
-extrap/fileio/cube_file_reader2.py
 extrap/fileio/experiment_io.py
-extrap/fileio/extrap3_experiment_reader.py
 extrap/fileio/io_helper.py
-extrap/fileio/json_file_reader.py
-extrap/fileio/jsonlines_file_reader.py
-extrap/fileio/talpas_file_reader.py
-extrap/fileio/text_file_reader.py
+extrap/fileio/output.py
+extrap/fileio/file_reader/__init__.py
+extrap/fileio/file_reader/abstract_directory_reader.py
+extrap/fileio/file_reader/cube_file_reader2.py
+extrap/fileio/file_reader/extrap3_experiment_reader.py
+extrap/fileio/file_reader/json_file_reader.py
+extrap/fileio/file_reader/jsonlines_file_reader.py
+extrap/fileio/file_reader/talpas_file_reader.py
+extrap/fileio/file_reader/text_file_reader.py
 extrap/gui/AdvancedPlotWidget.py
 extrap/gui/ColorWidget.py
 extrap/gui/CubeFileReader.py
 extrap/gui/DataDisplay.py
-extrap/gui/ExpanderWidget.py
 extrap/gui/GraphWidget.py
 extrap/gui/LogWidget.py
 extrap/gui/MainWidget.py
 extrap/gui/ModelerOptionsWidget.py
 extrap/gui/ModelerWidget.py
-extrap/gui/ParameterValueSlider.py
 extrap/gui/PlotTypeSelector.py
-extrap/gui/ProgressWindow.py
 extrap/gui/SelectorWidget.py
 extrap/gui/TreeModel.py
 extrap/gui/TreeView.py
 extrap/gui/Utils.py
 extrap/gui/__init__.py
+extrap/gui/components/ExpanderWidget.py
+extrap/gui/components/ParameterValueSlider.py
+extrap/gui/components/ProgressWindow.py
+extrap/gui/components/__init__.py
+extrap/gui/components/annotation_delegate.py
+extrap/gui/components/file_dialog.py
+extrap/gui/components/model_color_map.py
+extrap/gui/components/worker.py
 extrap/gui/plots/AllFunctionsAsDifferentSurfacePlotWidget.py
 extrap/gui/plots/AllFunctionsAsOneSurfacePlotWidget.py
 extrap/gui/plots/BaseGraphWidget.py
 extrap/gui/plots/DominatingFunctionsAsHeatMapWidget.py
 extrap/gui/plots/DominatingFunctionsAsSingleScatterPlotWidget.py
 extrap/gui/plots/HeatMapGraphWidget.py
 extrap/gui/plots/InterpolatedContourDisplayWidget.py
@@ -76,11 +87,12 @@
 extrap/modelers/single_parameter/basic.py
 extrap/modelers/single_parameter/refining.py
 extrap/util/__init__.py
 extrap/util/caching.py
 extrap/util/classproperty.py
 extrap/util/deprecation.py
 extrap/util/exceptions.py
+extrap/util/extension_loader.py
 extrap/util/options_parser.py
 extrap/util/progress_bar.py
 extrap/util/serialization_schema.py
 extrap/util/unique_list.py
```

### Comparing `extrap-4.0.4/setup.py` & `extrap-4.1.0a2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of the Extra-P software (http://www.scalasca.org/software/extra-p)
 #
-# Copyright (c) 2020-2021, Technical University of Darmstadt, Germany
+# Copyright (c) 2020-2023, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf8") as fh:
@@ -35,20 +35,30 @@
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    python_requires='>=3.7',
-    install_requires=["pyside2~=5.13", "numpy~=1.18", "matplotlib~=3.2", "tqdm~=4.47", "pycubexr~=1.1",
-                      "marshmallow~=3.7", "packaging~=20.0", "pyobjc-framework-Cocoa~=6.2; sys_platform == 'darwin'"]
+    python_requires='>=3.8',
+    install_requires=[
+        "pyside6~=6.4",
+        "numpy~=1.18",
+        "matplotlib~=3.4",
+        "tqdm~=4.47",
+        "pycubexr>=1.1,<3",
+        "marshmallow~=3.7",
+        "packaging~=20.0",
+        "pyobjc-framework-Cocoa~=9.0; sys_platform == 'darwin'"
+    ]
 )
```

