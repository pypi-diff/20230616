# Comparing `tmp/SpiffWorkflow-2.0.0.tar.gz` & `tmp/SpiffWorkflow-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiffWorkflow-2.0.0.tar", last modified: Fri Jun 16 19:24:00 2023, max compression
+gzip compressed data, was "SpiffWorkflow-2.0.0rc0.tar", last modified: Fri May 26 14:05:01 2023, max compression
```

## Comparing `SpiffWorkflow-2.0.0.tar` & `SpiffWorkflow-2.0.0rc0.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.910130 SpiffWorkflow-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-16 19:24:00.910130 SpiffWorkflow-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.890130 SpiffWorkflow-2.0.0/SpiffWorkflow/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.890130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/PythonScriptEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/PythonScriptEngineEnvironment.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.890130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/
--rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/BpmnParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/ProcessParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/TaskParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/ValidationException.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/event_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/node_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.890130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/BPMN20.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/BPMNDI.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/DC.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/DI.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    60913 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/Semantic.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/spec_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/task_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.894130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/event_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.894130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.894130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/version_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/version_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/version_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/process_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/task_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.894130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/bpmn_process_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/bpmn_task_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/event_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.898130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.898130 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/end_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/event_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/intermediate_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/start_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/exclusive_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/manual_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/multiinstance_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/none_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/script_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/service_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/subworkflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/unstructured_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/user_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.898130 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.898130 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/CamundaParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/event_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/task_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.898130 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/event_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/task_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.898130 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/business_rule_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/event_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/multiinstance_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/user_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.898130 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.902130 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/engine/DMNEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.902130 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/BpmnDmnParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/DMNParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.902130 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DC.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    20095 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMN.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    22615 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMN12.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMN13.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMNDI12.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMNDI13.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.902130 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/serializer/task_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.902130 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/specs/business_rule_task_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/specs/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.902130 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/dotv.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/prettyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    29876 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.906130 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/AcquireMutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/CancelTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Choose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ExclusiveChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/MultiChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/MultiInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ReleaseMutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/StartTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/SubWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ThreadMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ThreadSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ThreadStart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/WorkflowSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/specs/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.906130 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.906130 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/event_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/task_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.906130 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/event_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/task_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.910130 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/event_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.910130 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/mixins/service_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/spiff_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    23151 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.910130 SpiffWorkflow-2.0.0/SpiffWorkflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/util/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/util/deep_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/util/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/util/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/util/levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/util/weakmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/SpiffWorkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:24:00.890130 SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-16 19:24:00.000000 SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-16 19:24:00.000000 SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:24:00.000000 SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 19:24:00.000000 SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 19:24:00.000000 SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 19:24:00.910130 SpiffWorkflow-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-16 19:23:52.000000 SpiffWorkflow-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/PythonScriptEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/PythonScriptEngineEnvironment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/BpmnParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/ProcessParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/TaskParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/ValidationException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/node_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/BPMN20.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/BPMNDI.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/DC.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/DI.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    60913 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/Semantic.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/spec_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/task_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/event_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.632638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/bpmn_process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/bpmn_task_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/event_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/end_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/intermediate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/start_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/exclusive_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/manual_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/multiinstance_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/none_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/script_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/service_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/subworkflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/unstructured_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/user_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/CamundaParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/event_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/business_rule_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/event_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/multiinstance_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/user_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/DMNEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.636638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/BpmnDmnParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/DMNParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DC.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20095 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    22615 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN12.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN13.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMNDI12.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMNDI13.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/business_rule_task_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.640638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/prettyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29876 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/AcquireMutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/CancelTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Choose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ExclusiveChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ReleaseMutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/StartTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/SubWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadStart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/WorkflowSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/event_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/event_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/task_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/event_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/mixins/service_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/spiff_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/deep_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/weakmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-26 14:04:50.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:05:01.628638 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 14:05:01.000000 SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 14:04:51.000000 SpiffWorkflow-2.0.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:05:01.644638 SpiffWorkflow-2.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-26 14:04:51.000000 SpiffWorkflow-2.0.0rc0/setup.py
```

### Comparing `SpiffWorkflow-2.0.0/COPYING` & `SpiffWorkflow-2.0.0rc0/COPYING`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/PKG-INFO` & `SpiffWorkflow-2.0.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiffWorkflow
-Version: 2.0.0
+Version: 2.0.0rc0
 Summary: A workflow framework and BPMN/DMN Processor
 Home-page: https://github.com/sartography/SpiffWorkflow
 Author: Sartography
 Author-email: dan@sartography.com
 License: lGPLv2
 Keywords: spiff workflow bpmn engine
 Classifier: Development Status :: 4 - Beta
```

### Comparing `SpiffWorkflow-2.0.0/README.md` & `SpiffWorkflow-2.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/FeelLikeScriptEngine.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/PythonScriptEngine.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/PythonScriptEngine.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/PythonScriptEngineEnvironment.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/PythonScriptEngineEnvironment.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/exceptions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/exceptions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/BpmnParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/BpmnParser.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/ProcessParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/ProcessParser.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/TaskParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/TaskParser.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/ValidationException.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/ValidationException.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/event_parsers.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/event_parsers.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/node_parser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/node_parser.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/BPMN20.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/BPMN20.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/BPMNDI.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/BPMNDI.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/DC.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/DC.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/DI.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/DI.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/schema/Semantic.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/schema/Semantic.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/spec_description.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/spec_description.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/task_parsers.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/task_parsers.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/parser/util.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/parser/util.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/data_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/data_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/event_definition.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/event_definition.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/dictionary.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/dictionary.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/registry.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/registry.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/helpers/spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/helpers/spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/exceptions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/exceptions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/version_1_1.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_1_1.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/version_1_2.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_1_2.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/migration/version_migration.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/migration/version_migration.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/process_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/process_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/task_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/serializer/workflow.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/serializer/workflow.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/bpmn_process_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/bpmn_process_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/bpmn_task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/bpmn_task_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/control.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     # It would make more sense to have the boundary events and the task
     # they're attached to be inputs rather than outputs.
 
     def __init__(self, wf_spec, name, main_child_task_spec, **kwargs):
         super(_BoundaryEventParent, self).__init__(wf_spec, name, **kwargs)
         self.main_child_task_spec = main_child_task_spec
 
+    @property
+    def spec_type(self):
+        return 'Boundary Event Parent'
+
     def _run_hook(self, my_task):
         # Clear any events that our children might have received and wait for new events
         for child in my_task.children:
             if isinstance(child.task_spec, BoundaryEvent):
                 child.task_spec.event_definition.reset(child)
                 child._set_state(TaskState.WAITING)
         return True
```

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/data_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/data_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/defaults.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/defaults.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/event_definitions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/event_definitions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/bpmn_spec_mixin.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/end_event.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/end_event.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/event_types.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/event_types.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/intermediate_event.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/intermediate_event.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/events/start_event.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/events/start_event.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/exclusive_gateway.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/exclusive_gateway.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/inclusive_gateway.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/manual_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/manual_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/multiinstance_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/multiinstance_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
             return True
         else:
             # Execute again
             if my_task.state != TaskState.WAITING:
                 my_task._set_state(TaskState.WAITING)
             task_spec = my_task.workflow.spec.task_specs[self.task_spec]
             child = my_task._add_child(task_spec, TaskState.WAITING)
-            child.triggered = True
             child.data = deepcopy(my_task.data)
 
     def child_completed_action(self, my_task, child):
         DeepMerge.merge(my_task.data, child.data)
 
     def loop_complete(self, my_task):
         merged = my_task.internal_data.get('merged') or []
@@ -125,15 +124,14 @@
         else:
             DeepMerge.merge(my_task.data, child.data)
 
     def create_child(self, my_task, item, key_or_index=None):
 
         task_spec = my_task.workflow.spec.task_specs[self.task_spec]
         child = my_task._add_child(task_spec, TaskState.WAITING)
-        child.triggered = True
         child.data = deepcopy(my_task.data)
         if self.input_item is not None:
             child.data[self.input_item.bpmn_id] = deepcopy(item)
         if key_or_index is not None:
             child.internal_data['key_or_index'] = key_or_index
         child.task_spec._update(child)
```

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/none_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/none_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/parallel_gateway.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/script_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/script_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/service_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/service_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/subworkflow_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/subworkflow_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/unstructured_join.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/unstructured_join.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/specs/mixins/user_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/specs/mixins/user_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/bpmn/workflow.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/bpmn/workflow.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/CamundaParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/CamundaParser.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/event_parsers.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/event_parsers.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/parser/task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/parser/task_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/config.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/config.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/event_definition.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/event_definition.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/serializer/task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/serializer/task_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/event_definitions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/event_definitions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/multiinstance_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/multiinstance_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/camunda/specs/user_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/camunda/specs/user_task.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/engine/DMNEngine.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/DMNEngine.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/engine/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/BpmnDmnParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/BpmnDmnParser.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/DMNParser.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/DMNParser.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DC.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DC.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMN.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMN12.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN12.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMN13.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMN13.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMNDI12.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMNDI12.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/parser/schema/DMNDI13.xsd` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/parser/schema/DMNDI13.xsd`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/serializer/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/serializer/task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/serializer/task_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/specs/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/specs/business_rule_task_mixin.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/business_rule_task_mixin.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/dmn/specs/model.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/dmn/specs/model.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/exceptions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/operators.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/operators.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/base.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/base.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/dict.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dict.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/dotv.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/dotv.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/exceptions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/exceptions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/json.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/json.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/prettyxml.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/prettyxml.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/serializer/xml.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/serializer/xml.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/AcquireMutex.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/AcquireMutex.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Cancel.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Cancel.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/CancelTask.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/CancelTask.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Choose.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Choose.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ExclusiveChoice.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ExclusiveChoice.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Execute.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Execute.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Gate.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Gate.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Join.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Join.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Merge.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Merge.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/MultiChoice.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiChoice.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/MultiInstance.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/MultiInstance.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ReleaseMutex.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ReleaseMutex.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Simple.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Simple.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/StartTask.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/StartTask.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/SubWorkflow.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/SubWorkflow.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ThreadMerge.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadMerge.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ThreadSplit.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadSplit.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/ThreadStart.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/ThreadStart.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Transform.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Transform.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/Trigger.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/Trigger.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/WorkflowSpec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/WorkflowSpec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/specs/base.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/specs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,18 @@
         self.completed_event = Event()
         self.cancelled_event = Event()
         self.finished_event = Event()
 
         self._wf_spec._add_notify(self)
         self.data.update(self.defines)
 
+    @property
+    def spec_type(self):
+        return f'{self.__class__.__module__}.{self.__class__.__name__}'
+
     def _connect_notify(self, taskspec):
         """
         Called by the previous task to let us know that it exists.
 
         :type  taskspec: TaskSpec
         :param taskspec: The task by which this method is executed.
         """
```

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/event_parsers.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/event_parsers.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/process.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/process.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/parser/task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/parser/task_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/config.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/config.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/event_definition.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/event_definition.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/serializer/task_spec.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/serializer/task_spec.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/defaults.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/defaults.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/event_definitions.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/event_definitions.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/mixins/service_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/mixins/service_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 
     def __init__(self, wf_spec, name, operation_name, operation_params, result_variable, **kwargs):
         super().__init__(wf_spec, name, **kwargs)
         self.operation_name = operation_name
         self.operation_params = operation_params
         self.result_variable = result_variable
 
+    @property
+    def spec_type(self):
+        return 'Service Task'
+
     def _result_variable(self, task):
         if self.result_variable is not None and len(self.result_variable) > 0:
             return self.result_variable
 
         escaped_spec_name = task.task_spec.name.replace('-', '_')
 
         return f'spiff__{escaped_spec_name}_result'
```

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/spiff/specs/spiff_task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/spiff/specs/spiff_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 class SpiffBpmnTask(BpmnSpecMixin):
 
     def __init__(self, wf_spec, name, prescript=None, postscript=None, **kwargs):
         super().__init__(wf_spec, name, **kwargs)
         self.prescript = prescript
         self.postscript = postscript
 
+    @property
+    def spec_type(self):
+        return 'Spiff BPMN Task'
+
     def execute_script(self, my_task, script):
         try:
             my_task.workflow.script_engine.execute(my_task, script)
         except Exception as exc:
             my_task._set_state(TaskState.ERROR)
             raise exc
```

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/task.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,16 +258,17 @@
 
     def log_info(self, dct=None):
         extra = dct or {}
         extra.update({
             'workflow_spec': self.workflow.spec.name,
             'workflow_name': self.workflow.spec.description,
             'task_spec': self.task_spec.name,
+            'task_name': self.task_spec.description,
             'task_id': self.id,
-            'task_type': self.task_spec.__class__.__name__,
+            'task_type': self.task_spec.spec_type,
             'data': self.data if logger.level < 20 else None,
             'internal_data': self.internal_data if logger.level <= 10 else None,
         })
         return extra
 
     def update_data(self, data):
         """
```

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/util/__init__.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/util/compat.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/compat.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/util/deep_merge.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/util/event.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/event.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/util/impl.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/impl.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/util/levenshtein.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/levenshtein.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/util/weakmethod.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/util/weakmethod.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow/workflow.py` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow/workflow.py`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/PKG-INFO` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiffWorkflow
-Version: 2.0.0
+Version: 2.0.0rc0
 Summary: A workflow framework and BPMN/DMN Processor
 Home-page: https://github.com/sartography/SpiffWorkflow
 Author: Sartography
 Author-email: dan@sartography.com
 License: lGPLv2
 Keywords: spiff workflow bpmn engine
 Classifier: Development Status :: 4 - Beta
```

### Comparing `SpiffWorkflow-2.0.0/SpiffWorkflow.egg-info/SOURCES.txt` & `SpiffWorkflow-2.0.0rc0/SpiffWorkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpiffWorkflow-2.0.0/setup.py` & `SpiffWorkflow-2.0.0rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='SpiffWorkflow',
-      version='2.0.0',
+      version='2.0.0rc0',
       description='A workflow framework and BPMN/DMN Processor',
       long_description=README,
       long_description_content_type="text/markdown",
       author='Sartography',
       author_email='dan@sartography.com',
       license='lGPLv2',
       packages=find_packages(exclude=['tests', 'tests.*']),
```

