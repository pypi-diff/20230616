# Comparing `tmp/kuflow_rest-0.6.0.tar.gz` & `tmp/kuflow_rest-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_rest-0.6.0.tar", max compression
+gzip compressed data, was "kuflow_rest-0.6.1.tar", max compression
```

## Comparing `kuflow_rest-0.6.0.tar` & `kuflow_rest-0.6.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      875 2023-06-06 14:03:56.742027 kuflow_rest-0.6.0/README.md
--rw-r--r--   0        0        0        6 2023-06-06 14:03:56.742027 kuflow_rest-0.6.0/VERSION
--rw-r--r--   0        0        0     1335 2023-06-06 14:03:56.742027 kuflow_rest-0.6.0/kuflow_rest/__init__.py
--rw-r--r--   0        0        0     1907 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/__init__.py
--rw-r--r--   0        0        0      599 2023-06-06 14:05:04.171865 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6018 2023-06-06 14:05:04.171865 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
--rw-r--r--   0        0        0     2365 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
--rw-r--r--   0        0        0      732 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0    57905 2023-06-06 14:05:04.187866 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
--rw-r--r--   0        0        0      731 2023-06-06 14:05:04.199867 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc
--rw-r--r--   0        0        0      178 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0        0        0     7108 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_client.py
--rw-r--r--   0        0        0     3983 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_patch.py
--rw-r--r--   0        0        0    78834 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_serialization.py
--rw-r--r--   0        0        0     2007 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_vendor.py
--rw-r--r--   0        0        0     1517 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/_version.py
--rw-r--r--   0        0        0     1854 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/__init__.py
--rw-r--r--   0        0        0     7256 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_client.py
--rw-r--r--   0        0        0     4026 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_configuration.py
--rw-r--r--   0        0        0      674 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_patch.py
--rw-r--r--   0        0        0     2060 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     7284 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     7894 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_principal_operations.py
--rw-r--r--   0        0        0    35197 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_process_operations.py
--rw-r--r--   0        0        0    62010 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_task_operations.py
--rw-r--r--   0        0        0     5465 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__init__.py
--rw-r--r--   0        0        0     3261 2023-06-06 14:05:04.171865 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2558 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
--rw-r--r--   0        0        0    65326 2023-06-06 14:05:04.179865 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0      739 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     3294 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/_enums.py
--rw-r--r--   0        0        0    75667 2023-06-06 14:03:56.746028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/_models.py
--rw-r--r--   0        0        0      674 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/models/_patch.py
--rw-r--r--   0        0        0     2060 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__init__.py
--rw-r--r--   0        0        0      737 2023-06-06 14:05:04.195867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5603 2023-06-06 14:05:04.199867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0      743 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     6811 2023-06-06 14:05:04.199867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0    28491 2023-06-06 14:05:04.203867 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0    51369 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     7884 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_authentication_operations.py
--rw-r--r--   0        0        0      674 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_patch.py
--rw-r--r--   0        0        0     9804 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_principal_operations.py
--rw-r--r--   0        0        0    41967 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_process_operations.py
--rw-r--r--   0        0        0    76156 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_task_operations.py
--rw-r--r--   0        0        0       26 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_generated/py.typed
--rw-r--r--   0        0        0     7722 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/_kuflow_rest_client.py
--rw-r--r--   0        0        0     4771 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/models/__init__.py
--rw-r--r--   0        0        0     2858 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4588 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0     4581 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/models/_models.py
--rw-r--r--   0        0        0     1440 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/__init__.py
--rw-r--r--   0        0        0      460 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1691 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0     3429 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0     9070 2023-06-06 14:05:04.211868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0    16316 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     2324 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_authentication_operations.py
--rw-r--r--   0        0        0     4116 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_principal_operations.py
--rw-r--r--   0        0        0     9540 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_process_operations.py
--rw-r--r--   0        0        0    17441 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/operations/_task_operations.py
--rw-r--r--   0        0        0     6837 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/utils/__init__.py
--rw-r--r--   0        0        0     3980 2023-06-06 14:05:04.215868 kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    31360 2023-06-06 14:05:04.223869 kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc
--rw-r--r--   0        0        0    17040 2023-06-06 14:05:04.219869 kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc
--rw-r--r--   0        0        0    41580 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/utils/_element_values.py
--rw-r--r--   0        0        0    23171 2023-06-06 14:03:56.750028 kuflow_rest-0.6.0/kuflow_rest/utils/_json_forms.py
--rw-r--r--   0        0        0      977 2023-06-06 14:05:20.689295 kuflow_rest-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-0.6.0/setup.py
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      875 2023-06-16 09:00:12.903233 kuflow_rest-0.6.1/README.md
+-rw-r--r--   0        0        0        6 2023-06-16 09:00:12.903233 kuflow_rest-0.6.1/VERSION
+-rw-r--r--   0        0        0     1335 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/__init__.py
+-rw-r--r--   0        0        0     1907 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-16 09:01:21.056971 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6018 2023-06-16 09:01:21.056971 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
+-rw-r--r--   0        0        0     2365 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0    57905 2023-06-16 09:01:21.076973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
+-rw-r--r--   0        0        0      731 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc
+-rw-r--r--   0        0        0      178 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0        0        0     7108 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_client.py
+-rw-r--r--   0        0        0     3983 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_patch.py
+-rw-r--r--   0        0        0    78834 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_serialization.py
+-rw-r--r--   0        0        0     2007 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_vendor.py
+-rw-r--r--   0        0        0     1517 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/_version.py
+-rw-r--r--   0        0        0     1854 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/__init__.py
+-rw-r--r--   0        0        0     7256 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_client.py
+-rw-r--r--   0        0        0     4026 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_configuration.py
+-rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_patch.py
+-rw-r--r--   0        0        0     2060 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     7284 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     7894 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_principal_operations.py
+-rw-r--r--   0        0        0    35197 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_process_operations.py
+-rw-r--r--   0        0        0    62010 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_task_operations.py
+-rw-r--r--   0        0        0     5465 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__init__.py
+-rw-r--r--   0        0        0     3261 2023-06-16 09:01:21.060972 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2558 2023-06-16 09:01:21.080973 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
+-rw-r--r--   0        0        0    65326 2023-06-16 09:01:21.064972 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0      739 2023-06-16 09:01:21.080973 kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     3294 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/_enums.py
+-rw-r--r--   0        0        0    75667 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/_models.py
+-rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/models/_patch.py
+-rw-r--r--   0        0        0     2060 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__init__.py
+-rw-r--r--   0        0        0      737 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5603 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0      743 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     6811 2023-06-16 09:01:21.084973 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    28491 2023-06-16 09:01:21.088974 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    51369 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     7884 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      674 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_patch.py
+-rw-r--r--   0        0        0     9804 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_principal_operations.py
+-rw-r--r--   0        0        0    41967 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_process_operations.py
+-rw-r--r--   0        0        0    76156 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_task_operations.py
+-rw-r--r--   0        0        0       26 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_generated/py.typed
+-rw-r--r--   0        0        0     7722 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/_kuflow_rest_client.py
+-rw-r--r--   0        0        0     4771 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/models/__init__.py
+-rw-r--r--   0        0        0     2858 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4588 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0     4581 2023-06-16 09:00:12.907234 kuflow_rest-0.6.1/kuflow_rest/models/_models.py
+-rw-r--r--   0        0        0     1440 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-16 09:01:21.096974 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1665 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     3408 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     9051 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    16300 2023-06-16 09:01:21.100975 kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     2322 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_authentication_operations.py
+-rw-r--r--   0        0        0     4113 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_principal_operations.py
+-rw-r--r--   0        0        0     9530 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_process_operations.py
+-rw-r--r--   0        0        0    17424 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/operations/_task_operations.py
+-rw-r--r--   0        0        0     6837 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/utils/__init__.py
+-rw-r--r--   0        0        0     3980 2023-06-16 09:01:21.104975 kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    31360 2023-06-16 09:01:21.108976 kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc
+-rw-r--r--   0        0        0    17040 2023-06-16 09:01:21.104975 kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc
+-rw-r--r--   0        0        0    41580 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/utils/_element_values.py
+-rw-r--r--   0        0        0    23171 2023-06-16 09:00:12.911234 kuflow_rest-0.6.1/kuflow_rest/utils/_json_forms.py
+-rw-r--r--   0        0        0      977 2023-06-16 09:01:38.346427 kuflow_rest-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-0.6.1/setup.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-0.6.1/PKG-INFO
```

### Comparing `kuflow_rest-0.6.0/README.md` & `kuflow_rest-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from ._kuflow_rest_client import KuFlowRestClient
 from ._generated._serialization import Deserializer, Serializer, Model
 
 __all__ = ["Deserializer", "KuFlowRestClient", "Model", "Serializer"]
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 1907 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 7307 0000  U........<.ds...
+00000000: 550d 0d0a 0000 0000 9c24 8c64 7307 0000  U........$.ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6503 5a04 7a18 6400 6403  m.Z...e.Z.z.d.d.
 00000050: 6c05 6d06 5a07 0100 6400 6404 6c05 5400  l.m.Z...d.d.l.T.
 00000060: 5700 6e18 0400 6508 6b0a 724c 0100 0100  W.n...e.k.rL....
 00000070: 0100 6700 5a07 5900 6e02 5800 6400 6405  ..g.Z.Y.n.X.d.d.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 7108 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 c41b 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 c41b 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6405 6406 6c0a 6d0b 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6407 6c0d 6d0e 5a0e 0100 6405  ..d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 3983 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 8f0f 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 8f0f 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6502 7244 6400 6406 6c09 6d0a 5a0a  ..e.rDd.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6504 8303  ..G.d.d...d.e...
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 a202 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 a202 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 78834 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 f233 0100  U........<.d.3..
+00000000: 550d 0d0a 0000 0000 9c24 8c64 f233 0100  U........$.d.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c602 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6402 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 5a05 6400 6402 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 6400 6402 6c09  d.l.m.Z...d.d.l.
 00000070: 5a09 6400 6402 6c0a 5a0a 6400 6402 6c0b  Z.d.d.l.Z.d.d.l.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/__pycache__/_vendor.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 2007 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 d707 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 d707 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 8400 5a03 6404 5300 2905 e900 0000  d...Z.d.S.).....
 00000050: 0029 02da 044c 6973 74da 0463 6173 7463  .)...List..castc
 00000060: 0100 0000 0000 0000 0000 0000 0400 0000  ................
 00000070: 0a00 0000 0b00 0000 7376 0000 007c 00a0  ........sv...|..
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/_client.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/_configuration.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/_patch.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/_serialization.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/_vendor.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/_version.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
-VERSION = "0.6.0"
+VERSION = "0.6.1"
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_client.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_configuration.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/_patch.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_patch.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_principal_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_process_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/aio/operations/_task_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/aio/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 5465 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 5915 0000  U........<.dY...
+00000000: 550d 0d0a 0000 0000 9c24 8c64 5915 0000  U........$.dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0037 0000 0040 0000 0073 4403 0000 6400  .7...@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c00 6d05 5a05 0100 6400 6406 6c00  d.l.m.Z...d.d.l.
 00000070: 6d06 5a06 0100 6400 6407 6c00 6d07 5a07  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 3294 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 de0c 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 de0c 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 6501 6503 6405 8d05 5a05 4700 6406  e.e.e.d...Z.G.d.
 00000060: 6407 8400 6407 6504 6501 6503 6405 8d05  d...d.e.e.e.d...
 00000070: 5a06 4700 6408 6409 8400 6409 6504 6501  Z.G.d.d...d.e.e.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 75667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 9327 0100  U........<.d.'..
+00000000: 550d 0d0a 0000 0000 9c24 8c64 9327 0100  U........$.d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e03 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6403  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6501 6a0b 6405  d.l.m.Z...e.j.d.
 00000070: 6b05 7254 6400 6406 6c02 6d0c 5a0c 0100  k.rTd.d.l.m.Z...
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 a202 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 a202 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
@@ -27,21 +27,21 @@
 000001a0: 6820 7573 696e 6720 7468 6520 7465 6368  h using the tech
 000001b0: 6e69 7175 6573 2064 6573 6372 6962 6564  niques described
 000001c0: 2069 6e0a 2020 2020 6874 7470 733a 2f2f   in.    https://
 000001d0: 616b 612e 6d73 2f61 7a73 646b 2f70 7974  aka.ms/azsdk/pyt
 000001e0: 686f 6e2f 6470 636f 6465 6765 6e2f 7079  hon/dpcodegen/py
 000001f0: 7468 6f6e 2f63 7573 746f 6d69 7a65 0a20  thon/customize. 
 00000200: 2020 204e a900 7204 0000 0072 0400 0000     N..r....r....
-00000210: 7204 0000 00fa 4b2f 776f 726b 2f6b 7566  r.....K/work/kuf
+00000210: 7204 0000 00fa 4f2f 776f 726b 2f6b 7566  r.....O/work/kuf
 00000220: 6c6f 772d 7364 6b2d 7079 7468 6f6e 2f6b  low-sdk-python/k
 00000230: 7566 6c6f 772d 7265 7374 2f6b 7566 6c6f  uflow-rest/kuflo
 00000240: 775f 7265 7374 2f5f 6765 6e65 7261 7465  w_rest/_generate
-00000250: 642f 6d6f 6465 6c73 2f5f 7061 7463 682e  d/models/_patch.
-00000260: 7079 da09 7061 7463 685f 7364 6b0e 0000  py..patch_sdk...
-00000270: 0073 0200 0000 0001 7206 0000 004e 2907  .s......r....N).
-00000280: da07 5f5f 646f 635f 5fda 0674 7970 696e  ..__doc__..typin
-00000290: 6772 0200 0000 7203 0000 00da 0373 7472  gr....r......str
-000002a0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-000002b0: 5f72 0600 0000 7204 0000 0072 0400 0000  _r....r....r....
-000002c0: 7204 0000 0072 0500 0000 da08 3c6d 6f64  r....r......<mod
-000002d0: 756c 653e 0500 0000 7306 0000 0006 040c  ule>....s.......
-000002e0: 0210 03                                  ...
+00000250: 642f 6f70 6572 6174 696f 6e73 2f5f 7061  d/operations/_pa
+00000260: 7463 682e 7079 da09 7061 7463 685f 7364  tch.py..patch_sd
+00000270: 6b0e 0000 0073 0200 0000 0001 7206 0000  k....s......r...
+00000280: 004e 2907 da07 5f5f 646f 635f 5fda 0674  .N)...__doc__..t
+00000290: 7970 696e 6772 0200 0000 7203 0000 00da  ypingr....r.....
+000002a0: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
+000002b0: 6f6e 735f 5f72 0600 0000 7204 0000 0072  ons__r....r....r
+000002c0: 0400 0000 7204 0000 0072 0500 0000 da08  ....r....r......
+000002d0: 3c6d 6f64 756c 653e 0500 0000 7306 0000  <module>....s...
+000002e0: 0006 040c 0210 03                        .......
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/_enums.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/_models.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/models/_patch.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 2060 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 0c08 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 0c08 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a0a 0100 6400 6406 6c08  d.l.m.Z...d.d.l.
 00000070: 5400 6400 6407 6c08 6d0b 5a0c 0100 6408  T.d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 7884 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 cc1e 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 cc1e 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6403 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 9804 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 4c26 0000  U........<.dL&..
+00000000: 550d 0d0a 0000 0000 9c24 8c64 4c26 0000  U........$.dL&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4801 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6403 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 41967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 efa3 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 efa3 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 0100 6400 6403 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 76156 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 7c29 0100  U........<.d|)..
+00000000: 550d 0d0a 0000 0000 9c24 8c64 7c29 0100  U........$.d|)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 9c02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6400 6403 6c0d  m.Z.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_authentication_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_patch.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_principal_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_process_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_generated/operations/_task_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/_generated/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/_kuflow_rest_client.py` & `kuflow_rest-0.6.1/kuflow_rest/_kuflow_rest_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/models/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 4771 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 a312 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 a312 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 003d 0000 0040 0000 0073 aa01 0000 6400  .=...@...s....d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0f 5a0f 6d10 5a10 6d11 5a11 6d12 5a12  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 4581 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 e511 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 e511 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a05 4700 6406 6407 8400  ..d...Z.G.d.d...
 00000060: 6407 8302 5a06 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
 00000070: 8302 5a07 4700 640a 640b 8400 640b 8302  ..Z.G.d.d...d...
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/models/_models.py` & `kuflow_rest-0.6.1/kuflow_rest/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 2324 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 1409 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 1209 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 6d05 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a07 6406 5300 2907 e900  ..d...Z.d.S.)...
 00000060: 0000 0029 01da 0341 6e79 e902 0000 0029  ...)...Any.....)
 00000070: 02da 066d 6f64 656c 73da 104b 7546 6c6f  ...models..KuFlo
@@ -28,79 +28,78 @@
 000001b0: 5265 7374 436c 6965 6e74 6027 730a 2020  RestClient`'s.  
 000001c0: 2020 2020 2020 3a61 7474 723a 6061 7574        :attr:`aut
 000001d0: 6865 6e74 6963 6174 696f 6e60 2061 7474  hentication` att
 000001e0: 7269 6275 7465 2e0a 2020 2020 2901 da0d  ribute..    )...
 000001f0: 6b75 666c 6f77 5f63 6c69 656e 7463 0200  kuflow_clientc..
 00000200: 0000 0000 0000 0000 0000 0200 0000 0200  ................
 00000210: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-00000220: 0064 0053 0029 014e 2901 da28 5f41 7574  .d.S.).N)..(_Aut
-00000230: 6865 6e74 6963 6174 696f 6e4f 7065 7261  henticationOpera
-00000240: 7469 6f6e 735f 5f6b 7566 6c6f 775f 636c  tions__kuflow_cl
-00000250: 6965 6e74 2902 da04 7365 6c66 7207 0000  ient)...selfr...
-00000260: 00a9 0072 0a00 0000 fa58 2f77 6f72 6b2f  ...r.....X/work/
-00000270: 6b75 666c 6f77 2d73 646b 2d70 7974 686f  kuflow-sdk-pytho
-00000280: 6e2f 6b75 666c 6f77 2d72 6573 742f 6b75  n/kuflow-rest/ku
-00000290: 666c 6f77 5f72 6573 742f 6f70 6572 6174  flow_rest/operat
-000002a0: 696f 6e73 2f5f 6175 7468 656e 7469 6361  ions/_authentica
-000002b0: 7469 6f6e 5f6f 7065 7261 7469 6f6e 732e  tion_operations.
-000002c0: 7079 da08 5f5f 696e 6974 5f5f 2a00 0000  py..__init__*...
-000002d0: 7302 0000 0000 017a 2141 7574 6865 6e74  s......z!Authent
-000002e0: 6963 6174 696f 6e4f 7065 7261 7469 6f6e  icationOperation
-000002f0: 732e 5f5f 696e 6974 5f5f 2903 da0e 6175  s.__init__)...au
-00000300: 7468 656e 7469 6361 7469 6f6e da06 6b77  thentication..kw
-00000310: 6172 6773 da06 7265 7475 726e 6302 0000  args..returnc...
-00000320: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000330: 004b 0000 0073 1800 0000 7c00 6a00 6a01  .K...s....|.j.j.
-00000340: 6a02 6600 6401 7c01 6901 7c02 9702 8e01  j.f.d.|.i.|.....
-00000350: 5300 2902 61ba 0100 0043 7265 6174 6520  S.).a....Create 
-00000360: 616e 2061 7574 6865 6e74 6963 6174 696f  an authenticatio
-00000370: 6e20 666f 7220 7468 6520 6375 7272 656e  n for the curren
-00000380: 7420 7072 696e 6369 7061 6c2e 0a0a 2020  t principal...  
-00000390: 2020 2020 2020 4372 6561 7465 2061 6e20        Create an 
-000003a0: 6175 7468 656e 7469 6361 7469 6f6e 2066  authentication f
-000003b0: 6f72 2074 6865 2063 7572 7265 6e74 2070  or the current p
-000003c0: 7269 6e63 6970 616c 2e0a 0a20 2020 2020  rincipal...     
-000003d0: 2020 203a 7061 7261 6d20 6175 7468 656e     :param authen
-000003e0: 7469 6361 7469 6f6e 3a20 4175 7468 656e  tication: Authen
-000003f0: 7469 6361 7469 6f6e 2074 6f20 6265 2063  tication to be c
-00000400: 7265 6174 6564 2e20 4973 2065 6974 6865  reated. Is eithe
-00000410: 7220 6120 6d6f 6465 6c20 7479 7065 206f  r a model type o
-00000420: 7220 6120 494f 2074 7970 652e 2052 6571  r a IO type. Req
-00000430: 7569 7265 642e 0a20 2020 2020 2020 203a  uired..        :
-00000440: 7479 7065 2061 7574 6865 6e74 6963 6174  type authenticat
-00000450: 696f 6e3a 207e 6b75 666c 6f77 2e72 6573  ion: ~kuflow.res
-00000460: 742e 6d6f 6465 6c73 2e41 7574 6865 6e74  t.models.Authent
-00000470: 6963 6174 696f 6e20 6f72 2049 4f0a 2020  ication or IO.  
-00000480: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
-00000490: 7574 6865 6e74 6963 6174 696f 6e0a 2020  uthentication.  
-000004a0: 2020 2020 2020 3a72 7479 7065 3a20 7e6b        :rtype: ~k
-000004b0: 7566 6c6f 772e 7265 7374 2e6d 6f64 656c  uflow.rest.model
-000004c0: 732e 4175 7468 656e 7469 6361 7469 6f6e  s.Authentication
-000004d0: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
-000004e0: 207e 617a 7572 652e 636f 7265 2e65 7863   ~azure.core.exc
-000004f0: 6570 7469 6f6e 732e 4874 7470 5265 7370  eptions.HttpResp
-00000500: 6f6e 7365 4572 726f 723a 0a20 2020 2020  onseError:.     
-00000510: 2020 2072 0d00 0000 2903 7208 0000 0072     r....).r....r
-00000520: 0d00 0000 da15 6372 6561 7465 5f61 7574  ......create_aut
-00000530: 6865 6e74 6963 6174 696f 6e29 0372 0900  hentication).r..
-00000540: 0000 720d 0000 0072 0e00 0000 720a 0000  ..r....r....r...
-00000550: 0072 0a00 0000 720b 0000 0072 1000 0000  .r....r....r....
-00000560: 2d00 0000 7302 0000 0000 0b7a 2e41 7574  -...s......z.Aut
-00000570: 6865 6e74 6963 6174 696f 6e4f 7065 7261  henticationOpera
-00000580: 7469 6f6e 732e 6372 6561 7465 5f61 7574  tions.create_aut
-00000590: 6865 6e74 6963 6174 696f 6e4e 290a da08  henticationN)...
-000005a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000005b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000005c0: 5f5f da07 5f5f 646f 635f 5fda 194b 7546  __..__doc__..KuF
-000005d0: 6c6f 7752 6573 7443 6c69 656e 7447 656e  lowRestClientGen
-000005e0: 6572 6174 6564 720c 0000 00da 075f 6d6f  eratedr......_mo
-000005f0: 6465 6c73 da0e 4175 7468 656e 7469 6361  dels..Authentica
-00000600: 7469 6f6e 7202 0000 0072 1000 0000 720a  tionr....r....r.
-00000610: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
-00000620: 0000 7206 0000 0020 0000 0073 0600 0000  ..r.... ...s....
-00000630: 0801 0409 0e03 7206 0000 004e 2908 da06  ......r....N)...
-00000640: 7479 7069 6e67 7202 0000 00da 0a5f 6765  typingr......_ge
-00000650: 6e65 7261 7465 6472 0400 0000 7216 0000  neratedr....r...
-00000660: 0072 0500 0000 7215 0000 0072 0600 0000  .r....r....r....
-00000670: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000680: 0b00 0000 da08 3c6d 6f64 756c 653e 1b00  ......<module>..
-00000690: 0000 7304 0000 000c 0210 03              ..s........
+00000220: 0064 0053 0029 014e 2901 da0e 5f6b 7566  .d.S.).N)..._kuf
+00000230: 6c6f 775f 636c 6965 6e74 2902 da04 7365  low_client)...se
+00000240: 6c66 7207 0000 00a9 0072 0a00 0000 fa58  lfr......r.....X
+00000250: 2f77 6f72 6b2f 6b75 666c 6f77 2d73 646b  /work/kuflow-sdk
+00000260: 2d70 7974 686f 6e2f 6b75 666c 6f77 2d72  -python/kuflow-r
+00000270: 6573 742f 6b75 666c 6f77 5f72 6573 742f  est/kuflow_rest/
+00000280: 6f70 6572 6174 696f 6e73 2f5f 6175 7468  operations/_auth
+00000290: 656e 7469 6361 7469 6f6e 5f6f 7065 7261  entication_opera
+000002a0: 7469 6f6e 732e 7079 da08 5f5f 696e 6974  tions.py..__init
+000002b0: 5f5f 2a00 0000 7302 0000 0000 017a 2141  __*...s......z!A
+000002c0: 7574 6865 6e74 6963 6174 696f 6e4f 7065  uthenticationOpe
+000002d0: 7261 7469 6f6e 732e 5f5f 696e 6974 5f5f  rations.__init__
+000002e0: 2903 da0e 6175 7468 656e 7469 6361 7469  )...authenticati
+000002f0: 6f6e da06 6b77 6172 6773 da06 7265 7475  on..kwargs..retu
+00000300: 726e 6302 0000 0000 0000 0000 0000 0003  rnc.............
+00000310: 0000 0004 0000 004b 0000 0073 1800 0000  .......K...s....
+00000320: 7c00 6a00 6a01 6a02 6600 6401 7c01 6901  |.j.j.j.f.d.|.i.
+00000330: 7c02 9702 8e01 5300 2902 61ba 0100 0043  |.....S.).a....C
+00000340: 7265 6174 6520 616e 2061 7574 6865 6e74  reate an authent
+00000350: 6963 6174 696f 6e20 666f 7220 7468 6520  ication for the 
+00000360: 6375 7272 656e 7420 7072 696e 6369 7061  current principa
+00000370: 6c2e 0a0a 2020 2020 2020 2020 4372 6561  l...        Crea
+00000380: 7465 2061 6e20 6175 7468 656e 7469 6361  te an authentica
+00000390: 7469 6f6e 2066 6f72 2074 6865 2063 7572  tion for the cur
+000003a0: 7265 6e74 2070 7269 6e63 6970 616c 2e0a  rent principal..
+000003b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000003c0: 6175 7468 656e 7469 6361 7469 6f6e 3a20  authentication: 
+000003d0: 4175 7468 656e 7469 6361 7469 6f6e 2074  Authentication t
+000003e0: 6f20 6265 2063 7265 6174 6564 2e20 4973  o be created. Is
+000003f0: 2065 6974 6865 7220 6120 6d6f 6465 6c20   either a model 
+00000400: 7479 7065 206f 7220 6120 494f 2074 7970  type or a IO typ
+00000410: 652e 2052 6571 7569 7265 642e 0a20 2020  e. Required..   
+00000420: 2020 2020 203a 7479 7065 2061 7574 6865       :type authe
+00000430: 6e74 6963 6174 696f 6e3a 207e 6b75 666c  ntication: ~kufl
+00000440: 6f77 2e72 6573 742e 6d6f 6465 6c73 2e41  ow.rest.models.A
+00000450: 7574 6865 6e74 6963 6174 696f 6e20 6f72  uthentication or
+00000460: 2049 4f0a 2020 2020 2020 2020 3a72 6574   IO.        :ret
+00000470: 7572 6e3a 2041 7574 6865 6e74 6963 6174  urn: Authenticat
+00000480: 696f 6e0a 2020 2020 2020 2020 3a72 7479  ion.        :rty
+00000490: 7065 3a20 7e6b 7566 6c6f 772e 7265 7374  pe: ~kuflow.rest
+000004a0: 2e6d 6f64 656c 732e 4175 7468 656e 7469  .models.Authenti
+000004b0: 6361 7469 6f6e 0a20 2020 2020 2020 203a  cation.        :
+000004c0: 7261 6973 6573 207e 617a 7572 652e 636f  raises ~azure.co
+000004d0: 7265 2e65 7863 6570 7469 6f6e 732e 4874  re.exceptions.Ht
+000004e0: 7470 5265 7370 6f6e 7365 4572 726f 723a  tpResponseError:
+000004f0: 0a20 2020 2020 2020 2072 0d00 0000 2903  .        r....).
+00000500: 7208 0000 0072 0d00 0000 da15 6372 6561  r....r......crea
+00000510: 7465 5f61 7574 6865 6e74 6963 6174 696f  te_authenticatio
+00000520: 6e29 0372 0900 0000 720d 0000 0072 0e00  n).r....r....r..
+00000530: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000540: 0072 1000 0000 2d00 0000 7302 0000 0000  .r....-...s.....
+00000550: 0b7a 2e41 7574 6865 6e74 6963 6174 696f  .z.Authenticatio
+00000560: 6e4f 7065 7261 7469 6f6e 732e 6372 6561  nOperations.crea
+00000570: 7465 5f61 7574 6865 6e74 6963 6174 696f  te_authenticatio
+00000580: 6e4e 290a da08 5f5f 6e61 6d65 5f5f da0a  nN)...__name__..
+00000590: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000005a0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+000005b0: 5fda 194b 7546 6c6f 7752 6573 7443 6c69  _..KuFlowRestCli
+000005c0: 656e 7447 656e 6572 6174 6564 720c 0000  entGeneratedr...
+000005d0: 00da 075f 6d6f 6465 6c73 da0e 4175 7468  ..._models..Auth
+000005e0: 656e 7469 6361 7469 6f6e 7202 0000 0072  enticationr....r
+000005f0: 1000 0000 720a 0000 0072 0a00 0000 720a  ....r....r....r.
+00000600: 0000 0072 0b00 0000 7206 0000 0020 0000  ...r....r.... ..
+00000610: 0073 0600 0000 0801 0409 0e03 7206 0000  .s..........r...
+00000620: 004e 2908 da06 7479 7069 6e67 7202 0000  .N)...typingr...
+00000630: 00da 0a5f 6765 6e65 7261 7465 6472 0400  ..._generatedr..
+00000640: 0000 7216 0000 0072 0500 0000 7215 0000  ..r....r....r...
+00000650: 0072 0600 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000660: 720a 0000 0072 0b00 0000 da08 3c6d 6f64  r....r......<mod
+00000670: 756c 653e 1b00 0000 7304 0000 000c 0210  ule>....s.......
+00000680: 03                                       .
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 4116 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 1410 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 1110 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 6d08 5a09 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 8302 5a0a 6406 5300 2907 e900 0000 0029  ..Z.d.S.)......)
 00000070: 04da 0341 6e79 da04 4c69 7374 da08 4f70  ...Any..List..Op
@@ -34,182 +34,180 @@
 00000210: 5265 7374 436c 6965 6e74 6027 730a 2020  RestClient`'s.  
 00000220: 2020 2020 2020 3a61 7474 723a 6070 7269        :attr:`pri
 00000230: 6e63 6970 616c 6020 6174 7472 6962 7574  ncipal` attribut
 00000240: 652e 0a20 2020 2029 01da 0d6b 7566 6c6f  e..    )...kuflo
 00000250: 775f 636c 6965 6e74 6302 0000 0000 0000  w_clientc.......
 00000260: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000270: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
-00000280: 2901 4e29 01da 235f 5072 696e 6369 7061  ).N)..#_Principa
-00000290: 6c4f 7065 7261 7469 6f6e 735f 5f6b 7566  lOperations__kuf
-000002a0: 6c6f 775f 636c 6965 6e74 2902 da04 7365  low_client)...se
-000002b0: 6c66 720a 0000 00a9 0072 0d00 0000 fa53  lfr......r.....S
-000002c0: 2f77 6f72 6b2f 6b75 666c 6f77 2d73 646b  /work/kuflow-sdk
-000002d0: 2d70 7974 686f 6e2f 6b75 666c 6f77 2d72  -python/kuflow-r
-000002e0: 6573 742f 6b75 666c 6f77 5f72 6573 742f  est/kuflow_rest/
-000002f0: 6f70 6572 6174 696f 6e73 2f5f 7072 696e  operations/_prin
-00000300: 6369 7061 6c5f 6f70 6572 6174 696f 6e73  cipal_operations
-00000310: 2e70 79da 085f 5f69 6e69 745f 5f2a 0000  .py..__init__*..
-00000320: 0073 0200 0000 0001 7a1c 5072 696e 6369  .s......z.Princi
-00000330: 7061 6c4f 7065 7261 7469 6f6e 732e 5f5f  palOperations.__
-00000340: 696e 6974 5f5f e919 0000 0072 0100 0000  init__.....r....
-00000350: 4e29 07da 0473 697a 65da 0470 6167 65da  N)...size..page.
-00000360: 0473 6f72 74da 0474 7970 65da 0867 726f  .sort..type..gro
-00000370: 7570 5f69 64da 066b 7761 7267 73da 0672  up_id..kwargs..r
-00000380: 6574 7572 6e63 0600 0000 0000 0000 0000  eturnc..........
-00000390: 0000 0700 0000 0800 0000 4b00 0000 7350  ..........K...sP
-000003a0: 0000 007c 0364 016b 0972 1874 007c 0374  ...|.d.k.r.t.|.t
-000003b0: 0183 0272 187c 0367 017d 037c 0564 016b  ...r.|.g.}.|.d.k
-000003c0: 0972 3074 007c 0574 0183 0272 307c 0567  .r0t.|.t...r0|.g
-000003d0: 017d 057c 006a 026a 036a 0466 007c 017c  .}.|.j.j.j.f.|.|
-000003e0: 027c 037c 047c 0564 029c 057c 0697 028e  .|.|.|.d...|....
-000003f0: 0153 0029 0361 3605 0000 4669 6e64 2061  .S.).a6...Find a
-00000400: 6c6c 2061 6363 6573 7369 626c 6520 5072  ll accessible Pr
-00000410: 696e 6369 7061 6c73 2e0a 0a20 2020 2020  incipals...     
-00000420: 2020 204c 6973 7420 616c 6c20 7468 6520     List all the 
-00000430: 5072 696e 6369 7061 6c73 2074 6861 7420  Principals that 
-00000440: 6861 7665 2062 6565 6e20 6372 6561 7465  have been create
-00000450: 6420 616e 6420 7468 6520 7573 6564 2063  d and the used c
-00000460: 7265 6465 6e74 6961 6c73 2068 6173 2061  redentials has a
-00000470: 6363 6573 732e 0a0a 2020 2020 2020 2020  ccess...        
-00000480: 4176 6169 6c61 626c 6520 736f 7274 2071  Available sort q
-00000490: 7565 7279 2076 616c 7565 733a 2069 642c  uery values: id,
-000004a0: 206e 616d 652e 0a0a 2020 2020 2020 2020   name...        
-000004b0: 3a6b 6579 776f 7264 2073 697a 653a 2054  :keyword size: T
-000004c0: 6865 206e 756d 6265 7220 6f66 2072 6563  he number of rec
-000004d0: 6f72 6473 2072 6574 7572 6e65 6420 7769  ords returned wi
-000004e0: 7468 696e 2061 2073 696e 676c 6520 4150  thin a single AP
-000004f0: 4920 6361 6c6c 2e20 4465 6661 756c 7420  I call. Default 
-00000500: 7661 6c75 6520 6973 2032 352e 0a20 2020  value is 25..   
-00000510: 2020 2020 203a 7479 7065 2073 697a 653a       :type size:
-00000520: 2069 6e74 0a20 2020 2020 2020 203a 6b65   int.        :ke
-00000530: 7977 6f72 6420 7061 6765 3a20 5468 6520  yword page: The 
-00000540: 7061 6765 206e 756d 6265 7220 6f66 2074  page number of t
-00000550: 6865 2063 7572 7265 6e74 2070 6167 6520  he current page 
-00000560: 696e 2074 6865 2072 6574 7572 6e65 6420  in the returned 
-00000570: 7265 636f 7264 732c 2030 2069 7320 7468  records, 0 is th
-00000580: 6520 6669 7273 7420 7061 6765 2e0a 2020  e first page..  
-00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005a0: 2020 2020 2044 6566 6175 6c74 2076 616c       Default val
-000005b0: 7565 2069 7320 302e 0a20 2020 2020 2020  ue is 0..       
-000005c0: 203a 7479 7065 2070 6167 653a 2069 6e74   :type page: int
-000005d0: 0a20 2020 2020 2020 203a 6b65 7977 6f72  .        :keywor
-000005e0: 6420 736f 7274 3a20 536f 7274 696e 6720  d sort: Sorting 
-000005f0: 6372 6974 6572 6961 2069 6e20 7468 6520  criteria in the 
-00000600: 666f 726d 6174 3a20 7072 6f70 6572 7479  format: property
-00000610: 7b2c 6173 637c 6465 7363 7d2e 2045 7861  {,asc|desc}. Exa
-00000620: 6d70 6c65 3a20 6372 6561 7465 6441 742c  mple: createdAt,
-00000630: 6465 7363 0a20 2020 2020 2020 2020 2020  desc.           
-00000640: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00000650: 756c 7420 736f 7274 206f 7264 6572 2069  ult sort order i
-00000660: 7320 6173 6365 6e64 696e 672e 204d 756c  s ascending. Mul
-00000670: 7469 706c 6520 736f 7274 2063 7269 7465  tiple sort crite
-00000680: 7269 6120 6172 6520 7375 7070 6f72 7465  ria are supporte
-00000690: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-000006a0: 2020 2020 2020 2020 2020 506c 6561 7365            Please
-000006b0: 2072 6566 6572 2074 6f20 7468 6520 6d65   refer to the me
-000006c0: 7468 6f64 2064 6573 6372 6970 7469 6f6e  thod description
-000006d0: 2066 6f72 2073 7570 706f 7274 6564 2070   for supported p
-000006e0: 726f 7065 7274 6965 732e 2044 6566 6175  roperties. Defau
-000006f0: 6c74 2076 616c 7565 2069 7320 4e6f 6e65  lt value is None
-00000700: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00000710: 736f 7274 3a20 4f70 7469 6f6e 616c 5b55  sort: Optional[U
-00000720: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
-00000730: 7472 5d5d 5d0a 2020 2020 2020 2020 3a6b  tr]]].        :k
-00000740: 6579 776f 7264 2074 7970 653a 2046 696c  eyword type: Fil
-00000750: 7465 7220 7072 696e 6369 7061 6c73 2062  ter principals b
-00000760: 7920 7479 7065 2e20 4b6e 6f77 6e20 7661  y type. Known va
-00000770: 6c75 6573 2061 7265 3a20 2255 5345 5222  lues are: "USER"
-00000780: 2c20 2241 5050 4c49 4341 5449 4f4e 222c  , "APPLICATION",
-00000790: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-000007a0: 2020 2020 2020 2020 2020 2022 5359 5354             "SYST
-000007b0: 454d 222e 2044 6566 6175 6c74 2076 616c  EM". Default val
-000007c0: 7565 2069 7320 4e6f 6e65 2e0a 2020 2020  ue is None..    
-000007d0: 2020 2020 3a74 7970 6520 7479 7065 3a20      :type type: 
-000007e0: 4f70 7469 6f6e 616c 5b5f 6d6f 6465 6c73  Optional[_models
-000007f0: 2e50 7269 6e63 6970 616c 5479 7065 5d0a  .PrincipalType].
-00000800: 2020 2020 2020 2020 3a6b 6579 776f 7264          :keyword
-00000810: 2067 726f 7570 5f69 643a 2046 696c 7465   group_id: Filte
-00000820: 7220 7072 696e 6369 7061 6c73 2074 6861  r principals tha
-00000830: 7420 6578 6973 7473 2069 6e20 6f6e 6520  t exists in one 
-00000840: 6f66 2067 726f 7570 2069 6473 2e20 4465  of group ids. De
-00000850: 6661 756c 7420 7661 6c75 6520 6973 204e  fault value is N
-00000860: 6f6e 652e 0a20 2020 2020 2020 203a 7479  one..        :ty
-00000870: 7065 2067 726f 7570 5f69 643a 204f 7074  pe group_id: Opt
-00000880: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-00000890: 204c 6973 745b 7374 725d 5d5d 0a20 2020   List[str]]].   
-000008a0: 2020 2020 203a 7265 7475 726e 3a20 5072       :return: Pr
-000008b0: 696e 6369 7061 6c50 6167 650a 2020 2020  incipalPage.    
-000008c0: 2020 2020 3a72 7479 7065 3a20 7e6b 7566      :rtype: ~kuf
-000008d0: 6c6f 772e 7265 7374 2e6d 6f64 656c 732e  low.rest.models.
-000008e0: 5072 696e 6369 7061 6c50 6167 650a 2020  PrincipalPage.  
-000008f0: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
-00000900: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
-00000910: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
-00000920: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-00000930: 4e29 0572 1100 0000 7212 0000 0072 1300  N).r....r....r..
-00000940: 0000 7214 0000 0072 1500 0000 2905 da0a  ..r....r....)...
-00000950: 6973 696e 7374 616e 6365 da03 7374 7272  isinstance..strr
-00000960: 0b00 0000 da09 7072 696e 6369 7061 6cda  ......principal.
-00000970: 0f66 696e 645f 7072 696e 6369 7061 6c73  .find_principals
-00000980: 2907 720c 0000 0072 1100 0000 7212 0000  ).r....r....r...
-00000990: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-000009a0: 7216 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-000009b0: 0e00 0000 721b 0000 002d 0000 0073 1a00  ....r....-...s..
-000009c0: 0000 0021 1201 0602 1201 0602 0a01 0200  ...!............
-000009d0: 0200 0200 0200 02ff 0401 02ff 7a23 5072  ............z#Pr
-000009e0: 696e 6369 7061 6c4f 7065 7261 7469 6f6e  incipalOperation
-000009f0: 732e 6669 6e64 5f70 7269 6e63 6970 616c  s.find_principal
-00000a00: 7329 03da 0269 6472 1600 0000 7217 0000  s)...idr....r...
-00000a10: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-00000a20: 0000 0400 0000 4b00 0000 7318 0000 007c  ......K...s....|
-00000a30: 006a 006a 016a 0266 0064 017c 0169 017c  .j.j.j.f.d.|.i.|
-00000a40: 0297 028e 0153 0029 0261 2a01 0000 4765  .....S.).a*...Ge
-00000a50: 7420 6120 5072 696e 6369 7061 6c20 6279  t a Principal by
-00000a60: 2049 442e 0a0a 2020 2020 2020 2020 5265   ID...        Re
-00000a70: 7475 726e 7320 7468 6520 7265 7175 6573  turns the reques
-00000a80: 7465 6420 5072 696e 6369 7061 6c20 7768  ted Principal wh
-00000a90: 656e 2068 6173 2061 6363 6573 7320 746f  en has access to
-00000aa0: 2064 6f20 6974 2e0a 0a20 2020 2020 2020   do it...       
-00000ab0: 203a 7061 7261 6d20 6964 3a20 5468 6520   :param id: The 
-00000ac0: 7265 736f 7572 6365 2049 442e 2052 6571  resource ID. Req
-00000ad0: 7569 7265 642e 0a20 2020 2020 2020 203a  uired..        :
-00000ae0: 7479 7065 2069 643a 2073 7472 0a20 2020  type id: str.   
-00000af0: 2020 2020 203a 7265 7475 726e 3a20 5072       :return: Pr
-00000b00: 696e 6369 7061 6c0a 2020 2020 2020 2020  incipal.        
-00000b10: 3a72 7479 7065 3a20 7e6b 7566 6c6f 772e  :rtype: ~kuflow.
-00000b20: 7265 7374 2e6d 6f64 656c 732e 5072 696e  rest.models.Prin
-00000b30: 6369 7061 6c0a 2020 2020 2020 2020 3a72  cipal.        :r
-00000b40: 6169 7365 7320 7e61 7a75 7265 2e63 6f72  aises ~azure.cor
-00000b50: 652e 6578 6365 7074 696f 6e73 2e48 7474  e.exceptions.Htt
-00000b60: 7052 6573 706f 6e73 6545 7272 6f72 3a0a  pResponseError:.
-00000b70: 2020 2020 2020 2020 721c 0000 0029 0372          r....).r
-00000b80: 0b00 0000 721a 0000 00da 1272 6574 7269  ....r......retri
-00000b90: 6576 655f 7072 696e 6369 7061 6c29 0372  eve_principal).r
-00000ba0: 0c00 0000 721c 0000 0072 1600 0000 720d  ....r....r....r.
-00000bb0: 0000 0072 0d00 0000 720e 0000 0072 1d00  ...r....r....r..
-00000bc0: 0000 5800 0000 7302 0000 0000 0b7a 2650  ..X...s......z&P
-00000bd0: 7269 6e63 6970 616c 4f70 6572 6174 696f  rincipalOperatio
-00000be0: 6e73 2e72 6574 7269 6576 655f 7072 696e  ns.retrieve_prin
-00000bf0: 6369 7061 6c29 0572 1000 0000 7201 0000  cipal).r....r...
-00000c00: 004e 4e4e 2912 da08 5f5f 6e61 6d65 5f5f  .NNN)...__name__
-00000c10: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000c20: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000c30: 635f 5fda 194b 7546 6c6f 7752 6573 7443  c__..KuFlowRestC
-00000c40: 6c69 656e 7447 656e 6572 6174 6564 720f  lientGeneratedr.
-00000c50: 0000 00da 0369 6e74 7204 0000 0072 0500  .....intr....r..
-00000c60: 0000 7219 0000 0072 0300 0000 da07 5f6d  ..r....r......_m
-00000c70: 6f64 656c 73da 0d50 7269 6e63 6970 616c  odels..Principal
-00000c80: 5479 7065 7202 0000 00da 0d50 7269 6e63  Typer......Princ
-00000c90: 6970 616c 5061 6765 721b 0000 00da 0950  ipalPager......P
-00000ca0: 7269 6e63 6970 616c 721d 0000 0072 0d00  rincipalr....r..
-00000cb0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000cc0: 0072 0900 0000 2000 0000 7322 0000 0008  .r.... ...s"....
-00000cd0: 0104 090e 0500 0100 0100 0100 0100 fa02  ................
-00000ce0: 0202 0102 0112 0108 0112 0102 0104 f80c  ................
-00000cf0: 2b72 0900 0000 4e29 0bda 0674 7970 696e  +r....N)...typin
-00000d00: 6772 0200 0000 7203 0000 0072 0400 0000  gr....r....r....
-00000d10: 7205 0000 00da 0a5f 6765 6e65 7261 7465  r......_generate
-00000d20: 6472 0700 0000 7224 0000 0072 0800 0000  dr....r$...r....
-00000d30: 7222 0000 0072 0900 0000 720d 0000 0072  r"...r....r....r
-00000d40: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
-00000d50: 3c6d 6f64 756c 653e 1b00 0000 7304 0000  <module>....s...
-00000d60: 0018 0210 03                             .....
+00000280: 2901 4e29 01da 0e5f 6b75 666c 6f77 5f63  ).N)..._kuflow_c
+00000290: 6c69 656e 7429 02da 0473 656c 6672 0a00  lient)...selfr..
+000002a0: 0000 a900 720d 0000 00fa 532f 776f 726b  ....r.....S/work
+000002b0: 2f6b 7566 6c6f 772d 7364 6b2d 7079 7468  /kuflow-sdk-pyth
+000002c0: 6f6e 2f6b 7566 6c6f 772d 7265 7374 2f6b  on/kuflow-rest/k
+000002d0: 7566 6c6f 775f 7265 7374 2f6f 7065 7261  uflow_rest/opera
+000002e0: 7469 6f6e 732f 5f70 7269 6e63 6970 616c  tions/_principal
+000002f0: 5f6f 7065 7261 7469 6f6e 732e 7079 da08  _operations.py..
+00000300: 5f5f 696e 6974 5f5f 2a00 0000 7302 0000  __init__*...s...
+00000310: 0000 017a 1c50 7269 6e63 6970 616c 4f70  ...z.PrincipalOp
+00000320: 6572 6174 696f 6e73 2e5f 5f69 6e69 745f  erations.__init_
+00000330: 5fe9 1900 0000 7201 0000 004e 2907 da04  _.....r....N)...
+00000340: 7369 7a65 da04 7061 6765 da04 736f 7274  size..page..sort
+00000350: da04 7479 7065 da08 6772 6f75 705f 6964  ..type..group_id
+00000360: da06 6b77 6172 6773 da06 7265 7475 726e  ..kwargs..return
+00000370: 6306 0000 0000 0000 0000 0000 0007 0000  c...............
+00000380: 0008 0000 004b 0000 0073 5000 0000 7c03  .....K...sP...|.
+00000390: 6401 6b09 7218 7400 7c03 7401 8302 7218  d.k.r.t.|.t...r.
+000003a0: 7c03 6701 7d03 7c05 6401 6b09 7230 7400  |.g.}.|.d.k.r0t.
+000003b0: 7c05 7401 8302 7230 7c05 6701 7d05 7c00  |.t...r0|.g.}.|.
+000003c0: 6a02 6a03 6a04 6600 7c01 7c02 7c03 7c04  j.j.j.f.|.|.|.|.
+000003d0: 7c05 6402 9c05 7c06 9702 8e01 5300 2903  |.d...|.....S.).
+000003e0: 6136 0500 0046 696e 6420 616c 6c20 6163  a6...Find all ac
+000003f0: 6365 7373 6962 6c65 2050 7269 6e63 6970  cessible Princip
+00000400: 616c 732e 0a0a 2020 2020 2020 2020 4c69  als...        Li
+00000410: 7374 2061 6c6c 2074 6865 2050 7269 6e63  st all the Princ
+00000420: 6970 616c 7320 7468 6174 2068 6176 6520  ipals that have 
+00000430: 6265 656e 2063 7265 6174 6564 2061 6e64  been created and
+00000440: 2074 6865 2075 7365 6420 6372 6564 656e   the used creden
+00000450: 7469 616c 7320 6861 7320 6163 6365 7373  tials has access
+00000460: 2e0a 0a20 2020 2020 2020 2041 7661 696c  ...        Avail
+00000470: 6162 6c65 2073 6f72 7420 7175 6572 7920  able sort query 
+00000480: 7661 6c75 6573 3a20 6964 2c20 6e61 6d65  values: id, name
+00000490: 2e0a 0a20 2020 2020 2020 203a 6b65 7977  ...        :keyw
+000004a0: 6f72 6420 7369 7a65 3a20 5468 6520 6e75  ord size: The nu
+000004b0: 6d62 6572 206f 6620 7265 636f 7264 7320  mber of records 
+000004c0: 7265 7475 726e 6564 2077 6974 6869 6e20  returned within 
+000004d0: 6120 7369 6e67 6c65 2041 5049 2063 616c  a single API cal
+000004e0: 6c2e 2044 6566 6175 6c74 2076 616c 7565  l. Default value
+000004f0: 2069 7320 3235 2e0a 2020 2020 2020 2020   is 25..        
+00000500: 3a74 7970 6520 7369 7a65 3a20 696e 740a  :type size: int.
+00000510: 2020 2020 2020 2020 3a6b 6579 776f 7264          :keyword
+00000520: 2070 6167 653a 2054 6865 2070 6167 6520   page: The page 
+00000530: 6e75 6d62 6572 206f 6620 7468 6520 6375  number of the cu
+00000540: 7272 656e 7420 7061 6765 2069 6e20 7468  rrent page in th
+00000550: 6520 7265 7475 726e 6564 2072 6563 6f72  e returned recor
+00000560: 6473 2c20 3020 6973 2074 6865 2066 6972  ds, 0 is the fir
+00000570: 7374 2070 6167 652e 0a20 2020 2020 2020  st page..       
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 4465 6661 756c 7420 7661 6c75 6520 6973  Default value is
+000005a0: 2030 2e0a 2020 2020 2020 2020 3a74 7970   0..        :typ
+000005b0: 6520 7061 6765 3a20 696e 740a 2020 2020  e page: int.    
+000005c0: 2020 2020 3a6b 6579 776f 7264 2073 6f72      :keyword sor
+000005d0: 743a 2053 6f72 7469 6e67 2063 7269 7465  t: Sorting crite
+000005e0: 7269 6120 696e 2074 6865 2066 6f72 6d61  ria in the forma
+000005f0: 743a 2070 726f 7065 7274 797b 2c61 7363  t: property{,asc
+00000600: 7c64 6573 637d 2e20 4578 616d 706c 653a  |desc}. Example:
+00000610: 2063 7265 6174 6564 4174 2c64 6573 630a   createdAt,desc.
+00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000630: 2020 2020 2020 2044 6566 6175 6c74 2073         Default s
+00000640: 6f72 7420 6f72 6465 7220 6973 2061 7363  ort order is asc
+00000650: 656e 6469 6e67 2e20 4d75 6c74 6970 6c65  ending. Multiple
+00000660: 2073 6f72 7420 6372 6974 6572 6961 2061   sort criteria a
+00000670: 7265 2073 7570 706f 7274 6564 2e0a 2020  re supported..  
+00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000690: 2020 2020 2050 6c65 6173 6520 7265 6665       Please refe
+000006a0: 7220 746f 2074 6865 206d 6574 686f 6420  r to the method 
+000006b0: 6465 7363 7269 7074 696f 6e20 666f 7220  description for 
+000006c0: 7375 7070 6f72 7465 6420 7072 6f70 6572  supported proper
+000006d0: 7469 6573 2e20 4465 6661 756c 7420 7661  ties. Default va
+000006e0: 6c75 6520 6973 204e 6f6e 652e 0a20 2020  lue is None..   
+000006f0: 2020 2020 203a 7479 7065 2073 6f72 743a       :type sort:
+00000700: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+00000710: 7374 722c 204c 6973 745b 7374 725d 5d5d  str, List[str]]]
+00000720: 0a20 2020 2020 2020 203a 6b65 7977 6f72  .        :keywor
+00000730: 6420 7479 7065 3a20 4669 6c74 6572 2070  d type: Filter p
+00000740: 7269 6e63 6970 616c 7320 6279 2074 7970  rincipals by typ
+00000750: 652e 204b 6e6f 776e 2076 616c 7565 7320  e. Known values 
+00000760: 6172 653a 2022 5553 4552 222c 2022 4150  are: "USER", "AP
+00000770: 504c 4943 4154 494f 4e22 2c20 616e 640a  PLICATION", and.
+00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000790: 2020 2020 2020 2253 5953 5445 4d22 2e20        "SYSTEM". 
+000007a0: 4465 6661 756c 7420 7661 6c75 6520 6973  Default value is
+000007b0: 204e 6f6e 652e 0a20 2020 2020 2020 203a   None..        :
+000007c0: 7479 7065 2074 7970 653a 204f 7074 696f  type type: Optio
+000007d0: 6e61 6c5b 5f6d 6f64 656c 732e 5072 696e  nal[_models.Prin
+000007e0: 6369 7061 6c54 7970 655d 0a20 2020 2020  cipalType].     
+000007f0: 2020 203a 6b65 7977 6f72 6420 6772 6f75     :keyword grou
+00000800: 705f 6964 3a20 4669 6c74 6572 2070 7269  p_id: Filter pri
+00000810: 6e63 6970 616c 7320 7468 6174 2065 7869  ncipals that exi
+00000820: 7374 7320 696e 206f 6e65 206f 6620 6772  sts in one of gr
+00000830: 6f75 7020 6964 732e 2044 6566 6175 6c74  oup ids. Default
+00000840: 2076 616c 7565 2069 7320 4e6f 6e65 2e0a   value is None..
+00000850: 2020 2020 2020 2020 3a74 7970 6520 6772          :type gr
+00000860: 6f75 705f 6964 3a20 4f70 7469 6f6e 616c  oup_id: Optional
+00000870: 5b55 6e69 6f6e 5b73 7472 2c20 4c69 7374  [Union[str, List
+00000880: 5b73 7472 5d5d 5d0a 2020 2020 2020 2020  [str]]].        
+00000890: 3a72 6574 7572 6e3a 2050 7269 6e63 6970  :return: Princip
+000008a0: 616c 5061 6765 0a20 2020 2020 2020 203a  alPage.        :
+000008b0: 7274 7970 653a 207e 6b75 666c 6f77 2e72  rtype: ~kuflow.r
+000008c0: 6573 742e 6d6f 6465 6c73 2e50 7269 6e63  est.models.Princ
+000008d0: 6970 616c 5061 6765 0a20 2020 2020 2020  ipalPage.       
+000008e0: 203a 7261 6973 6573 207e 617a 7572 652e   :raises ~azure.
+000008f0: 636f 7265 2e65 7863 6570 7469 6f6e 732e  core.exceptions.
+00000900: 4874 7470 5265 7370 6f6e 7365 4572 726f  HttpResponseErro
+00000910: 723a 0a20 2020 2020 2020 204e 2905 7211  r:.        N).r.
+00000920: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00000930: 0000 7215 0000 0029 05da 0a69 7369 6e73  ..r....)...isins
+00000940: 7461 6e63 65da 0373 7472 720b 0000 00da  tance..strr.....
+00000950: 0970 7269 6e63 6970 616c da0f 6669 6e64  .principal..find
+00000960: 5f70 7269 6e63 6970 616c 7329 0772 0c00  _principals).r..
+00000970: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000980: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000990: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+000009a0: 1b00 0000 2d00 0000 731a 0000 0000 2112  ....-...s.....!.
+000009b0: 0106 0212 0106 020a 0102 0002 0002 0002  ................
+000009c0: 0002 ff04 0102 ff7a 2350 7269 6e63 6970  .......z#Princip
+000009d0: 616c 4f70 6572 6174 696f 6e73 2e66 696e  alOperations.fin
+000009e0: 645f 7072 696e 6369 7061 6c73 2903 da02  d_principals)...
+000009f0: 6964 7216 0000 0072 1700 0000 6302 0000  idr....r....c...
+00000a00: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00000a10: 004b 0000 0073 1800 0000 7c00 6a00 6a01  .K...s....|.j.j.
+00000a20: 6a02 6600 6401 7c01 6901 7c02 9702 8e01  j.f.d.|.i.|.....
+00000a30: 5300 2902 612a 0100 0047 6574 2061 2050  S.).a*...Get a P
+00000a40: 7269 6e63 6970 616c 2062 7920 4944 2e0a  rincipal by ID..
+00000a50: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00000a60: 2074 6865 2072 6571 7565 7374 6564 2050   the requested P
+00000a70: 7269 6e63 6970 616c 2077 6865 6e20 6861  rincipal when ha
+00000a80: 7320 6163 6365 7373 2074 6f20 646f 2069  s access to do i
+00000a90: 742e 0a0a 2020 2020 2020 2020 3a70 6172  t...        :par
+00000aa0: 616d 2069 643a 2054 6865 2072 6573 6f75  am id: The resou
+00000ab0: 7263 6520 4944 2e20 5265 7175 6972 6564  rce ID. Required
+00000ac0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00000ad0: 6964 3a20 7374 720a 2020 2020 2020 2020  id: str.        
+00000ae0: 3a72 6574 7572 6e3a 2050 7269 6e63 6970  :return: Princip
+00000af0: 616c 0a20 2020 2020 2020 203a 7274 7970  al.        :rtyp
+00000b00: 653a 207e 6b75 666c 6f77 2e72 6573 742e  e: ~kuflow.rest.
+00000b10: 6d6f 6465 6c73 2e50 7269 6e63 6970 616c  models.Principal
+00000b20: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+00000b30: 207e 617a 7572 652e 636f 7265 2e65 7863   ~azure.core.exc
+00000b40: 6570 7469 6f6e 732e 4874 7470 5265 7370  eptions.HttpResp
+00000b50: 6f6e 7365 4572 726f 723a 0a20 2020 2020  onseError:.     
+00000b60: 2020 2072 1c00 0000 2903 720b 0000 0072     r....).r....r
+00000b70: 1a00 0000 da12 7265 7472 6965 7665 5f70  ......retrieve_p
+00000b80: 7269 6e63 6970 616c 2903 720c 0000 0072  rincipal).r....r
+00000b90: 1c00 0000 7216 0000 0072 0d00 0000 720d  ....r....r....r.
+00000ba0: 0000 0072 0e00 0000 721d 0000 0058 0000  ...r....r....X..
+00000bb0: 0073 0200 0000 000b 7a26 5072 696e 6369  .s......z&Princi
+00000bc0: 7061 6c4f 7065 7261 7469 6f6e 732e 7265  palOperations.re
+00000bd0: 7472 6965 7665 5f70 7269 6e63 6970 616c  trieve_principal
+00000be0: 2905 7210 0000 0072 0100 0000 4e4e 4e29  ).r....r....NNN)
+00000bf0: 12da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000c00: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000c10: 616d 655f 5fda 075f 5f64 6f63 5f5f da19  ame__..__doc__..
+00000c20: 4b75 466c 6f77 5265 7374 436c 6965 6e74  KuFlowRestClient
+00000c30: 4765 6e65 7261 7465 6472 0f00 0000 da03  Generatedr......
+00000c40: 696e 7472 0400 0000 7205 0000 0072 1900  intr....r....r..
+00000c50: 0000 7203 0000 00da 075f 6d6f 6465 6c73  ..r......_models
+00000c60: da0d 5072 696e 6369 7061 6c54 7970 6572  ..PrincipalTyper
+00000c70: 0200 0000 da0d 5072 696e 6369 7061 6c50  ......PrincipalP
+00000c80: 6167 6572 1b00 0000 da09 5072 696e 6369  ager......Princi
+00000c90: 7061 6c72 1d00 0000 720d 0000 0072 0d00  palr....r....r..
+00000ca0: 0000 720d 0000 0072 0e00 0000 7209 0000  ..r....r....r...
+00000cb0: 0020 0000 0073 2200 0000 0801 0409 0e05  . ...s".........
+00000cc0: 0001 0001 0001 0001 00fa 0202 0201 0201  ................
+00000cd0: 1201 0801 1201 0201 04f8 0c2b 7209 0000  ...........+r...
+00000ce0: 004e 290b da06 7479 7069 6e67 7202 0000  .N)...typingr...
+00000cf0: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
+00000d00: da0a 5f67 656e 6572 6174 6564 7207 0000  .._generatedr...
+00000d10: 0072 2400 0000 7208 0000 0072 2200 0000  .r$...r....r"...
+00000d20: 7209 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000d30: 0d00 0000 720e 0000 00da 083c 6d6f 6475  ....r......<modu
+00000d40: 6c65 3e1b 0000 0073 0400 0000 1802 1003  le>....s........
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 9540 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 4425 0000  U........<.dD%..
+00000000: 550d 0d0a 0000 0000 9c24 8c64 3a25 0000  U........$.d:%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6404 6c08 6d09 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a0b 6407 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 04da 0341 6e79 da04  )......)...Any..
@@ -43,525 +43,524 @@
 000002a0: 466c 6f77 5265 7374 436c 6965 6e74 6027  FlowRestClient`'
 000002b0: 730a 2020 2020 2020 2020 3a61 7474 723a  s.        :attr:
 000002c0: 6070 726f 6365 7373 6020 6174 7472 6962  `process` attrib
 000002d0: 7574 652e 0a20 2020 2029 01da 0d6b 7566  ute..    )...kuf
 000002e0: 6c6f 775f 636c 6965 6e74 6302 0000 0000  low_clientc.....
 000002f0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
 00000300: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
-00000310: 5300 2901 4e29 01da 215f 5072 6f63 6573  S.).N)..!_Proces
-00000320: 734f 7065 7261 7469 6f6e 735f 5f6b 7566  sOperations__kuf
-00000330: 6c6f 775f 636c 6965 6e74 2902 da04 7365  low_client)...se
-00000340: 6c66 720a 0000 00a9 0072 0d00 0000 fa51  lfr......r.....Q
-00000350: 2f77 6f72 6b2f 6b75 666c 6f77 2d73 646b  /work/kuflow-sdk
-00000360: 2d70 7974 686f 6e2f 6b75 666c 6f77 2d72  -python/kuflow-r
-00000370: 6573 742f 6b75 666c 6f77 5f72 6573 742f  est/kuflow_rest/
-00000380: 6f70 6572 6174 696f 6e73 2f5f 7072 6f63  operations/_proc
-00000390: 6573 735f 6f70 6572 6174 696f 6e73 2e70  ess_operations.p
-000003a0: 79da 085f 5f69 6e69 745f 5f2b 0000 0073  y..__init__+...s
-000003b0: 0200 0000 0001 7a1a 5072 6f63 6573 734f  ......z.ProcessO
-000003c0: 7065 7261 7469 6f6e 732e 5f5f 696e 6974  perations.__init
-000003d0: 5f5f e919 0000 0072 0100 0000 4e29 05da  __.....r....N)..
-000003e0: 0473 697a 65da 0470 6167 65da 0473 6f72  .size..page..sor
-000003f0: 74da 066b 7761 7267 73da 0672 6574 7572  t..kwargs..retur
-00000400: 6e63 0400 0000 0000 0000 0000 0000 0500  nc..............
-00000410: 0000 0600 0000 4b00 0000 7334 0000 007c  ......K...s4...|
-00000420: 0364 016b 0972 1874 007c 0374 0183 0272  .d.k.r.t.|.t...r
-00000430: 187c 0367 017d 037c 006a 026a 036a 0466  .|.g.}.|.j.j.j.f
-00000440: 007c 017c 027c 0364 029c 037c 0497 028e  .|.|.|.d...|....
-00000450: 0153 0029 0361 db03 0000 4669 6e64 2061  .S.).a....Find a
-00000460: 6c6c 2061 6363 6573 7369 626c 6520 5072  ll accessible Pr
-00000470: 6f63 6573 7365 732e 0a0a 2020 2020 2020  ocesses...      
-00000480: 2020 4c69 7374 2061 6c6c 2074 6865 2050    List all the P
-00000490: 726f 6365 7373 6573 2074 6861 7420 6861  rocesses that ha
-000004a0: 7665 2062 6565 6e20 6372 6561 7465 6420  ve been created 
-000004b0: 616e 6420 7468 6520 6372 6564 656e 7469  and the credenti
-000004c0: 616c 7320 6861 7320 6163 6365 7373 2e0a  als has access..
-000004d0: 0a20 2020 2020 2020 2041 7661 696c 6162  .        Availab
-000004e0: 6c65 2073 6f72 7420 7175 6572 7920 7661  le sort query va
-000004f0: 6c75 6573 3a20 6964 2c20 6372 6561 7465  lues: id, create
-00000500: 6441 742c 206c 6173 744d 6f64 6966 6965  dAt, lastModifie
-00000510: 6441 742e 0a0a 2020 2020 2020 2020 3a6b  dAt...        :k
-00000520: 6579 776f 7264 2073 697a 653a 2054 6865  eyword size: The
-00000530: 206e 756d 6265 7220 6f66 2072 6563 6f72   number of recor
-00000540: 6473 2072 6574 7572 6e65 6420 7769 7468  ds returned with
-00000550: 696e 2061 2073 696e 676c 6520 4150 4920  in a single API 
-00000560: 6361 6c6c 2e20 4465 6661 756c 7420 7661  call. Default va
-00000570: 6c75 6520 6973 2032 352e 0a20 2020 2020  lue is 25..     
-00000580: 2020 203a 7479 7065 2073 697a 653a 2069     :type size: i
-00000590: 6e74 0a20 2020 2020 2020 203a 6b65 7977  nt.        :keyw
-000005a0: 6f72 6420 7061 6765 3a20 5468 6520 7061  ord page: The pa
-000005b0: 6765 206e 756d 6265 7220 6f66 2074 6865  ge number of the
-000005c0: 2063 7572 7265 6e74 2070 6167 6520 696e   current page in
-000005d0: 2074 6865 2072 6574 7572 6e65 6420 7265   the returned re
-000005e0: 636f 7264 732c 2030 2069 7320 7468 6520  cords, 0 is the 
-000005f0: 6669 7273 7420 7061 6765 2e0a 2020 2020  first page..    
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 2044 6566 6175 6c74 2076 616c 7565     Default value
-00000620: 2069 7320 302e 0a20 2020 2020 2020 203a   is 0..        :
-00000630: 7479 7065 2070 6167 653a 2069 6e74 0a20  type page: int. 
-00000640: 2020 2020 2020 203a 6b65 7977 6f72 6420         :keyword 
-00000650: 736f 7274 3a20 536f 7274 696e 6720 6372  sort: Sorting cr
-00000660: 6974 6572 6961 2069 6e20 7468 6520 666f  iteria in the fo
-00000670: 726d 6174 3a20 7072 6f70 6572 7479 7b2c  rmat: property{,
-00000680: 6173 637c 6465 7363 7d2e 2045 7861 6d70  asc|desc}. Examp
-00000690: 6c65 3a20 6372 6561 7465 6441 742c 6465  le: createdAt,de
-000006a0: 7363 0a0a 2020 2020 2020 2020 2020 2020  sc..            
-000006b0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-000006c0: 6c74 2073 6f72 7420 6f72 6465 7220 6973  lt sort order is
-000006d0: 2061 7363 656e 6469 6e67 2e20 4d75 6c74   ascending. Mult
-000006e0: 6970 6c65 2073 6f72 7420 6372 6974 6572  iple sort criter
-000006f0: 6961 2061 7265 2073 7570 706f 7274 6564  ia are supported
-00000700: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00000710: 2020 2020 2020 2020 2020 506c 6561 7365            Please
-00000720: 2072 6566 6572 2074 6f20 7468 6520 6d65   refer to the me
-00000730: 7468 6f64 2064 6573 6372 6970 7469 6f6e  thod description
-00000740: 2066 6f72 2073 7570 706f 7274 6564 2070   for supported p
-00000750: 726f 7065 7274 6965 732e 2044 6566 6175  roperties. Defau
-00000760: 6c74 2076 616c 7565 2069 7320 4e6f 6e65  lt value is None
-00000770: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00000780: 736f 7274 3a20 4f70 7469 6f6e 616c 5b55  sort: Optional[U
-00000790: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
-000007a0: 7472 5d5d 5d0a 2020 2020 2020 2020 3a72  tr]]].        :r
-000007b0: 6574 7572 6e3a 2050 726f 6365 7373 5061  eturn: ProcessPa
-000007c0: 6765 0a20 2020 2020 2020 203a 7274 7970  ge.        :rtyp
-000007d0: 653a 207e 6b75 666c 6f77 2e72 6573 742e  e: ~kuflow.rest.
-000007e0: 6d6f 6465 6c73 2e50 726f 6365 7373 5061  models.ProcessPa
-000007f0: 6765 0a20 2020 2020 2020 203a 7261 6973  ge.        :rais
-00000800: 6573 207e 617a 7572 652e 636f 7265 2e65  es ~azure.core.e
-00000810: 7863 6570 7469 6f6e 732e 4874 7470 5265  xceptions.HttpRe
-00000820: 7370 6f6e 7365 4572 726f 723a 0a20 2020  sponseError:.   
-00000830: 2020 2020 204e 2903 7211 0000 0072 1200       N).r....r..
-00000840: 0000 7213 0000 0029 05da 0a69 7369 6e73  ..r....)...isins
-00000850: 7461 6e63 65da 0373 7472 720b 0000 00da  tance..strr.....
-00000860: 0770 726f 6365 7373 da0e 6669 6e64 5f70  .process..find_p
-00000870: 726f 6365 7373 6573 2905 720c 0000 0072  rocesses).r....r
-00000880: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00000890: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-000008a0: 0000 7219 0000 002e 0000 0073 0600 0000  ..r........s....
-000008b0: 0018 1201 0602 7a20 5072 6f63 6573 734f  ......z ProcessO
-000008c0: 7065 7261 7469 6f6e 732e 6669 6e64 5f70  perations.find_p
-000008d0: 726f 6365 7373 6573 2903 7218 0000 0072  rocesses).r....r
-000008e0: 1400 0000 7215 0000 0063 0200 0000 0000  ....r....c......
-000008f0: 0000 0000 0000 0300 0000 0400 0000 4b00  ..............K.
-00000900: 0000 7318 0000 007c 006a 006a 016a 0266  ..s....|.j.j.j.f
-00000910: 0064 017c 0169 017c 0297 028e 0153 0029  .d.|.i.|.....S.)
-00000920: 0261 0104 0000 4372 6561 7465 2061 206e  .a....Create a n
-00000930: 6577 2070 726f 6365 7373 2e0a 0a20 2020  ew process...   
-00000940: 2020 2020 2043 7265 6174 6573 2061 2070       Creates a p
-00000950: 726f 6365 7373 2e20 5468 6973 206f 7074  rocess. This opt
-00000960: 696f 6e20 6861 7320 6469 7265 6374 2063  ion has direct c
-00000970: 6f72 7265 7370 6f6e 6465 6e63 6520 746f  orrespondence to
-00000980: 2074 6865 2061 6374 696f 6e20 6f66 2073   the action of s
-00000990: 7461 7274 696e 6720 6120 7072 6f63 6573  tarting a proces
-000009a0: 7320 696e 0a20 2020 2020 2020 2074 6865  s in.        the
-000009b0: 204b 7566 6c6f 7720 4755 492e 0a0a 2020   Kuflow GUI...  
-000009c0: 2020 2020 2020 5768 656e 2061 2070 726f        When a pro
-000009d0: 6365 7373 2069 7320 6372 6561 7465 642c  cess is created,
-000009e0: 2074 6865 2063 7572 7265 6e74 2075 7365   the current use
-000009f0: 7220 6973 2061 7373 6967 6e65 6420 6173  r is assigned as
-00000a00: 2074 6865 2070 726f 6365 7373 2069 6e69   the process ini
-00000a10: 7469 6174 6f72 2c20 6966 2079 6f75 2077  tiator, if you w
-00000a20: 616e 740a 2020 2020 2020 2020 746f 2063  ant.        to c
-00000a30: 6861 6e67 6520 6974 2c20 796f 7520 6361  hange it, you ca
-00000a40: 6e20 7061 7373 2061 2076 616c 6964 2069  n pass a valid i
-00000a50: 6e69 7469 6174 6f72 2075 7369 6e67 2074  nitiator using t
-00000a60: 6865 2066 6f6c 6c6f 7769 6e67 206f 7074  he following opt
-00000a70: 696f 6e73 3a0a 0a0a 2020 2020 2020 2020  ions:...        
-00000a80: 2a20 4966 2079 6f75 206b 6e6f 7720 7468  * If you know th
-00000a90: 6520 6060 7072 696e 6369 7061 6c20 4944  e ``principal ID
-00000aa0: 6060 2079 6f75 2063 616e 2061 7373 6967  `` you can assig
-00000ab0: 6e20 6974 2074 6f20 6060 696e 6974 6961  n it to ``initia
-00000ac0: 746f 722e 6964 6060 0a20 2020 2020 2020  tor.id``.       
-00000ad0: 202a 2049 6620 796f 7520 6b6e 6f77 2074   * If you know t
-00000ae0: 6865 2060 6075 7365 7220 4944 6060 2079  he ``user ID`` y
-00000af0: 6f75 2063 616e 2061 7373 6967 6e20 6974  ou can assign it
-00000b00: 2074 6f20 6060 696e 6974 6961 746f 722e   to ``initiator.
-00000b10: 7573 6572 2e69 6460 600a 2020 2020 2020  user.id``.      
-00000b20: 2020 2a20 4966 2079 6f75 206b 6e6f 7720    * If you know 
-00000b30: 7468 6520 6060 7573 6572 2065 6d61 696c  the ``user email
-00000b40: 6060 2079 6f75 2063 616e 2061 7373 6967  `` you can assig
-00000b50: 6e20 6974 2074 6f20 6060 696e 6974 6961  n it to ``initia
-00000b60: 746f 722e 7573 6572 2e65 6d61 696c 6060  tor.user.email``
-00000b70: 0a20 2020 2020 2020 202a 2049 6620 796f  .        * If yo
-00000b80: 7520 6b6e 6f77 2074 6865 2060 6061 7070  u know the ``app
-00000b90: 6c69 6361 7469 6f6e 2049 4460 6020 796f  lication ID`` yo
-00000ba0: 7520 6361 6e20 6173 7369 676e 2069 7420  u can assign it 
-00000bb0: 746f 2060 6069 6e69 7469 6174 6f72 2e61  to ``initiator.a
-00000bc0: 7070 6c69 6361 7469 6f6e 2e69 6460 600a  pplication.id``.
-00000bd0: 0a20 2020 2020 2020 2049 6620 796f 7520  .        If you 
-00000be0: 7761 6e74 2074 6865 206d 6574 686f 6420  want the method 
-00000bf0: 746f 2062 6520 6964 656d 706f 7465 6e74  to be idempotent
-00000c00: 2c20 706c 6561 7365 2073 7065 6369 6679  , please specify
-00000c10: 2074 6865 2060 6069 6460 6020 6669 656c   the ``id`` fiel
-00000c20: 6420 696e 2074 6865 2072 6571 7565 7374  d in the request
-00000c30: 2062 6f64 792e 0a0a 2020 2020 2020 2020   body...        
-00000c40: 3a70 6172 616d 2070 726f 6365 7373 3a20  :param process: 
-00000c50: 5072 6f63 6573 7320 746f 2063 7265 6174  Process to creat
-00000c60: 652e 2052 6571 7569 7265 642e 0a20 2020  e. Required..   
-00000c70: 2020 2020 203a 7479 7065 2070 726f 6365       :type proce
-00000c80: 7373 3a20 7e6b 7566 6c6f 772e 7265 7374  ss: ~kuflow.rest
-00000c90: 2e6d 6f64 656c 732e 5072 6f63 6573 730a  .models.Process.
-00000ca0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000cb0: 2050 726f 6365 7373 0a20 2020 2020 2020   Process.       
-00000cc0: 203a 7274 7970 653a 207e 6b75 666c 6f77   :rtype: ~kuflow
-00000cd0: 2e72 6573 742e 6d6f 6465 6c73 2e50 726f  .rest.models.Pro
-00000ce0: 6365 7373 0a20 2020 2020 2020 203a 7261  cess.        :ra
-00000cf0: 6973 6573 207e 617a 7572 652e 636f 7265  ises ~azure.core
-00000d00: 2e65 7863 6570 7469 6f6e 732e 4874 7470  .exceptions.Http
-00000d10: 5265 7370 6f6e 7365 4572 726f 723a 0a20  ResponseError:. 
-00000d20: 2020 2020 2020 2072 1800 0000 2903 720b         r....).r.
-00000d30: 0000 0072 1800 0000 da0e 6372 6561 7465  ...r......create
-00000d40: 5f70 726f 6365 7373 2903 720c 0000 0072  _process).r....r
-00000d50: 1800 0000 7214 0000 0072 0d00 0000 720d  ....r....r....r.
-00000d60: 0000 0072 0e00 0000 721a 0000 004b 0000  ...r....r....K..
-00000d70: 0073 0200 0000 0017 7a20 5072 6f63 6573  .s......z Proces
-00000d80: 734f 7065 7261 7469 6f6e 732e 6372 6561  sOperations.crea
-00000d90: 7465 5f70 726f 6365 7373 2903 da02 6964  te_process)...id
-00000da0: 7214 0000 0072 1500 0000 6302 0000 0000  r....r....c.....
-00000db0: 0000 0000 0000 0003 0000 0004 0000 004b  ...............K
-00000dc0: 0000 0073 1800 0000 7c00 6a00 6a01 6a02  ...s....|.j.j.j.
-00000dd0: 6600 6401 7c01 6901 7c02 9702 8e01 5300  f.d.|.i.|.....S.
-00000de0: 2902 6122 0100 0047 6574 2061 2050 726f  ).a"...Get a Pro
-00000df0: 6365 7373 2062 7920 4944 2e0a 0a20 2020  cess by ID...   
-00000e00: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
-00000e10: 2072 6571 7565 7374 6564 2050 726f 6365   requested Proce
-00000e20: 7373 2077 6865 6e20 6861 7320 6163 6365  ss when has acce
-00000e30: 7373 2074 6f20 646f 2069 742e 0a0a 2020  ss to do it...  
-00000e40: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
-00000e50: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
-00000e60: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
-00000e70: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
-00000e80: 720a 2020 2020 2020 2020 3a72 6574 7572  r.        :retur
-00000e90: 6e3a 2050 726f 6365 7373 0a20 2020 2020  n: Process.     
-00000ea0: 2020 203a 7274 7970 653a 207e 6b75 666c     :rtype: ~kufl
-00000eb0: 6f77 2e72 6573 742e 6d6f 6465 6c73 2e50  ow.rest.models.P
-00000ec0: 726f 6365 7373 0a20 2020 2020 2020 203a  rocess.        :
-00000ed0: 7261 6973 6573 207e 617a 7572 652e 636f  raises ~azure.co
-00000ee0: 7265 2e65 7863 6570 7469 6f6e 732e 4874  re.exceptions.Ht
-00000ef0: 7470 5265 7370 6f6e 7365 4572 726f 723a  tpResponseError:
-00000f00: 0a20 2020 2020 2020 2072 1b00 0000 2903  .        r....).
-00000f10: 720b 0000 0072 1800 0000 da10 7265 7472  r....r......retr
-00000f20: 6965 7665 5f70 726f 6365 7373 a903 720c  ieve_process..r.
-00000f30: 0000 0072 1b00 0000 7214 0000 0072 0d00  ...r....r....r..
-00000f40: 0000 720d 0000 0072 0e00 0000 721c 0000  ..r....r....r...
-00000f50: 0064 0000 0073 0200 0000 000b 7a22 5072  .d...s......z"Pr
-00000f60: 6f63 6573 734f 7065 7261 7469 6f6e 732e  ocessOperations.
-00000f70: 7265 7472 6965 7665 5f70 726f 6365 7373  retrieve_process
-00000f80: 2904 721b 0000 00da 0763 6f6d 6d61 6e64  ).r......command
-00000f90: 7214 0000 0072 1500 0000 6303 0000 0000  r....r....c.....
-00000fa0: 0000 0000 0000 0004 0000 0005 0000 004b  ...............K
-00000fb0: 0000 0073 1a00 0000 7c00 6a00 6a01 6a02  ...s....|.j.j.j.
-00000fc0: 6600 7c01 7c02 6401 9c02 7c03 9702 8e01  f.|.|.d...|.....
-00000fd0: 5300 2902 6153 0200 0043 6861 6e67 6520  S.).aS...Change 
-00000fe0: 7072 6f63 6573 7320 696e 6974 6961 746f  process initiato
-00000ff0: 722e 0a0a 2020 2020 2020 2020 4368 616e  r...        Chan
-00001000: 6765 2074 6865 2063 7572 7265 6e74 2069  ge the current i
-00001010: 6e69 7469 6174 6f72 206f 6620 6120 7072  nitiator of a pr
-00001020: 6f63 6573 732e 0a0a 2020 2020 2020 2020  ocess...        
-00001030: 416c 6c6f 7773 2079 6f75 2074 6f20 6368  Allows you to ch
-00001040: 6f6f 7365 2061 2075 7365 7220 2862 7920  oose a user (by 
-00001050: 656d 6169 6c20 6f72 2070 7269 6e63 6970  email or princip
-00001060: 616c 2069 6465 6e74 6966 6965 7229 206f  al identifier) o
-00001070: 7220 616e 2061 7070 6c69 6361 7469 6f6e  r an application
-00001080: 2028 7072 696e 6369 7061 6c0a 2020 2020   (principal.    
-00001090: 2020 2020 6964 656e 7469 6669 6572 292e      identifier).
-000010a0: 0a20 2020 2020 2020 204f 6e6c 7920 6f6e  .        Only on
-000010b0: 6520 6f70 7469 6f6e 2077 696c 6c20 6265  e option will be
-000010c0: 206e 6563 6573 7361 7279 2e0a 0a20 2020   necessary...   
-000010d0: 2020 2020 203a 7061 7261 6d20 6964 3a20       :param id: 
-000010e0: 5468 6520 7265 736f 7572 6365 2049 442e  The resource ID.
-000010f0: 2052 6571 7569 7265 642e 0a20 2020 2020   Required..     
-00001100: 2020 203a 7479 7065 2069 643a 2073 7472     :type id: str
-00001110: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001120: 636f 6d6d 616e 643a 2043 6f6d 6d61 6e64  command: Command
-00001130: 2074 6f20 6368 616e 6765 2074 6865 2070   to change the p
-00001140: 726f 6365 7373 2069 6e69 7469 6174 6f72  rocess initiator
-00001150: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
-00001160: 2020 2020 3a74 7970 6520 636f 6d6d 616e      :type comman
-00001170: 643a 207e 6b75 666c 6f77 2e72 6573 742e  d: ~kuflow.rest.
-00001180: 6d6f 6465 6c73 2e50 726f 6365 7373 4368  models.ProcessCh
-00001190: 616e 6765 496e 6974 6961 746f 7243 6f6d  angeInitiatorCom
-000011a0: 6d61 6e64 0a20 2020 2020 2020 203a 7265  mand.        :re
-000011b0: 7475 726e 3a20 5072 6f63 6573 730a 2020  turn: Process.  
-000011c0: 2020 2020 2020 3a72 7479 7065 3a20 7e6b        :rtype: ~k
-000011d0: 7566 6c6f 772e 7265 7374 2e6d 6f64 656c  uflow.rest.model
-000011e0: 732e 5072 6f63 6573 730a 2020 2020 2020  s.Process.      
-000011f0: 2020 3a72 6169 7365 7320 7e61 7a75 7265    :raises ~azure
-00001200: 2e63 6f72 652e 6578 6365 7074 696f 6e73  .core.exceptions
-00001210: 2e48 7474 7052 6573 706f 6e73 6545 7272  .HttpResponseErr
-00001220: 6f72 3a0a 2020 2020 2020 2020 a902 721b  or:.        ..r.
-00001230: 0000 0072 1e00 0000 2903 720b 0000 0072  ...r....).r....r
-00001240: 1800 0000 da20 6163 7469 6f6e 735f 7072  ..... actions_pr
-00001250: 6f63 6573 735f 6368 616e 6765 5f69 6e69  ocess_change_ini
-00001260: 7469 6174 6f72 a904 720c 0000 0072 1b00  tiator..r....r..
-00001270: 0000 721e 0000 0072 1400 0000 720d 0000  ..r....r....r...
-00001280: 0072 0d00 0000 720e 0000 0072 2000 0000  .r....r....r ...
-00001290: 7100 0000 7302 0000 0000 137a 3250 726f  q...s......z2Pro
-000012a0: 6365 7373 4f70 6572 6174 696f 6e73 2e61  cessOperations.a
-000012b0: 6374 696f 6e73 5f70 726f 6365 7373 5f63  ctions_process_c
-000012c0: 6861 6e67 655f 696e 6974 6961 746f 7263  hange_initiatorc
-000012d0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-000012e0: 0500 0000 4b00 0000 731a 0000 007c 006a  ....K...s....|.j
-000012f0: 006a 016a 0266 007c 017c 0264 019c 027c  .j.j.f.|.|.d...|
-00001300: 0397 028e 0153 0029 0261 c302 0000 5361  .....S.).a....Sa
-00001310: 7665 2061 2070 726f 6365 7373 2065 6c65  ve a process ele
-00001320: 6d65 6e74 2c20 616b 613a 206d 6574 6164  ment, aka: metad
-00001330: 6174 612e 0a0a 2020 2020 2020 2020 416c  ata...        Al
-00001340: 6c6f 7720 746f 2073 6176 6520 616e 2065  low to save an e
-00001350: 6c65 6d65 6e74 2e0a 0a20 2020 2020 2020  lement...       
-00001360: 2049 6620 7661 6c75 6573 2061 6c72 6561   If values alrea
-00001370: 6479 2065 7869 7374 2066 6f72 2074 6865  dy exist for the
-00001380: 2070 726f 7669 6465 6420 656c 656d 656e   provided elemen
-00001390: 7420 636f 6465 2c20 6974 2072 6570 6c61  t code, it repla
-000013a0: 6365 7320 7468 656d 2077 6974 6820 7468  ces them with th
-000013b0: 6520 6e65 7720 6f6e 6573 2c0a 2020 2020  e new ones,.    
-000013c0: 2020 2020 6f74 6865 7277 6973 6520 6974      otherwise it
-000013d0: 2063 7265 6174 6573 2074 6865 6d2e 2054   creates them. T
-000013e0: 6865 2076 616c 7565 7320 6f66 2074 6865  he values of the
-000013f0: 2070 7265 7669 6f75 7320 656c 656d 656e   previous elemen
-00001400: 7473 2074 6861 7420 6e6f 206c 6f6e 6765  ts that no longe
-00001410: 7220 6578 6973 7420 7769 6c6c 2062 650a  r exist will be.
-00001420: 2020 2020 2020 2020 6465 6c65 7465 642e          deleted.
-00001430: 0a0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
-00001440: 2070 726f 6365 7373 2069 7320 616c 7265   process is alre
-00001450: 6164 7920 6669 6e69 7368 6564 2074 6865  ady finished the
-00001460: 2069 6e76 6f63 6174 696f 6e73 2066 6169   invocations fai
-00001470: 6c73 2077 6974 6820 616e 2065 7272 6f72  ls with an error
-00001480: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00001490: 6d20 6964 3a20 5468 6520 7265 736f 7572  m id: The resour
-000014a0: 6365 2049 442e 2052 6571 7569 7265 642e  ce ID. Required.
-000014b0: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
-000014c0: 643a 2073 7472 0a20 2020 2020 2020 203a  d: str.        :
-000014d0: 7061 7261 6d20 636f 6d6d 616e 643a 2043  param command: C
-000014e0: 6f6d 6d61 6e64 2074 6f20 7361 7665 2061  ommand to save a
-000014f0: 6e20 656c 656d 656e 742e 2052 6571 7569  n element. Requi
-00001500: 7265 642e 0a20 2020 2020 2020 203a 7479  red..        :ty
-00001510: 7065 2063 6f6d 6d61 6e64 3a20 7e6b 7566  pe command: ~kuf
-00001520: 6c6f 772e 7265 7374 2e6d 6f64 656c 732e  low.rest.models.
-00001530: 5072 6f63 6573 7353 6176 6545 6c65 6d65  ProcessSaveEleme
-00001540: 6e74 436f 6d6d 616e 640a 2020 2020 2020  ntCommand.      
-00001550: 2020 3a72 6574 7572 6e3a 2050 726f 6365    :return: Proce
-00001560: 7373 0a20 2020 2020 2020 203a 7274 7970  ss.        :rtyp
-00001570: 653a 207e 6b75 666c 6f77 2e72 6573 742e  e: ~kuflow.rest.
-00001580: 6d6f 6465 6c73 2e50 726f 6365 7373 0a20  models.Process. 
-00001590: 2020 2020 2020 203a 7261 6973 6573 207e         :raises ~
-000015a0: 617a 7572 652e 636f 7265 2e65 7863 6570  azure.core.excep
-000015b0: 7469 6f6e 732e 4874 7470 5265 7370 6f6e  tions.HttpRespon
-000015c0: 7365 4572 726f 723a 0a20 2020 2020 2020  seError:.       
-000015d0: 2072 1f00 0000 2903 720b 0000 0072 1800   r....).r....r..
-000015e0: 0000 da1c 6163 7469 6f6e 735f 7072 6f63  ....actions_proc
-000015f0: 6573 735f 7361 7665 5f65 6c65 6d65 6e74  ess_save_element
-00001600: 7221 0000 0072 0d00 0000 720d 0000 0072  r!...r....r....r
-00001610: 0e00 0000 7222 0000 0086 0000 0073 0200  ....r".......s..
-00001620: 0000 0015 7a2e 5072 6f63 6573 734f 7065  ....z.ProcessOpe
-00001630: 7261 7469 6f6e 732e 6163 7469 6f6e 735f  rations.actions_
-00001640: 7072 6f63 6573 735f 7361 7665 5f65 6c65  process_save_ele
-00001650: 6d65 6e74 6303 0000 0000 0000 0000 0000  mentc...........
-00001660: 0004 0000 0005 0000 004b 0000 0073 1a00  .........K...s..
-00001670: 0000 7c00 6a00 6a01 6a02 6600 7c01 7c02  ..|.j.j.j.f.|.|.
-00001680: 6401 9c02 7c03 9702 8e01 5300 2902 61e9  d...|.....S.).a.
-00001690: 0100 0044 656c 6574 6520 616e 2065 6c65  ...Delete an ele
-000016a0: 6d65 6e74 2062 7920 636f 6465 2e0a 0a20  ment by code... 
-000016b0: 2020 2020 2020 2041 6c6c 6f77 2074 6f20         Allow to 
-000016c0: 6465 6c65 7465 2061 2070 726f 6365 7373  delete a process
-000016d0: 2065 6c65 6d65 6e74 2062 7920 7370 6563   element by spec
-000016e0: 6966 7969 6e67 2074 6865 2069 7465 6d20  ifying the item 
-000016f0: 6465 6669 6e69 7469 6f6e 2063 6f64 652e  definition code.
-00001700: 0a0a 2020 2020 2020 2020 5265 6d6f 7665  ..        Remove
-00001710: 2061 6c6c 2074 6865 2065 6c65 6d65 6e74   all the element
-00001720: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
-00001730: 2020 3a70 6172 616d 2069 643a 2054 6865    :param id: The
-00001740: 2072 6573 6f75 7263 6520 4944 2e20 5265   resource ID. Re
-00001750: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-00001760: 3a74 7970 6520 6964 3a20 7374 720a 2020  :type id: str.  
-00001770: 2020 2020 2020 3a70 6172 616d 2063 6f6d        :param com
-00001780: 6d61 6e64 3a20 436f 6d6d 616e 6420 746f  mand: Command to
-00001790: 2064 656c 6574 6520 616e 2065 6c65 6d65   delete an eleme
-000017a0: 6e74 2e20 5265 7175 6972 6564 2e0a 2020  nt. Required..  
-000017b0: 2020 2020 2020 3a74 7970 6520 636f 6d6d        :type comm
-000017c0: 616e 643a 207e 6b75 666c 6f77 2e72 6573  and: ~kuflow.res
-000017d0: 742e 6d6f 6465 6c73 2e50 726f 6365 7373  t.models.Process
-000017e0: 4465 6c65 7465 456c 656d 656e 7443 6f6d  DeleteElementCom
-000017f0: 6d61 6e64 0a20 2020 2020 2020 203a 7265  mand.        :re
-00001800: 7475 726e 3a20 5072 6f63 6573 730a 2020  turn: Process.  
-00001810: 2020 2020 2020 3a72 7479 7065 3a20 7e6b        :rtype: ~k
-00001820: 7566 6c6f 772e 7265 7374 2e6d 6f64 656c  uflow.rest.model
-00001830: 732e 5072 6f63 6573 730a 2020 2020 2020  s.Process.      
-00001840: 2020 3a72 6169 7365 7320 7e61 7a75 7265    :raises ~azure
-00001850: 2e63 6f72 652e 6578 6365 7074 696f 6e73  .core.exceptions
-00001860: 2e48 7474 7052 6573 706f 6e73 6545 7272  .HttpResponseErr
-00001870: 6f72 3a0a 2020 2020 2020 2020 721f 0000  or:.        r...
-00001880: 0029 0372 0b00 0000 7218 0000 00da 1e61  .).r....r......a
-00001890: 6374 696f 6e73 5f70 726f 6365 7373 5f64  ctions_process_d
-000018a0: 656c 6574 655f 656c 656d 656e 7472 2100  elete_elementr!.
-000018b0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-000018c0: 0072 2300 0000 9d00 0000 7302 0000 0000  .r#.......s.....
-000018d0: 117a 3050 726f 6365 7373 4f70 6572 6174  .z0ProcessOperat
-000018e0: 696f 6e73 2e61 6374 696f 6e73 5f70 726f  ions.actions_pro
-000018f0: 6365 7373 5f64 656c 6574 655f 656c 656d  cess_delete_elem
-00001900: 656e 7463 0200 0000 0000 0000 0000 0000  entc............
-00001910: 0300 0000 0400 0000 4b00 0000 7318 0000  ........K...s...
-00001920: 007c 006a 006a 016a 0266 0064 017c 0169  .|.j.j.j.f.d.|.i
-00001930: 017c 0297 028e 0153 0029 0261 6801 0000  .|.....S.).ah...
-00001940: 436f 6d70 6c65 7465 2061 2050 726f 6365  Complete a Proce
-00001950: 7373 2e0a 0a20 2020 2020 2020 2043 6f6d  ss...        Com
-00001960: 706c 6574 6520 6120 5072 6f63 6573 732e  plete a Process.
-00001970: 2054 6865 2073 7461 7465 206f 6620 5072   The state of Pr
-00001980: 6f63 6573 7320 6973 2073 6574 2074 6f20  ocess is set to 
-00001990: 2763 6f6d 706c 6574 6564 272e 0a0a 2020  'completed'...  
-000019a0: 2020 2020 2020 4966 2079 6f75 2061 7265        If you are
-000019b0: 2061 6c72 6561 6479 2069 6e20 7468 6973   already in this
-000019c0: 2073 7461 7465 2c20 6e6f 2061 6374 696f   state, no actio
-000019d0: 6e20 6973 2074 616b 656e 2e0a 0a20 2020  n is taken...   
-000019e0: 2020 2020 203a 7061 7261 6d20 6964 3a20       :param id: 
-000019f0: 5468 6520 7265 736f 7572 6365 2049 442e  The resource ID.
-00001a00: 2052 6571 7569 7265 642e 0a20 2020 2020   Required..     
-00001a10: 2020 203a 7479 7065 2069 643a 2073 7472     :type id: str
-00001a20: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00001a30: 3a20 5072 6f63 6573 730a 2020 2020 2020  : Process.      
-00001a40: 2020 3a72 7479 7065 3a20 7e6b 7566 6c6f    :rtype: ~kuflo
-00001a50: 772e 7265 7374 2e6d 6f64 656c 732e 5072  w.rest.models.Pr
-00001a60: 6f63 6573 730a 2020 2020 2020 2020 3a72  ocess.        :r
-00001a70: 6169 7365 7320 7e61 7a75 7265 2e63 6f72  aises ~azure.cor
-00001a80: 652e 6578 6365 7074 696f 6e73 2e48 7474  e.exceptions.Htt
-00001a90: 7052 6573 706f 6e73 6545 7272 6f72 3a0a  pResponseError:.
-00001aa0: 2020 2020 2020 2020 721b 0000 0029 0372          r....).r
-00001ab0: 0b00 0000 7218 0000 00da 1861 6374 696f  ....r......actio
-00001ac0: 6e73 5f70 726f 6365 7373 5f63 6f6d 706c  ns_process_compl
-00001ad0: 6574 6572 1d00 0000 720d 0000 0072 0d00  eter....r....r..
-00001ae0: 0000 720e 0000 0072 2400 0000 b000 0000  ..r....r$.......
-00001af0: 7302 0000 0000 0d7a 2a50 726f 6365 7373  s......z*Process
-00001b00: 4f70 6572 6174 696f 6e73 2e61 6374 696f  Operations.actio
-00001b10: 6e73 5f70 726f 6365 7373 5f63 6f6d 706c  ns_process_compl
-00001b20: 6574 6563 0200 0000 0000 0000 0000 0000  etec............
-00001b30: 0300 0000 0400 0000 4b00 0000 7318 0000  ........K...s...
-00001b40: 007c 006a 006a 016a 0266 0064 017c 0169  .|.j.j.j.f.d.|.i
-00001b50: 017c 0297 028e 0153 0029 0261 a001 0000  .|.....S.).a....
-00001b60: 4361 6e63 656c 2061 2050 726f 6365 7373  Cancel a Process
-00001b70: 2e0a 0a20 2020 2020 2020 2043 616e 6365  ...        Cance
-00001b80: 6c20 6120 5072 6f63 6573 732e 2054 6865  l a Process. The
-00001b90: 2050 726f 6365 7373 2073 7461 7465 2069   Process state i
-00001ba0: 7320 7365 7420 746f 2027 6361 6e63 656c  s set to 'cancel
-00001bb0: 6c65 6427 2e0a 0a20 2020 2020 2020 2041  led'...        A
-00001bc0: 6c6c 2074 6865 2061 6374 6976 6520 7461  ll the active ta
-00001bd0: 736b 7320 7769 6c6c 2062 6520 6d61 726b  sks will be mark
-00001be0: 6564 2061 7320 6361 6e63 656c 6c65 6420  ed as cancelled 
-00001bf0: 746f 6f2e 0a0a 2020 2020 2020 2020 4966  too...        If
-00001c00: 2079 6f75 2061 7265 2061 6c72 6561 6479   you are already
-00001c10: 2069 6e20 7468 6973 2073 7461 7465 2c20   in this state, 
-00001c20: 6e6f 2061 6374 696f 6e20 6973 2074 616b  no action is tak
-00001c30: 656e 2e0a 0a20 2020 2020 2020 203a 7061  en...        :pa
-00001c40: 7261 6d20 6964 3a20 5468 6520 7265 736f  ram id: The reso
-00001c50: 7572 6365 2049 442e 2052 6571 7569 7265  urce ID. Require
-00001c60: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
-00001c70: 2069 643a 2073 7472 0a20 2020 2020 2020   id: str.       
-00001c80: 203a 7265 7475 726e 3a20 5072 6f63 6573   :return: Proces
-00001c90: 730a 2020 2020 2020 2020 3a72 7479 7065  s.        :rtype
-00001ca0: 3a20 7e6b 7566 6c6f 772e 7265 7374 2e6d  : ~kuflow.rest.m
-00001cb0: 6f64 656c 732e 5072 6f63 6573 730a 2020  odels.Process.  
-00001cc0: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
-00001cd0: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
-00001ce0: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
-00001cf0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-00001d00: 721b 0000 0029 0372 0b00 0000 7218 0000  r....).r....r...
-00001d10: 00da 1661 6374 696f 6e73 5f70 726f 6365  ...actions_proce
-00001d20: 7373 5f63 616e 6365 6c72 1d00 0000 720d  ss_cancelr....r.
-00001d30: 0000 0072 0d00 0000 720e 0000 0072 2500  ...r....r....r%.
-00001d40: 0000 bf00 0000 7302 0000 0000 0f7a 2850  ......s......z(P
-00001d50: 726f 6365 7373 4f70 6572 6174 696f 6e73  rocessOperations
-00001d60: 2e61 6374 696f 6e73 5f70 726f 6365 7373  .actions_process
-00001d70: 5f63 616e 6365 6c29 0572 1b00 0000 da04  _cancel).r......
-00001d80: 6669 6c65 721e 0000 0072 1400 0000 7215  filer....r....r.
-00001d90: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
-00001da0: 0500 0000 0800 0000 4b00 0000 7328 0000  ........K...s(..
-00001db0: 007c 006a 006a 016a 0266 007c 017c 026a  .|.j.j.j.f.|.|.j
-00001dc0: 037c 026a 047c 026a 057c 036a 0664 019c  .|.j.|.j.|.j.d..
-00001dd0: 057c 0497 028e 0153 0029 0261 2202 0000  .|.....S.).a"...
-00001de0: 5570 6c6f 6164 2061 6e64 2073 6176 6520  Upload and save 
-00001df0: 6120 646f 6375 6d65 6e74 2069 6e20 6120  a document in a 
-00001e00: 7573 6572 2061 6374 696f 6e2e 0a0a 2020  user action...  
-00001e10: 2020 2020 2020 416c 6c6f 7720 7361 7669        Allow savi
-00001e20: 6e67 2061 2075 7365 7220 6163 7469 6f6e  ng a user action
-00001e30: 2064 6f63 756d 656e 7420 7570 6c6f 6164   document upload
-00001e40: 696e 6720 7468 6520 636f 6e74 656e 742e  ing the content.
-00001e50: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00001e60: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
-00001e70: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
-00001e80: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
-00001e90: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
-00001ea0: 6172 616d 2066 696c 653a 2044 6f63 756d  aram file: Docum
-00001eb0: 656e 7420 746f 2073 6176 652e 2052 6571  ent to save. Req
-00001ec0: 7569 7265 642e 0a20 2020 2020 2020 203a  uired..        :
-00001ed0: 7479 7065 2066 696c 653a 205f 6d6f 6465  type file: _mode
-00001ee0: 6c73 2e44 6f63 756d 656e 740a 2020 2020  ls.Document.    
-00001ef0: 2020 2020 3a6b 6579 776f 7264 2063 6f6d      :keyword com
-00001f00: 6d61 6e64 3a20 5573 6572 2061 6374 696f  mand: User actio
-00001f10: 6e20 696e 666f 2e20 5265 7175 6972 6564  n info. Required
-00001f20: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00001f30: 636f 6d6d 616e 643a 205f 6d6f 6465 6c73  command: _models
-00001f40: 2e50 726f 6365 7373 5361 7665 5573 6572  .ProcessSaveUser
-00001f50: 4163 7469 6f6e 5661 6c75 6544 6f63 756d  ActionValueDocum
-00001f60: 656e 7443 6f6d 6d61 6e64 0a20 2020 2020  entCommand.     
-00001f70: 2020 203a 7265 7475 726e 3a20 5072 6f63     :return: Proc
-00001f80: 6573 7320 6f72 204e 6f6e 650a 2020 2020  ess or None.    
-00001f90: 2020 2020 3a72 7479 7065 3a20 7e6b 7566      :rtype: ~kuf
-00001fa0: 6c6f 772e 7265 7374 2e6d 6f64 656c 732e  low.rest.models.
-00001fb0: 5072 6f63 6573 7320 6f72 204e 6f6e 650a  Process or None.
-00001fc0: 2020 2020 2020 2020 3a72 6169 7365 7320          :raises 
-00001fd0: 7e61 7a75 7265 2e63 6f72 652e 6578 6365  ~azure.core.exce
-00001fe0: 7074 696f 6e73 2e48 7474 7052 6573 706f  ptions.HttpRespo
-00001ff0: 6e73 6545 7272 6f72 3a0a 2020 2020 2020  nseError:.      
-00002000: 2020 2905 721b 0000 0072 2600 0000 da11    ).r....r&.....
-00002010: 6669 6c65 5f63 6f6e 7465 6e74 5f74 7970  file_content_typ
-00002020: 65da 0966 696c 655f 6e61 6d65 da14 7573  e..file_name..us
-00002030: 6572 5f61 6374 696f 6e5f 7661 6c75 655f  er_action_value_
-00002040: 6964 2907 720b 0000 0072 1800 0000 da2f  id).r....r...../
-00002050: 6163 7469 6f6e 735f 7072 6f63 6573 735f  actions_process_
-00002060: 7361 7665 5f75 7365 725f 6163 7469 6f6e  save_user_action
-00002070: 5f76 616c 7565 5f64 6f63 756d 656e 745a  _value_documentZ
-00002080: 0c66 696c 655f 636f 6e74 656e 74da 0c63  .file_content..c
-00002090: 6f6e 7465 6e74 5f74 7970 655a 0966 696c  ontent_typeZ.fil
-000020a0: 655f 6d61 6d65 7229 0000 0029 0572 0c00  e_mamer)...).r..
-000020b0: 0000 721b 0000 0072 2600 0000 721e 0000  ..r....r&...r...
-000020c0: 0072 1400 0000 720d 0000 0072 0d00 0000  .r....r....r....
-000020d0: 720e 0000 0072 2a00 0000 d000 0000 7312  r....r*.......s.
-000020e0: 0000 0000 110a 0102 0104 0104 0104 0104  ................
-000020f0: fb04 0602 fa7a 4150 726f 6365 7373 4f70  .....zAProcessOp
-00002100: 6572 6174 696f 6e73 2e61 6374 696f 6e73  erations.actions
-00002110: 5f70 726f 6365 7373 5f73 6176 655f 7573  _process_save_us
-00002120: 6572 5f61 6374 696f 6e5f 7661 6c75 655f  er_action_value_
-00002130: 646f 6375 6d65 6e74 2903 7210 0000 0072  document).r....r
-00002140: 0100 0000 4e29 1dda 085f 5f6e 616d 655f  ....N)...__name_
-00002150: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00002160: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00002170: 6f63 5f5f da19 4b75 466c 6f77 5265 7374  oc__..KuFlowRest
-00002180: 436c 6965 6e74 4765 6e65 7261 7465 6472  ClientGeneratedr
-00002190: 0f00 0000 da03 696e 7472 0400 0000 7205  ......intr....r.
-000021a0: 0000 0072 1700 0000 7203 0000 0072 0200  ...r....r....r..
-000021b0: 0000 da07 5f6d 6f64 656c 73da 0b50 726f  ...._models..Pro
-000021c0: 6365 7373 5061 6765 7219 0000 00da 0750  cessPager......P
-000021d0: 726f 6365 7373 721a 0000 0072 1c00 0000  rocessr....r....
-000021e0: da1d 5072 6f63 6573 7343 6861 6e67 6549  ..ProcessChangeI
-000021f0: 6e69 7469 6174 6f72 436f 6d6d 616e 6472  nitiatorCommandr
-00002200: 2000 0000 da19 5072 6f63 6573 7353 6176   .....ProcessSav
-00002210: 6545 6c65 6d65 6e74 436f 6d6d 616e 6472  eElementCommandr
-00002220: 2200 0000 da1b 5072 6f63 6573 7344 656c  ".....ProcessDel
-00002230: 6574 6545 6c65 6d65 6e74 436f 6d6d 616e  eteElementComman
-00002240: 6472 2300 0000 7224 0000 0072 2500 0000  dr#...r$...r%...
-00002250: 5a08 446f 6375 6d65 6e74 5a29 5072 6f63  Z.DocumentZ)Proc
-00002260: 6573 7353 6176 6555 7365 7241 6374 696f  essSaveUserActio
-00002270: 6e56 616c 7565 446f 6375 6d65 6e74 436f  nValueDocumentCo
-00002280: 6d6d 616e 6472 2a00 0000 720d 0000 0072  mmandr*...r....r
-00002290: 0d00 0000 720d 0000 0072 0e00 0000 7209  ....r....r....r.
-000022a0: 0000 0021 0000 0073 4a00 0000 0801 0409  ...!...sJ.......
-000022b0: 0e04 0000 0000 00ff 0201 0200 0200 1200  ................
-000022c0: 0201 04fe 0c1d 1619 140e 0200 0400 0201  ................
-000022d0: 04fe 0c16 0200 0400 0201 04fe 0c18 0200  ................
-000022e0: 0400 0201 04fe 0c13 140f 1412 0200 0400  ................
-000022f0: 0400 0201 08fe 7209 0000 004e 290c da06  ......r....N)...
-00002300: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00002310: 7204 0000 0072 0500 0000 da0a 5f67 656e  r....r......_gen
-00002320: 6572 6174 6564 7207 0000 0072 3000 0000  eratedr....r0...
-00002330: da00 7208 0000 0072 3200 0000 7209 0000  ..r....r2...r...
-00002340: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00002350: 720e 0000 00da 083c 6d6f 6475 6c65 3e1a  r......<module>.
-00002360: 0000 0073 0600 0000 1802 0c02 0c03       ...s..........
+00000310: 5300 2901 4e29 01da 0e5f 6b75 666c 6f77  S.).N)..._kuflow
+00000320: 5f63 6c69 656e 7429 02da 0473 656c 6672  _client)...selfr
+00000330: 0a00 0000 a900 720d 0000 00fa 512f 776f  ......r.....Q/wo
+00000340: 726b 2f6b 7566 6c6f 772d 7364 6b2d 7079  rk/kuflow-sdk-py
+00000350: 7468 6f6e 2f6b 7566 6c6f 772d 7265 7374  thon/kuflow-rest
+00000360: 2f6b 7566 6c6f 775f 7265 7374 2f6f 7065  /kuflow_rest/ope
+00000370: 7261 7469 6f6e 732f 5f70 726f 6365 7373  rations/_process
+00000380: 5f6f 7065 7261 7469 6f6e 732e 7079 da08  _operations.py..
+00000390: 5f5f 696e 6974 5f5f 2b00 0000 7302 0000  __init__+...s...
+000003a0: 0000 017a 1a50 726f 6365 7373 4f70 6572  ...z.ProcessOper
+000003b0: 6174 696f 6e73 2e5f 5f69 6e69 745f 5fe9  ations.__init__.
+000003c0: 1900 0000 7201 0000 004e 2905 da04 7369  ....r....N)...si
+000003d0: 7a65 da04 7061 6765 da04 736f 7274 da06  ze..page..sort..
+000003e0: 6b77 6172 6773 da06 7265 7475 726e 6304  kwargs..returnc.
+000003f0: 0000 0000 0000 0000 0000 0005 0000 0006  ................
+00000400: 0000 004b 0000 0073 3400 0000 7c03 6401  ...K...s4...|.d.
+00000410: 6b09 7218 7400 7c03 7401 8302 7218 7c03  k.r.t.|.t...r.|.
+00000420: 6701 7d03 7c00 6a02 6a03 6a04 6600 7c01  g.}.|.j.j.j.f.|.
+00000430: 7c02 7c03 6402 9c03 7c04 9702 8e01 5300  |.|.d...|.....S.
+00000440: 2903 61db 0300 0046 696e 6420 616c 6c20  ).a....Find all 
+00000450: 6163 6365 7373 6962 6c65 2050 726f 6365  accessible Proce
+00000460: 7373 6573 2e0a 0a20 2020 2020 2020 204c  sses...        L
+00000470: 6973 7420 616c 6c20 7468 6520 5072 6f63  ist all the Proc
+00000480: 6573 7365 7320 7468 6174 2068 6176 6520  esses that have 
+00000490: 6265 656e 2063 7265 6174 6564 2061 6e64  been created and
+000004a0: 2074 6865 2063 7265 6465 6e74 6961 6c73   the credentials
+000004b0: 2068 6173 2061 6363 6573 732e 0a0a 2020   has access...  
+000004c0: 2020 2020 2020 4176 6169 6c61 626c 6520        Available 
+000004d0: 736f 7274 2071 7565 7279 2076 616c 7565  sort query value
+000004e0: 733a 2069 642c 2063 7265 6174 6564 4174  s: id, createdAt
+000004f0: 2c20 6c61 7374 4d6f 6469 6669 6564 4174  , lastModifiedAt
+00000500: 2e0a 0a20 2020 2020 2020 203a 6b65 7977  ...        :keyw
+00000510: 6f72 6420 7369 7a65 3a20 5468 6520 6e75  ord size: The nu
+00000520: 6d62 6572 206f 6620 7265 636f 7264 7320  mber of records 
+00000530: 7265 7475 726e 6564 2077 6974 6869 6e20  returned within 
+00000540: 6120 7369 6e67 6c65 2041 5049 2063 616c  a single API cal
+00000550: 6c2e 2044 6566 6175 6c74 2076 616c 7565  l. Default value
+00000560: 2069 7320 3235 2e0a 2020 2020 2020 2020   is 25..        
+00000570: 3a74 7970 6520 7369 7a65 3a20 696e 740a  :type size: int.
+00000580: 2020 2020 2020 2020 3a6b 6579 776f 7264          :keyword
+00000590: 2070 6167 653a 2054 6865 2070 6167 6520   page: The page 
+000005a0: 6e75 6d62 6572 206f 6620 7468 6520 6375  number of the cu
+000005b0: 7272 656e 7420 7061 6765 2069 6e20 7468  rrent page in th
+000005c0: 6520 7265 7475 726e 6564 2072 6563 6f72  e returned recor
+000005d0: 6473 2c20 3020 6973 2074 6865 2066 6972  ds, 0 is the fir
+000005e0: 7374 2070 6167 652e 0a20 2020 2020 2020  st page..       
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 4465 6661 756c 7420 7661 6c75 6520 6973  Default value is
+00000610: 2030 2e0a 2020 2020 2020 2020 3a74 7970   0..        :typ
+00000620: 6520 7061 6765 3a20 696e 740a 2020 2020  e page: int.    
+00000630: 2020 2020 3a6b 6579 776f 7264 2073 6f72      :keyword sor
+00000640: 743a 2053 6f72 7469 6e67 2063 7269 7465  t: Sorting crite
+00000650: 7269 6120 696e 2074 6865 2066 6f72 6d61  ria in the forma
+00000660: 743a 2070 726f 7065 7274 797b 2c61 7363  t: property{,asc
+00000670: 7c64 6573 637d 2e20 4578 616d 706c 653a  |desc}. Example:
+00000680: 2063 7265 6174 6564 4174 2c64 6573 630a   createdAt,desc.
+00000690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000006a0: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+000006b0: 736f 7274 206f 7264 6572 2069 7320 6173  sort order is as
+000006c0: 6365 6e64 696e 672e 204d 756c 7469 706c  cending. Multipl
+000006d0: 6520 736f 7274 2063 7269 7465 7269 6120  e sort criteria 
+000006e0: 6172 6520 7375 7070 6f72 7465 642e 0a0a  are supported...
+000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000700: 2020 2020 2020 2050 6c65 6173 6520 7265         Please re
+00000710: 6665 7220 746f 2074 6865 206d 6574 686f  fer to the metho
+00000720: 6420 6465 7363 7269 7074 696f 6e20 666f  d description fo
+00000730: 7220 7375 7070 6f72 7465 6420 7072 6f70  r supported prop
+00000740: 6572 7469 6573 2e20 4465 6661 756c 7420  erties. Default 
+00000750: 7661 6c75 6520 6973 204e 6f6e 652e 0a20  value is None.. 
+00000760: 2020 2020 2020 203a 7479 7065 2073 6f72         :type sor
+00000770: 743a 204f 7074 696f 6e61 6c5b 556e 696f  t: Optional[Unio
+00000780: 6e5b 7374 722c 204c 6973 745b 7374 725d  n[str, List[str]
+00000790: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
+000007a0: 726e 3a20 5072 6f63 6573 7350 6167 650a  rn: ProcessPage.
+000007b0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000007c0: 7e6b 7566 6c6f 772e 7265 7374 2e6d 6f64  ~kuflow.rest.mod
+000007d0: 656c 732e 5072 6f63 6573 7350 6167 650a  els.ProcessPage.
+000007e0: 2020 2020 2020 2020 3a72 6169 7365 7320          :raises 
+000007f0: 7e61 7a75 7265 2e63 6f72 652e 6578 6365  ~azure.core.exce
+00000800: 7074 696f 6e73 2e48 7474 7052 6573 706f  ptions.HttpRespo
+00000810: 6e73 6545 7272 6f72 3a0a 2020 2020 2020  nseError:.      
+00000820: 2020 4e29 0372 1100 0000 7212 0000 0072    N).r....r....r
+00000830: 1300 0000 2905 da0a 6973 696e 7374 616e  ....)...isinstan
+00000840: 6365 da03 7374 7272 0b00 0000 da07 7072  ce..strr......pr
+00000850: 6f63 6573 73da 0e66 696e 645f 7072 6f63  ocess..find_proc
+00000860: 6573 7365 7329 0572 0c00 0000 7211 0000  esses).r....r...
+00000870: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000880: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000890: 1900 0000 2e00 0000 7306 0000 0000 1812  ........s.......
+000008a0: 0106 027a 2050 726f 6365 7373 4f70 6572  ...z ProcessOper
+000008b0: 6174 696f 6e73 2e66 696e 645f 7072 6f63  ations.find_proc
+000008c0: 6573 7365 7329 0372 1800 0000 7214 0000  esses).r....r...
+000008d0: 0072 1500 0000 6302 0000 0000 0000 0000  .r....c.........
+000008e0: 0000 0003 0000 0004 0000 004b 0000 0073  ...........K...s
+000008f0: 1800 0000 7c00 6a00 6a01 6a02 6600 6401  ....|.j.j.j.f.d.
+00000900: 7c01 6901 7c02 9702 8e01 5300 2902 6101  |.i.|.....S.).a.
+00000910: 0400 0043 7265 6174 6520 6120 6e65 7720  ...Create a new 
+00000920: 7072 6f63 6573 732e 0a0a 2020 2020 2020  process...      
+00000930: 2020 4372 6561 7465 7320 6120 7072 6f63    Creates a proc
+00000940: 6573 732e 2054 6869 7320 6f70 7469 6f6e  ess. This option
+00000950: 2068 6173 2064 6972 6563 7420 636f 7272   has direct corr
+00000960: 6573 706f 6e64 656e 6365 2074 6f20 7468  espondence to th
+00000970: 6520 6163 7469 6f6e 206f 6620 7374 6172  e action of star
+00000980: 7469 6e67 2061 2070 726f 6365 7373 2069  ting a process i
+00000990: 6e0a 2020 2020 2020 2020 7468 6520 4b75  n.        the Ku
+000009a0: 666c 6f77 2047 5549 2e0a 0a20 2020 2020  flow GUI...     
+000009b0: 2020 2057 6865 6e20 6120 7072 6f63 6573     When a proces
+000009c0: 7320 6973 2063 7265 6174 6564 2c20 7468  s is created, th
+000009d0: 6520 6375 7272 656e 7420 7573 6572 2069  e current user i
+000009e0: 7320 6173 7369 676e 6564 2061 7320 7468  s assigned as th
+000009f0: 6520 7072 6f63 6573 7320 696e 6974 6961  e process initia
+00000a00: 746f 722c 2069 6620 796f 7520 7761 6e74  tor, if you want
+00000a10: 0a20 2020 2020 2020 2074 6f20 6368 616e  .        to chan
+00000a20: 6765 2069 742c 2079 6f75 2063 616e 2070  ge it, you can p
+00000a30: 6173 7320 6120 7661 6c69 6420 696e 6974  ass a valid init
+00000a40: 6961 746f 7220 7573 696e 6720 7468 6520  iator using the 
+00000a50: 666f 6c6c 6f77 696e 6720 6f70 7469 6f6e  following option
+00000a60: 733a 0a0a 0a20 2020 2020 2020 202a 2049  s:...        * I
+00000a70: 6620 796f 7520 6b6e 6f77 2074 6865 2060  f you know the `
+00000a80: 6070 7269 6e63 6970 616c 2049 4460 6020  `principal ID`` 
+00000a90: 796f 7520 6361 6e20 6173 7369 676e 2069  you can assign i
+00000aa0: 7420 746f 2060 6069 6e69 7469 6174 6f72  t to ``initiator
+00000ab0: 2e69 6460 600a 2020 2020 2020 2020 2a20  .id``.        * 
+00000ac0: 4966 2079 6f75 206b 6e6f 7720 7468 6520  If you know the 
+00000ad0: 6060 7573 6572 2049 4460 6020 796f 7520  ``user ID`` you 
+00000ae0: 6361 6e20 6173 7369 676e 2069 7420 746f  can assign it to
+00000af0: 2060 6069 6e69 7469 6174 6f72 2e75 7365   ``initiator.use
+00000b00: 722e 6964 6060 0a20 2020 2020 2020 202a  r.id``.        *
+00000b10: 2049 6620 796f 7520 6b6e 6f77 2074 6865   If you know the
+00000b20: 2060 6075 7365 7220 656d 6169 6c60 6020   ``user email`` 
+00000b30: 796f 7520 6361 6e20 6173 7369 676e 2069  you can assign i
+00000b40: 7420 746f 2060 6069 6e69 7469 6174 6f72  t to ``initiator
+00000b50: 2e75 7365 722e 656d 6169 6c60 600a 2020  .user.email``.  
+00000b60: 2020 2020 2020 2a20 4966 2079 6f75 206b        * If you k
+00000b70: 6e6f 7720 7468 6520 6060 6170 706c 6963  now the ``applic
+00000b80: 6174 696f 6e20 4944 6060 2079 6f75 2063  ation ID`` you c
+00000b90: 616e 2061 7373 6967 6e20 6974 2074 6f20  an assign it to 
+00000ba0: 6060 696e 6974 6961 746f 722e 6170 706c  ``initiator.appl
+00000bb0: 6963 6174 696f 6e2e 6964 6060 0a0a 2020  ication.id``..  
+00000bc0: 2020 2020 2020 4966 2079 6f75 2077 616e        If you wan
+00000bd0: 7420 7468 6520 6d65 7468 6f64 2074 6f20  t the method to 
+00000be0: 6265 2069 6465 6d70 6f74 656e 742c 2070  be idempotent, p
+00000bf0: 6c65 6173 6520 7370 6563 6966 7920 7468  lease specify th
+00000c00: 6520 6060 6964 6060 2066 6965 6c64 2069  e ``id`` field i
+00000c10: 6e20 7468 6520 7265 7175 6573 7420 626f  n the request bo
+00000c20: 6479 2e0a 0a20 2020 2020 2020 203a 7061  dy...        :pa
+00000c30: 7261 6d20 7072 6f63 6573 733a 2050 726f  ram process: Pro
+00000c40: 6365 7373 2074 6f20 6372 6561 7465 2e20  cess to create. 
+00000c50: 5265 7175 6972 6564 2e0a 2020 2020 2020  Required..      
+00000c60: 2020 3a74 7970 6520 7072 6f63 6573 733a    :type process:
+00000c70: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
+00000c80: 6465 6c73 2e50 726f 6365 7373 0a20 2020  dels.Process.   
+00000c90: 2020 2020 203a 7265 7475 726e 3a20 5072       :return: Pr
+00000ca0: 6f63 6573 730a 2020 2020 2020 2020 3a72  ocess.        :r
+00000cb0: 7479 7065 3a20 7e6b 7566 6c6f 772e 7265  type: ~kuflow.re
+00000cc0: 7374 2e6d 6f64 656c 732e 5072 6f63 6573  st.models.Proces
+00000cd0: 730a 2020 2020 2020 2020 3a72 6169 7365  s.        :raise
+00000ce0: 7320 7e61 7a75 7265 2e63 6f72 652e 6578  s ~azure.core.ex
+00000cf0: 6365 7074 696f 6e73 2e48 7474 7052 6573  ceptions.HttpRes
+00000d00: 706f 6e73 6545 7272 6f72 3a0a 2020 2020  ponseError:.    
+00000d10: 2020 2020 7218 0000 0029 0372 0b00 0000      r....).r....
+00000d20: 7218 0000 00da 0e63 7265 6174 655f 7072  r......create_pr
+00000d30: 6f63 6573 7329 0372 0c00 0000 7218 0000  ocess).r....r...
+00000d40: 0072 1400 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000d50: 720e 0000 0072 1a00 0000 4b00 0000 7302  r....r....K...s.
+00000d60: 0000 0000 177a 2050 726f 6365 7373 4f70  .....z ProcessOp
+00000d70: 6572 6174 696f 6e73 2e63 7265 6174 655f  erations.create_
+00000d80: 7072 6f63 6573 7329 03da 0269 6472 1400  process)...idr..
+00000d90: 0000 7215 0000 0063 0200 0000 0000 0000  ..r....c........
+00000da0: 0000 0000 0300 0000 0400 0000 4b00 0000  ............K...
+00000db0: 7318 0000 007c 006a 006a 016a 0266 0064  s....|.j.j.j.f.d
+00000dc0: 017c 0169 017c 0297 028e 0153 0029 0261  .|.i.|.....S.).a
+00000dd0: 2201 0000 4765 7420 6120 5072 6f63 6573  "...Get a Proces
+00000de0: 7320 6279 2049 442e 0a0a 2020 2020 2020  s by ID...      
+00000df0: 2020 5265 7475 726e 7320 7468 6520 7265    Returns the re
+00000e00: 7175 6573 7465 6420 5072 6f63 6573 7320  quested Process 
+00000e10: 7768 656e 2068 6173 2061 6363 6573 7320  when has access 
+00000e20: 746f 2064 6f20 6974 2e0a 0a20 2020 2020  to do it...     
+00000e30: 2020 203a 7061 7261 6d20 6964 3a20 5468     :param id: Th
+00000e40: 6520 7265 736f 7572 6365 2049 442e 2052  e resource ID. R
+00000e50: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
+00000e60: 203a 7479 7065 2069 643a 2073 7472 0a20   :type id: str. 
+00000e70: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00000e80: 5072 6f63 6573 730a 2020 2020 2020 2020  Process.        
+00000e90: 3a72 7479 7065 3a20 7e6b 7566 6c6f 772e  :rtype: ~kuflow.
+00000ea0: 7265 7374 2e6d 6f64 656c 732e 5072 6f63  rest.models.Proc
+00000eb0: 6573 730a 2020 2020 2020 2020 3a72 6169  ess.        :rai
+00000ec0: 7365 7320 7e61 7a75 7265 2e63 6f72 652e  ses ~azure.core.
+00000ed0: 6578 6365 7074 696f 6e73 2e48 7474 7052  exceptions.HttpR
+00000ee0: 6573 706f 6e73 6545 7272 6f72 3a0a 2020  esponseError:.  
+00000ef0: 2020 2020 2020 721b 0000 0029 0372 0b00        r....).r..
+00000f00: 0000 7218 0000 00da 1072 6574 7269 6576  ..r......retriev
+00000f10: 655f 7072 6f63 6573 73a9 0372 0c00 0000  e_process..r....
+00000f20: 721b 0000 0072 1400 0000 720d 0000 0072  r....r....r....r
+00000f30: 0d00 0000 720e 0000 0072 1c00 0000 6400  ....r....r....d.
+00000f40: 0000 7302 0000 0000 0b7a 2250 726f 6365  ..s......z"Proce
+00000f50: 7373 4f70 6572 6174 696f 6e73 2e72 6574  ssOperations.ret
+00000f60: 7269 6576 655f 7072 6f63 6573 7329 0472  rieve_process).r
+00000f70: 1b00 0000 da07 636f 6d6d 616e 6472 1400  ......commandr..
+00000f80: 0000 7215 0000 0063 0300 0000 0000 0000  ..r....c........
+00000f90: 0000 0000 0400 0000 0500 0000 4b00 0000  ............K...
+00000fa0: 731a 0000 007c 006a 006a 016a 0266 007c  s....|.j.j.j.f.|
+00000fb0: 017c 0264 019c 027c 0397 028e 0153 0029  .|.d...|.....S.)
+00000fc0: 0261 5302 0000 4368 616e 6765 2070 726f  .aS...Change pro
+00000fd0: 6365 7373 2069 6e69 7469 6174 6f72 2e0a  cess initiator..
+00000fe0: 0a20 2020 2020 2020 2043 6861 6e67 6520  .        Change 
+00000ff0: 7468 6520 6375 7272 656e 7420 696e 6974  the current init
+00001000: 6961 746f 7220 6f66 2061 2070 726f 6365  iator of a proce
+00001010: 7373 2e0a 0a20 2020 2020 2020 2041 6c6c  ss...        All
+00001020: 6f77 7320 796f 7520 746f 2063 686f 6f73  ows you to choos
+00001030: 6520 6120 7573 6572 2028 6279 2065 6d61  e a user (by ema
+00001040: 696c 206f 7220 7072 696e 6369 7061 6c20  il or principal 
+00001050: 6964 656e 7469 6669 6572 2920 6f72 2061  identifier) or a
+00001060: 6e20 6170 706c 6963 6174 696f 6e20 2870  n application (p
+00001070: 7269 6e63 6970 616c 0a20 2020 2020 2020  rincipal.       
+00001080: 2069 6465 6e74 6966 6965 7229 2e0a 2020   identifier)..  
+00001090: 2020 2020 2020 4f6e 6c79 206f 6e65 206f        Only one o
+000010a0: 7074 696f 6e20 7769 6c6c 2062 6520 6e65  ption will be ne
+000010b0: 6365 7373 6172 792e 0a0a 2020 2020 2020  cessary...      
+000010c0: 2020 3a70 6172 616d 2069 643a 2054 6865    :param id: The
+000010d0: 2072 6573 6f75 7263 6520 4944 2e20 5265   resource ID. Re
+000010e0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+000010f0: 3a74 7970 6520 6964 3a20 7374 720a 2020  :type id: str.  
+00001100: 2020 2020 2020 3a70 6172 616d 2063 6f6d        :param com
+00001110: 6d61 6e64 3a20 436f 6d6d 616e 6420 746f  mand: Command to
+00001120: 2063 6861 6e67 6520 7468 6520 7072 6f63   change the proc
+00001130: 6573 7320 696e 6974 6961 746f 722e 2052  ess initiator. R
+00001140: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
+00001150: 203a 7479 7065 2063 6f6d 6d61 6e64 3a20   :type command: 
+00001160: 7e6b 7566 6c6f 772e 7265 7374 2e6d 6f64  ~kuflow.rest.mod
+00001170: 656c 732e 5072 6f63 6573 7343 6861 6e67  els.ProcessChang
+00001180: 6549 6e69 7469 6174 6f72 436f 6d6d 616e  eInitiatorComman
+00001190: 640a 2020 2020 2020 2020 3a72 6574 7572  d.        :retur
+000011a0: 6e3a 2050 726f 6365 7373 0a20 2020 2020  n: Process.     
+000011b0: 2020 203a 7274 7970 653a 207e 6b75 666c     :rtype: ~kufl
+000011c0: 6f77 2e72 6573 742e 6d6f 6465 6c73 2e50  ow.rest.models.P
+000011d0: 726f 6365 7373 0a20 2020 2020 2020 203a  rocess.        :
+000011e0: 7261 6973 6573 207e 617a 7572 652e 636f  raises ~azure.co
+000011f0: 7265 2e65 7863 6570 7469 6f6e 732e 4874  re.exceptions.Ht
+00001200: 7470 5265 7370 6f6e 7365 4572 726f 723a  tpResponseError:
+00001210: 0a20 2020 2020 2020 20a9 0272 1b00 0000  .        ..r....
+00001220: 721e 0000 0029 0372 0b00 0000 7218 0000  r....).r....r...
+00001230: 00da 2061 6374 696f 6e73 5f70 726f 6365  .. actions_proce
+00001240: 7373 5f63 6861 6e67 655f 696e 6974 6961  ss_change_initia
+00001250: 746f 72a9 0472 0c00 0000 721b 0000 0072  tor..r....r....r
+00001260: 1e00 0000 7214 0000 0072 0d00 0000 720d  ....r....r....r.
+00001270: 0000 0072 0e00 0000 7220 0000 0071 0000  ...r....r ...q..
+00001280: 0073 0200 0000 0013 7a32 5072 6f63 6573  .s......z2Proces
+00001290: 734f 7065 7261 7469 6f6e 732e 6163 7469  sOperations.acti
+000012a0: 6f6e 735f 7072 6f63 6573 735f 6368 616e  ons_process_chan
+000012b0: 6765 5f69 6e69 7469 6174 6f72 6303 0000  ge_initiatorc...
+000012c0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+000012d0: 004b 0000 0073 1a00 0000 7c00 6a00 6a01  .K...s....|.j.j.
+000012e0: 6a02 6600 7c01 7c02 6401 9c02 7c03 9702  j.f.|.|.d...|...
+000012f0: 8e01 5300 2902 61c3 0200 0053 6176 6520  ..S.).a....Save 
+00001300: 6120 7072 6f63 6573 7320 656c 656d 656e  a process elemen
+00001310: 742c 2061 6b61 3a20 6d65 7461 6461 7461  t, aka: metadata
+00001320: 2e0a 0a20 2020 2020 2020 2041 6c6c 6f77  ...        Allow
+00001330: 2074 6f20 7361 7665 2061 6e20 656c 656d   to save an elem
+00001340: 656e 742e 0a0a 2020 2020 2020 2020 4966  ent...        If
+00001350: 2076 616c 7565 7320 616c 7265 6164 7920   values already 
+00001360: 6578 6973 7420 666f 7220 7468 6520 7072  exist for the pr
+00001370: 6f76 6964 6564 2065 6c65 6d65 6e74 2063  ovided element c
+00001380: 6f64 652c 2069 7420 7265 706c 6163 6573  ode, it replaces
+00001390: 2074 6865 6d20 7769 7468 2074 6865 206e   them with the n
+000013a0: 6577 206f 6e65 732c 0a20 2020 2020 2020  ew ones,.       
+000013b0: 206f 7468 6572 7769 7365 2069 7420 6372   otherwise it cr
+000013c0: 6561 7465 7320 7468 656d 2e20 5468 6520  eates them. The 
+000013d0: 7661 6c75 6573 206f 6620 7468 6520 7072  values of the pr
+000013e0: 6576 696f 7573 2065 6c65 6d65 6e74 7320  evious elements 
+000013f0: 7468 6174 206e 6f20 6c6f 6e67 6572 2065  that no longer e
+00001400: 7869 7374 2077 696c 6c20 6265 0a20 2020  xist will be.   
+00001410: 2020 2020 2064 656c 6574 6564 2e0a 0a20       deleted... 
+00001420: 2020 2020 2020 2049 6620 7468 6520 7072         If the pr
+00001430: 6f63 6573 7320 6973 2061 6c72 6561 6479  ocess is already
+00001440: 2066 696e 6973 6865 6420 7468 6520 696e   finished the in
+00001450: 766f 6361 7469 6f6e 7320 6661 696c 7320  vocations fails 
+00001460: 7769 7468 2061 6e20 6572 726f 722e 0a0a  with an error...
+00001470: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00001480: 643a 2054 6865 2072 6573 6f75 7263 6520  d: The resource 
+00001490: 4944 2e20 5265 7175 6972 6564 2e0a 2020  ID. Required..  
+000014a0: 2020 2020 2020 3a74 7970 6520 6964 3a20        :type id: 
+000014b0: 7374 720a 2020 2020 2020 2020 3a70 6172  str.        :par
+000014c0: 616d 2063 6f6d 6d61 6e64 3a20 436f 6d6d  am command: Comm
+000014d0: 616e 6420 746f 2073 6176 6520 616e 2065  and to save an e
+000014e0: 6c65 6d65 6e74 2e20 5265 7175 6972 6564  lement. Required
+000014f0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00001500: 636f 6d6d 616e 643a 207e 6b75 666c 6f77  command: ~kuflow
+00001510: 2e72 6573 742e 6d6f 6465 6c73 2e50 726f  .rest.models.Pro
+00001520: 6365 7373 5361 7665 456c 656d 656e 7443  cessSaveElementC
+00001530: 6f6d 6d61 6e64 0a20 2020 2020 2020 203a  ommand.        :
+00001540: 7265 7475 726e 3a20 5072 6f63 6573 730a  return: Process.
+00001550: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00001560: 7e6b 7566 6c6f 772e 7265 7374 2e6d 6f64  ~kuflow.rest.mod
+00001570: 656c 732e 5072 6f63 6573 730a 2020 2020  els.Process.    
+00001580: 2020 2020 3a72 6169 7365 7320 7e61 7a75      :raises ~azu
+00001590: 7265 2e63 6f72 652e 6578 6365 7074 696f  re.core.exceptio
+000015a0: 6e73 2e48 7474 7052 6573 706f 6e73 6545  ns.HttpResponseE
+000015b0: 7272 6f72 3a0a 2020 2020 2020 2020 721f  rror:.        r.
+000015c0: 0000 0029 0372 0b00 0000 7218 0000 00da  ...).r....r.....
+000015d0: 1c61 6374 696f 6e73 5f70 726f 6365 7373  .actions_process
+000015e0: 5f73 6176 655f 656c 656d 656e 7472 2100  _save_elementr!.
+000015f0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00001600: 0072 2200 0000 8600 0000 7302 0000 0000  .r".......s.....
+00001610: 157a 2e50 726f 6365 7373 4f70 6572 6174  .z.ProcessOperat
+00001620: 696f 6e73 2e61 6374 696f 6e73 5f70 726f  ions.actions_pro
+00001630: 6365 7373 5f73 6176 655f 656c 656d 656e  cess_save_elemen
+00001640: 7463 0300 0000 0000 0000 0000 0000 0400  tc..............
+00001650: 0000 0500 0000 4b00 0000 731a 0000 007c  ......K...s....|
+00001660: 006a 006a 016a 0266 007c 017c 0264 019c  .j.j.j.f.|.|.d..
+00001670: 027c 0397 028e 0153 0029 0261 e901 0000  .|.....S.).a....
+00001680: 4465 6c65 7465 2061 6e20 656c 656d 656e  Delete an elemen
+00001690: 7420 6279 2063 6f64 652e 0a0a 2020 2020  t by code...    
+000016a0: 2020 2020 416c 6c6f 7720 746f 2064 656c      Allow to del
+000016b0: 6574 6520 6120 7072 6f63 6573 7320 656c  ete a process el
+000016c0: 656d 656e 7420 6279 2073 7065 6369 6679  ement by specify
+000016d0: 696e 6720 7468 6520 6974 656d 2064 6566  ing the item def
+000016e0: 696e 6974 696f 6e20 636f 6465 2e0a 0a20  inition code... 
+000016f0: 2020 2020 2020 2052 656d 6f76 6520 616c         Remove al
+00001700: 6c20 7468 6520 656c 656d 656e 7420 7661  l the element va
+00001710: 6c75 6573 2e0a 0a20 2020 2020 2020 203a  lues...        :
+00001720: 7061 7261 6d20 6964 3a20 5468 6520 7265  param id: The re
+00001730: 736f 7572 6365 2049 442e 2052 6571 7569  source ID. Requi
+00001740: 7265 642e 0a20 2020 2020 2020 203a 7479  red..        :ty
+00001750: 7065 2069 643a 2073 7472 0a20 2020 2020  pe id: str.     
+00001760: 2020 203a 7061 7261 6d20 636f 6d6d 616e     :param comman
+00001770: 643a 2043 6f6d 6d61 6e64 2074 6f20 6465  d: Command to de
+00001780: 6c65 7465 2061 6e20 656c 656d 656e 742e  lete an element.
+00001790: 2052 6571 7569 7265 642e 0a20 2020 2020   Required..     
+000017a0: 2020 203a 7479 7065 2063 6f6d 6d61 6e64     :type command
+000017b0: 3a20 7e6b 7566 6c6f 772e 7265 7374 2e6d  : ~kuflow.rest.m
+000017c0: 6f64 656c 732e 5072 6f63 6573 7344 656c  odels.ProcessDel
+000017d0: 6574 6545 6c65 6d65 6e74 436f 6d6d 616e  eteElementComman
+000017e0: 640a 2020 2020 2020 2020 3a72 6574 7572  d.        :retur
+000017f0: 6e3a 2050 726f 6365 7373 0a20 2020 2020  n: Process.     
+00001800: 2020 203a 7274 7970 653a 207e 6b75 666c     :rtype: ~kufl
+00001810: 6f77 2e72 6573 742e 6d6f 6465 6c73 2e50  ow.rest.models.P
+00001820: 726f 6365 7373 0a20 2020 2020 2020 203a  rocess.        :
+00001830: 7261 6973 6573 207e 617a 7572 652e 636f  raises ~azure.co
+00001840: 7265 2e65 7863 6570 7469 6f6e 732e 4874  re.exceptions.Ht
+00001850: 7470 5265 7370 6f6e 7365 4572 726f 723a  tpResponseError:
+00001860: 0a20 2020 2020 2020 2072 1f00 0000 2903  .        r....).
+00001870: 720b 0000 0072 1800 0000 da1e 6163 7469  r....r......acti
+00001880: 6f6e 735f 7072 6f63 6573 735f 6465 6c65  ons_process_dele
+00001890: 7465 5f65 6c65 6d65 6e74 7221 0000 0072  te_elementr!...r
+000018a0: 0d00 0000 720d 0000 0072 0e00 0000 7223  ....r....r....r#
+000018b0: 0000 009d 0000 0073 0200 0000 0011 7a30  .......s......z0
+000018c0: 5072 6f63 6573 734f 7065 7261 7469 6f6e  ProcessOperation
+000018d0: 732e 6163 7469 6f6e 735f 7072 6f63 6573  s.actions_proces
+000018e0: 735f 6465 6c65 7465 5f65 6c65 6d65 6e74  s_delete_element
+000018f0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00001900: 0004 0000 004b 0000 0073 1800 0000 7c00  .....K...s....|.
+00001910: 6a00 6a01 6a02 6600 6401 7c01 6901 7c02  j.j.j.f.d.|.i.|.
+00001920: 9702 8e01 5300 2902 6168 0100 0043 6f6d  ....S.).ah...Com
+00001930: 706c 6574 6520 6120 5072 6f63 6573 732e  plete a Process.
+00001940: 0a0a 2020 2020 2020 2020 436f 6d70 6c65  ..        Comple
+00001950: 7465 2061 2050 726f 6365 7373 2e20 5468  te a Process. Th
+00001960: 6520 7374 6174 6520 6f66 2050 726f 6365  e state of Proce
+00001970: 7373 2069 7320 7365 7420 746f 2027 636f  ss is set to 'co
+00001980: 6d70 6c65 7465 6427 2e0a 0a20 2020 2020  mpleted'...     
+00001990: 2020 2049 6620 796f 7520 6172 6520 616c     If you are al
+000019a0: 7265 6164 7920 696e 2074 6869 7320 7374  ready in this st
+000019b0: 6174 652c 206e 6f20 6163 7469 6f6e 2069  ate, no action i
+000019c0: 7320 7461 6b65 6e2e 0a0a 2020 2020 2020  s taken...      
+000019d0: 2020 3a70 6172 616d 2069 643a 2054 6865    :param id: The
+000019e0: 2072 6573 6f75 7263 6520 4944 2e20 5265   resource ID. Re
+000019f0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+00001a00: 3a74 7970 6520 6964 3a20 7374 720a 2020  :type id: str.  
+00001a10: 2020 2020 2020 3a72 6574 7572 6e3a 2050        :return: P
+00001a20: 726f 6365 7373 0a20 2020 2020 2020 203a  rocess.        :
+00001a30: 7274 7970 653a 207e 6b75 666c 6f77 2e72  rtype: ~kuflow.r
+00001a40: 6573 742e 6d6f 6465 6c73 2e50 726f 6365  est.models.Proce
+00001a50: 7373 0a20 2020 2020 2020 203a 7261 6973  ss.        :rais
+00001a60: 6573 207e 617a 7572 652e 636f 7265 2e65  es ~azure.core.e
+00001a70: 7863 6570 7469 6f6e 732e 4874 7470 5265  xceptions.HttpRe
+00001a80: 7370 6f6e 7365 4572 726f 723a 0a20 2020  sponseError:.   
+00001a90: 2020 2020 2072 1b00 0000 2903 720b 0000       r....).r...
+00001aa0: 0072 1800 0000 da18 6163 7469 6f6e 735f  .r......actions_
+00001ab0: 7072 6f63 6573 735f 636f 6d70 6c65 7465  process_complete
+00001ac0: 721d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00001ad0: 0e00 0000 7224 0000 00b0 0000 0073 0200  ....r$.......s..
+00001ae0: 0000 000d 7a2a 5072 6f63 6573 734f 7065  ....z*ProcessOpe
+00001af0: 7261 7469 6f6e 732e 6163 7469 6f6e 735f  rations.actions_
+00001b00: 7072 6f63 6573 735f 636f 6d70 6c65 7465  process_complete
+00001b10: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00001b20: 0004 0000 004b 0000 0073 1800 0000 7c00  .....K...s....|.
+00001b30: 6a00 6a01 6a02 6600 6401 7c01 6901 7c02  j.j.j.f.d.|.i.|.
+00001b40: 9702 8e01 5300 2902 61a0 0100 0043 616e  ....S.).a....Can
+00001b50: 6365 6c20 6120 5072 6f63 6573 732e 0a0a  cel a Process...
+00001b60: 2020 2020 2020 2020 4361 6e63 656c 2061          Cancel a
+00001b70: 2050 726f 6365 7373 2e20 5468 6520 5072   Process. The Pr
+00001b80: 6f63 6573 7320 7374 6174 6520 6973 2073  ocess state is s
+00001b90: 6574 2074 6f20 2763 616e 6365 6c6c 6564  et to 'cancelled
+00001ba0: 272e 0a0a 2020 2020 2020 2020 416c 6c20  '...        All 
+00001bb0: 7468 6520 6163 7469 7665 2074 6173 6b73  the active tasks
+00001bc0: 2077 696c 6c20 6265 206d 6172 6b65 6420   will be marked 
+00001bd0: 6173 2063 616e 6365 6c6c 6564 2074 6f6f  as cancelled too
+00001be0: 2e0a 0a20 2020 2020 2020 2049 6620 796f  ...        If yo
+00001bf0: 7520 6172 6520 616c 7265 6164 7920 696e  u are already in
+00001c00: 2074 6869 7320 7374 6174 652c 206e 6f20   this state, no 
+00001c10: 6163 7469 6f6e 2069 7320 7461 6b65 6e2e  action is taken.
+00001c20: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001c30: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
+00001c40: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
+00001c50: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
+00001c60: 3a20 7374 720a 2020 2020 2020 2020 3a72  : str.        :r
+00001c70: 6574 7572 6e3a 2050 726f 6365 7373 0a20  eturn: Process. 
+00001c80: 2020 2020 2020 203a 7274 7970 653a 207e         :rtype: ~
+00001c90: 6b75 666c 6f77 2e72 6573 742e 6d6f 6465  kuflow.rest.mode
+00001ca0: 6c73 2e50 726f 6365 7373 0a20 2020 2020  ls.Process.     
+00001cb0: 2020 203a 7261 6973 6573 207e 617a 7572     :raises ~azur
+00001cc0: 652e 636f 7265 2e65 7863 6570 7469 6f6e  e.core.exception
+00001cd0: 732e 4874 7470 5265 7370 6f6e 7365 4572  s.HttpResponseEr
+00001ce0: 726f 723a 0a20 2020 2020 2020 2072 1b00  ror:.        r..
+00001cf0: 0000 2903 720b 0000 0072 1800 0000 da16  ..).r....r......
+00001d00: 6163 7469 6f6e 735f 7072 6f63 6573 735f  actions_process_
+00001d10: 6361 6e63 656c 721d 0000 0072 0d00 0000  cancelr....r....
+00001d20: 720d 0000 0072 0e00 0000 7225 0000 00bf  r....r....r%....
+00001d30: 0000 0073 0200 0000 000f 7a28 5072 6f63  ...s......z(Proc
+00001d40: 6573 734f 7065 7261 7469 6f6e 732e 6163  essOperations.ac
+00001d50: 7469 6f6e 735f 7072 6f63 6573 735f 6361  tions_process_ca
+00001d60: 6e63 656c 2905 721b 0000 00da 0466 696c  ncel).r......fil
+00001d70: 6572 1e00 0000 7214 0000 0072 1500 0000  er....r....r....
+00001d80: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
+00001d90: 0008 0000 004b 0000 0073 2800 0000 7c00  .....K...s(...|.
+00001da0: 6a00 6a01 6a02 6600 7c01 7c02 6a03 7c02  j.j.j.f.|.|.j.|.
+00001db0: 6a04 7c02 6a05 7c03 6a06 6401 9c05 7c04  j.|.j.|.j.d...|.
+00001dc0: 9702 8e01 5300 2902 6122 0200 0055 706c  ....S.).a"...Upl
+00001dd0: 6f61 6420 616e 6420 7361 7665 2061 2064  oad and save a d
+00001de0: 6f63 756d 656e 7420 696e 2061 2075 7365  ocument in a use
+00001df0: 7220 6163 7469 6f6e 2e0a 0a20 2020 2020  r action...     
+00001e00: 2020 2041 6c6c 6f77 2073 6176 696e 6720     Allow saving 
+00001e10: 6120 7573 6572 2061 6374 696f 6e20 646f  a user action do
+00001e20: 6375 6d65 6e74 2075 706c 6f61 6469 6e67  cument uploading
+00001e30: 2074 6865 2063 6f6e 7465 6e74 2e0a 0a20   the content... 
+00001e40: 2020 2020 2020 203a 7061 7261 6d20 6964         :param id
+00001e50: 3a20 5468 6520 7265 736f 7572 6365 2049  : The resource I
+00001e60: 442e 2052 6571 7569 7265 642e 0a20 2020  D. Required..   
+00001e70: 2020 2020 203a 7479 7065 2069 643a 2073       :type id: s
+00001e80: 7472 0a20 2020 2020 2020 203a 7061 7261  tr.        :para
+00001e90: 6d20 6669 6c65 3a20 446f 6375 6d65 6e74  m file: Document
+00001ea0: 2074 6f20 7361 7665 2e20 5265 7175 6972   to save. Requir
+00001eb0: 6564 2e0a 2020 2020 2020 2020 3a74 7970  ed..        :typ
+00001ec0: 6520 6669 6c65 3a20 5f6d 6f64 656c 732e  e file: _models.
+00001ed0: 446f 6375 6d65 6e74 0a20 2020 2020 2020  Document.       
+00001ee0: 203a 6b65 7977 6f72 6420 636f 6d6d 616e   :keyword comman
+00001ef0: 643a 2055 7365 7220 6163 7469 6f6e 2069  d: User action i
+00001f00: 6e66 6f2e 2052 6571 7569 7265 642e 0a20  nfo. Required.. 
+00001f10: 2020 2020 2020 203a 7479 7065 2063 6f6d         :type com
+00001f20: 6d61 6e64 3a20 5f6d 6f64 656c 732e 5072  mand: _models.Pr
+00001f30: 6f63 6573 7353 6176 6555 7365 7241 6374  ocessSaveUserAct
+00001f40: 696f 6e56 616c 7565 446f 6375 6d65 6e74  ionValueDocument
+00001f50: 436f 6d6d 616e 640a 2020 2020 2020 2020  Command.        
+00001f60: 3a72 6574 7572 6e3a 2050 726f 6365 7373  :return: Process
+00001f70: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+00001f80: 203a 7274 7970 653a 207e 6b75 666c 6f77   :rtype: ~kuflow
+00001f90: 2e72 6573 742e 6d6f 6465 6c73 2e50 726f  .rest.models.Pro
+00001fa0: 6365 7373 206f 7220 4e6f 6e65 0a20 2020  cess or None.   
+00001fb0: 2020 2020 203a 7261 6973 6573 207e 617a       :raises ~az
+00001fc0: 7572 652e 636f 7265 2e65 7863 6570 7469  ure.core.excepti
+00001fd0: 6f6e 732e 4874 7470 5265 7370 6f6e 7365  ons.HttpResponse
+00001fe0: 4572 726f 723a 0a20 2020 2020 2020 2029  Error:.        )
+00001ff0: 0572 1b00 0000 7226 0000 00da 1166 696c  .r....r&.....fil
+00002000: 655f 636f 6e74 656e 745f 7479 7065 da09  e_content_type..
+00002010: 6669 6c65 5f6e 616d 65da 1475 7365 725f  file_name..user_
+00002020: 6163 7469 6f6e 5f76 616c 7565 5f69 6429  action_value_id)
+00002030: 0772 0b00 0000 7218 0000 00da 2f61 6374  .r....r...../act
+00002040: 696f 6e73 5f70 726f 6365 7373 5f73 6176  ions_process_sav
+00002050: 655f 7573 6572 5f61 6374 696f 6e5f 7661  e_user_action_va
+00002060: 6c75 655f 646f 6375 6d65 6e74 5a0c 6669  lue_documentZ.fi
+00002070: 6c65 5f63 6f6e 7465 6e74 da0c 636f 6e74  le_content..cont
+00002080: 656e 745f 7479 7065 5a09 6669 6c65 5f6d  ent_typeZ.file_m
+00002090: 616d 6572 2900 0000 2905 720c 0000 0072  amer)...).r....r
+000020a0: 1b00 0000 7226 0000 0072 1e00 0000 7214  ....r&...r....r.
+000020b0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000020c0: 0000 722a 0000 00d0 0000 0073 1200 0000  ..r*.......s....
+000020d0: 0011 0a01 0201 0401 0401 0401 04fb 0406  ................
+000020e0: 02fa 7a41 5072 6f63 6573 734f 7065 7261  ..zAProcessOpera
+000020f0: 7469 6f6e 732e 6163 7469 6f6e 735f 7072  tions.actions_pr
+00002100: 6f63 6573 735f 7361 7665 5f75 7365 725f  ocess_save_user_
+00002110: 6163 7469 6f6e 5f76 616c 7565 5f64 6f63  action_value_doc
+00002120: 756d 656e 7429 0372 1000 0000 7201 0000  ument).r....r...
+00002130: 004e 291d da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
+00002140: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00002150: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00002160: 5fda 194b 7546 6c6f 7752 6573 7443 6c69  _..KuFlowRestCli
+00002170: 656e 7447 656e 6572 6174 6564 720f 0000  entGeneratedr...
+00002180: 00da 0369 6e74 7204 0000 0072 0500 0000  ...intr....r....
+00002190: 7217 0000 0072 0300 0000 7202 0000 00da  r....r....r.....
+000021a0: 075f 6d6f 6465 6c73 da0b 5072 6f63 6573  ._models..Proces
+000021b0: 7350 6167 6572 1900 0000 da07 5072 6f63  sPager......Proc
+000021c0: 6573 7372 1a00 0000 721c 0000 00da 1d50  essr....r......P
+000021d0: 726f 6365 7373 4368 616e 6765 496e 6974  rocessChangeInit
+000021e0: 6961 746f 7243 6f6d 6d61 6e64 7220 0000  iatorCommandr ..
+000021f0: 00da 1950 726f 6365 7373 5361 7665 456c  ...ProcessSaveEl
+00002200: 656d 656e 7443 6f6d 6d61 6e64 7222 0000  ementCommandr"..
+00002210: 00da 1b50 726f 6365 7373 4465 6c65 7465  ...ProcessDelete
+00002220: 456c 656d 656e 7443 6f6d 6d61 6e64 7223  ElementCommandr#
+00002230: 0000 0072 2400 0000 7225 0000 005a 0844  ...r$...r%...Z.D
+00002240: 6f63 756d 656e 745a 2950 726f 6365 7373  ocumentZ)Process
+00002250: 5361 7665 5573 6572 4163 7469 6f6e 5661  SaveUserActionVa
+00002260: 6c75 6544 6f63 756d 656e 7443 6f6d 6d61  lueDocumentComma
+00002270: 6e64 722a 0000 0072 0d00 0000 720d 0000  ndr*...r....r...
+00002280: 0072 0d00 0000 720e 0000 0072 0900 0000  .r....r....r....
+00002290: 2100 0000 734a 0000 0008 0104 090e 0400  !...sJ..........
+000022a0: 0000 0000 ff02 0102 0002 0012 0002 0104  ................
+000022b0: fe0c 1d16 1914 0e02 0004 0002 0104 fe0c  ................
+000022c0: 1602 0004 0002 0104 fe0c 1802 0004 0002  ................
+000022d0: 0104 fe0c 1314 0f14 1202 0004 0004 0002  ................
+000022e0: 0108 fe72 0900 0000 4e29 0cda 0674 7970  ...r....N)...typ
+000022f0: 696e 6772 0200 0000 7203 0000 0072 0400  ingr....r....r..
+00002300: 0000 7205 0000 00da 0a5f 6765 6e65 7261  ..r......_genera
+00002310: 7465 6472 0700 0000 7230 0000 00da 0072  tedr....r0.....r
+00002320: 0800 0000 7232 0000 0072 0900 0000 720d  ....r2...r....r.
+00002330: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00002340: 0000 da08 3c6d 6f64 756c 653e 1a00 0000  ....<module>....
+00002350: 7306 0000 0018 020c 020c 03              s..........
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 17441 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 2144 0000  U........<.d!D..
+00000000: 550d 0d0a 0000 0000 9c24 8c64 1044 0000  U........$.d.D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6402 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6402 6404 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a0c  ..G.d.d...d...Z.
 00000070: 6407 5300 2908 e900 0000 0029 05da 0341  d.S.)......)...A
@@ -58,963 +58,962 @@
 00000390: 6e74 2e4b 7546 6c6f 7752 6573 7443 6c69  nt.KuFlowRestCli
 000003a0: 656e 7460 2773 0a20 2020 2020 2020 203a  ent`'s.        :
 000003b0: 6174 7472 3a60 7461 736b 6020 6174 7472  attr:`task` attr
 000003c0: 6962 7574 652e 0a20 2020 2029 01da 0d6b  ibute..    )...k
 000003d0: 7566 6c6f 775f 636c 6965 6e74 6302 0000  uflow_clientc...
 000003e0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
 000003f0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
-00000400: 6400 5300 2901 4e29 01da 1e5f 5461 736b  d.S.).N)..._Task
-00000410: 4f70 6572 6174 696f 6e73 5f5f 6b75 666c  Operations__kufl
-00000420: 6f77 5f63 6c69 656e 7429 02da 0473 656c  ow_client)...sel
-00000430: 6672 0b00 0000 a900 720e 0000 00fa 4e2f  fr......r.....N/
-00000440: 776f 726b 2f6b 7566 6c6f 772d 7364 6b2d  work/kuflow-sdk-
-00000450: 7079 7468 6f6e 2f6b 7566 6c6f 772d 7265  python/kuflow-re
-00000460: 7374 2f6b 7566 6c6f 775f 7265 7374 2f6f  st/kuflow_rest/o
-00000470: 7065 7261 7469 6f6e 732f 5f74 6173 6b5f  perations/_task_
-00000480: 6f70 6572 6174 696f 6e73 2e70 79da 085f  operations.py.._
-00000490: 5f69 6e69 745f 5f2c 0000 0073 0200 0000  _init__,...s....
-000004a0: 0001 7a17 5461 736b 4f70 6572 6174 696f  ..z.TaskOperatio
-000004b0: 6e73 2e5f 5f69 6e69 745f 5fe9 1900 0000  ns.__init__.....
-000004c0: 7201 0000 004e 2908 da04 7369 7a65 da04  r....N)...size..
-000004d0: 7061 6765 da04 736f 7274 da0a 7072 6f63  page..sort..proc
-000004e0: 6573 735f 6964 da05 7374 6174 65da 1474  ess_id..state..t
-000004f0: 6173 6b5f 6465 6669 6e69 7469 6f6e 5f63  ask_definition_c
-00000500: 6f64 65da 066b 7761 7267 73da 0672 6574  ode..kwargs..ret
-00000510: 7572 6e63 0700 0000 0000 0000 0000 0000  urnc............
-00000520: 0800 0000 0900 0000 4b00 0000 7384 0000  ........K...s...
-00000530: 007c 0364 016b 0972 1874 007c 0374 0183  .|.d.k.r.t.|.t..
-00000540: 0272 187c 0367 017d 037c 0464 016b 0972  .r.|.g.}.|.d.k.r
-00000550: 3074 007c 0474 0183 0272 307c 0467 017d  0t.|.t...r0|.g.}
-00000560: 047c 0564 016b 0972 4a74 007c 0574 026a  .|.d.k.rJt.|.t.j
-00000570: 0383 0272 4a7c 0567 017d 057c 0664 016b  ...rJ|.g.}.|.d.k
-00000580: 0972 6274 007c 0674 0183 0272 627c 0667  .rbt.|.t...rb|.g
-00000590: 017d 067c 006a 046a 056a 0666 007c 017c  .}.|.j.j.j.f.|.|
-000005a0: 027c 037c 047c 057c 0664 029c 067c 0797  .|.|.|.|.d...|..
-000005b0: 028e 0153 0029 0361 8405 0000 4669 6e64  ...S.).a....Find
-000005c0: 2061 6c6c 2061 6363 6573 7369 626c 6520   all accessible 
-000005d0: 5461 736b 732e 0a0a 2020 2020 2020 2020  Tasks...        
-000005e0: 4c69 7374 2061 6c6c 2054 6173 6b73 2074  List all Tasks t
-000005f0: 6861 7420 6861 7665 2062 6565 6e20 6372  hat have been cr
-00000600: 6561 7465 6420 616e 6420 7468 6520 6372  eated and the cr
-00000610: 6564 656e 7469 616c 7320 6861 7320 6163  edentials has ac
-00000620: 6365 7373 2e0a 0a20 2020 2020 2020 2041  cess...        A
-00000630: 7661 696c 6162 6c65 2073 6f72 7420 7175  vailable sort qu
-00000640: 6572 7920 7661 6c75 6573 3a20 6964 2c20  ery values: id, 
-00000650: 6372 6561 7465 6441 742c 206c 6173 744d  createdAt, lastM
-00000660: 6f64 6966 6965 6441 742c 2063 6c61 696d  odifiedAt, claim
-00000670: 6564 4174 2c20 636f 6d70 6c65 7465 6441  edAt, completedA
-00000680: 742c 0a20 2020 2020 2020 2063 616e 6365  t,.        cance
-00000690: 6c6c 6564 4174 2e0a 0a20 2020 2020 2020  lledAt...       
-000006a0: 203a 6b65 7977 6f72 6420 7369 7a65 3a20   :keyword size: 
-000006b0: 5468 6520 6e75 6d62 6572 206f 6620 7265  The number of re
-000006c0: 636f 7264 7320 7265 7475 726e 6564 2077  cords returned w
-000006d0: 6974 6869 6e20 6120 7369 6e67 6c65 2041  ithin a single A
-000006e0: 5049 2063 616c 6c2e 2044 6566 6175 6c74  PI call. Default
-000006f0: 2076 616c 7565 2069 7320 3235 2e0a 2020   value is 25..  
-00000700: 2020 2020 2020 3a74 7970 6520 7369 7a65        :type size
-00000710: 3a20 696e 740a 2020 2020 2020 2020 3a6b  : int.        :k
-00000720: 6579 776f 7264 2070 6167 653a 2054 6865  eyword page: The
-00000730: 2070 6167 6520 6e75 6d62 6572 206f 6620   page number of 
-00000740: 7468 6520 6375 7272 656e 7420 7061 6765  the current page
-00000750: 2069 6e20 7468 6520 7265 7475 726e 6564   in the returned
-00000760: 2072 6563 6f72 6473 2c20 3020 6973 2074   records, 0 is t
-00000770: 6865 2066 6972 7374 2070 6167 652e 0a20  he first page.. 
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2020 2020 4465 6661 756c 7420 7661        Default va
-000007a0: 6c75 6520 6973 2030 2e0a 2020 2020 2020  lue is 0..      
-000007b0: 2020 3a74 7970 6520 7061 6765 3a20 696e    :type page: in
-000007c0: 740a 2020 2020 2020 2020 3a6b 6579 776f  t.        :keywo
-000007d0: 7264 2073 6f72 743a 2053 6f72 7469 6e67  rd sort: Sorting
-000007e0: 2063 7269 7465 7269 6120 696e 2074 6865   criteria in the
-000007f0: 2066 6f72 6d61 743a 2070 726f 7065 7274   format: propert
-00000800: 797b 2c61 7363 7c64 6573 637d 2e20 4578  y{,asc|desc}. Ex
-00000810: 616d 706c 653a 2063 7265 6174 6564 4174  ample: createdAt
-00000820: 2c64 6573 630a 2020 2020 2020 2020 2020  ,desc.          
-00000830: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00000840: 6175 6c74 2073 6f72 7420 6f72 6465 7220  ault sort order 
-00000850: 6973 2061 7363 656e 6469 6e67 2e20 4d75  is ascending. Mu
-00000860: 6c74 6970 6c65 2073 6f72 7420 6372 6974  ltiple sort crit
-00000870: 6572 6961 2061 7265 2073 7570 706f 7274  eria are support
-00000880: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00000890: 2020 2020 2020 2020 2020 2050 6c65 6173             Pleas
-000008a0: 6520 7265 6665 7220 746f 2074 6865 206d  e refer to the m
-000008b0: 6574 686f 6420 6465 7363 7269 7074 696f  ethod descriptio
-000008c0: 6e20 666f 7220 7375 7070 6f72 7465 6420  n for supported 
-000008d0: 7072 6f70 6572 7469 6573 2e20 4465 6661  properties. Defa
-000008e0: 756c 7420 7661 6c75 6520 6973 204e 6f6e  ult value is Non
-000008f0: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-00000900: 2073 6f72 743a 206c 6973 745b 7374 725d   sort: list[str]
-00000910: 0a20 2020 2020 2020 203a 6b65 7977 6f72  .        :keywor
-00000920: 6420 7072 6f63 6573 735f 6964 3a20 4669  d process_id: Fi
-00000930: 6c74 6572 2062 7920 616e 2061 7272 6179  lter by an array
-00000940: 206f 6620 7072 6f63 6573 7320 6964 732e   of process ids.
-00000950: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
-00000960: 7320 4e6f 6e65 2e0a 2020 2020 2020 2020  s None..        
-00000970: 3a74 7970 6520 7072 6f63 6573 735f 6964  :type process_id
-00000980: 3a20 6c69 7374 5b73 7472 5d0a 2020 2020  : list[str].    
-00000990: 2020 2020 3a6b 6579 776f 7264 2073 7461      :keyword sta
-000009a0: 7465 3a20 4669 6c74 6572 2062 7920 616e  te: Filter by an
-000009b0: 2061 7272 6179 206f 6620 7461 736b 2073   array of task s
-000009c0: 7461 7465 732e 2044 6566 6175 6c74 2076  tates. Default v
-000009d0: 616c 7565 2069 7320 4e6f 6e65 2e0a 2020  alue is None..  
-000009e0: 2020 2020 2020 3a74 7970 6520 7374 6174        :type stat
-000009f0: 653a 206c 6973 745b 7374 7220 6f72 207e  e: list[str or ~
-00000a00: 6b75 666c 6f77 2e72 6573 742e 6d6f 6465  kuflow.rest.mode
-00000a10: 6c73 2e54 6173 6b53 7461 7465 5d0a 2020  ls.TaskState].  
-00000a20: 2020 2020 2020 3a6b 6579 776f 7264 2074        :keyword t
-00000a30: 6173 6b5f 6465 6669 6e69 7469 6f6e 5f63  ask_definition_c
-00000a40: 6f64 653a 2046 696c 7465 7220 6279 2061  ode: Filter by a
-00000a50: 6e20 6172 7261 7920 6f66 2074 6173 6b20  n array of task 
-00000a60: 6465 6669 6e69 7469 6f6e 2063 6f64 6573  definition codes
-00000a70: 2e20 4465 6661 756c 7420 7661 6c75 6520  . Default value 
-00000a80: 6973 204e 6f6e 652e 0a20 2020 2020 2020  is None..       
-00000a90: 203a 7479 7065 2074 6173 6b5f 6465 6669   :type task_defi
-00000aa0: 6e69 7469 6f6e 5f63 6f64 653a 206c 6973  nition_code: lis
-00000ab0: 745b 7374 725d 0a20 2020 2020 2020 203a  t[str].        :
-00000ac0: 7265 7475 726e 3a20 5461 736b 5061 6765  return: TaskPage
-00000ad0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00000ae0: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
-00000af0: 6465 6c73 2e54 6173 6b50 6167 650a 2020  dels.TaskPage.  
-00000b00: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
-00000b10: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
-00000b20: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
-00000b30: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-00000b40: 4e29 0672 1200 0000 7213 0000 0072 1400  N).r....r....r..
-00000b50: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000b60: 0029 07da 0a69 7369 6e73 7461 6e63 65da  .)...isinstance.
-00000b70: 0373 7472 da07 5f6d 6f64 656c 73da 0954  .str.._models..T
-00000b80: 6173 6b53 7461 7465 720c 0000 00da 0474  askStater......t
-00000b90: 6173 6bda 0a66 696e 645f 7461 736b 7329  ask..find_tasks)
-00000ba0: 0872 0d00 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000bb0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000bc0: 1700 0000 7218 0000 0072 0e00 0000 720e  ....r....r....r.
-00000bd0: 0000 0072 0f00 0000 721f 0000 002f 0000  ...r....r..../..
-00000be0: 0073 2400 0000 0024 1201 0601 1201 0601  .s$....$........
-00000bf0: 1401 0601 1201 0602 0a01 0201 0201 0201  ................
-00000c00: 0201 0201 02fa 0407 02f9 7a19 5461 736b  ..........z.Task
-00000c10: 4f70 6572 6174 696f 6e73 2e66 696e 645f  Operations.find_
-00000c20: 7461 736b 7329 0472 1e00 0000 da0e 6163  tasks).r......ac
-00000c30: 7469 7669 7479 5f74 6f6b 656e 7218 0000  tivity_tokenr...
-00000c40: 0072 1900 0000 6303 0000 0000 0000 0000  .r....c.........
-00000c50: 0000 0004 0000 0005 0000 004b 0000 0073  ...........K...s
-00000c60: 1a00 0000 7c00 6a00 6a01 6a02 6600 7c01  ....|.j.j.j.f.|.
-00000c70: 7c02 6401 9c02 7c03 9702 8e01 5300 2902  |.d...|.....S.).
-00000c80: 61ba 0500 0043 7265 6174 6520 6120 6e65  a....Create a ne
-00000c90: 7720 5461 736b 2069 6e20 7468 6520 7365  w Task in the se
-00000ca0: 6c65 6374 6564 2050 726f 6365 7373 2e0a  lected Process..
-00000cb0: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
-00000cc0: 6120 5461 736b 2061 6e64 206f 7074 696f  a Task and optio
-00000cd0: 6e61 6c6c 7920 6669 6c6c 2069 7473 2065  nally fill its e
-00000ce0: 6c65 6d65 6e74 732e 2057 6520 6361 6e20  lements. We can 
-00000cf0: 6669 6c6c 2069 6e20 616e 7920 7479 7065  fill in any type
-00000d00: 206f 6620 656c 656d 656e 7420 6578 6365   of element exce
-00000d10: 7074 0a20 2020 2020 2020 2064 6f63 756d  pt.        docum
-00000d20: 656e 7473 2e0a 0a20 2020 2020 2020 2049  ents...        I
-00000d30: 6620 796f 7520 7761 6e74 2074 6f20 6164  f you want to ad
-00000d40: 6420 646f 6375 6d65 6e74 2074 7970 6520  d document type 
-00000d50: 656c 656d 656e 7473 2c20 796f 7520 6361  elements, you ca
-00000d60: 6e20 7061 7373 2061 2072 6566 6572 656e  n pass a referen
-00000d70: 6365 2074 6f20 616e 2065 7869 7374 696e  ce to an existin
-00000d80: 6720 646f 6375 6d65 6e74 0a20 2020 2020  g document.     
-00000d90: 2020 2074 7970 6520 656c 656d 656e 7420     type element 
-00000da0: 696e 6469 6361 7469 6e67 2069 7473 2027  indicating its '
-00000db0: 7572 6927 2e20 5468 6973 2077 696c 6c20  uri'. This will 
-00000dc0: 636f 7079 2074 6861 7420 646f 6375 6d65  copy that docume
-00000dd0: 6e74 2069 6e74 6f20 7468 6520 656c 656d  nt into the elem
-00000de0: 656e 742e 2049 6e20 6361 7365 2079 6f75  ent. In case you
-00000df0: 0a20 2020 2020 2020 2077 616e 7420 746f  .        want to
-00000e00: 2061 6464 2061 206e 6577 2064 6f63 756d   add a new docum
-00000e10: 656e 742c 2070 6c65 6173 6520 7573 6520  ent, please use 
-00000e20: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
-00000e30: 6720 4150 4920 6d65 7468 6f64 2e0a 0a20  g API method... 
-00000e40: 2020 2020 2020 2049 6620 796f 7520 7761         If you wa
-00000e50: 6e74 2074 6861 7420 7468 6520 7461 736b  nt that the task
-00000e60: 2063 7265 6174 6564 2069 7320 636c 6169   created is clai
-00000e70: 6d65 6420 796f 7520 6361 6e20 6120 7661  med you can a va
-00000e80: 6c69 6420 6f77 6e65 7220 7573 696e 6720  lid owner using 
-00000e90: 7468 6520 666f 6c6c 6f77 696e 6720 6f70  the following op
-00000ea0: 7469 6f6e 733a 0a0a 0a20 2020 2020 2020  tions:...       
-00000eb0: 202a 2049 6620 796f 7520 6b6e 6f77 2074   * If you know t
-00000ec0: 6865 2060 6070 7269 6e63 6970 616c 2049  he ``principal I
-00000ed0: 4460 6020 796f 7520 6361 6e20 6173 7369  D`` you can assi
-00000ee0: 676e 2069 7420 746f 2060 606f 776e 6572  gn it to ``owner
-00000ef0: 2e69 6460 600a 2020 2020 2020 2020 2a20  .id``.        * 
-00000f00: 4966 2079 6f75 206b 6e6f 7720 7468 6520  If you know the 
-00000f10: 6060 7573 6572 2049 4460 6020 796f 7520  ``user ID`` you 
-00000f20: 6361 6e20 6173 7369 676e 2069 7420 746f  can assign it to
-00000f30: 2060 606f 776e 6572 2e75 7365 722e 6964   ``owner.user.id
-00000f40: 6060 0a20 2020 2020 2020 202a 2049 6620  ``.        * If 
-00000f50: 796f 7520 6b6e 6f77 2074 6865 2060 6075  you know the ``u
-00000f60: 7365 7220 656d 6169 6c60 6020 796f 7520  ser email`` you 
-00000f70: 6361 6e20 6173 7369 676e 2069 7420 746f  can assign it to
-00000f80: 2060 606f 776e 6572 2e75 7365 722e 656d   ``owner.user.em
-00000f90: 6169 6c60 600a 2020 2020 2020 2020 2a20  ail``.        * 
-00000fa0: 4966 2079 6f75 206b 6e6f 7720 7468 6520  If you know the 
-00000fb0: 6060 6170 706c 6963 6174 696f 6e20 4944  ``application ID
-00000fc0: 6060 2079 6f75 2063 616e 2061 7373 6967  `` you can assig
-00000fd0: 6e20 6974 2074 6f20 6060 6f77 6e65 722e  n it to ``owner.
-00000fe0: 6170 706c 6963 6174 696f 6e2e 6964 6060  application.id``
-00000ff0: 0a0a 2020 2020 2020 2020 4966 2079 6f75  ..        If you
-00001000: 2077 616e 7420 7468 6520 6d65 7468 6f64   want the method
-00001010: 2074 6f20 6265 2069 6465 6d70 6f74 656e   to be idempoten
-00001020: 742c 2070 6c65 6173 6520 7370 6563 6966  t, please specif
-00001030: 7920 7468 6520 6060 6964 6060 2066 6965  y the ``id`` fie
-00001040: 6c64 2069 6e20 7468 6520 7265 7175 6573  ld in the reques
-00001050: 7420 626f 6479 2e0a 0a20 2020 2020 2020  t body...       
-00001060: 203a 7061 7261 6d20 7461 736b 3a20 5461   :param task: Ta
-00001070: 736b 2074 6f20 6265 2063 7265 6174 6564  sk to be created
-00001080: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
-00001090: 2020 2020 3a74 7970 6520 7461 736b 3a20      :type task: 
-000010a0: 7e6b 7566 6c6f 772e 7265 7374 2e6d 6f64  ~kuflow.rest.mod
-000010b0: 656c 732e 5461 736b 0a20 2020 2020 2020  els.Task.       
-000010c0: 203a 6b65 7977 6f72 6420 6163 7469 7669   :keyword activi
-000010d0: 7479 5f74 6f6b 656e 3a20 5768 656e 2063  ty_token: When c
-000010e0: 7265 6174 6520 6120 4b75 666c 6f77 2054  reate a Kuflow T
-000010f0: 6173 6b20 6261 636b 6564 2077 6974 6820  ask backed with 
-00001100: 6120 5465 6d70 6f72 616c 2e69 6f20 7365  a Temporal.io se
-00001110: 7276 6572 732c 2074 6869 730a 2020 2020  rvers, this.    
-00001120: 2020 2020 2076 616c 7565 2069 7320 7265       value is re
-00001130: 7175 6972 6564 2061 6e64 206d 7573 7420  quired and must 
-00001140: 6265 2073 6574 2077 6974 6820 7468 6520  be set with the 
-00001150: 636f 6e74 6578 7420 7461 736b 2074 6f6b  context task tok
-00001160: 656e 206f 6620 5465 6d70 6f72 616c 2e69  en of Temporal.i
-00001170: 6f20 6163 7469 7669 7479 2e20 4465 6661  o activity. Defa
-00001180: 756c 740a 2020 2020 2020 2020 2076 616c  ult.         val
-00001190: 7565 2069 7320 4e6f 6e65 2e0a 2020 2020  ue is None..    
-000011a0: 2020 2020 3a74 7970 6520 6163 7469 7669      :type activi
-000011b0: 7479 5f74 6f6b 656e 3a20 7374 720a 2020  ty_token: str.  
-000011c0: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
-000011d0: 6173 6b0a 2020 2020 2020 2020 3a72 7479  ask.        :rty
-000011e0: 7065 3a20 7e6b 7566 6c6f 772e 7265 7374  pe: ~kuflow.rest
-000011f0: 2e6d 6f64 656c 732e 5461 736b 0a20 2020  .models.Task.   
-00001200: 2020 2020 203a 7261 6973 6573 207e 617a       :raises ~az
-00001210: 7572 652e 636f 7265 2e65 7863 6570 7469  ure.core.excepti
-00001220: 6f6e 732e 4874 7470 5265 7370 6f6e 7365  ons.HttpResponse
-00001230: 4572 726f 723a 0a20 2020 2020 2020 2029  Error:.        )
-00001240: 0272 1e00 0000 7220 0000 0029 0372 0c00  .r....r ...).r..
-00001250: 0000 721e 0000 00da 0b63 7265 6174 655f  ..r......create_
-00001260: 7461 736b 2904 720d 0000 0072 1e00 0000  task).r....r....
-00001270: 7220 0000 0072 1800 0000 720e 0000 0072  r ...r....r....r
-00001280: 0e00 0000 720f 0000 0072 2100 0000 6600  ....r....r!...f.
-00001290: 0000 7302 0000 0000 1e7a 1a54 6173 6b4f  ..s......z.TaskO
-000012a0: 7065 7261 7469 6f6e 732e 6372 6561 7465  perations.create
-000012b0: 5f74 6173 6b29 03da 0269 6472 1800 0000  _task)...idr....
-000012c0: 7219 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000012d0: 0000 0300 0000 0400 0000 4b00 0000 7318  ..........K...s.
-000012e0: 0000 007c 006a 006a 016a 0266 0064 017c  ...|.j.j.j.f.d.|
-000012f0: 0169 017c 0297 028e 0153 0029 0261 0201  .i.|.....S.).a..
-00001300: 0000 4765 7420 6120 7461 736b 2067 6976  ..Get a task giv
-00001310: 656e 2069 7420 4944 2e0a 0a20 2020 2020  en it ID...     
-00001320: 2020 2041 6c6c 6f77 2074 6f20 6765 7420     Allow to get 
-00001330: 6120 7461 736b 2062 7920 4944 2e0a 0a20  a task by ID... 
-00001340: 2020 2020 2020 203a 7061 7261 6d20 6964         :param id
-00001350: 3a20 5468 6520 7265 736f 7572 6365 2049  : The resource I
-00001360: 442e 2052 6571 7569 7265 642e 0a20 2020  D. Required..   
-00001370: 2020 2020 203a 7479 7065 2069 643a 2073       :type id: s
-00001380: 7472 0a20 2020 2020 2020 203a 7265 7475  tr.        :retu
-00001390: 726e 3a20 5461 736b 0a20 2020 2020 2020  rn: Task.       
-000013a0: 203a 7274 7970 653a 207e 6b75 666c 6f77   :rtype: ~kuflow
-000013b0: 2e72 6573 742e 6d6f 6465 6c73 2e54 6173  .rest.models.Tas
-000013c0: 6b0a 2020 2020 2020 2020 3a72 6169 7365  k.        :raise
-000013d0: 7320 7e61 7a75 7265 2e63 6f72 652e 6578  s ~azure.core.ex
-000013e0: 6365 7074 696f 6e73 2e48 7474 7052 6573  ceptions.HttpRes
-000013f0: 706f 6e73 6545 7272 6f72 3a0a 2020 2020  ponseError:.    
-00001400: 2020 2020 7222 0000 0029 0372 0c00 0000      r"...).r....
-00001410: 721e 0000 00da 0d72 6574 7269 6576 655f  r......retrieve_
-00001420: 7461 736b a903 720d 0000 0072 2200 0000  task..r....r"...
-00001430: 7218 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00001440: 0f00 0000 7223 0000 0086 0000 0073 0200  ....r#.......s..
-00001450: 0000 000b 7a1c 5461 736b 4f70 6572 6174  ....z.TaskOperat
-00001460: 696f 6e73 2e72 6574 7269 6576 655f 7461  ions.retrieve_ta
-00001470: 736b 6302 0000 0000 0000 0000 0000 0003  skc.............
-00001480: 0000 0004 0000 004b 0000 0073 1800 0000  .......K...s....
-00001490: 7c00 6a00 6a01 6a02 6600 6401 7c01 6901  |.j.j.j.f.d.|.i.
-000014a0: 7c02 9702 8e01 5300 2902 7af4 436c 6169  |.....S.).z.Clai
-000014b0: 6d20 6120 7461 736b 2e0a 0a20 2020 2020  m a task...     
-000014c0: 2020 2041 6c6c 6f77 2074 6f20 636c 6169     Allow to clai
-000014d0: 6d20 6120 7461 736b 2e0a 0a20 2020 2020  m a task...     
-000014e0: 2020 203a 7061 7261 6d20 6964 3a20 5468     :param id: Th
-000014f0: 6520 7265 736f 7572 6365 2049 442e 2052  e resource ID. R
-00001500: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
-00001510: 203a 7479 7065 2069 643a 2073 7472 0a20   :type id: str. 
-00001520: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00001530: 5461 736b 0a20 2020 2020 2020 203a 7274  Task.        :rt
-00001540: 7970 653a 207e 6b75 666c 6f77 2e72 6573  ype: ~kuflow.res
-00001550: 742e 6d6f 6465 6c73 2e54 6173 6b0a 2020  t.models.Task.  
-00001560: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
-00001570: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
-00001580: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
-00001590: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-000015a0: 7222 0000 0029 0372 0c00 0000 721e 0000  r"...).r....r...
-000015b0: 00da 1261 6374 696f 6e73 5f74 6173 6b5f  ...actions_task_
-000015c0: 636c 6169 6d72 2400 0000 720e 0000 0072  claimr$...r....r
-000015d0: 0e00 0000 720f 0000 0072 2500 0000 9300  ....r....r%.....
-000015e0: 0000 7302 0000 0000 0b7a 2154 6173 6b4f  ..s......z!TaskO
-000015f0: 7065 7261 7469 6f6e 732e 6163 7469 6f6e  perations.action
-00001600: 735f 7461 736b 5f63 6c61 696d 2904 7222  s_task_claim).r"
-00001610: 0000 00da 0763 6f6d 6d61 6e64 7218 0000  .....commandr...
-00001620: 0072 1900 0000 6303 0000 0000 0000 0000  .r....c.........
-00001630: 0000 0004 0000 0005 0000 004b 0000 0073  ...........K...s
-00001640: 1a00 0000 7c00 6a00 6a01 6a02 6600 7c01  ....|.j.j.j.f.|.
-00001650: 7c02 6401 9c02 7c03 9702 8e01 5300 2902  |.d...|.....S.).
-00001660: 61b3 0100 0041 7373 6967 6e20 6120 7461  a....Assign a ta
-00001670: 736b 2e0a 0a20 2020 2020 2020 2041 6c6c  sk...        All
-00001680: 6f77 2074 6f20 6173 7369 676e 2061 2074  ow to assign a t
-00001690: 6173 6b20 746f 2061 2075 7365 7220 6f72  ask to a user or
-000016a0: 2061 7070 6c69 6361 7469 6f6e 2e20 4f6e   application. On
-000016b0: 6c79 206f 6e65 206f 7074 696f 6e20 7769  ly one option wi
-000016c0: 6c6c 2062 6520 6e65 6365 7373 6172 792e  ll be necessary.
-000016d0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000016e0: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
-000016f0: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
-00001700: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
-00001710: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
-00001720: 6172 616d 2063 6f6d 6d61 6e64 3a20 436f  aram command: Co
-00001730: 6d6d 616e 6420 746f 2063 6861 6e67 6520  mmand to change 
-00001740: 7468 6520 7461 736b 206f 776e 6572 2e20  the task owner. 
-00001750: 5265 7175 6972 6564 2e0a 2020 2020 2020  Required..      
-00001760: 2020 3a74 7970 6520 636f 6d6d 616e 643a    :type command:
-00001770: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
-00001780: 6465 6c73 2e54 6173 6b41 7373 6967 6e43  dels.TaskAssignC
-00001790: 6f6d 6d61 6e64 0a20 2020 2020 2020 203a  ommand.        :
-000017a0: 7265 7475 726e 3a20 5461 736b 0a20 2020  return: Task.   
-000017b0: 2020 2020 203a 7274 7970 653a 207e 6b75       :rtype: ~ku
-000017c0: 666c 6f77 2e72 6573 742e 6d6f 6465 6c73  flow.rest.models
-000017d0: 2e54 6173 6b0a 2020 2020 2020 2020 3a72  .Task.        :r
-000017e0: 6169 7365 7320 7e61 7a75 7265 2e63 6f72  aises ~azure.cor
-000017f0: 652e 6578 6365 7074 696f 6e73 2e48 7474  e.exceptions.Htt
-00001800: 7052 6573 706f 6e73 6545 7272 6f72 3a0a  pResponseError:.
-00001810: 2020 2020 2020 2020 a902 7222 0000 0072          ..r"...r
-00001820: 2600 0000 2903 720c 0000 0072 1e00 0000  &...).r....r....
-00001830: da13 6163 7469 6f6e 735f 7461 736b 5f61  ..actions_task_a
-00001840: 7373 6967 6ea9 0472 0d00 0000 7222 0000  ssign..r....r"..
-00001850: 0072 2600 0000 7218 0000 0072 0e00 0000  .r&...r....r....
-00001860: 720e 0000 0072 0f00 0000 7228 0000 00a0  r....r....r(....
-00001870: 0000 0073 0200 0000 000d 7a22 5461 736b  ...s......z"Task
-00001880: 4f70 6572 6174 696f 6e73 2e61 6374 696f  Operations.actio
-00001890: 6e73 5f74 6173 6b5f 6173 7369 676e 6303  ns_task_assignc.
-000018a0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-000018b0: 0000 004b 0000 0073 1a00 0000 7c00 6a00  ...K...s....|.j.
-000018c0: 6a01 6a02 6600 7c01 7c02 6401 9c02 7c03  j.j.f.|.|.d...|.
-000018d0: 9702 8e01 5300 2902 613d 0400 0053 6176  ....S.).a=...Sav
-000018e0: 6520 616e 2065 6c65 6d65 6e74 2e0a 0a20  e an element... 
-000018f0: 2020 2020 2020 2041 6c6c 6f77 2074 6f20         Allow to 
-00001900: 7361 7665 2061 6e20 656c 656d 656e 7420  save an element 
-00001910: 692e 652e 2c20 6120 6669 656c 642c 2061  i.e., a field, a
-00001920: 2064 6563 6973 696f 6e2c 2061 2066 6f72   decision, a for
-00001930: 6d2c 2061 2070 7269 6e63 6970 616c 206f  m, a principal o
-00001940: 7220 646f 6375 6d65 6e74 2e0a 0a20 2020  r document...   
-00001950: 2020 2020 2049 6e20 7468 6520 6361 7365       In the case
-00001960: 206f 6620 646f 6375 6d65 6e74 2074 7970   of document typ
-00001970: 6520 656c 656d 656e 7473 2c20 7468 6973  e elements, this
-00001980: 206d 6574 686f 6420 6f6e 6c79 2061 6c6c   method only all
-00001990: 6f77 7320 7265 6665 7265 6e63 6573 2074  ows references t
-000019a0: 6f20 6265 206d 6164 6520 746f 206f 7468  o be made to oth
-000019b0: 6572 0a20 2020 2020 2020 2065 7869 7374  er.        exist
-000019c0: 696e 6720 646f 6375 6d65 6e74 2074 7970  ing document typ
-000019d0: 6520 656c 656d 656e 7473 2066 6f72 2074  e elements for t
-000019e0: 6865 2070 7572 706f 7365 206f 6620 636f  he purpose of co
-000019f0: 7079 696e 6720 7468 6174 2066 696c 6520  pying that file 
-00001a00: 696e 746f 2074 6865 2065 6c65 6d65 6e74  into the element
-00001a10: 2e20 546f 2064 6f0a 2020 2020 2020 2020  . To do.        
-00001a20: 7468 6973 2079 6f75 206e 6565 6420 746f  this you need to
-00001a30: 2070 6173 7320 6120 7265 6665 7265 6e63   pass a referenc
-00001a40: 6520 746f 2074 6865 2064 6f63 756d 656e  e to the documen
-00001a50: 7420 7573 696e 6720 7468 6520 2775 7269  t using the 'uri
-00001a60: 2720 6174 7472 6962 7574 652e 2049 6e20  ' attribute. In 
-00001a70: 6361 7365 2079 6f75 2077 616e 740a 2020  case you want.  
-00001a80: 2020 2020 2020 746f 2061 6464 2061 206e        to add a n
-00001a90: 6577 2064 6f63 756d 656e 742c 2070 6c65  ew document, ple
-00001aa0: 6173 6520 7573 6520 7468 6520 636f 7272  ase use the corr
-00001ab0: 6573 706f 6e64 696e 6720 4150 4920 6d65  esponding API me
-00001ac0: 7468 6f64 2e20 4966 2076 616c 7565 7320  thod. If values 
-00001ad0: 616c 7265 6164 7920 6578 6973 7420 666f  already exist fo
-00001ae0: 7220 7468 650a 2020 2020 2020 2020 7072  r the.        pr
-00001af0: 6f76 6964 6564 2065 6c65 6d65 6e74 2063  ovided element c
-00001b00: 6f64 652c 2069 7420 7265 706c 6163 6573  ode, it replaces
-00001b10: 2074 6865 6d20 7769 7468 2074 6865 206e   them with the n
-00001b20: 6577 206f 6e65 732c 206f 7468 6572 7769  ew ones, otherwi
-00001b30: 7365 2069 7420 6372 6561 7465 7320 7468  se it creates th
-00001b40: 656d 2e20 5468 650a 2020 2020 2020 2020  em. The.        
-00001b50: 7661 6c75 6573 206f 6620 7468 6520 7072  values of the pr
-00001b60: 6576 696f 7573 2065 6c65 6d65 6e74 7320  evious elements 
-00001b70: 7468 6174 206e 6f20 6c6f 6e67 6572 2065  that no longer e
-00001b80: 7869 7374 2077 696c 6c20 6265 2064 656c  xist will be del
-00001b90: 6574 6564 2e20 546f 2072 656d 6f76 6520  eted. To remove 
-00001ba0: 616e 2065 6c65 6d65 6e74 2c20 7573 650a  an element, use.
-00001bb0: 2020 2020 2020 2020 7468 6520 6170 7072          the appr
-00001bc0: 6f70 7269 6174 6520 4150 4920 6d65 7468  opriate API meth
-00001bd0: 6f64 2e0a 0a20 2020 2020 2020 203a 7061  od...        :pa
-00001be0: 7261 6d20 6964 3a20 5468 6520 7265 736f  ram id: The reso
-00001bf0: 7572 6365 2049 442e 2052 6571 7569 7265  urce ID. Require
-00001c00: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
-00001c10: 2069 643a 2073 7472 0a20 2020 2020 2020   id: str.       
-00001c20: 203a 7061 7261 6d20 636f 6d6d 616e 643a   :param command:
-00001c30: 2043 6f6d 6d61 6e64 2074 6f20 7361 7665   Command to save
-00001c40: 2061 6e20 656c 656d 656e 742e 2052 6571   an element. Req
-00001c50: 7569 7265 642e 0a20 2020 2020 2020 203a  uired..        :
-00001c60: 7479 7065 2063 6f6d 6d61 6e64 3a20 7e6b  type command: ~k
-00001c70: 7566 6c6f 772e 7265 7374 2e6d 6f64 656c  uflow.rest.model
-00001c80: 732e 5461 736b 5361 7665 456c 656d 656e  s.TaskSaveElemen
-00001c90: 7443 6f6d 6d61 6e64 0a20 2020 2020 2020  tCommand.       
-00001ca0: 203a 7265 7475 726e 3a20 5461 736b 0a20   :return: Task. 
-00001cb0: 2020 2020 2020 203a 7274 7970 653a 207e         :rtype: ~
-00001cc0: 6b75 666c 6f77 2e72 6573 742e 6d6f 6465  kuflow.rest.mode
-00001cd0: 6c73 2e54 6173 6b0a 2020 2020 2020 2020  ls.Task.        
-00001ce0: 3a72 6169 7365 7320 7e61 7a75 7265 2e63  :raises ~azure.c
-00001cf0: 6f72 652e 6578 6365 7074 696f 6e73 2e48  ore.exceptions.H
-00001d00: 7474 7052 6573 706f 6e73 6545 7272 6f72  ttpResponseError
-00001d10: 3a0a 2020 2020 2020 2020 7227 0000 0029  :.        r'...)
-00001d20: 0372 0c00 0000 721e 0000 00da 1961 6374  .r....r......act
-00001d30: 696f 6e73 5f74 6173 6b5f 7361 7665 5f65  ions_task_save_e
-00001d40: 6c65 6d65 6e74 7229 0000 0072 0e00 0000  lementr)...r....
-00001d50: 720e 0000 0072 0f00 0000 722a 0000 00af  r....r....r*....
-00001d60: 0000 0073 0200 0000 0017 7a28 5461 736b  ...s......z(Task
-00001d70: 4f70 6572 6174 696f 6e73 2e61 6374 696f  Operations.actio
-00001d80: 6e73 5f74 6173 6b5f 7361 7665 5f65 6c65  ns_task_save_ele
-00001d90: 6d65 6e74 2905 7222 0000 00da 0466 696c  ment).r".....fil
-00001da0: 6572 2600 0000 7218 0000 0072 1900 0000  er&...r....r....
-00001db0: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
-00001dc0: 000a 0000 004b 0000 0073 3000 0000 7c00  .....K...s0...|.
-00001dd0: 6a00 6a01 6a02 6600 7c01 7c02 6a03 7c02  j.j.j.f.|.|.j.|.
-00001de0: 6a04 7c02 6a05 7c03 6a06 7c03 6a07 7c03  j.|.j.|.j.|.j.|.
-00001df0: 6a08 6401 9c07 7c04 9702 8e01 5300 2902  j.d...|.....S.).
-00001e00: 610f 0300 0053 6176 6520 616e 2065 6c65  a....Save an ele
-00001e10: 6d65 6e74 2064 6f63 756d 656e 742e 0a0a  ment document...
-00001e20: 2020 2020 2020 2020 416c 6c6f 7720 746f          Allow to
-00001e30: 2073 6176 6520 616e 2065 6c65 6d65 6e74   save an element
-00001e40: 2064 6f63 756d 656e 7420 7570 6c6f 6164   document upload
-00001e50: 696e 6720 7468 6520 636f 6e74 656e 742e  ing the content.
-00001e60: 0a0a 2020 2020 2020 2020 4966 2069 7420  ..        If it 
-00001e70: 6973 2061 206d 756c 7469 706c 6520 656c  is a multiple el
-00001e80: 656d 656e 742c 2061 6e64 2074 6865 2049  ement, and the I
-00001e90: 4420 7265 6665 7265 6e63 6564 2069 6e20  D referenced in 
-00001ea0: 7468 6520 626f 6479 2064 6f65 7320 6e6f  the body does no
-00001eb0: 7420 6578 6973 7420 6f72 2069 7320 656d  t exist or is em
-00001ec0: 7074 792c 2074 6865 0a20 2020 2020 2020  pty, the.       
-00001ed0: 2064 6f63 756d 656e 7420 7769 6c6c 2062   document will b
-00001ee0: 6520 6164 6465 6420 746f 2074 6865 2065  e added to the e
-00001ef0: 6c65 6d65 6e74 2e20 4966 2074 6865 2065  lement. If the e
-00001f00: 6c65 6d65 6e74 2061 6c72 6561 6479 2065  lement already e
-00001f10: 7869 7374 7320 2874 6865 2049 4420 7265  xists (the ID re
-00001f20: 6665 7265 6e63 6564 2069 6e20 7468 650a  ferenced in the.
-00001f30: 2020 2020 2020 2020 626f 6479 2063 6f72          body cor
-00001f40: 7265 7370 6f6e 6473 2074 6f20 616e 2065  responds to an e
-00001f50: 7869 7374 696e 6720 6f6e 6529 2c20 6974  xisting one), it
-00001f60: 2075 7064 6174 6573 2069 742e 0a0a 2020   updates it...  
-00001f70: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
-00001f80: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
-00001f90: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
-00001fa0: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
-00001fb0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
-00001fc0: 2066 696c 653a 2044 6f63 756d 656e 7420   file: Document 
-00001fd0: 746f 2073 6176 652e 2052 6571 7569 7265  to save. Require
-00001fe0: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
-00001ff0: 2066 696c 653a 207e 6b75 666c 6f77 2e72   file: ~kuflow.r
-00002000: 6573 742e 6d6f 6465 6c73 2e44 6f63 756d  est.models.Docum
-00002010: 656e 740a 2020 2020 2020 2020 3a70 6172  ent.        :par
-00002020: 616d 2063 6f6d 6d61 6e64 3a20 436f 6d6d  am command: Comm
-00002030: 616e 6420 696e 666f 2e20 5265 7175 6972  and info. Requir
-00002040: 6564 2e0a 2020 2020 2020 2020 3a74 7970  ed..        :typ
-00002050: 6520 636f 6d6d 616e 643a 207e 6b75 666c  e command: ~kufl
-00002060: 6f77 2e72 6573 742e 6d6f 6465 6c73 2e54  ow.rest.models.T
-00002070: 6173 6b53 6176 6545 6c65 6d65 6e74 5661  askSaveElementVa
-00002080: 6c75 6544 6f63 756d 656e 7443 6f6d 6d61  lueDocumentComma
-00002090: 6e64 0a20 2020 2020 2020 203a 7265 7475  nd.        :retu
-000020a0: 726e 3a20 5461 736b 0a20 2020 2020 2020  rn: Task.       
-000020b0: 203a 7274 7970 653a 207e 6b75 666c 6f77   :rtype: ~kuflow
-000020c0: 2e72 6573 742e 6d6f 6465 6c73 2e54 6173  .rest.models.Tas
-000020d0: 6b0a 2020 2020 2020 2020 3a72 6169 7365  k.        :raise
-000020e0: 7320 7e61 7a75 7265 2e63 6f72 652e 6578  s ~azure.core.ex
-000020f0: 6365 7074 696f 6e73 2e48 7474 7052 6573  ceptions.HttpRes
-00002100: 706f 6e73 6545 7272 6f72 3a0a 2020 2020  ponseError:.    
-00002110: 2020 2020 2907 7222 0000 0072 2b00 0000      ).r"...r+...
-00002120: da11 6669 6c65 5f63 6f6e 7465 6e74 5f74  ..file_content_t
-00002130: 7970 65da 0966 696c 655f 6e61 6d65 da17  ype..file_name..
-00002140: 656c 656d 656e 745f 6465 6669 6e69 7469  element_definiti
-00002150: 6f6e 5f63 6f64 65da 1065 6c65 6d65 6e74  on_code..element
-00002160: 5f76 616c 7565 5f69 64da 1365 6c65 6d65  _value_id..eleme
-00002170: 6e74 5f76 616c 7565 5f76 616c 6964 2909  nt_value_valid).
-00002180: 720c 0000 0072 1e00 0000 da28 6163 7469  r....r.....(acti
-00002190: 6f6e 735f 7461 736b 5f73 6176 655f 656c  ons_task_save_el
-000021a0: 656d 656e 745f 7661 6c75 655f 646f 6375  ement_value_docu
-000021b0: 6d65 6e74 da0c 6669 6c65 5f63 6f6e 7465  ment..file_conte
-000021c0: 6e74 da0c 636f 6e74 656e 745f 7479 7065  nt..content_type
-000021d0: da09 6669 6c65 5f6d 616d 6572 2e00 0000  ..file_mamer....
-000021e0: 722f 0000 0072 3000 0000 a905 720d 0000  r/...r0.....r...
-000021f0: 0072 2200 0000 722b 0000 0072 2600 0000  .r"...r+...r&...
-00002200: 7218 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00002210: 0f00 0000 7231 0000 00c8 0000 0073 1600  ....r1.......s..
-00002220: 0000 0015 0a01 0201 0401 0401 0401 0401  ................
-00002230: 0401 04f9 0408 02f8 7a37 5461 736b 4f70  ........z7TaskOp
-00002240: 6572 6174 696f 6e73 2e61 6374 696f 6e73  erations.actions
-00002250: 5f74 6173 6b5f 7361 7665 5f65 6c65 6d65  _task_save_eleme
-00002260: 6e74 5f76 616c 7565 5f64 6f63 756d 656e  nt_value_documen
-00002270: 7463 0300 0000 0000 0000 0000 0000 0400  tc..............
-00002280: 0000 0500 0000 4b00 0000 731a 0000 007c  ......K...s....|
-00002290: 006a 006a 016a 0266 007c 017c 0264 019c  .j.j.j.f.|.|.d..
-000022a0: 027c 0397 028e 0153 0029 0261 db01 0000  .|.....S.).a....
-000022b0: 4465 6c65 7465 2061 6e20 656c 656d 656e  Delete an elemen
-000022c0: 7420 6279 2063 6f64 652e 0a0a 2020 2020  t by code...    
-000022d0: 2020 2020 416c 6c6f 7720 746f 2064 656c      Allow to del
-000022e0: 6574 6520 7461 736b 2065 6c65 6d65 6e74  ete task element
-000022f0: 2062 7920 7370 6563 6966 7969 6e67 2074   by specifying t
-00002300: 6865 2069 7465 6d20 6465 6669 6e69 7469  he item definiti
-00002310: 6f6e 2063 6f64 652e 0a0a 2020 2020 2020  on code...      
-00002320: 2020 5265 6d6f 7665 2061 6c6c 2074 6865    Remove all the
-00002330: 2065 6c65 6d65 6e74 2076 616c 7565 732e   element values.
-00002340: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00002350: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
-00002360: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
-00002370: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
-00002380: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
-00002390: 6172 616d 2063 6f6d 6d61 6e64 3a20 436f  aram command: Co
-000023a0: 6d6d 616e 6420 746f 2064 656c 6574 6520  mmand to delete 
-000023b0: 616e 2065 6c65 6d65 6e74 2e20 5265 7175  an element. Requ
-000023c0: 6972 6564 2e0a 2020 2020 2020 2020 3a74  ired..        :t
-000023d0: 7970 6520 636f 6d6d 616e 643a 207e 6b75  ype command: ~ku
-000023e0: 666c 6f77 2e72 6573 742e 6d6f 6465 6c73  flow.rest.models
-000023f0: 2e54 6173 6b44 656c 6574 6545 6c65 6d65  .TaskDeleteEleme
-00002400: 6e74 436f 6d6d 616e 640a 2020 2020 2020  ntCommand.      
-00002410: 2020 3a72 6574 7572 6e3a 2054 6173 6b0a    :return: Task.
-00002420: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00002430: 7e6b 7566 6c6f 772e 7265 7374 2e6d 6f64  ~kuflow.rest.mod
-00002440: 656c 732e 5461 736b 0a20 2020 2020 2020  els.Task.       
-00002450: 203a 7261 6973 6573 207e 617a 7572 652e   :raises ~azure.
-00002460: 636f 7265 2e65 7863 6570 7469 6f6e 732e  core.exceptions.
-00002470: 4874 7470 5265 7370 6f6e 7365 4572 726f  HttpResponseErro
-00002480: 723a 0a20 2020 2020 2020 2072 2700 0000  r:.        r'...
-00002490: 2903 720c 0000 0072 1e00 0000 da1b 6163  ).r....r......ac
-000024a0: 7469 6f6e 735f 7461 736b 5f64 656c 6574  tions_task_delet
-000024b0: 655f 656c 656d 656e 7472 2900 0000 720e  e_elementr)...r.
-000024c0: 0000 0072 0e00 0000 720f 0000 0072 3600  ...r....r....r6.
-000024d0: 0000 e800 0000 7302 0000 0000 117a 2a54  ......s......z*T
-000024e0: 6173 6b4f 7065 7261 7469 6f6e 732e 6163  askOperations.ac
-000024f0: 7469 6f6e 735f 7461 736b 5f64 656c 6574  tions_task_delet
-00002500: 655f 656c 656d 656e 7463 0300 0000 0000  e_elementc......
-00002510: 0000 0000 0000 0400 0000 0500 0000 4b00  ..............K.
-00002520: 0000 731a 0000 007c 006a 006a 016a 0266  ..s....|.j.j.j.f
-00002530: 007c 017c 0264 019c 027c 0397 028e 0153  .|.|.d...|.....S
-00002540: 0029 0261 9902 0000 4465 6c65 7465 2061  .).a....Delete a
-00002550: 6e20 656c 656d 656e 7420 646f 6375 6d65  n element docume
-00002560: 6e74 2076 616c 7565 2e0a 0a20 2020 2020  nt value...     
-00002570: 2020 2041 6c6c 6f77 2074 6f20 6465 6c65     Allow to dele
-00002580: 7465 2061 2073 7065 6369 6669 6320 646f  te a specific do
-00002590: 6375 6d65 6e74 2066 726f 6d20 616e 2065  cument from an e
-000025a0: 6c65 6d65 6e74 206f 6620 646f 6375 6d65  lement of docume
-000025b0: 6e74 2074 7970 6520 7573 696e 6720 6974  nt type using it
-000025c0: 7320 6964 2e0a 0a20 2020 2020 2020 204e  s id...        N
-000025d0: 6f74 653a 2049 6620 6974 2069 7320 6120  ote: If it is a 
-000025e0: 6d75 6c74 6970 6c65 2069 7465 6d2c 2069  multiple item, i
-000025f0: 7420 7769 6c6c 206f 6e6c 7920 6465 6c65  t will only dele
-00002600: 7465 2074 6865 2073 7065 6369 6669 6564  te the specified
-00002610: 2064 6f63 756d 656e 742e 2049 6620 6974   document. If it
-00002620: 2069 7320 6120 7369 6e67 6c65 0a20 2020   is a single.   
-00002630: 2020 2020 2065 6c65 6d65 6e74 2c20 696e       element, in
-00002640: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
-00002650: 2064 6f63 756d 656e 742c 2069 7420 7769   document, it wi
-00002660: 6c6c 2061 6c73 6f20 6465 6c65 7465 2074  ll also delete t
-00002670: 6865 2065 6c65 6d65 6e74 2e0a 0a20 2020  he element...   
-00002680: 2020 2020 203a 7061 7261 6d20 6964 3a20       :param id: 
-00002690: 5468 6520 7265 736f 7572 6365 2049 442e  The resource ID.
-000026a0: 2052 6571 7569 7265 642e 0a20 2020 2020   Required..     
-000026b0: 2020 203a 7479 7065 2069 643a 2073 7472     :type id: str
-000026c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000026d0: 636f 6d6d 616e 643a 2043 6f6d 6d61 6e64  command: Command
-000026e0: 2074 6f20 6465 6c65 7465 2061 2064 6f63   to delete a doc
-000026f0: 756d 656e 7420 656c 656d 656e 7420 7661  ument element va
-00002700: 6c75 652e 2052 6571 7569 7265 642e 0a20  lue. Required.. 
-00002710: 2020 2020 2020 203a 7479 7065 2063 6f6d         :type com
-00002720: 6d61 6e64 3a20 7e6b 7566 6c6f 772e 7265  mand: ~kuflow.re
-00002730: 7374 2e6d 6f64 656c 732e 5461 736b 4465  st.models.TaskDe
-00002740: 6c65 7465 456c 656d 656e 7456 616c 7565  leteElementValue
-00002750: 446f 6375 6d65 6e74 436f 6d6d 616e 640a  DocumentCommand.
-00002760: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00002770: 2054 6173 6b0a 2020 2020 2020 2020 3a72   Task.        :r
-00002780: 7479 7065 3a20 7e6b 7566 6c6f 772e 7265  type: ~kuflow.re
-00002790: 7374 2e6d 6f64 656c 732e 5461 736b 0a20  st.models.Task. 
-000027a0: 2020 2020 2020 203a 7261 6973 6573 207e         :raises ~
-000027b0: 617a 7572 652e 636f 7265 2e65 7863 6570  azure.core.excep
-000027c0: 7469 6f6e 732e 4874 7470 5265 7370 6f6e  tions.HttpRespon
-000027d0: 7365 4572 726f 723a 0a20 2020 2020 2020  seError:.       
-000027e0: 2072 2700 0000 2903 720c 0000 0072 1e00   r'...).r....r..
-000027f0: 0000 da2a 6163 7469 6f6e 735f 7461 736b  ...*actions_task
-00002800: 5f64 656c 6574 655f 656c 656d 656e 745f  _delete_element_
-00002810: 7661 6c75 655f 646f 6375 6d65 6e74 7229  value_documentr)
-00002820: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
-00002830: 0000 7237 0000 00fb 0000 0073 0200 0000  ..r7.......s....
-00002840: 0012 7a39 5461 736b 4f70 6572 6174 696f  ..z9TaskOperatio
-00002850: 6e73 2e61 6374 696f 6e73 5f74 6173 6b5f  ns.actions_task_
-00002860: 6465 6c65 7465 5f65 6c65 6d65 6e74 5f76  delete_element_v
-00002870: 616c 7565 5f64 6f63 756d 656e 7429 0472  alue_document).r
-00002880: 2200 0000 da0b 646f 6375 6d65 6e74 5f69  ".....document_i
-00002890: 6472 1800 0000 7219 0000 0063 0300 0000  dr....r....c....
-000028a0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-000028b0: 4b00 0000 731a 0000 007c 006a 006a 016a  K...s....|.j.j.j
-000028c0: 0266 007c 017c 0264 019c 027c 0397 028e  .f.|.|.d...|....
-000028d0: 0153 0029 0261 9701 0000 446f 776e 6c6f  .S.).a....Downlo
-000028e0: 6164 2064 6f63 756d 656e 742e 0a0a 2020  ad document...  
-000028f0: 2020 2020 2020 4769 7665 6e20 6120 7461        Given a ta
-00002900: 736b 2c20 646f 776e 6c6f 6164 2061 2064  sk, download a d
-00002910: 6f63 756d 656e 7420 6672 6f6d 2061 6e20  ocument from an 
-00002920: 656c 656d 656e 7420 6f66 2064 6f63 756d  element of docum
-00002930: 656e 7420 7479 7065 2e0a 0a20 2020 2020  ent type...     
-00002940: 2020 203a 7061 7261 6d20 6964 3a20 5468     :param id: Th
-00002950: 6520 7265 736f 7572 6365 2049 442e 2052  e resource ID. R
-00002960: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
-00002970: 203a 7479 7065 2069 643a 2073 7472 0a20   :type id: str. 
-00002980: 2020 2020 2020 203a 6b65 7977 6f72 6420         :keyword 
-00002990: 646f 6375 6d65 6e74 5f69 643a 2044 6f63  document_id: Doc
-000029a0: 756d 656e 7420 4944 2074 6f20 646f 776e  ument ID to down
-000029b0: 6c6f 6164 2e20 5265 7175 6972 6564 2e0a  load. Required..
-000029c0: 2020 2020 2020 2020 3a74 7970 6520 646f          :type do
-000029d0: 6375 6d65 6e74 5f69 643a 2073 7472 0a20  cument_id: str. 
-000029e0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-000029f0: 4974 6572 6174 6f72 206f 6620 7468 6520  Iterator of the 
-00002a00: 7265 7370 6f6e 7365 2062 7974 6573 0a20  response bytes. 
-00002a10: 2020 2020 2020 203a 7274 7970 653a 2049         :rtype: I
-00002a20: 7465 7261 746f 725b 6279 7465 735d 0a20  terator[bytes]. 
-00002a30: 2020 2020 2020 203a 7261 6973 6573 207e         :raises ~
-00002a40: 617a 7572 652e 636f 7265 2e65 7863 6570  azure.core.excep
-00002a50: 7469 6f6e 732e 4874 7470 5265 7370 6f6e  tions.HttpRespon
-00002a60: 7365 4572 726f 723a 0a20 2020 2020 2020  seError:.       
-00002a70: 2029 0272 2200 0000 7238 0000 0029 0372   ).r"...r8...).r
-00002a80: 0c00 0000 721e 0000 00da 2c61 6374 696f  ....r.....,actio
-00002a90: 6e73 5f74 6173 6b5f 646f 776e 6c6f 6164  ns_task_download
-00002aa0: 5f65 6c65 6d65 6e74 5f76 616c 7565 5f64  _element_value_d
-00002ab0: 6f63 756d 656e 7429 0472 0d00 0000 7222  ocument).r....r"
-00002ac0: 0000 0072 3800 0000 7218 0000 0072 0e00  ...r8...r....r..
-00002ad0: 0000 720e 0000 0072 0f00 0000 7239 0000  ..r....r....r9..
-00002ae0: 000f 0100 0073 0c00 0000 000d 0a01 0200  .....s..........
-00002af0: 02ff 0401 02ff 7a3b 5461 736b 4f70 6572  ......z;TaskOper
-00002b00: 6174 696f 6e73 2e61 6374 696f 6e73 5f74  ations.actions_t
-00002b10: 6173 6b5f 646f 776e 6c6f 6164 5f65 6c65  ask_download_ele
-00002b20: 6d65 6e74 5f76 616c 7565 5f64 6f63 756d  ment_value_docum
-00002b30: 656e 7429 0472 2200 0000 722e 0000 0072  ent).r"...r....r
-00002b40: 1800 0000 7219 0000 0063 0300 0000 0000  ....r....c......
-00002b50: 0000 0000 0000 0400 0000 0500 0000 4b00  ..............K.
-00002b60: 0000 731a 0000 007c 006a 006a 016a 0266  ..s....|.j.j.j.f
-00002b70: 007c 017c 0264 019c 027c 0397 028e 0153  .|.|.d...|.....S
-00002b80: 0029 0261 a602 0000 446f 776e 6c6f 6164  .).a....Download
-00002b90: 2061 2046 6f72 6d20 7265 6e64 6572 6564   a Form rendered
-00002ba0: 2061 7320 5044 4620 6f72 205a 6970 206f   as PDF or Zip o
-00002bb0: 6620 5044 4673 2028 7768 656e 2074 6865  f PDFs (when the
-00002bc0: 2065 6c65 6d65 6e74 2069 7320 6d75 6c74   element is mult
-00002bd0: 6970 6c65 292e 0a0a 2020 2020 2020 2020  iple)...        
-00002be0: 4769 7665 6e20 6120 7461 736b 2c20 6765  Given a task, ge
-00002bf0: 6e65 7261 7465 2061 2050 4446 2066 726f  nerate a PDF fro
-00002c00: 6d20 6120 466f 726d 2074 7970 6520 656c  m a Form type el
-00002c10: 656d 656e 7420 7769 7468 2074 6865 2064  ement with the d
-00002c20: 6174 6120 6669 6c6c 6564 2069 6e2c 2069  ata filled in, i
-00002c30: 6620 616e 792e 2049 6620 7468 6572 650a  f any. If there.
-00002c40: 2020 2020 2020 2020 6172 6520 6d75 6c74          are mult
-00002c50: 6970 6c65 2066 6f72 6d20 7661 6c75 6573  iple form values
-00002c60: 2c20 7468 6579 2061 7265 2070 6163 6b65  , they are packe
-00002c70: 6420 696e 746f 2061 205a 4950 2e0a 0a20  d into a ZIP... 
-00002c80: 2020 2020 2020 2049 6d70 6f72 7461 6e74         Important
-00002c90: 213a 2054 6f20 7573 6520 7468 6973 2066  !: To use this f
-00002ca0: 6561 7475 7265 2c20 706c 6561 7365 2063  eature, please c
-00002cb0: 6f6e 7461 6374 2074 6f20 6b75 666c 6f77  ontact to kuflow
-00002cc0: 406b 7566 6c6f 772e 636f 6d2e 0a0a 2020  @kuflow.com...  
-00002cd0: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
-00002ce0: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
-00002cf0: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
-00002d00: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
-00002d10: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
-00002d20: 2065 6c65 6d65 6e74 5f64 6566 696e 6974   element_definit
-00002d30: 696f 6e5f 636f 6465 3a20 456c 656d 656e  ion_code: Elemen
-00002d40: 7420 6465 6669 6e69 7469 6f6e 2063 6f64  t definition cod
-00002d50: 6520 6f66 2061 2046 6f72 6d20 456c 656d  e of a Form Elem
-00002d60: 656e 7420 746f 2064 6f77 6e6c 6f61 642e  ent to download.
-00002d70: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
-00002d80: 6c65 6d65 6e74 5f64 6566 696e 6974 696f  lement_definitio
-00002d90: 6e5f 636f 6465 3a20 7374 720a 2020 2020  n_code: str.    
-00002da0: 2020 2020 3a72 6574 7572 6e3a 2049 7465      :return: Ite
-00002db0: 7261 746f 7220 6f66 2074 6865 2072 6573  rator of the res
-00002dc0: 706f 6e73 6520 6279 7465 730a 2020 2020  ponse bytes.    
-00002dd0: 2020 2020 3a72 7479 7065 3a20 4974 6572      :rtype: Iter
-00002de0: 6174 6f72 5b62 7974 6573 5d0a 2020 2020  ator[bytes].    
-00002df0: 2020 2020 3a72 6169 7365 7320 7e61 7a75      :raises ~azu
-00002e00: 7265 2e63 6f72 652e 6578 6365 7074 696f  re.core.exceptio
-00002e10: 6e73 2e48 7474 7052 6573 706f 6e73 6545  ns.HttpResponseE
-00002e20: 7272 6f72 3a0a 2020 2020 2020 2020 2902  rror:.        ).
-00002e30: 7222 0000 0072 2e00 0000 2903 720c 0000  r"...r....).r...
-00002e40: 0072 1e00 0000 da2c 6163 7469 6f6e 735f  .r.....,actions_
-00002e50: 7461 736b 5f64 6f77 6e6c 6f61 645f 656c  task_download_el
-00002e60: 656d 656e 745f 7661 6c75 655f 7265 6e64  ement_value_rend
-00002e70: 6572 6564 2904 720d 0000 0072 2200 0000  ered).r....r"...
-00002e80: 722e 0000 0072 1800 0000 720e 0000 0072  r....r....r....r
-00002e90: 0e00 0000 720f 0000 0072 3a00 0000 2001  ....r....r:... .
-00002ea0: 0000 730c 0000 0000 120a 0102 0002 ff04  ..s.............
-00002eb0: 0102 ff7a 3b54 6173 6b4f 7065 7261 7469  ...z;TaskOperati
-00002ec0: 6f6e 732e 6163 7469 6f6e 735f 7461 736b  ons.actions_task
-00002ed0: 5f64 6f77 6e6c 6f61 645f 656c 656d 656e  _download_elemen
-00002ee0: 745f 7661 6c75 655f 7265 6e64 6572 6564  t_value_rendered
-00002ef0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00002f00: 0005 0000 004b 0000 0073 1a00 0000 7c00  .....K...s....|.
-00002f10: 6a00 6a01 6a02 6600 7c01 7c02 6401 9c02  j.j.j.f.|.|.d...
-00002f20: 7c03 9702 8e01 5300 2902 610d 0200 0053  |.....S.).a....S
-00002f30: 6176 6520 4a53 4f4e 2064 6174 612e 0a0a  ave JSON data...
-00002f40: 2020 2020 2020 2020 416c 6c6f 7720 746f          Allow to
-00002f50: 2073 6176 6520 6120 4a53 4f4e 2064 6174   save a JSON dat
-00002f60: 6120 7661 6c69 6461 7469 6e67 2074 6861  a validating tha
-00002f70: 7420 7468 6520 6461 7461 2066 6f6c 6c6f  t the data follo
-00002f80: 7720 7468 6520 7265 6c61 7465 6420 7363  w the related sc
-00002f90: 6865 6d61 2e20 4966 2074 6865 2064 6174  hema. If the dat
-00002fa0: 6120 6973 0a20 2020 2020 2020 2069 6e76  a is.        inv
-00002fb0: 616c 6964 2c20 7468 656e 0a20 2020 2020  alid, then.     
-00002fc0: 2020 2074 6865 206a 736f 6e20 666f 726d     the json form
-00002fd0: 2069 7320 6d61 726b 6564 2061 7320 696e   is marked as in
-00002fe0: 7661 6c69 642e 0a0a 2020 2020 2020 2020  valid...        
-00002ff0: 3a70 6172 616d 2069 643a 2054 6865 2072  :param id: The r
-00003000: 6573 6f75 7263 6520 4944 2e20 5265 7175  esource ID. Requ
-00003010: 6972 6564 2e0a 2020 2020 2020 2020 3a74  ired..        :t
-00003020: 7970 6520 6964 3a20 7374 720a 2020 2020  ype id: str.    
-00003030: 2020 2020 3a70 6172 616d 2063 6f6d 6d61      :param comma
-00003040: 6e64 3a20 436f 6d6d 616e 6420 746f 2073  nd: Command to s
-00003050: 6176 6520 7468 6520 4a53 4f4e 2076 616c  ave the JSON val
-00003060: 7565 2e20 5265 7175 6972 6564 2e0a 2020  ue. Required..  
-00003070: 2020 2020 2020 3a74 7970 6520 636f 6d6d        :type comm
-00003080: 616e 643a 207e 6b75 666c 6f77 2e72 6573  and: ~kuflow.res
-00003090: 742e 6d6f 6465 6c73 2e54 6173 6b53 6176  t.models.TaskSav
-000030a0: 654a 736f 6e46 6f72 6d73 5661 6c75 6544  eJsonFormsValueD
-000030b0: 6174 6143 6f6d 6d61 6e64 0a20 2020 2020  ataCommand.     
-000030c0: 2020 203a 7265 7475 726e 3a20 5461 736b     :return: Task
-000030d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-000030e0: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
-000030f0: 6465 6c73 2e54 6173 6b0a 2020 2020 2020  dels.Task.      
-00003100: 2020 3a72 6169 7365 7320 7e61 7a75 7265    :raises ~azure
-00003110: 2e63 6f72 652e 6578 6365 7074 696f 6e73  .core.exceptions
-00003120: 2e48 7474 7052 6573 706f 6e73 6545 7272  .HttpResponseErr
-00003130: 6f72 3a0a 2020 2020 2020 2020 7227 0000  or:.        r'..
-00003140: 0029 0372 0c00 0000 721e 0000 00da 2761  .).r....r.....'a
-00003150: 6374 696f 6e73 5f74 6173 6b5f 7361 7665  ctions_task_save
-00003160: 5f6a 736f 6e5f 666f 726d 735f 7661 6c75  _json_forms_valu
-00003170: 655f 6461 7461 7229 0000 0072 0e00 0000  e_datar)...r....
-00003180: 720e 0000 0072 0f00 0000 723b 0000 0036  r....r....r;...6
-00003190: 0100 0073 0200 0000 0014 7a36 5461 736b  ...s......z6Task
-000031a0: 4f70 6572 6174 696f 6e73 2e61 6374 696f  Operations.actio
-000031b0: 6e73 5f74 6173 6b5f 7361 7665 5f6a 736f  ns_task_save_jso
-000031c0: 6e5f 666f 726d 735f 7661 6c75 655f 6461  n_forms_value_da
-000031d0: 7461 6304 0000 0000 0000 0000 0000 0005  tac.............
-000031e0: 0000 0008 0000 004b 0000 0073 2800 0000  .......K...s(...
-000031f0: 7c00 6a00 6a01 6a02 6600 7c01 7c02 6a03  |.j.j.j.f.|.|.j.
-00003200: 7c02 6a04 7c02 6a05 7c03 6a06 6401 9c05  |.j.|.j.|.j.d...
-00003210: 7c04 9702 8e01 5300 2902 6171 0200 0053  |.....S.).aq...S
-00003220: 6176 6520 6120 4a53 4f4e 2046 6f72 6d73  ave a JSON Forms
-00003230: 2064 6f63 756d 656e 742e 0a0a 2020 2020   document...    
-00003240: 2020 2020 5361 7665 2061 2064 6f63 756d      Save a docum
-00003250: 656e 7420 696e 2074 6865 2074 6173 6b20  ent in the task 
-00003260: 746f 206c 6174 6572 2062 6520 6c69 6e6b  to later be link
-00003270: 6564 2069 6e74 6f20 7468 6520 4a53 4f4e  ed into the JSON
-00003280: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
-00003290: 3a70 6172 616d 2069 643a 2054 6865 2072  :param id: The r
-000032a0: 6573 6f75 7263 6520 4944 2e20 5265 7175  esource ID. Requ
-000032b0: 6972 6564 2e0a 2020 2020 2020 2020 3a74  ired..        :t
-000032c0: 7970 6520 6964 3a20 7374 720a 2020 2020  ype id: str.    
-000032d0: 2020 2020 3a70 6172 616d 2066 696c 653a      :param file:
-000032e0: 2044 6f63 756d 656e 7420 746f 2073 6176   Document to sav
-000032f0: 652e 2052 6571 7569 7265 642e 0a20 2020  e. Required..   
-00003300: 2020 2020 203a 7479 7065 2066 696c 653a       :type file:
-00003310: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
-00003320: 6465 6c73 2e44 6f63 756d 656e 740a 2020  dels.Document.  
-00003330: 2020 2020 2020 3a70 6172 616d 2063 6f6d        :param com
-00003340: 6d61 6e64 3a20 436f 6d6d 616e 6420 746f  mand: Command to
-00003350: 2073 6176 6520 7468 6520 4a53 4f4e 2076   save the JSON v
-00003360: 616c 7565 2e20 5265 7175 6972 6564 2e0a  alue. Required..
-00003370: 2020 2020 2020 2020 3a74 7970 6520 636f          :type co
-00003380: 6d6d 616e 643a 207e 6b75 666c 6f77 2e72  mmand: ~kuflow.r
-00003390: 6573 742e 6d6f 6465 6c73 2e54 6173 6b53  est.models.TaskS
-000033a0: 6176 654a 736f 6e46 6f72 6d73 5661 6c75  aveJsonFormsValu
-000033b0: 6544 6174 6143 6f6d 6d61 6e64 0a20 2020  eDataCommand.   
-000033c0: 2020 2020 203a 7265 7475 726e 3a20 5461       :return: Ta
-000033d0: 736b 5361 7665 4a73 6f6e 466f 726d 7356  skSaveJsonFormsV
-000033e0: 616c 7565 446f 6375 6d65 6e74 5265 7370  alueDocumentResp
-000033f0: 6f6e 7365 436f 6d6d 616e 640a 2020 2020  onseCommand.    
-00003400: 2020 2020 3a72 7479 7065 3a20 7e6b 7566      :rtype: ~kuf
-00003410: 6c6f 772e 7265 7374 2e6d 6f64 656c 732e  low.rest.models.
-00003420: 5461 736b 5361 7665 4a73 6f6e 466f 726d  TaskSaveJsonForm
-00003430: 7356 616c 7565 446f 6375 6d65 6e74 5265  sValueDocumentRe
-00003440: 7370 6f6e 7365 436f 6d6d 616e 640a 2020  sponseCommand.  
-00003450: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
-00003460: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
-00003470: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
-00003480: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-00003490: 2905 7222 0000 0072 2b00 0000 722c 0000  ).r"...r+...r,..
-000034a0: 0072 2d00 0000 da0b 7363 6865 6d61 5f70  .r-.....schema_p
-000034b0: 6174 6829 0772 0c00 0000 721e 0000 00da  ath).r....r.....
-000034c0: 2b61 6374 696f 6e73 5f74 6173 6b5f 7361  +actions_task_sa
-000034d0: 7665 5f6a 736f 6e5f 666f 726d 735f 7661  ve_json_forms_va
-000034e0: 6c75 655f 646f 6375 6d65 6e74 7232 0000  lue_documentr2..
-000034f0: 0072 3300 0000 7234 0000 0072 3c00 0000  .r3...r4...r<...
-00003500: 7235 0000 0072 0e00 0000 720e 0000 0072  r5...r....r....r
-00003510: 0f00 0000 723d 0000 004c 0100 0073 1200  ....r=...L...s..
-00003520: 0000 0015 0a01 0201 0401 0401 0401 04fb  ................
-00003530: 0406 02fa 7a3a 5461 736b 4f70 6572 6174  ....z:TaskOperat
-00003540: 696f 6e73 2e61 6374 696f 6e73 5f74 6173  ions.actions_tas
-00003550: 6b5f 7361 7665 5f6a 736f 6e5f 666f 726d  k_save_json_form
-00003560: 735f 7661 6c75 655f 646f 6375 6d65 6e74  s_value_document
-00003570: 2904 7222 0000 00da 0c64 6f63 756d 656e  ).r".....documen
-00003580: 745f 7572 6972 1800 0000 7219 0000 0063  t_urir....r....c
-00003590: 0200 0000 0000 0000 0100 0000 0400 0000  ................
-000035a0: 0500 0000 4b00 0000 731a 0000 007c 006a  ....K...s....|.j
-000035b0: 006a 016a 0266 007c 017c 0264 019c 027c  .j.j.f.|.|.d...|
-000035c0: 0397 028e 0153 0029 0261 8d01 0000 446f  .....S.).a....Do
-000035d0: 776e 6c6f 6164 2064 6f63 756d 656e 742e  wnload document.
-000035e0: 0a0a 2020 2020 2020 2020 4769 7665 6e20  ..        Given 
-000035f0: 6120 7461 736b 2c20 646f 776e 6c6f 6164  a task, download
-00003600: 2061 2064 6f63 756d 656e 7420 6672 6f6d   a document from
-00003610: 2061 206a 736f 6e20 666f 726d 2064 6174   a json form dat
-00003620: 612e 0a0a 2020 2020 2020 2020 3a70 6172  a...        :par
-00003630: 616d 2069 643a 2054 6865 2072 6573 6f75  am id: The resou
-00003640: 7263 6520 4944 2e20 5265 7175 6972 6564  rce ID. Required
-00003650: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00003660: 6964 3a20 7374 720a 2020 2020 2020 2020  id: str.        
-00003670: 3a70 6172 616d 2064 6f63 756d 656e 745f  :param document_
-00003680: 7572 693a 2044 6f63 756d 656e 7420 5552  uri: Document UR
-00003690: 4920 746f 2064 6f77 6e6c 6f61 642e 2052  I to download. R
-000036a0: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
-000036b0: 203a 7479 7065 2064 6f63 756d 656e 745f   :type document_
-000036c0: 7572 693a 2073 7472 0a20 2020 2020 2020  uri: str.       
-000036d0: 203a 7265 7475 726e 3a20 4974 6572 6174   :return: Iterat
-000036e0: 6f72 206f 6620 7468 6520 7265 7370 6f6e  or of the respon
-000036f0: 7365 2062 7974 6573 0a20 2020 2020 2020  se bytes.       
-00003700: 203a 7274 7970 653a 2049 7465 7261 746f   :rtype: Iterato
-00003710: 725b 6279 7465 735d 0a20 2020 2020 2020  r[bytes].       
-00003720: 203a 7261 6973 6573 207e 617a 7572 652e   :raises ~azure.
-00003730: 636f 7265 2e65 7863 6570 7469 6f6e 732e  core.exceptions.
-00003740: 4874 7470 5265 7370 6f6e 7365 4572 726f  HttpResponseErro
-00003750: 723a 0a20 2020 2020 2020 2029 0272 2200  r:.        ).r".
-00003760: 0000 723e 0000 0029 0372 0c00 0000 721e  ..r>...).r....r.
-00003770: 0000 00da 2f61 6374 696f 6e73 5f74 6173  ..../actions_tas
-00003780: 6b5f 646f 776e 6c6f 6164 5f6a 736f 6e5f  k_download_json_
-00003790: 666f 726d 735f 7661 6c75 655f 646f 6375  forms_value_docu
-000037a0: 6d65 6e74 2904 720d 0000 0072 2200 0000  ment).r....r"...
-000037b0: 723e 0000 0072 1800 0000 720e 0000 0072  r>...r....r....r
-000037c0: 0e00 0000 720f 0000 0072 3f00 0000 6a01  ....r....r?...j.
-000037d0: 0000 730c 0000 0000 0f0a 0102 0102 fe04  ..s.............
-000037e0: 0302 fd7a 3e54 6173 6b4f 7065 7261 7469  ...z>TaskOperati
-000037f0: 6f6e 732e 6163 7469 6f6e 735f 7461 736b  ons.actions_task
-00003800: 5f64 6f77 6e6c 6f61 645f 6a73 6f6e 5f66  _download_json_f
-00003810: 6f72 6d73 5f76 616c 7565 5f64 6f63 756d  orms_value_docum
-00003820: 656e 7463 0200 0000 0000 0000 0000 0000  entc............
-00003830: 0300 0000 0400 0000 4b00 0000 7318 0000  ........K...s...
-00003840: 007c 006a 006a 016a 0266 0064 017c 0169  .|.j.j.j.f.d.|.i
-00003850: 017c 0297 028e 0153 0029 0261 1301 0000  .|.....S.).a....
-00003860: 436f 6d70 6c65 7465 2061 2074 6173 6b2e  Complete a task.
-00003870: 0a0a 2020 2020 2020 2020 416c 6c6f 7720  ..        Allow 
-00003880: 746f 2063 6f6d 706c 6574 6520 6120 636c  to complete a cl
-00003890: 6169 6d65 6420 7461 736b 2062 7920 7468  aimed task by th
-000038a0: 6520 7072 696e 6369 7061 6c2e 0a0a 2020  e principal...  
-000038b0: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
-000038c0: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
-000038d0: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
-000038e0: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
-000038f0: 720a 2020 2020 2020 2020 3a72 6574 7572  r.        :retur
-00003900: 6e3a 2054 6173 6b0a 2020 2020 2020 2020  n: Task.        
-00003910: 3a72 7479 7065 3a20 7e6b 7566 6c6f 772e  :rtype: ~kuflow.
-00003920: 7265 7374 2e6d 6f64 656c 732e 5461 736b  rest.models.Task
-00003930: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
-00003940: 207e 617a 7572 652e 636f 7265 2e65 7863   ~azure.core.exc
-00003950: 6570 7469 6f6e 732e 4874 7470 5265 7370  eptions.HttpResp
-00003960: 6f6e 7365 4572 726f 723a 0a20 2020 2020  onseError:.     
-00003970: 2020 2072 2200 0000 2903 720c 0000 0072     r"...).r....r
-00003980: 1e00 0000 da15 6163 7469 6f6e 735f 7461  ......actions_ta
-00003990: 736b 5f63 6f6d 706c 6574 6572 2400 0000  sk_completer$...
-000039a0: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-000039b0: 4000 0000 7f01 0000 7302 0000 0000 0b7a  @.......s......z
-000039c0: 2454 6173 6b4f 7065 7261 7469 6f6e 732e  $TaskOperations.
-000039d0: 6163 7469 6f6e 735f 7461 736b 5f63 6f6d  actions_task_com
-000039e0: 706c 6574 6529 0472 2200 0000 da03 6c6f  plete).r".....lo
-000039f0: 6772 1800 0000 7219 0000 0063 0300 0000  gr....r....c....
-00003a00: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00003a10: 4b00 0000 731a 0000 007c 006a 006a 016a  K...s....|.j.j.j
-00003a20: 0266 007c 017c 0264 019c 027c 0397 028e  .f.|.|.d...|....
-00003a30: 0153 0029 0261 b901 0000 4170 7065 6e64  .S.).a....Append
-00003a40: 2061 206c 6f67 2074 6f20 7468 6520 7461   a log to the ta
-00003a50: 736b 2e0a 0a20 2020 2020 2020 2041 206c  sk...        A l
-00003a60: 6f67 2065 6e74 7279 2069 7320 6164 6465  og entry is adde
-00003a70: 6420 746f 2074 6865 2074 6173 6b2e 2049  d to the task. I
-00003a80: 6620 7468 6520 6e75 6d62 6572 206f 6620  f the number of 
-00003a90: 6c6f 6720 656e 7472 6965 7320 6973 2072  log entries is r
-00003aa0: 6561 6368 6564 2c20 7468 6520 6f6c 6465  eached, the olde
-00003ab0: 7374 206c 6f67 2065 6e74 7279 0a20 2020  st log entry.   
-00003ac0: 2020 2020 2069 7320 7265 6d6f 7665 642e       is removed.
-00003ad0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00003ae0: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
-00003af0: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
-00003b00: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
-00003b10: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
-00003b20: 6172 616d 206c 6f67 3a20 4c6f 6720 746f  aram log: Log to
-00003b30: 2062 6520 6372 6561 7465 642e 2052 6571   be created. Req
-00003b40: 7569 7265 642e 0a20 2020 2020 2020 203a  uired..        :
-00003b50: 7479 7065 206c 6f67 3a20 7e6b 7566 6c6f  type log: ~kuflo
-00003b60: 772e 7265 7374 2e6d 6f64 656c 732e 4c6f  w.rest.models.Lo
-00003b70: 670a 2020 2020 2020 2020 3a72 6574 7572  g.        :retur
-00003b80: 6e3a 2054 6173 6b0a 2020 2020 2020 2020  n: Task.        
-00003b90: 3a72 7479 7065 3a20 7e6b 7566 6c6f 772e  :rtype: ~kuflow.
-00003ba0: 7265 7374 2e6d 6f64 656c 732e 5461 736b  rest.models.Task
-00003bb0: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
-00003bc0: 207e 617a 7572 652e 636f 7265 2e65 7863   ~azure.core.exc
-00003bd0: 6570 7469 6f6e 732e 4874 7470 5265 7370  eptions.HttpResp
-00003be0: 6f6e 7365 4572 726f 723a 0a20 2020 2020  onseError:.     
-00003bf0: 2020 2029 0272 2200 0000 7241 0000 0029     ).r"...rA...)
-00003c00: 0372 0c00 0000 721e 0000 00da 1761 6374  .r....r......act
-00003c10: 696f 6e73 5f74 6173 6b5f 6170 7065 6e64  ions_task_append
-00003c20: 5f6c 6f67 2904 720d 0000 0072 2200 0000  _log).r....r"...
-00003c30: 7241 0000 0072 1800 0000 720e 0000 0072  rA...r....r....r
-00003c40: 0e00 0000 720f 0000 0072 4200 0000 8c01  ....r....rB.....
-00003c50: 0000 7302 0000 0000 0e7a 2654 6173 6b4f  ..s......z&TaskO
-00003c60: 7065 7261 7469 6f6e 732e 6163 7469 6f6e  perations.action
-00003c70: 735f 7461 736b 5f61 7070 656e 645f 6c6f  s_task_append_lo
-00003c80: 6729 0672 1100 0000 7201 0000 004e 4e4e  g).r....r....NNN
-00003c90: 4e29 014e 292c da08 5f5f 6e61 6d65 5f5f  N).N),..__name__
-00003ca0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00003cb0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00003cc0: 635f 5fda 194b 7546 6c6f 7752 6573 7443  c__..KuFlowRestC
-00003cd0: 6c69 656e 7447 656e 6572 6174 6564 7210  lientGeneratedr.
-00003ce0: 0000 00da 0369 6e74 7205 0000 0072 0600  .....intr....r..
-00003cf0: 0000 721b 0000 0072 0400 0000 721c 0000  ..r....r....r...
-00003d00: 0072 1d00 0000 7202 0000 00da 0854 6173  .r....r......Tas
-00003d10: 6b50 6167 6572 1f00 0000 da04 5461 736b  kPager......Task
-00003d20: 7221 0000 0072 2300 0000 7225 0000 00da  r!...r#...r%....
-00003d30: 1154 6173 6b41 7373 6967 6e43 6f6d 6d61  .TaskAssignComma
-00003d40: 6e64 7228 0000 00da 1654 6173 6b53 6176  ndr(.....TaskSav
-00003d50: 6545 6c65 6d65 6e74 436f 6d6d 616e 6472  eElementCommandr
-00003d60: 2a00 0000 da08 446f 6375 6d65 6e74 da23  *.....Document.#
-00003d70: 5461 736b 5361 7665 456c 656d 656e 7456  TaskSaveElementV
-00003d80: 616c 7565 446f 6375 6d65 6e74 436f 6d6d  alueDocumentComm
-00003d90: 616e 6472 3100 0000 da18 5461 736b 4465  andr1.....TaskDe
-00003da0: 6c65 7465 456c 656d 656e 7443 6f6d 6d61  leteElementComma
-00003db0: 6e64 7236 0000 00da 2554 6173 6b44 656c  ndr6....%TaskDel
-00003dc0: 6574 6545 6c65 6d65 6e74 5661 6c75 6544  eteElementValueD
-00003dd0: 6f63 756d 656e 7443 6f6d 6d61 6e64 7237  ocumentCommandr7
-00003de0: 0000 0072 0300 0000 da05 6279 7465 7372  ...r......bytesr
-00003df0: 3900 0000 723a 0000 00da 2154 6173 6b53  9...r:....!TaskS
-00003e00: 6176 654a 736f 6e46 6f72 6d73 5661 6c75  aveJsonFormsValu
-00003e10: 6544 6174 6143 6f6d 6d61 6e64 723b 0000  eDataCommandr;..
-00003e20: 00da 2c54 6173 6b53 6176 654a 736f 6e46  ..,TaskSaveJsonF
-00003e30: 6f72 6d73 5661 6c75 6544 6f63 756d 656e  ormsValueDocumen
-00003e40: 7452 6571 7565 7374 436f 6d6d 616e 64da  tRequestCommand.
-00003e50: 2d54 6173 6b53 6176 654a 736f 6e46 6f72  -TaskSaveJsonFor
-00003e60: 6d73 5661 6c75 6544 6f63 756d 656e 7452  msValueDocumentR
-00003e70: 6573 706f 6e73 6543 6f6d 6d61 6e64 723d  esponseCommandr=
-00003e80: 0000 0072 3f00 0000 7240 0000 00da 034c  ...r?...r@.....L
-00003e90: 6f67 7242 0000 0072 0e00 0000 720e 0000  ogrB...r....r...
-00003ea0: 0072 0e00 0000 720f 0000 0072 0a00 0000  .r....r....r....
-00003eb0: 2200 0000 7386 0000 0008 0104 090e 0500  "...s...........
-00003ec0: 0100 0100 0100 0100 0100 f902 0202 0102  ................
-00003ed0: 0112 0112 0116 0112 0102 0104 f70c 371e  ..............7.
-00003ee0: 2014 0d14 0d18 1002 0004 0002 0104 fe0c   ...............
-00003ef0: 1a02 0004 0004 0002 0104 fe0c 2102 0004  ............!...
-00003f00: 0002 0104 fe0c 1402 0004 0002 0104 fe0c  ................
-00003f10: 1418 1202 0002 0002 0106 fe0c 1802 0104  ................
-00003f20: 0102 0104 fb0c 1802 0104 0104 0102 0104  ................
-00003f30: fa0c 1f02 0002 0002 0106 fe0c 1514 0d72  ...............r
-00003f40: 0a00 0000 4e29 0dda 0674 7970 696e 6772  ....N)...typingr
-00003f50: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
-00003f60: 0000 0072 0600 0000 da0a 5f67 656e 6572  ...r......_gener
-00003f70: 6174 6564 7208 0000 0072 4700 0000 da00  atedr....rG.....
-00003f80: 7209 0000 0072 1c00 0000 720a 0000 0072  r....r....r....r
-00003f90: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00003fa0: 0000 00da 083c 6d6f 6475 6c65 3e1b 0000  .....<module>...
-00003fb0: 0073 0600 0000 1c02 0c02 0c03            .s..........
+00000400: 6400 5300 2901 4e29 01da 0e5f 6b75 666c  d.S.).N)..._kufl
+00000410: 6f77 5f63 6c69 656e 7429 02da 0473 656c  ow_client)...sel
+00000420: 6672 0b00 0000 a900 720e 0000 00fa 4e2f  fr......r.....N/
+00000430: 776f 726b 2f6b 7566 6c6f 772d 7364 6b2d  work/kuflow-sdk-
+00000440: 7079 7468 6f6e 2f6b 7566 6c6f 772d 7265  python/kuflow-re
+00000450: 7374 2f6b 7566 6c6f 775f 7265 7374 2f6f  st/kuflow_rest/o
+00000460: 7065 7261 7469 6f6e 732f 5f74 6173 6b5f  perations/_task_
+00000470: 6f70 6572 6174 696f 6e73 2e70 79da 085f  operations.py.._
+00000480: 5f69 6e69 745f 5f2c 0000 0073 0200 0000  _init__,...s....
+00000490: 0001 7a17 5461 736b 4f70 6572 6174 696f  ..z.TaskOperatio
+000004a0: 6e73 2e5f 5f69 6e69 745f 5fe9 1900 0000  ns.__init__.....
+000004b0: 7201 0000 004e 2908 da04 7369 7a65 da04  r....N)...size..
+000004c0: 7061 6765 da04 736f 7274 da0a 7072 6f63  page..sort..proc
+000004d0: 6573 735f 6964 da05 7374 6174 65da 1474  ess_id..state..t
+000004e0: 6173 6b5f 6465 6669 6e69 7469 6f6e 5f63  ask_definition_c
+000004f0: 6f64 65da 066b 7761 7267 73da 0672 6574  ode..kwargs..ret
+00000500: 7572 6e63 0700 0000 0000 0000 0000 0000  urnc............
+00000510: 0800 0000 0900 0000 4b00 0000 7384 0000  ........K...s...
+00000520: 007c 0364 016b 0972 1874 007c 0374 0183  .|.d.k.r.t.|.t..
+00000530: 0272 187c 0367 017d 037c 0464 016b 0972  .r.|.g.}.|.d.k.r
+00000540: 3074 007c 0474 0183 0272 307c 0467 017d  0t.|.t...r0|.g.}
+00000550: 047c 0564 016b 0972 4a74 007c 0574 026a  .|.d.k.rJt.|.t.j
+00000560: 0383 0272 4a7c 0567 017d 057c 0664 016b  ...rJ|.g.}.|.d.k
+00000570: 0972 6274 007c 0674 0183 0272 627c 0667  .rbt.|.t...rb|.g
+00000580: 017d 067c 006a 046a 056a 0666 007c 017c  .}.|.j.j.j.f.|.|
+00000590: 027c 037c 047c 057c 0664 029c 067c 0797  .|.|.|.|.d...|..
+000005a0: 028e 0153 0029 0361 8405 0000 4669 6e64  ...S.).a....Find
+000005b0: 2061 6c6c 2061 6363 6573 7369 626c 6520   all accessible 
+000005c0: 5461 736b 732e 0a0a 2020 2020 2020 2020  Tasks...        
+000005d0: 4c69 7374 2061 6c6c 2054 6173 6b73 2074  List all Tasks t
+000005e0: 6861 7420 6861 7665 2062 6565 6e20 6372  hat have been cr
+000005f0: 6561 7465 6420 616e 6420 7468 6520 6372  eated and the cr
+00000600: 6564 656e 7469 616c 7320 6861 7320 6163  edentials has ac
+00000610: 6365 7373 2e0a 0a20 2020 2020 2020 2041  cess...        A
+00000620: 7661 696c 6162 6c65 2073 6f72 7420 7175  vailable sort qu
+00000630: 6572 7920 7661 6c75 6573 3a20 6964 2c20  ery values: id, 
+00000640: 6372 6561 7465 6441 742c 206c 6173 744d  createdAt, lastM
+00000650: 6f64 6966 6965 6441 742c 2063 6c61 696d  odifiedAt, claim
+00000660: 6564 4174 2c20 636f 6d70 6c65 7465 6441  edAt, completedA
+00000670: 742c 0a20 2020 2020 2020 2063 616e 6365  t,.        cance
+00000680: 6c6c 6564 4174 2e0a 0a20 2020 2020 2020  lledAt...       
+00000690: 203a 6b65 7977 6f72 6420 7369 7a65 3a20   :keyword size: 
+000006a0: 5468 6520 6e75 6d62 6572 206f 6620 7265  The number of re
+000006b0: 636f 7264 7320 7265 7475 726e 6564 2077  cords returned w
+000006c0: 6974 6869 6e20 6120 7369 6e67 6c65 2041  ithin a single A
+000006d0: 5049 2063 616c 6c2e 2044 6566 6175 6c74  PI call. Default
+000006e0: 2076 616c 7565 2069 7320 3235 2e0a 2020   value is 25..  
+000006f0: 2020 2020 2020 3a74 7970 6520 7369 7a65        :type size
+00000700: 3a20 696e 740a 2020 2020 2020 2020 3a6b  : int.        :k
+00000710: 6579 776f 7264 2070 6167 653a 2054 6865  eyword page: The
+00000720: 2070 6167 6520 6e75 6d62 6572 206f 6620   page number of 
+00000730: 7468 6520 6375 7272 656e 7420 7061 6765  the current page
+00000740: 2069 6e20 7468 6520 7265 7475 726e 6564   in the returned
+00000750: 2072 6563 6f72 6473 2c20 3020 6973 2074   records, 0 is t
+00000760: 6865 2066 6972 7374 2070 6167 652e 0a20  he first page.. 
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 2020 2020 2020 4465 6661 756c 7420 7661        Default va
+00000790: 6c75 6520 6973 2030 2e0a 2020 2020 2020  lue is 0..      
+000007a0: 2020 3a74 7970 6520 7061 6765 3a20 696e    :type page: in
+000007b0: 740a 2020 2020 2020 2020 3a6b 6579 776f  t.        :keywo
+000007c0: 7264 2073 6f72 743a 2053 6f72 7469 6e67  rd sort: Sorting
+000007d0: 2063 7269 7465 7269 6120 696e 2074 6865   criteria in the
+000007e0: 2066 6f72 6d61 743a 2070 726f 7065 7274   format: propert
+000007f0: 797b 2c61 7363 7c64 6573 637d 2e20 4578  y{,asc|desc}. Ex
+00000800: 616d 706c 653a 2063 7265 6174 6564 4174  ample: createdAt
+00000810: 2c64 6573 630a 2020 2020 2020 2020 2020  ,desc.          
+00000820: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00000830: 6175 6c74 2073 6f72 7420 6f72 6465 7220  ault sort order 
+00000840: 6973 2061 7363 656e 6469 6e67 2e20 4d75  is ascending. Mu
+00000850: 6c74 6970 6c65 2073 6f72 7420 6372 6974  ltiple sort crit
+00000860: 6572 6961 2061 7265 2073 7570 706f 7274  eria are support
+00000870: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00000880: 2020 2020 2020 2020 2020 2050 6c65 6173             Pleas
+00000890: 6520 7265 6665 7220 746f 2074 6865 206d  e refer to the m
+000008a0: 6574 686f 6420 6465 7363 7269 7074 696f  ethod descriptio
+000008b0: 6e20 666f 7220 7375 7070 6f72 7465 6420  n for supported 
+000008c0: 7072 6f70 6572 7469 6573 2e20 4465 6661  properties. Defa
+000008d0: 756c 7420 7661 6c75 6520 6973 204e 6f6e  ult value is Non
+000008e0: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
+000008f0: 2073 6f72 743a 206c 6973 745b 7374 725d   sort: list[str]
+00000900: 0a20 2020 2020 2020 203a 6b65 7977 6f72  .        :keywor
+00000910: 6420 7072 6f63 6573 735f 6964 3a20 4669  d process_id: Fi
+00000920: 6c74 6572 2062 7920 616e 2061 7272 6179  lter by an array
+00000930: 206f 6620 7072 6f63 6573 7320 6964 732e   of process ids.
+00000940: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
+00000950: 7320 4e6f 6e65 2e0a 2020 2020 2020 2020  s None..        
+00000960: 3a74 7970 6520 7072 6f63 6573 735f 6964  :type process_id
+00000970: 3a20 6c69 7374 5b73 7472 5d0a 2020 2020  : list[str].    
+00000980: 2020 2020 3a6b 6579 776f 7264 2073 7461      :keyword sta
+00000990: 7465 3a20 4669 6c74 6572 2062 7920 616e  te: Filter by an
+000009a0: 2061 7272 6179 206f 6620 7461 736b 2073   array of task s
+000009b0: 7461 7465 732e 2044 6566 6175 6c74 2076  tates. Default v
+000009c0: 616c 7565 2069 7320 4e6f 6e65 2e0a 2020  alue is None..  
+000009d0: 2020 2020 2020 3a74 7970 6520 7374 6174        :type stat
+000009e0: 653a 206c 6973 745b 7374 7220 6f72 207e  e: list[str or ~
+000009f0: 6b75 666c 6f77 2e72 6573 742e 6d6f 6465  kuflow.rest.mode
+00000a00: 6c73 2e54 6173 6b53 7461 7465 5d0a 2020  ls.TaskState].  
+00000a10: 2020 2020 2020 3a6b 6579 776f 7264 2074        :keyword t
+00000a20: 6173 6b5f 6465 6669 6e69 7469 6f6e 5f63  ask_definition_c
+00000a30: 6f64 653a 2046 696c 7465 7220 6279 2061  ode: Filter by a
+00000a40: 6e20 6172 7261 7920 6f66 2074 6173 6b20  n array of task 
+00000a50: 6465 6669 6e69 7469 6f6e 2063 6f64 6573  definition codes
+00000a60: 2e20 4465 6661 756c 7420 7661 6c75 6520  . Default value 
+00000a70: 6973 204e 6f6e 652e 0a20 2020 2020 2020  is None..       
+00000a80: 203a 7479 7065 2074 6173 6b5f 6465 6669   :type task_defi
+00000a90: 6e69 7469 6f6e 5f63 6f64 653a 206c 6973  nition_code: lis
+00000aa0: 745b 7374 725d 0a20 2020 2020 2020 203a  t[str].        :
+00000ab0: 7265 7475 726e 3a20 5461 736b 5061 6765  return: TaskPage
+00000ac0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00000ad0: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
+00000ae0: 6465 6c73 2e54 6173 6b50 6167 650a 2020  dels.TaskPage.  
+00000af0: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
+00000b00: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
+00000b10: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
+00000b20: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00000b30: 4e29 0672 1200 0000 7213 0000 0072 1400  N).r....r....r..
+00000b40: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000b50: 0029 07da 0a69 7369 6e73 7461 6e63 65da  .)...isinstance.
+00000b60: 0373 7472 da07 5f6d 6f64 656c 73da 0954  .str.._models..T
+00000b70: 6173 6b53 7461 7465 720c 0000 00da 0474  askStater......t
+00000b80: 6173 6bda 0a66 696e 645f 7461 736b 7329  ask..find_tasks)
+00000b90: 0872 0d00 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000ba0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000bb0: 1700 0000 7218 0000 0072 0e00 0000 720e  ....r....r....r.
+00000bc0: 0000 0072 0f00 0000 721f 0000 002f 0000  ...r....r..../..
+00000bd0: 0073 2400 0000 0024 1201 0601 1201 0601  .s$....$........
+00000be0: 1401 0601 1201 0602 0a01 0201 0201 0201  ................
+00000bf0: 0201 0201 02fa 0407 02f9 7a19 5461 736b  ..........z.Task
+00000c00: 4f70 6572 6174 696f 6e73 2e66 696e 645f  Operations.find_
+00000c10: 7461 736b 7329 0472 1e00 0000 da0e 6163  tasks).r......ac
+00000c20: 7469 7669 7479 5f74 6f6b 656e 7218 0000  tivity_tokenr...
+00000c30: 0072 1900 0000 6303 0000 0000 0000 0000  .r....c.........
+00000c40: 0000 0004 0000 0005 0000 004b 0000 0073  ...........K...s
+00000c50: 1a00 0000 7c00 6a00 6a01 6a02 6600 7c01  ....|.j.j.j.f.|.
+00000c60: 7c02 6401 9c02 7c03 9702 8e01 5300 2902  |.d...|.....S.).
+00000c70: 61ba 0500 0043 7265 6174 6520 6120 6e65  a....Create a ne
+00000c80: 7720 5461 736b 2069 6e20 7468 6520 7365  w Task in the se
+00000c90: 6c65 6374 6564 2050 726f 6365 7373 2e0a  lected Process..
+00000ca0: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
+00000cb0: 6120 5461 736b 2061 6e64 206f 7074 696f  a Task and optio
+00000cc0: 6e61 6c6c 7920 6669 6c6c 2069 7473 2065  nally fill its e
+00000cd0: 6c65 6d65 6e74 732e 2057 6520 6361 6e20  lements. We can 
+00000ce0: 6669 6c6c 2069 6e20 616e 7920 7479 7065  fill in any type
+00000cf0: 206f 6620 656c 656d 656e 7420 6578 6365   of element exce
+00000d00: 7074 0a20 2020 2020 2020 2064 6f63 756d  pt.        docum
+00000d10: 656e 7473 2e0a 0a20 2020 2020 2020 2049  ents...        I
+00000d20: 6620 796f 7520 7761 6e74 2074 6f20 6164  f you want to ad
+00000d30: 6420 646f 6375 6d65 6e74 2074 7970 6520  d document type 
+00000d40: 656c 656d 656e 7473 2c20 796f 7520 6361  elements, you ca
+00000d50: 6e20 7061 7373 2061 2072 6566 6572 656e  n pass a referen
+00000d60: 6365 2074 6f20 616e 2065 7869 7374 696e  ce to an existin
+00000d70: 6720 646f 6375 6d65 6e74 0a20 2020 2020  g document.     
+00000d80: 2020 2074 7970 6520 656c 656d 656e 7420     type element 
+00000d90: 696e 6469 6361 7469 6e67 2069 7473 2027  indicating its '
+00000da0: 7572 6927 2e20 5468 6973 2077 696c 6c20  uri'. This will 
+00000db0: 636f 7079 2074 6861 7420 646f 6375 6d65  copy that docume
+00000dc0: 6e74 2069 6e74 6f20 7468 6520 656c 656d  nt into the elem
+00000dd0: 656e 742e 2049 6e20 6361 7365 2079 6f75  ent. In case you
+00000de0: 0a20 2020 2020 2020 2077 616e 7420 746f  .        want to
+00000df0: 2061 6464 2061 206e 6577 2064 6f63 756d   add a new docum
+00000e00: 656e 742c 2070 6c65 6173 6520 7573 6520  ent, please use 
+00000e10: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+00000e20: 6720 4150 4920 6d65 7468 6f64 2e0a 0a20  g API method... 
+00000e30: 2020 2020 2020 2049 6620 796f 7520 7761         If you wa
+00000e40: 6e74 2074 6861 7420 7468 6520 7461 736b  nt that the task
+00000e50: 2063 7265 6174 6564 2069 7320 636c 6169   created is clai
+00000e60: 6d65 6420 796f 7520 6361 6e20 6120 7661  med you can a va
+00000e70: 6c69 6420 6f77 6e65 7220 7573 696e 6720  lid owner using 
+00000e80: 7468 6520 666f 6c6c 6f77 696e 6720 6f70  the following op
+00000e90: 7469 6f6e 733a 0a0a 0a20 2020 2020 2020  tions:...       
+00000ea0: 202a 2049 6620 796f 7520 6b6e 6f77 2074   * If you know t
+00000eb0: 6865 2060 6070 7269 6e63 6970 616c 2049  he ``principal I
+00000ec0: 4460 6020 796f 7520 6361 6e20 6173 7369  D`` you can assi
+00000ed0: 676e 2069 7420 746f 2060 606f 776e 6572  gn it to ``owner
+00000ee0: 2e69 6460 600a 2020 2020 2020 2020 2a20  .id``.        * 
+00000ef0: 4966 2079 6f75 206b 6e6f 7720 7468 6520  If you know the 
+00000f00: 6060 7573 6572 2049 4460 6020 796f 7520  ``user ID`` you 
+00000f10: 6361 6e20 6173 7369 676e 2069 7420 746f  can assign it to
+00000f20: 2060 606f 776e 6572 2e75 7365 722e 6964   ``owner.user.id
+00000f30: 6060 0a20 2020 2020 2020 202a 2049 6620  ``.        * If 
+00000f40: 796f 7520 6b6e 6f77 2074 6865 2060 6075  you know the ``u
+00000f50: 7365 7220 656d 6169 6c60 6020 796f 7520  ser email`` you 
+00000f60: 6361 6e20 6173 7369 676e 2069 7420 746f  can assign it to
+00000f70: 2060 606f 776e 6572 2e75 7365 722e 656d   ``owner.user.em
+00000f80: 6169 6c60 600a 2020 2020 2020 2020 2a20  ail``.        * 
+00000f90: 4966 2079 6f75 206b 6e6f 7720 7468 6520  If you know the 
+00000fa0: 6060 6170 706c 6963 6174 696f 6e20 4944  ``application ID
+00000fb0: 6060 2079 6f75 2063 616e 2061 7373 6967  `` you can assig
+00000fc0: 6e20 6974 2074 6f20 6060 6f77 6e65 722e  n it to ``owner.
+00000fd0: 6170 706c 6963 6174 696f 6e2e 6964 6060  application.id``
+00000fe0: 0a0a 2020 2020 2020 2020 4966 2079 6f75  ..        If you
+00000ff0: 2077 616e 7420 7468 6520 6d65 7468 6f64   want the method
+00001000: 2074 6f20 6265 2069 6465 6d70 6f74 656e   to be idempoten
+00001010: 742c 2070 6c65 6173 6520 7370 6563 6966  t, please specif
+00001020: 7920 7468 6520 6060 6964 6060 2066 6965  y the ``id`` fie
+00001030: 6c64 2069 6e20 7468 6520 7265 7175 6573  ld in the reques
+00001040: 7420 626f 6479 2e0a 0a20 2020 2020 2020  t body...       
+00001050: 203a 7061 7261 6d20 7461 736b 3a20 5461   :param task: Ta
+00001060: 736b 2074 6f20 6265 2063 7265 6174 6564  sk to be created
+00001070: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
+00001080: 2020 2020 3a74 7970 6520 7461 736b 3a20      :type task: 
+00001090: 7e6b 7566 6c6f 772e 7265 7374 2e6d 6f64  ~kuflow.rest.mod
+000010a0: 656c 732e 5461 736b 0a20 2020 2020 2020  els.Task.       
+000010b0: 203a 6b65 7977 6f72 6420 6163 7469 7669   :keyword activi
+000010c0: 7479 5f74 6f6b 656e 3a20 5768 656e 2063  ty_token: When c
+000010d0: 7265 6174 6520 6120 4b75 666c 6f77 2054  reate a Kuflow T
+000010e0: 6173 6b20 6261 636b 6564 2077 6974 6820  ask backed with 
+000010f0: 6120 5465 6d70 6f72 616c 2e69 6f20 7365  a Temporal.io se
+00001100: 7276 6572 732c 2074 6869 730a 2020 2020  rvers, this.    
+00001110: 2020 2020 2076 616c 7565 2069 7320 7265       value is re
+00001120: 7175 6972 6564 2061 6e64 206d 7573 7420  quired and must 
+00001130: 6265 2073 6574 2077 6974 6820 7468 6520  be set with the 
+00001140: 636f 6e74 6578 7420 7461 736b 2074 6f6b  context task tok
+00001150: 656e 206f 6620 5465 6d70 6f72 616c 2e69  en of Temporal.i
+00001160: 6f20 6163 7469 7669 7479 2e20 4465 6661  o activity. Defa
+00001170: 756c 740a 2020 2020 2020 2020 2076 616c  ult.         val
+00001180: 7565 2069 7320 4e6f 6e65 2e0a 2020 2020  ue is None..    
+00001190: 2020 2020 3a74 7970 6520 6163 7469 7669      :type activi
+000011a0: 7479 5f74 6f6b 656e 3a20 7374 720a 2020  ty_token: str.  
+000011b0: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
+000011c0: 6173 6b0a 2020 2020 2020 2020 3a72 7479  ask.        :rty
+000011d0: 7065 3a20 7e6b 7566 6c6f 772e 7265 7374  pe: ~kuflow.rest
+000011e0: 2e6d 6f64 656c 732e 5461 736b 0a20 2020  .models.Task.   
+000011f0: 2020 2020 203a 7261 6973 6573 207e 617a       :raises ~az
+00001200: 7572 652e 636f 7265 2e65 7863 6570 7469  ure.core.excepti
+00001210: 6f6e 732e 4874 7470 5265 7370 6f6e 7365  ons.HttpResponse
+00001220: 4572 726f 723a 0a20 2020 2020 2020 2029  Error:.        )
+00001230: 0272 1e00 0000 7220 0000 0029 0372 0c00  .r....r ...).r..
+00001240: 0000 721e 0000 00da 0b63 7265 6174 655f  ..r......create_
+00001250: 7461 736b 2904 720d 0000 0072 1e00 0000  task).r....r....
+00001260: 7220 0000 0072 1800 0000 720e 0000 0072  r ...r....r....r
+00001270: 0e00 0000 720f 0000 0072 2100 0000 6600  ....r....r!...f.
+00001280: 0000 7302 0000 0000 1e7a 1a54 6173 6b4f  ..s......z.TaskO
+00001290: 7065 7261 7469 6f6e 732e 6372 6561 7465  perations.create
+000012a0: 5f74 6173 6b29 03da 0269 6472 1800 0000  _task)...idr....
+000012b0: 7219 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000012c0: 0000 0300 0000 0400 0000 4b00 0000 7318  ..........K...s.
+000012d0: 0000 007c 006a 006a 016a 0266 0064 017c  ...|.j.j.j.f.d.|
+000012e0: 0169 017c 0297 028e 0153 0029 0261 0201  .i.|.....S.).a..
+000012f0: 0000 4765 7420 6120 7461 736b 2067 6976  ..Get a task giv
+00001300: 656e 2069 7420 4944 2e0a 0a20 2020 2020  en it ID...     
+00001310: 2020 2041 6c6c 6f77 2074 6f20 6765 7420     Allow to get 
+00001320: 6120 7461 736b 2062 7920 4944 2e0a 0a20  a task by ID... 
+00001330: 2020 2020 2020 203a 7061 7261 6d20 6964         :param id
+00001340: 3a20 5468 6520 7265 736f 7572 6365 2049  : The resource I
+00001350: 442e 2052 6571 7569 7265 642e 0a20 2020  D. Required..   
+00001360: 2020 2020 203a 7479 7065 2069 643a 2073       :type id: s
+00001370: 7472 0a20 2020 2020 2020 203a 7265 7475  tr.        :retu
+00001380: 726e 3a20 5461 736b 0a20 2020 2020 2020  rn: Task.       
+00001390: 203a 7274 7970 653a 207e 6b75 666c 6f77   :rtype: ~kuflow
+000013a0: 2e72 6573 742e 6d6f 6465 6c73 2e54 6173  .rest.models.Tas
+000013b0: 6b0a 2020 2020 2020 2020 3a72 6169 7365  k.        :raise
+000013c0: 7320 7e61 7a75 7265 2e63 6f72 652e 6578  s ~azure.core.ex
+000013d0: 6365 7074 696f 6e73 2e48 7474 7052 6573  ceptions.HttpRes
+000013e0: 706f 6e73 6545 7272 6f72 3a0a 2020 2020  ponseError:.    
+000013f0: 2020 2020 7222 0000 0029 0372 0c00 0000      r"...).r....
+00001400: 721e 0000 00da 0d72 6574 7269 6576 655f  r......retrieve_
+00001410: 7461 736b a903 720d 0000 0072 2200 0000  task..r....r"...
+00001420: 7218 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00001430: 0f00 0000 7223 0000 0086 0000 0073 0200  ....r#.......s..
+00001440: 0000 000b 7a1c 5461 736b 4f70 6572 6174  ....z.TaskOperat
+00001450: 696f 6e73 2e72 6574 7269 6576 655f 7461  ions.retrieve_ta
+00001460: 736b 6302 0000 0000 0000 0000 0000 0003  skc.............
+00001470: 0000 0004 0000 004b 0000 0073 1800 0000  .......K...s....
+00001480: 7c00 6a00 6a01 6a02 6600 6401 7c01 6901  |.j.j.j.f.d.|.i.
+00001490: 7c02 9702 8e01 5300 2902 7af4 436c 6169  |.....S.).z.Clai
+000014a0: 6d20 6120 7461 736b 2e0a 0a20 2020 2020  m a task...     
+000014b0: 2020 2041 6c6c 6f77 2074 6f20 636c 6169     Allow to clai
+000014c0: 6d20 6120 7461 736b 2e0a 0a20 2020 2020  m a task...     
+000014d0: 2020 203a 7061 7261 6d20 6964 3a20 5468     :param id: Th
+000014e0: 6520 7265 736f 7572 6365 2049 442e 2052  e resource ID. R
+000014f0: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
+00001500: 203a 7479 7065 2069 643a 2073 7472 0a20   :type id: str. 
+00001510: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00001520: 5461 736b 0a20 2020 2020 2020 203a 7274  Task.        :rt
+00001530: 7970 653a 207e 6b75 666c 6f77 2e72 6573  ype: ~kuflow.res
+00001540: 742e 6d6f 6465 6c73 2e54 6173 6b0a 2020  t.models.Task.  
+00001550: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
+00001560: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
+00001570: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
+00001580: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00001590: 7222 0000 0029 0372 0c00 0000 721e 0000  r"...).r....r...
+000015a0: 00da 1261 6374 696f 6e73 5f74 6173 6b5f  ...actions_task_
+000015b0: 636c 6169 6d72 2400 0000 720e 0000 0072  claimr$...r....r
+000015c0: 0e00 0000 720f 0000 0072 2500 0000 9300  ....r....r%.....
+000015d0: 0000 7302 0000 0000 0b7a 2154 6173 6b4f  ..s......z!TaskO
+000015e0: 7065 7261 7469 6f6e 732e 6163 7469 6f6e  perations.action
+000015f0: 735f 7461 736b 5f63 6c61 696d 2904 7222  s_task_claim).r"
+00001600: 0000 00da 0763 6f6d 6d61 6e64 7218 0000  .....commandr...
+00001610: 0072 1900 0000 6303 0000 0000 0000 0000  .r....c.........
+00001620: 0000 0004 0000 0005 0000 004b 0000 0073  ...........K...s
+00001630: 1a00 0000 7c00 6a00 6a01 6a02 6600 7c01  ....|.j.j.j.f.|.
+00001640: 7c02 6401 9c02 7c03 9702 8e01 5300 2902  |.d...|.....S.).
+00001650: 61b3 0100 0041 7373 6967 6e20 6120 7461  a....Assign a ta
+00001660: 736b 2e0a 0a20 2020 2020 2020 2041 6c6c  sk...        All
+00001670: 6f77 2074 6f20 6173 7369 676e 2061 2074  ow to assign a t
+00001680: 6173 6b20 746f 2061 2075 7365 7220 6f72  ask to a user or
+00001690: 2061 7070 6c69 6361 7469 6f6e 2e20 4f6e   application. On
+000016a0: 6c79 206f 6e65 206f 7074 696f 6e20 7769  ly one option wi
+000016b0: 6c6c 2062 6520 6e65 6365 7373 6172 792e  ll be necessary.
+000016c0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000016d0: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
+000016e0: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
+000016f0: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
+00001700: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
+00001710: 6172 616d 2063 6f6d 6d61 6e64 3a20 436f  aram command: Co
+00001720: 6d6d 616e 6420 746f 2063 6861 6e67 6520  mmand to change 
+00001730: 7468 6520 7461 736b 206f 776e 6572 2e20  the task owner. 
+00001740: 5265 7175 6972 6564 2e0a 2020 2020 2020  Required..      
+00001750: 2020 3a74 7970 6520 636f 6d6d 616e 643a    :type command:
+00001760: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
+00001770: 6465 6c73 2e54 6173 6b41 7373 6967 6e43  dels.TaskAssignC
+00001780: 6f6d 6d61 6e64 0a20 2020 2020 2020 203a  ommand.        :
+00001790: 7265 7475 726e 3a20 5461 736b 0a20 2020  return: Task.   
+000017a0: 2020 2020 203a 7274 7970 653a 207e 6b75       :rtype: ~ku
+000017b0: 666c 6f77 2e72 6573 742e 6d6f 6465 6c73  flow.rest.models
+000017c0: 2e54 6173 6b0a 2020 2020 2020 2020 3a72  .Task.        :r
+000017d0: 6169 7365 7320 7e61 7a75 7265 2e63 6f72  aises ~azure.cor
+000017e0: 652e 6578 6365 7074 696f 6e73 2e48 7474  e.exceptions.Htt
+000017f0: 7052 6573 706f 6e73 6545 7272 6f72 3a0a  pResponseError:.
+00001800: 2020 2020 2020 2020 a902 7222 0000 0072          ..r"...r
+00001810: 2600 0000 2903 720c 0000 0072 1e00 0000  &...).r....r....
+00001820: da13 6163 7469 6f6e 735f 7461 736b 5f61  ..actions_task_a
+00001830: 7373 6967 6ea9 0472 0d00 0000 7222 0000  ssign..r....r"..
+00001840: 0072 2600 0000 7218 0000 0072 0e00 0000  .r&...r....r....
+00001850: 720e 0000 0072 0f00 0000 7228 0000 00a0  r....r....r(....
+00001860: 0000 0073 0200 0000 000d 7a22 5461 736b  ...s......z"Task
+00001870: 4f70 6572 6174 696f 6e73 2e61 6374 696f  Operations.actio
+00001880: 6e73 5f74 6173 6b5f 6173 7369 676e 6303  ns_task_assignc.
+00001890: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+000018a0: 0000 004b 0000 0073 1a00 0000 7c00 6a00  ...K...s....|.j.
+000018b0: 6a01 6a02 6600 7c01 7c02 6401 9c02 7c03  j.j.f.|.|.d...|.
+000018c0: 9702 8e01 5300 2902 613d 0400 0053 6176  ....S.).a=...Sav
+000018d0: 6520 616e 2065 6c65 6d65 6e74 2e0a 0a20  e an element... 
+000018e0: 2020 2020 2020 2041 6c6c 6f77 2074 6f20         Allow to 
+000018f0: 7361 7665 2061 6e20 656c 656d 656e 7420  save an element 
+00001900: 692e 652e 2c20 6120 6669 656c 642c 2061  i.e., a field, a
+00001910: 2064 6563 6973 696f 6e2c 2061 2066 6f72   decision, a for
+00001920: 6d2c 2061 2070 7269 6e63 6970 616c 206f  m, a principal o
+00001930: 7220 646f 6375 6d65 6e74 2e0a 0a20 2020  r document...   
+00001940: 2020 2020 2049 6e20 7468 6520 6361 7365       In the case
+00001950: 206f 6620 646f 6375 6d65 6e74 2074 7970   of document typ
+00001960: 6520 656c 656d 656e 7473 2c20 7468 6973  e elements, this
+00001970: 206d 6574 686f 6420 6f6e 6c79 2061 6c6c   method only all
+00001980: 6f77 7320 7265 6665 7265 6e63 6573 2074  ows references t
+00001990: 6f20 6265 206d 6164 6520 746f 206f 7468  o be made to oth
+000019a0: 6572 0a20 2020 2020 2020 2065 7869 7374  er.        exist
+000019b0: 696e 6720 646f 6375 6d65 6e74 2074 7970  ing document typ
+000019c0: 6520 656c 656d 656e 7473 2066 6f72 2074  e elements for t
+000019d0: 6865 2070 7572 706f 7365 206f 6620 636f  he purpose of co
+000019e0: 7079 696e 6720 7468 6174 2066 696c 6520  pying that file 
+000019f0: 696e 746f 2074 6865 2065 6c65 6d65 6e74  into the element
+00001a00: 2e20 546f 2064 6f0a 2020 2020 2020 2020  . To do.        
+00001a10: 7468 6973 2079 6f75 206e 6565 6420 746f  this you need to
+00001a20: 2070 6173 7320 6120 7265 6665 7265 6e63   pass a referenc
+00001a30: 6520 746f 2074 6865 2064 6f63 756d 656e  e to the documen
+00001a40: 7420 7573 696e 6720 7468 6520 2775 7269  t using the 'uri
+00001a50: 2720 6174 7472 6962 7574 652e 2049 6e20  ' attribute. In 
+00001a60: 6361 7365 2079 6f75 2077 616e 740a 2020  case you want.  
+00001a70: 2020 2020 2020 746f 2061 6464 2061 206e        to add a n
+00001a80: 6577 2064 6f63 756d 656e 742c 2070 6c65  ew document, ple
+00001a90: 6173 6520 7573 6520 7468 6520 636f 7272  ase use the corr
+00001aa0: 6573 706f 6e64 696e 6720 4150 4920 6d65  esponding API me
+00001ab0: 7468 6f64 2e20 4966 2076 616c 7565 7320  thod. If values 
+00001ac0: 616c 7265 6164 7920 6578 6973 7420 666f  already exist fo
+00001ad0: 7220 7468 650a 2020 2020 2020 2020 7072  r the.        pr
+00001ae0: 6f76 6964 6564 2065 6c65 6d65 6e74 2063  ovided element c
+00001af0: 6f64 652c 2069 7420 7265 706c 6163 6573  ode, it replaces
+00001b00: 2074 6865 6d20 7769 7468 2074 6865 206e   them with the n
+00001b10: 6577 206f 6e65 732c 206f 7468 6572 7769  ew ones, otherwi
+00001b20: 7365 2069 7420 6372 6561 7465 7320 7468  se it creates th
+00001b30: 656d 2e20 5468 650a 2020 2020 2020 2020  em. The.        
+00001b40: 7661 6c75 6573 206f 6620 7468 6520 7072  values of the pr
+00001b50: 6576 696f 7573 2065 6c65 6d65 6e74 7320  evious elements 
+00001b60: 7468 6174 206e 6f20 6c6f 6e67 6572 2065  that no longer e
+00001b70: 7869 7374 2077 696c 6c20 6265 2064 656c  xist will be del
+00001b80: 6574 6564 2e20 546f 2072 656d 6f76 6520  eted. To remove 
+00001b90: 616e 2065 6c65 6d65 6e74 2c20 7573 650a  an element, use.
+00001ba0: 2020 2020 2020 2020 7468 6520 6170 7072          the appr
+00001bb0: 6f70 7269 6174 6520 4150 4920 6d65 7468  opriate API meth
+00001bc0: 6f64 2e0a 0a20 2020 2020 2020 203a 7061  od...        :pa
+00001bd0: 7261 6d20 6964 3a20 5468 6520 7265 736f  ram id: The reso
+00001be0: 7572 6365 2049 442e 2052 6571 7569 7265  urce ID. Require
+00001bf0: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
+00001c00: 2069 643a 2073 7472 0a20 2020 2020 2020   id: str.       
+00001c10: 203a 7061 7261 6d20 636f 6d6d 616e 643a   :param command:
+00001c20: 2043 6f6d 6d61 6e64 2074 6f20 7361 7665   Command to save
+00001c30: 2061 6e20 656c 656d 656e 742e 2052 6571   an element. Req
+00001c40: 7569 7265 642e 0a20 2020 2020 2020 203a  uired..        :
+00001c50: 7479 7065 2063 6f6d 6d61 6e64 3a20 7e6b  type command: ~k
+00001c60: 7566 6c6f 772e 7265 7374 2e6d 6f64 656c  uflow.rest.model
+00001c70: 732e 5461 736b 5361 7665 456c 656d 656e  s.TaskSaveElemen
+00001c80: 7443 6f6d 6d61 6e64 0a20 2020 2020 2020  tCommand.       
+00001c90: 203a 7265 7475 726e 3a20 5461 736b 0a20   :return: Task. 
+00001ca0: 2020 2020 2020 203a 7274 7970 653a 207e         :rtype: ~
+00001cb0: 6b75 666c 6f77 2e72 6573 742e 6d6f 6465  kuflow.rest.mode
+00001cc0: 6c73 2e54 6173 6b0a 2020 2020 2020 2020  ls.Task.        
+00001cd0: 3a72 6169 7365 7320 7e61 7a75 7265 2e63  :raises ~azure.c
+00001ce0: 6f72 652e 6578 6365 7074 696f 6e73 2e48  ore.exceptions.H
+00001cf0: 7474 7052 6573 706f 6e73 6545 7272 6f72  ttpResponseError
+00001d00: 3a0a 2020 2020 2020 2020 7227 0000 0029  :.        r'...)
+00001d10: 0372 0c00 0000 721e 0000 00da 1961 6374  .r....r......act
+00001d20: 696f 6e73 5f74 6173 6b5f 7361 7665 5f65  ions_task_save_e
+00001d30: 6c65 6d65 6e74 7229 0000 0072 0e00 0000  lementr)...r....
+00001d40: 720e 0000 0072 0f00 0000 722a 0000 00af  r....r....r*....
+00001d50: 0000 0073 0200 0000 0017 7a28 5461 736b  ...s......z(Task
+00001d60: 4f70 6572 6174 696f 6e73 2e61 6374 696f  Operations.actio
+00001d70: 6e73 5f74 6173 6b5f 7361 7665 5f65 6c65  ns_task_save_ele
+00001d80: 6d65 6e74 2905 7222 0000 00da 0466 696c  ment).r".....fil
+00001d90: 6572 2600 0000 7218 0000 0072 1900 0000  er&...r....r....
+00001da0: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
+00001db0: 000a 0000 004b 0000 0073 3000 0000 7c00  .....K...s0...|.
+00001dc0: 6a00 6a01 6a02 6600 7c01 7c02 6a03 7c02  j.j.j.f.|.|.j.|.
+00001dd0: 6a04 7c02 6a05 7c03 6a06 7c03 6a07 7c03  j.|.j.|.j.|.j.|.
+00001de0: 6a08 6401 9c07 7c04 9702 8e01 5300 2902  j.d...|.....S.).
+00001df0: 610f 0300 0053 6176 6520 616e 2065 6c65  a....Save an ele
+00001e00: 6d65 6e74 2064 6f63 756d 656e 742e 0a0a  ment document...
+00001e10: 2020 2020 2020 2020 416c 6c6f 7720 746f          Allow to
+00001e20: 2073 6176 6520 616e 2065 6c65 6d65 6e74   save an element
+00001e30: 2064 6f63 756d 656e 7420 7570 6c6f 6164   document upload
+00001e40: 696e 6720 7468 6520 636f 6e74 656e 742e  ing the content.
+00001e50: 0a0a 2020 2020 2020 2020 4966 2069 7420  ..        If it 
+00001e60: 6973 2061 206d 756c 7469 706c 6520 656c  is a multiple el
+00001e70: 656d 656e 742c 2061 6e64 2074 6865 2049  ement, and the I
+00001e80: 4420 7265 6665 7265 6e63 6564 2069 6e20  D referenced in 
+00001e90: 7468 6520 626f 6479 2064 6f65 7320 6e6f  the body does no
+00001ea0: 7420 6578 6973 7420 6f72 2069 7320 656d  t exist or is em
+00001eb0: 7074 792c 2074 6865 0a20 2020 2020 2020  pty, the.       
+00001ec0: 2064 6f63 756d 656e 7420 7769 6c6c 2062   document will b
+00001ed0: 6520 6164 6465 6420 746f 2074 6865 2065  e added to the e
+00001ee0: 6c65 6d65 6e74 2e20 4966 2074 6865 2065  lement. If the e
+00001ef0: 6c65 6d65 6e74 2061 6c72 6561 6479 2065  lement already e
+00001f00: 7869 7374 7320 2874 6865 2049 4420 7265  xists (the ID re
+00001f10: 6665 7265 6e63 6564 2069 6e20 7468 650a  ferenced in the.
+00001f20: 2020 2020 2020 2020 626f 6479 2063 6f72          body cor
+00001f30: 7265 7370 6f6e 6473 2074 6f20 616e 2065  responds to an e
+00001f40: 7869 7374 696e 6720 6f6e 6529 2c20 6974  xisting one), it
+00001f50: 2075 7064 6174 6573 2069 742e 0a0a 2020   updates it...  
+00001f60: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
+00001f70: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
+00001f80: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
+00001f90: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
+00001fa0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+00001fb0: 2066 696c 653a 2044 6f63 756d 656e 7420   file: Document 
+00001fc0: 746f 2073 6176 652e 2052 6571 7569 7265  to save. Require
+00001fd0: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
+00001fe0: 2066 696c 653a 207e 6b75 666c 6f77 2e72   file: ~kuflow.r
+00001ff0: 6573 742e 6d6f 6465 6c73 2e44 6f63 756d  est.models.Docum
+00002000: 656e 740a 2020 2020 2020 2020 3a70 6172  ent.        :par
+00002010: 616d 2063 6f6d 6d61 6e64 3a20 436f 6d6d  am command: Comm
+00002020: 616e 6420 696e 666f 2e20 5265 7175 6972  and info. Requir
+00002030: 6564 2e0a 2020 2020 2020 2020 3a74 7970  ed..        :typ
+00002040: 6520 636f 6d6d 616e 643a 207e 6b75 666c  e command: ~kufl
+00002050: 6f77 2e72 6573 742e 6d6f 6465 6c73 2e54  ow.rest.models.T
+00002060: 6173 6b53 6176 6545 6c65 6d65 6e74 5661  askSaveElementVa
+00002070: 6c75 6544 6f63 756d 656e 7443 6f6d 6d61  lueDocumentComma
+00002080: 6e64 0a20 2020 2020 2020 203a 7265 7475  nd.        :retu
+00002090: 726e 3a20 5461 736b 0a20 2020 2020 2020  rn: Task.       
+000020a0: 203a 7274 7970 653a 207e 6b75 666c 6f77   :rtype: ~kuflow
+000020b0: 2e72 6573 742e 6d6f 6465 6c73 2e54 6173  .rest.models.Tas
+000020c0: 6b0a 2020 2020 2020 2020 3a72 6169 7365  k.        :raise
+000020d0: 7320 7e61 7a75 7265 2e63 6f72 652e 6578  s ~azure.core.ex
+000020e0: 6365 7074 696f 6e73 2e48 7474 7052 6573  ceptions.HttpRes
+000020f0: 706f 6e73 6545 7272 6f72 3a0a 2020 2020  ponseError:.    
+00002100: 2020 2020 2907 7222 0000 0072 2b00 0000      ).r"...r+...
+00002110: da11 6669 6c65 5f63 6f6e 7465 6e74 5f74  ..file_content_t
+00002120: 7970 65da 0966 696c 655f 6e61 6d65 da17  ype..file_name..
+00002130: 656c 656d 656e 745f 6465 6669 6e69 7469  element_definiti
+00002140: 6f6e 5f63 6f64 65da 1065 6c65 6d65 6e74  on_code..element
+00002150: 5f76 616c 7565 5f69 64da 1365 6c65 6d65  _value_id..eleme
+00002160: 6e74 5f76 616c 7565 5f76 616c 6964 2909  nt_value_valid).
+00002170: 720c 0000 0072 1e00 0000 da28 6163 7469  r....r.....(acti
+00002180: 6f6e 735f 7461 736b 5f73 6176 655f 656c  ons_task_save_el
+00002190: 656d 656e 745f 7661 6c75 655f 646f 6375  ement_value_docu
+000021a0: 6d65 6e74 da0c 6669 6c65 5f63 6f6e 7465  ment..file_conte
+000021b0: 6e74 da0c 636f 6e74 656e 745f 7479 7065  nt..content_type
+000021c0: da09 6669 6c65 5f6d 616d 6572 2e00 0000  ..file_mamer....
+000021d0: 722f 0000 0072 3000 0000 a905 720d 0000  r/...r0.....r...
+000021e0: 0072 2200 0000 722b 0000 0072 2600 0000  .r"...r+...r&...
+000021f0: 7218 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00002200: 0f00 0000 7231 0000 00c8 0000 0073 1600  ....r1.......s..
+00002210: 0000 0015 0a01 0201 0401 0401 0401 0401  ................
+00002220: 0401 04f9 0408 02f8 7a37 5461 736b 4f70  ........z7TaskOp
+00002230: 6572 6174 696f 6e73 2e61 6374 696f 6e73  erations.actions
+00002240: 5f74 6173 6b5f 7361 7665 5f65 6c65 6d65  _task_save_eleme
+00002250: 6e74 5f76 616c 7565 5f64 6f63 756d 656e  nt_value_documen
+00002260: 7463 0300 0000 0000 0000 0000 0000 0400  tc..............
+00002270: 0000 0500 0000 4b00 0000 731a 0000 007c  ......K...s....|
+00002280: 006a 006a 016a 0266 007c 017c 0264 019c  .j.j.j.f.|.|.d..
+00002290: 027c 0397 028e 0153 0029 0261 db01 0000  .|.....S.).a....
+000022a0: 4465 6c65 7465 2061 6e20 656c 656d 656e  Delete an elemen
+000022b0: 7420 6279 2063 6f64 652e 0a0a 2020 2020  t by code...    
+000022c0: 2020 2020 416c 6c6f 7720 746f 2064 656c      Allow to del
+000022d0: 6574 6520 7461 736b 2065 6c65 6d65 6e74  ete task element
+000022e0: 2062 7920 7370 6563 6966 7969 6e67 2074   by specifying t
+000022f0: 6865 2069 7465 6d20 6465 6669 6e69 7469  he item definiti
+00002300: 6f6e 2063 6f64 652e 0a0a 2020 2020 2020  on code...      
+00002310: 2020 5265 6d6f 7665 2061 6c6c 2074 6865    Remove all the
+00002320: 2065 6c65 6d65 6e74 2076 616c 7565 732e   element values.
+00002330: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00002340: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
+00002350: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
+00002360: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
+00002370: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
+00002380: 6172 616d 2063 6f6d 6d61 6e64 3a20 436f  aram command: Co
+00002390: 6d6d 616e 6420 746f 2064 656c 6574 6520  mmand to delete 
+000023a0: 616e 2065 6c65 6d65 6e74 2e20 5265 7175  an element. Requ
+000023b0: 6972 6564 2e0a 2020 2020 2020 2020 3a74  ired..        :t
+000023c0: 7970 6520 636f 6d6d 616e 643a 207e 6b75  ype command: ~ku
+000023d0: 666c 6f77 2e72 6573 742e 6d6f 6465 6c73  flow.rest.models
+000023e0: 2e54 6173 6b44 656c 6574 6545 6c65 6d65  .TaskDeleteEleme
+000023f0: 6e74 436f 6d6d 616e 640a 2020 2020 2020  ntCommand.      
+00002400: 2020 3a72 6574 7572 6e3a 2054 6173 6b0a    :return: Task.
+00002410: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00002420: 7e6b 7566 6c6f 772e 7265 7374 2e6d 6f64  ~kuflow.rest.mod
+00002430: 656c 732e 5461 736b 0a20 2020 2020 2020  els.Task.       
+00002440: 203a 7261 6973 6573 207e 617a 7572 652e   :raises ~azure.
+00002450: 636f 7265 2e65 7863 6570 7469 6f6e 732e  core.exceptions.
+00002460: 4874 7470 5265 7370 6f6e 7365 4572 726f  HttpResponseErro
+00002470: 723a 0a20 2020 2020 2020 2072 2700 0000  r:.        r'...
+00002480: 2903 720c 0000 0072 1e00 0000 da1b 6163  ).r....r......ac
+00002490: 7469 6f6e 735f 7461 736b 5f64 656c 6574  tions_task_delet
+000024a0: 655f 656c 656d 656e 7472 2900 0000 720e  e_elementr)...r.
+000024b0: 0000 0072 0e00 0000 720f 0000 0072 3600  ...r....r....r6.
+000024c0: 0000 e800 0000 7302 0000 0000 117a 2a54  ......s......z*T
+000024d0: 6173 6b4f 7065 7261 7469 6f6e 732e 6163  askOperations.ac
+000024e0: 7469 6f6e 735f 7461 736b 5f64 656c 6574  tions_task_delet
+000024f0: 655f 656c 656d 656e 7463 0300 0000 0000  e_elementc......
+00002500: 0000 0000 0000 0400 0000 0500 0000 4b00  ..............K.
+00002510: 0000 731a 0000 007c 006a 006a 016a 0266  ..s....|.j.j.j.f
+00002520: 007c 017c 0264 019c 027c 0397 028e 0153  .|.|.d...|.....S
+00002530: 0029 0261 9902 0000 4465 6c65 7465 2061  .).a....Delete a
+00002540: 6e20 656c 656d 656e 7420 646f 6375 6d65  n element docume
+00002550: 6e74 2076 616c 7565 2e0a 0a20 2020 2020  nt value...     
+00002560: 2020 2041 6c6c 6f77 2074 6f20 6465 6c65     Allow to dele
+00002570: 7465 2061 2073 7065 6369 6669 6320 646f  te a specific do
+00002580: 6375 6d65 6e74 2066 726f 6d20 616e 2065  cument from an e
+00002590: 6c65 6d65 6e74 206f 6620 646f 6375 6d65  lement of docume
+000025a0: 6e74 2074 7970 6520 7573 696e 6720 6974  nt type using it
+000025b0: 7320 6964 2e0a 0a20 2020 2020 2020 204e  s id...        N
+000025c0: 6f74 653a 2049 6620 6974 2069 7320 6120  ote: If it is a 
+000025d0: 6d75 6c74 6970 6c65 2069 7465 6d2c 2069  multiple item, i
+000025e0: 7420 7769 6c6c 206f 6e6c 7920 6465 6c65  t will only dele
+000025f0: 7465 2074 6865 2073 7065 6369 6669 6564  te the specified
+00002600: 2064 6f63 756d 656e 742e 2049 6620 6974   document. If it
+00002610: 2069 7320 6120 7369 6e67 6c65 0a20 2020   is a single.   
+00002620: 2020 2020 2065 6c65 6d65 6e74 2c20 696e       element, in
+00002630: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
+00002640: 2064 6f63 756d 656e 742c 2069 7420 7769   document, it wi
+00002650: 6c6c 2061 6c73 6f20 6465 6c65 7465 2074  ll also delete t
+00002660: 6865 2065 6c65 6d65 6e74 2e0a 0a20 2020  he element...   
+00002670: 2020 2020 203a 7061 7261 6d20 6964 3a20       :param id: 
+00002680: 5468 6520 7265 736f 7572 6365 2049 442e  The resource ID.
+00002690: 2052 6571 7569 7265 642e 0a20 2020 2020   Required..     
+000026a0: 2020 203a 7479 7065 2069 643a 2073 7472     :type id: str
+000026b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000026c0: 636f 6d6d 616e 643a 2043 6f6d 6d61 6e64  command: Command
+000026d0: 2074 6f20 6465 6c65 7465 2061 2064 6f63   to delete a doc
+000026e0: 756d 656e 7420 656c 656d 656e 7420 7661  ument element va
+000026f0: 6c75 652e 2052 6571 7569 7265 642e 0a20  lue. Required.. 
+00002700: 2020 2020 2020 203a 7479 7065 2063 6f6d         :type com
+00002710: 6d61 6e64 3a20 7e6b 7566 6c6f 772e 7265  mand: ~kuflow.re
+00002720: 7374 2e6d 6f64 656c 732e 5461 736b 4465  st.models.TaskDe
+00002730: 6c65 7465 456c 656d 656e 7456 616c 7565  leteElementValue
+00002740: 446f 6375 6d65 6e74 436f 6d6d 616e 640a  DocumentCommand.
+00002750: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00002760: 2054 6173 6b0a 2020 2020 2020 2020 3a72   Task.        :r
+00002770: 7479 7065 3a20 7e6b 7566 6c6f 772e 7265  type: ~kuflow.re
+00002780: 7374 2e6d 6f64 656c 732e 5461 736b 0a20  st.models.Task. 
+00002790: 2020 2020 2020 203a 7261 6973 6573 207e         :raises ~
+000027a0: 617a 7572 652e 636f 7265 2e65 7863 6570  azure.core.excep
+000027b0: 7469 6f6e 732e 4874 7470 5265 7370 6f6e  tions.HttpRespon
+000027c0: 7365 4572 726f 723a 0a20 2020 2020 2020  seError:.       
+000027d0: 2072 2700 0000 2903 720c 0000 0072 1e00   r'...).r....r..
+000027e0: 0000 da2a 6163 7469 6f6e 735f 7461 736b  ...*actions_task
+000027f0: 5f64 656c 6574 655f 656c 656d 656e 745f  _delete_element_
+00002800: 7661 6c75 655f 646f 6375 6d65 6e74 7229  value_documentr)
+00002810: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+00002820: 0000 7237 0000 00fb 0000 0073 0200 0000  ..r7.......s....
+00002830: 0012 7a39 5461 736b 4f70 6572 6174 696f  ..z9TaskOperatio
+00002840: 6e73 2e61 6374 696f 6e73 5f74 6173 6b5f  ns.actions_task_
+00002850: 6465 6c65 7465 5f65 6c65 6d65 6e74 5f76  delete_element_v
+00002860: 616c 7565 5f64 6f63 756d 656e 7429 0472  alue_document).r
+00002870: 2200 0000 da0b 646f 6375 6d65 6e74 5f69  ".....document_i
+00002880: 6472 1800 0000 7219 0000 0063 0300 0000  dr....r....c....
+00002890: 0000 0000 0000 0000 0400 0000 0500 0000  ................
+000028a0: 4b00 0000 731a 0000 007c 006a 006a 016a  K...s....|.j.j.j
+000028b0: 0266 007c 017c 0264 019c 027c 0397 028e  .f.|.|.d...|....
+000028c0: 0153 0029 0261 9701 0000 446f 776e 6c6f  .S.).a....Downlo
+000028d0: 6164 2064 6f63 756d 656e 742e 0a0a 2020  ad document...  
+000028e0: 2020 2020 2020 4769 7665 6e20 6120 7461        Given a ta
+000028f0: 736b 2c20 646f 776e 6c6f 6164 2061 2064  sk, download a d
+00002900: 6f63 756d 656e 7420 6672 6f6d 2061 6e20  ocument from an 
+00002910: 656c 656d 656e 7420 6f66 2064 6f63 756d  element of docum
+00002920: 656e 7420 7479 7065 2e0a 0a20 2020 2020  ent type...     
+00002930: 2020 203a 7061 7261 6d20 6964 3a20 5468     :param id: Th
+00002940: 6520 7265 736f 7572 6365 2049 442e 2052  e resource ID. R
+00002950: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
+00002960: 203a 7479 7065 2069 643a 2073 7472 0a20   :type id: str. 
+00002970: 2020 2020 2020 203a 6b65 7977 6f72 6420         :keyword 
+00002980: 646f 6375 6d65 6e74 5f69 643a 2044 6f63  document_id: Doc
+00002990: 756d 656e 7420 4944 2074 6f20 646f 776e  ument ID to down
+000029a0: 6c6f 6164 2e20 5265 7175 6972 6564 2e0a  load. Required..
+000029b0: 2020 2020 2020 2020 3a74 7970 6520 646f          :type do
+000029c0: 6375 6d65 6e74 5f69 643a 2073 7472 0a20  cument_id: str. 
+000029d0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000029e0: 4974 6572 6174 6f72 206f 6620 7468 6520  Iterator of the 
+000029f0: 7265 7370 6f6e 7365 2062 7974 6573 0a20  response bytes. 
+00002a00: 2020 2020 2020 203a 7274 7970 653a 2049         :rtype: I
+00002a10: 7465 7261 746f 725b 6279 7465 735d 0a20  terator[bytes]. 
+00002a20: 2020 2020 2020 203a 7261 6973 6573 207e         :raises ~
+00002a30: 617a 7572 652e 636f 7265 2e65 7863 6570  azure.core.excep
+00002a40: 7469 6f6e 732e 4874 7470 5265 7370 6f6e  tions.HttpRespon
+00002a50: 7365 4572 726f 723a 0a20 2020 2020 2020  seError:.       
+00002a60: 2029 0272 2200 0000 7238 0000 0029 0372   ).r"...r8...).r
+00002a70: 0c00 0000 721e 0000 00da 2c61 6374 696f  ....r.....,actio
+00002a80: 6e73 5f74 6173 6b5f 646f 776e 6c6f 6164  ns_task_download
+00002a90: 5f65 6c65 6d65 6e74 5f76 616c 7565 5f64  _element_value_d
+00002aa0: 6f63 756d 656e 7429 0472 0d00 0000 7222  ocument).r....r"
+00002ab0: 0000 0072 3800 0000 7218 0000 0072 0e00  ...r8...r....r..
+00002ac0: 0000 720e 0000 0072 0f00 0000 7239 0000  ..r....r....r9..
+00002ad0: 000f 0100 0073 0c00 0000 000d 0a01 0200  .....s..........
+00002ae0: 02ff 0401 02ff 7a3b 5461 736b 4f70 6572  ......z;TaskOper
+00002af0: 6174 696f 6e73 2e61 6374 696f 6e73 5f74  ations.actions_t
+00002b00: 6173 6b5f 646f 776e 6c6f 6164 5f65 6c65  ask_download_ele
+00002b10: 6d65 6e74 5f76 616c 7565 5f64 6f63 756d  ment_value_docum
+00002b20: 656e 7429 0472 2200 0000 722e 0000 0072  ent).r"...r....r
+00002b30: 1800 0000 7219 0000 0063 0300 0000 0000  ....r....c......
+00002b40: 0000 0000 0000 0400 0000 0500 0000 4b00  ..............K.
+00002b50: 0000 731a 0000 007c 006a 006a 016a 0266  ..s....|.j.j.j.f
+00002b60: 007c 017c 0264 019c 027c 0397 028e 0153  .|.|.d...|.....S
+00002b70: 0029 0261 a602 0000 446f 776e 6c6f 6164  .).a....Download
+00002b80: 2061 2046 6f72 6d20 7265 6e64 6572 6564   a Form rendered
+00002b90: 2061 7320 5044 4620 6f72 205a 6970 206f   as PDF or Zip o
+00002ba0: 6620 5044 4673 2028 7768 656e 2074 6865  f PDFs (when the
+00002bb0: 2065 6c65 6d65 6e74 2069 7320 6d75 6c74   element is mult
+00002bc0: 6970 6c65 292e 0a0a 2020 2020 2020 2020  iple)...        
+00002bd0: 4769 7665 6e20 6120 7461 736b 2c20 6765  Given a task, ge
+00002be0: 6e65 7261 7465 2061 2050 4446 2066 726f  nerate a PDF fro
+00002bf0: 6d20 6120 466f 726d 2074 7970 6520 656c  m a Form type el
+00002c00: 656d 656e 7420 7769 7468 2074 6865 2064  ement with the d
+00002c10: 6174 6120 6669 6c6c 6564 2069 6e2c 2069  ata filled in, i
+00002c20: 6620 616e 792e 2049 6620 7468 6572 650a  f any. If there.
+00002c30: 2020 2020 2020 2020 6172 6520 6d75 6c74          are mult
+00002c40: 6970 6c65 2066 6f72 6d20 7661 6c75 6573  iple form values
+00002c50: 2c20 7468 6579 2061 7265 2070 6163 6b65  , they are packe
+00002c60: 6420 696e 746f 2061 205a 4950 2e0a 0a20  d into a ZIP... 
+00002c70: 2020 2020 2020 2049 6d70 6f72 7461 6e74         Important
+00002c80: 213a 2054 6f20 7573 6520 7468 6973 2066  !: To use this f
+00002c90: 6561 7475 7265 2c20 706c 6561 7365 2063  eature, please c
+00002ca0: 6f6e 7461 6374 2074 6f20 6b75 666c 6f77  ontact to kuflow
+00002cb0: 406b 7566 6c6f 772e 636f 6d2e 0a0a 2020  @kuflow.com...  
+00002cc0: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
+00002cd0: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
+00002ce0: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
+00002cf0: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
+00002d00: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+00002d10: 2065 6c65 6d65 6e74 5f64 6566 696e 6974   element_definit
+00002d20: 696f 6e5f 636f 6465 3a20 456c 656d 656e  ion_code: Elemen
+00002d30: 7420 6465 6669 6e69 7469 6f6e 2063 6f64  t definition cod
+00002d40: 6520 6f66 2061 2046 6f72 6d20 456c 656d  e of a Form Elem
+00002d50: 656e 7420 746f 2064 6f77 6e6c 6f61 642e  ent to download.
+00002d60: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
+00002d70: 6c65 6d65 6e74 5f64 6566 696e 6974 696f  lement_definitio
+00002d80: 6e5f 636f 6465 3a20 7374 720a 2020 2020  n_code: str.    
+00002d90: 2020 2020 3a72 6574 7572 6e3a 2049 7465      :return: Ite
+00002da0: 7261 746f 7220 6f66 2074 6865 2072 6573  rator of the res
+00002db0: 706f 6e73 6520 6279 7465 730a 2020 2020  ponse bytes.    
+00002dc0: 2020 2020 3a72 7479 7065 3a20 4974 6572      :rtype: Iter
+00002dd0: 6174 6f72 5b62 7974 6573 5d0a 2020 2020  ator[bytes].    
+00002de0: 2020 2020 3a72 6169 7365 7320 7e61 7a75      :raises ~azu
+00002df0: 7265 2e63 6f72 652e 6578 6365 7074 696f  re.core.exceptio
+00002e00: 6e73 2e48 7474 7052 6573 706f 6e73 6545  ns.HttpResponseE
+00002e10: 7272 6f72 3a0a 2020 2020 2020 2020 2902  rror:.        ).
+00002e20: 7222 0000 0072 2e00 0000 2903 720c 0000  r"...r....).r...
+00002e30: 0072 1e00 0000 da2c 6163 7469 6f6e 735f  .r.....,actions_
+00002e40: 7461 736b 5f64 6f77 6e6c 6f61 645f 656c  task_download_el
+00002e50: 656d 656e 745f 7661 6c75 655f 7265 6e64  ement_value_rend
+00002e60: 6572 6564 2904 720d 0000 0072 2200 0000  ered).r....r"...
+00002e70: 722e 0000 0072 1800 0000 720e 0000 0072  r....r....r....r
+00002e80: 0e00 0000 720f 0000 0072 3a00 0000 2001  ....r....r:... .
+00002e90: 0000 730c 0000 0000 120a 0102 0002 ff04  ..s.............
+00002ea0: 0102 ff7a 3b54 6173 6b4f 7065 7261 7469  ...z;TaskOperati
+00002eb0: 6f6e 732e 6163 7469 6f6e 735f 7461 736b  ons.actions_task
+00002ec0: 5f64 6f77 6e6c 6f61 645f 656c 656d 656e  _download_elemen
+00002ed0: 745f 7661 6c75 655f 7265 6e64 6572 6564  t_value_rendered
+00002ee0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00002ef0: 0005 0000 004b 0000 0073 1a00 0000 7c00  .....K...s....|.
+00002f00: 6a00 6a01 6a02 6600 7c01 7c02 6401 9c02  j.j.j.f.|.|.d...
+00002f10: 7c03 9702 8e01 5300 2902 610d 0200 0053  |.....S.).a....S
+00002f20: 6176 6520 4a53 4f4e 2064 6174 612e 0a0a  ave JSON data...
+00002f30: 2020 2020 2020 2020 416c 6c6f 7720 746f          Allow to
+00002f40: 2073 6176 6520 6120 4a53 4f4e 2064 6174   save a JSON dat
+00002f50: 6120 7661 6c69 6461 7469 6e67 2074 6861  a validating tha
+00002f60: 7420 7468 6520 6461 7461 2066 6f6c 6c6f  t the data follo
+00002f70: 7720 7468 6520 7265 6c61 7465 6420 7363  w the related sc
+00002f80: 6865 6d61 2e20 4966 2074 6865 2064 6174  hema. If the dat
+00002f90: 6120 6973 0a20 2020 2020 2020 2069 6e76  a is.        inv
+00002fa0: 616c 6964 2c20 7468 656e 0a20 2020 2020  alid, then.     
+00002fb0: 2020 2074 6865 206a 736f 6e20 666f 726d     the json form
+00002fc0: 2069 7320 6d61 726b 6564 2061 7320 696e   is marked as in
+00002fd0: 7661 6c69 642e 0a0a 2020 2020 2020 2020  valid...        
+00002fe0: 3a70 6172 616d 2069 643a 2054 6865 2072  :param id: The r
+00002ff0: 6573 6f75 7263 6520 4944 2e20 5265 7175  esource ID. Requ
+00003000: 6972 6564 2e0a 2020 2020 2020 2020 3a74  ired..        :t
+00003010: 7970 6520 6964 3a20 7374 720a 2020 2020  ype id: str.    
+00003020: 2020 2020 3a70 6172 616d 2063 6f6d 6d61      :param comma
+00003030: 6e64 3a20 436f 6d6d 616e 6420 746f 2073  nd: Command to s
+00003040: 6176 6520 7468 6520 4a53 4f4e 2076 616c  ave the JSON val
+00003050: 7565 2e20 5265 7175 6972 6564 2e0a 2020  ue. Required..  
+00003060: 2020 2020 2020 3a74 7970 6520 636f 6d6d        :type comm
+00003070: 616e 643a 207e 6b75 666c 6f77 2e72 6573  and: ~kuflow.res
+00003080: 742e 6d6f 6465 6c73 2e54 6173 6b53 6176  t.models.TaskSav
+00003090: 654a 736f 6e46 6f72 6d73 5661 6c75 6544  eJsonFormsValueD
+000030a0: 6174 6143 6f6d 6d61 6e64 0a20 2020 2020  ataCommand.     
+000030b0: 2020 203a 7265 7475 726e 3a20 5461 736b     :return: Task
+000030c0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000030d0: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
+000030e0: 6465 6c73 2e54 6173 6b0a 2020 2020 2020  dels.Task.      
+000030f0: 2020 3a72 6169 7365 7320 7e61 7a75 7265    :raises ~azure
+00003100: 2e63 6f72 652e 6578 6365 7074 696f 6e73  .core.exceptions
+00003110: 2e48 7474 7052 6573 706f 6e73 6545 7272  .HttpResponseErr
+00003120: 6f72 3a0a 2020 2020 2020 2020 7227 0000  or:.        r'..
+00003130: 0029 0372 0c00 0000 721e 0000 00da 2761  .).r....r.....'a
+00003140: 6374 696f 6e73 5f74 6173 6b5f 7361 7665  ctions_task_save
+00003150: 5f6a 736f 6e5f 666f 726d 735f 7661 6c75  _json_forms_valu
+00003160: 655f 6461 7461 7229 0000 0072 0e00 0000  e_datar)...r....
+00003170: 720e 0000 0072 0f00 0000 723b 0000 0036  r....r....r;...6
+00003180: 0100 0073 0200 0000 0014 7a36 5461 736b  ...s......z6Task
+00003190: 4f70 6572 6174 696f 6e73 2e61 6374 696f  Operations.actio
+000031a0: 6e73 5f74 6173 6b5f 7361 7665 5f6a 736f  ns_task_save_jso
+000031b0: 6e5f 666f 726d 735f 7661 6c75 655f 6461  n_forms_value_da
+000031c0: 7461 6304 0000 0000 0000 0000 0000 0005  tac.............
+000031d0: 0000 0008 0000 004b 0000 0073 2800 0000  .......K...s(...
+000031e0: 7c00 6a00 6a01 6a02 6600 7c01 7c02 6a03  |.j.j.j.f.|.|.j.
+000031f0: 7c02 6a04 7c02 6a05 7c03 6a06 6401 9c05  |.j.|.j.|.j.d...
+00003200: 7c04 9702 8e01 5300 2902 6171 0200 0053  |.....S.).aq...S
+00003210: 6176 6520 6120 4a53 4f4e 2046 6f72 6d73  ave a JSON Forms
+00003220: 2064 6f63 756d 656e 742e 0a0a 2020 2020   document...    
+00003230: 2020 2020 5361 7665 2061 2064 6f63 756d      Save a docum
+00003240: 656e 7420 696e 2074 6865 2074 6173 6b20  ent in the task 
+00003250: 746f 206c 6174 6572 2062 6520 6c69 6e6b  to later be link
+00003260: 6564 2069 6e74 6f20 7468 6520 4a53 4f4e  ed into the JSON
+00003270: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
+00003280: 3a70 6172 616d 2069 643a 2054 6865 2072  :param id: The r
+00003290: 6573 6f75 7263 6520 4944 2e20 5265 7175  esource ID. Requ
+000032a0: 6972 6564 2e0a 2020 2020 2020 2020 3a74  ired..        :t
+000032b0: 7970 6520 6964 3a20 7374 720a 2020 2020  ype id: str.    
+000032c0: 2020 2020 3a70 6172 616d 2066 696c 653a      :param file:
+000032d0: 2044 6f63 756d 656e 7420 746f 2073 6176   Document to sav
+000032e0: 652e 2052 6571 7569 7265 642e 0a20 2020  e. Required..   
+000032f0: 2020 2020 203a 7479 7065 2066 696c 653a       :type file:
+00003300: 207e 6b75 666c 6f77 2e72 6573 742e 6d6f   ~kuflow.rest.mo
+00003310: 6465 6c73 2e44 6f63 756d 656e 740a 2020  dels.Document.  
+00003320: 2020 2020 2020 3a70 6172 616d 2063 6f6d        :param com
+00003330: 6d61 6e64 3a20 436f 6d6d 616e 6420 746f  mand: Command to
+00003340: 2073 6176 6520 7468 6520 4a53 4f4e 2076   save the JSON v
+00003350: 616c 7565 2e20 5265 7175 6972 6564 2e0a  alue. Required..
+00003360: 2020 2020 2020 2020 3a74 7970 6520 636f          :type co
+00003370: 6d6d 616e 643a 207e 6b75 666c 6f77 2e72  mmand: ~kuflow.r
+00003380: 6573 742e 6d6f 6465 6c73 2e54 6173 6b53  est.models.TaskS
+00003390: 6176 654a 736f 6e46 6f72 6d73 5661 6c75  aveJsonFormsValu
+000033a0: 6544 6174 6143 6f6d 6d61 6e64 0a20 2020  eDataCommand.   
+000033b0: 2020 2020 203a 7265 7475 726e 3a20 5461       :return: Ta
+000033c0: 736b 5361 7665 4a73 6f6e 466f 726d 7356  skSaveJsonFormsV
+000033d0: 616c 7565 446f 6375 6d65 6e74 5265 7370  alueDocumentResp
+000033e0: 6f6e 7365 436f 6d6d 616e 640a 2020 2020  onseCommand.    
+000033f0: 2020 2020 3a72 7479 7065 3a20 7e6b 7566      :rtype: ~kuf
+00003400: 6c6f 772e 7265 7374 2e6d 6f64 656c 732e  low.rest.models.
+00003410: 5461 736b 5361 7665 4a73 6f6e 466f 726d  TaskSaveJsonForm
+00003420: 7356 616c 7565 446f 6375 6d65 6e74 5265  sValueDocumentRe
+00003430: 7370 6f6e 7365 436f 6d6d 616e 640a 2020  sponseCommand.  
+00003440: 2020 2020 2020 3a72 6169 7365 7320 7e61        :raises ~a
+00003450: 7a75 7265 2e63 6f72 652e 6578 6365 7074  zure.core.except
+00003460: 696f 6e73 2e48 7474 7052 6573 706f 6e73  ions.HttpRespons
+00003470: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00003480: 2905 7222 0000 0072 2b00 0000 722c 0000  ).r"...r+...r,..
+00003490: 0072 2d00 0000 da0b 7363 6865 6d61 5f70  .r-.....schema_p
+000034a0: 6174 6829 0772 0c00 0000 721e 0000 00da  ath).r....r.....
+000034b0: 2b61 6374 696f 6e73 5f74 6173 6b5f 7361  +actions_task_sa
+000034c0: 7665 5f6a 736f 6e5f 666f 726d 735f 7661  ve_json_forms_va
+000034d0: 6c75 655f 646f 6375 6d65 6e74 7232 0000  lue_documentr2..
+000034e0: 0072 3300 0000 7234 0000 0072 3c00 0000  .r3...r4...r<...
+000034f0: 7235 0000 0072 0e00 0000 720e 0000 0072  r5...r....r....r
+00003500: 0f00 0000 723d 0000 004c 0100 0073 1200  ....r=...L...s..
+00003510: 0000 0015 0a01 0201 0401 0401 0401 04fb  ................
+00003520: 0406 02fa 7a3a 5461 736b 4f70 6572 6174  ....z:TaskOperat
+00003530: 696f 6e73 2e61 6374 696f 6e73 5f74 6173  ions.actions_tas
+00003540: 6b5f 7361 7665 5f6a 736f 6e5f 666f 726d  k_save_json_form
+00003550: 735f 7661 6c75 655f 646f 6375 6d65 6e74  s_value_document
+00003560: 2904 7222 0000 00da 0c64 6f63 756d 656e  ).r".....documen
+00003570: 745f 7572 6972 1800 0000 7219 0000 0063  t_urir....r....c
+00003580: 0200 0000 0000 0000 0100 0000 0400 0000  ................
+00003590: 0500 0000 4b00 0000 731a 0000 007c 006a  ....K...s....|.j
+000035a0: 006a 016a 0266 007c 017c 0264 019c 027c  .j.j.f.|.|.d...|
+000035b0: 0397 028e 0153 0029 0261 8d01 0000 446f  .....S.).a....Do
+000035c0: 776e 6c6f 6164 2064 6f63 756d 656e 742e  wnload document.
+000035d0: 0a0a 2020 2020 2020 2020 4769 7665 6e20  ..        Given 
+000035e0: 6120 7461 736b 2c20 646f 776e 6c6f 6164  a task, download
+000035f0: 2061 2064 6f63 756d 656e 7420 6672 6f6d   a document from
+00003600: 2061 206a 736f 6e20 666f 726d 2064 6174   a json form dat
+00003610: 612e 0a0a 2020 2020 2020 2020 3a70 6172  a...        :par
+00003620: 616d 2069 643a 2054 6865 2072 6573 6f75  am id: The resou
+00003630: 7263 6520 4944 2e20 5265 7175 6972 6564  rce ID. Required
+00003640: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00003650: 6964 3a20 7374 720a 2020 2020 2020 2020  id: str.        
+00003660: 3a70 6172 616d 2064 6f63 756d 656e 745f  :param document_
+00003670: 7572 693a 2044 6f63 756d 656e 7420 5552  uri: Document UR
+00003680: 4920 746f 2064 6f77 6e6c 6f61 642e 2052  I to download. R
+00003690: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
+000036a0: 203a 7479 7065 2064 6f63 756d 656e 745f   :type document_
+000036b0: 7572 693a 2073 7472 0a20 2020 2020 2020  uri: str.       
+000036c0: 203a 7265 7475 726e 3a20 4974 6572 6174   :return: Iterat
+000036d0: 6f72 206f 6620 7468 6520 7265 7370 6f6e  or of the respon
+000036e0: 7365 2062 7974 6573 0a20 2020 2020 2020  se bytes.       
+000036f0: 203a 7274 7970 653a 2049 7465 7261 746f   :rtype: Iterato
+00003700: 725b 6279 7465 735d 0a20 2020 2020 2020  r[bytes].       
+00003710: 203a 7261 6973 6573 207e 617a 7572 652e   :raises ~azure.
+00003720: 636f 7265 2e65 7863 6570 7469 6f6e 732e  core.exceptions.
+00003730: 4874 7470 5265 7370 6f6e 7365 4572 726f  HttpResponseErro
+00003740: 723a 0a20 2020 2020 2020 2029 0272 2200  r:.        ).r".
+00003750: 0000 723e 0000 0029 0372 0c00 0000 721e  ..r>...).r....r.
+00003760: 0000 00da 2f61 6374 696f 6e73 5f74 6173  ..../actions_tas
+00003770: 6b5f 646f 776e 6c6f 6164 5f6a 736f 6e5f  k_download_json_
+00003780: 666f 726d 735f 7661 6c75 655f 646f 6375  forms_value_docu
+00003790: 6d65 6e74 2904 720d 0000 0072 2200 0000  ment).r....r"...
+000037a0: 723e 0000 0072 1800 0000 720e 0000 0072  r>...r....r....r
+000037b0: 0e00 0000 720f 0000 0072 3f00 0000 6a01  ....r....r?...j.
+000037c0: 0000 730c 0000 0000 0f0a 0102 0102 fe04  ..s.............
+000037d0: 0302 fd7a 3e54 6173 6b4f 7065 7261 7469  ...z>TaskOperati
+000037e0: 6f6e 732e 6163 7469 6f6e 735f 7461 736b  ons.actions_task
+000037f0: 5f64 6f77 6e6c 6f61 645f 6a73 6f6e 5f66  _download_json_f
+00003800: 6f72 6d73 5f76 616c 7565 5f64 6f63 756d  orms_value_docum
+00003810: 656e 7463 0200 0000 0000 0000 0000 0000  entc............
+00003820: 0300 0000 0400 0000 4b00 0000 7318 0000  ........K...s...
+00003830: 007c 006a 006a 016a 0266 0064 017c 0169  .|.j.j.j.f.d.|.i
+00003840: 017c 0297 028e 0153 0029 0261 1301 0000  .|.....S.).a....
+00003850: 436f 6d70 6c65 7465 2061 2074 6173 6b2e  Complete a task.
+00003860: 0a0a 2020 2020 2020 2020 416c 6c6f 7720  ..        Allow 
+00003870: 746f 2063 6f6d 706c 6574 6520 6120 636c  to complete a cl
+00003880: 6169 6d65 6420 7461 736b 2062 7920 7468  aimed task by th
+00003890: 6520 7072 696e 6369 7061 6c2e 0a0a 2020  e principal...  
+000038a0: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
+000038b0: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
+000038c0: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
+000038d0: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
+000038e0: 720a 2020 2020 2020 2020 3a72 6574 7572  r.        :retur
+000038f0: 6e3a 2054 6173 6b0a 2020 2020 2020 2020  n: Task.        
+00003900: 3a72 7479 7065 3a20 7e6b 7566 6c6f 772e  :rtype: ~kuflow.
+00003910: 7265 7374 2e6d 6f64 656c 732e 5461 736b  rest.models.Task
+00003920: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+00003930: 207e 617a 7572 652e 636f 7265 2e65 7863   ~azure.core.exc
+00003940: 6570 7469 6f6e 732e 4874 7470 5265 7370  eptions.HttpResp
+00003950: 6f6e 7365 4572 726f 723a 0a20 2020 2020  onseError:.     
+00003960: 2020 2072 2200 0000 2903 720c 0000 0072     r"...).r....r
+00003970: 1e00 0000 da15 6163 7469 6f6e 735f 7461  ......actions_ta
+00003980: 736b 5f63 6f6d 706c 6574 6572 2400 0000  sk_completer$...
+00003990: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+000039a0: 4000 0000 7f01 0000 7302 0000 0000 0b7a  @.......s......z
+000039b0: 2454 6173 6b4f 7065 7261 7469 6f6e 732e  $TaskOperations.
+000039c0: 6163 7469 6f6e 735f 7461 736b 5f63 6f6d  actions_task_com
+000039d0: 706c 6574 6529 0472 2200 0000 da03 6c6f  plete).r".....lo
+000039e0: 6772 1800 0000 7219 0000 0063 0300 0000  gr....r....c....
+000039f0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
+00003a00: 4b00 0000 731a 0000 007c 006a 006a 016a  K...s....|.j.j.j
+00003a10: 0266 007c 017c 0264 019c 027c 0397 028e  .f.|.|.d...|....
+00003a20: 0153 0029 0261 b901 0000 4170 7065 6e64  .S.).a....Append
+00003a30: 2061 206c 6f67 2074 6f20 7468 6520 7461   a log to the ta
+00003a40: 736b 2e0a 0a20 2020 2020 2020 2041 206c  sk...        A l
+00003a50: 6f67 2065 6e74 7279 2069 7320 6164 6465  og entry is adde
+00003a60: 6420 746f 2074 6865 2074 6173 6b2e 2049  d to the task. I
+00003a70: 6620 7468 6520 6e75 6d62 6572 206f 6620  f the number of 
+00003a80: 6c6f 6720 656e 7472 6965 7320 6973 2072  log entries is r
+00003a90: 6561 6368 6564 2c20 7468 6520 6f6c 6465  eached, the olde
+00003aa0: 7374 206c 6f67 2065 6e74 7279 0a20 2020  st log entry.   
+00003ab0: 2020 2020 2069 7320 7265 6d6f 7665 642e       is removed.
+00003ac0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00003ad0: 2069 643a 2054 6865 2072 6573 6f75 7263   id: The resourc
+00003ae0: 6520 4944 2e20 5265 7175 6972 6564 2e0a  e ID. Required..
+00003af0: 2020 2020 2020 2020 3a74 7970 6520 6964          :type id
+00003b00: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
+00003b10: 6172 616d 206c 6f67 3a20 4c6f 6720 746f  aram log: Log to
+00003b20: 2062 6520 6372 6561 7465 642e 2052 6571   be created. Req
+00003b30: 7569 7265 642e 0a20 2020 2020 2020 203a  uired..        :
+00003b40: 7479 7065 206c 6f67 3a20 7e6b 7566 6c6f  type log: ~kuflo
+00003b50: 772e 7265 7374 2e6d 6f64 656c 732e 4c6f  w.rest.models.Lo
+00003b60: 670a 2020 2020 2020 2020 3a72 6574 7572  g.        :retur
+00003b70: 6e3a 2054 6173 6b0a 2020 2020 2020 2020  n: Task.        
+00003b80: 3a72 7479 7065 3a20 7e6b 7566 6c6f 772e  :rtype: ~kuflow.
+00003b90: 7265 7374 2e6d 6f64 656c 732e 5461 736b  rest.models.Task
+00003ba0: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+00003bb0: 207e 617a 7572 652e 636f 7265 2e65 7863   ~azure.core.exc
+00003bc0: 6570 7469 6f6e 732e 4874 7470 5265 7370  eptions.HttpResp
+00003bd0: 6f6e 7365 4572 726f 723a 0a20 2020 2020  onseError:.     
+00003be0: 2020 2029 0272 2200 0000 7241 0000 0029     ).r"...rA...)
+00003bf0: 0372 0c00 0000 721e 0000 00da 1761 6374  .r....r......act
+00003c00: 696f 6e73 5f74 6173 6b5f 6170 7065 6e64  ions_task_append
+00003c10: 5f6c 6f67 2904 720d 0000 0072 2200 0000  _log).r....r"...
+00003c20: 7241 0000 0072 1800 0000 720e 0000 0072  rA...r....r....r
+00003c30: 0e00 0000 720f 0000 0072 4200 0000 8c01  ....r....rB.....
+00003c40: 0000 7302 0000 0000 0e7a 2654 6173 6b4f  ..s......z&TaskO
+00003c50: 7065 7261 7469 6f6e 732e 6163 7469 6f6e  perations.action
+00003c60: 735f 7461 736b 5f61 7070 656e 645f 6c6f  s_task_append_lo
+00003c70: 6729 0672 1100 0000 7201 0000 004e 4e4e  g).r....r....NNN
+00003c80: 4e29 014e 292c da08 5f5f 6e61 6d65 5f5f  N).N),..__name__
+00003c90: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00003ca0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00003cb0: 635f 5fda 194b 7546 6c6f 7752 6573 7443  c__..KuFlowRestC
+00003cc0: 6c69 656e 7447 656e 6572 6174 6564 7210  lientGeneratedr.
+00003cd0: 0000 00da 0369 6e74 7205 0000 0072 0600  .....intr....r..
+00003ce0: 0000 721b 0000 0072 0400 0000 721c 0000  ..r....r....r...
+00003cf0: 0072 1d00 0000 7202 0000 00da 0854 6173  .r....r......Tas
+00003d00: 6b50 6167 6572 1f00 0000 da04 5461 736b  kPager......Task
+00003d10: 7221 0000 0072 2300 0000 7225 0000 00da  r!...r#...r%....
+00003d20: 1154 6173 6b41 7373 6967 6e43 6f6d 6d61  .TaskAssignComma
+00003d30: 6e64 7228 0000 00da 1654 6173 6b53 6176  ndr(.....TaskSav
+00003d40: 6545 6c65 6d65 6e74 436f 6d6d 616e 6472  eElementCommandr
+00003d50: 2a00 0000 da08 446f 6375 6d65 6e74 da23  *.....Document.#
+00003d60: 5461 736b 5361 7665 456c 656d 656e 7456  TaskSaveElementV
+00003d70: 616c 7565 446f 6375 6d65 6e74 436f 6d6d  alueDocumentComm
+00003d80: 616e 6472 3100 0000 da18 5461 736b 4465  andr1.....TaskDe
+00003d90: 6c65 7465 456c 656d 656e 7443 6f6d 6d61  leteElementComma
+00003da0: 6e64 7236 0000 00da 2554 6173 6b44 656c  ndr6....%TaskDel
+00003db0: 6574 6545 6c65 6d65 6e74 5661 6c75 6544  eteElementValueD
+00003dc0: 6f63 756d 656e 7443 6f6d 6d61 6e64 7237  ocumentCommandr7
+00003dd0: 0000 0072 0300 0000 da05 6279 7465 7372  ...r......bytesr
+00003de0: 3900 0000 723a 0000 00da 2154 6173 6b53  9...r:....!TaskS
+00003df0: 6176 654a 736f 6e46 6f72 6d73 5661 6c75  aveJsonFormsValu
+00003e00: 6544 6174 6143 6f6d 6d61 6e64 723b 0000  eDataCommandr;..
+00003e10: 00da 2c54 6173 6b53 6176 654a 736f 6e46  ..,TaskSaveJsonF
+00003e20: 6f72 6d73 5661 6c75 6544 6f63 756d 656e  ormsValueDocumen
+00003e30: 7452 6571 7565 7374 436f 6d6d 616e 64da  tRequestCommand.
+00003e40: 2d54 6173 6b53 6176 654a 736f 6e46 6f72  -TaskSaveJsonFor
+00003e50: 6d73 5661 6c75 6544 6f63 756d 656e 7452  msValueDocumentR
+00003e60: 6573 706f 6e73 6543 6f6d 6d61 6e64 723d  esponseCommandr=
+00003e70: 0000 0072 3f00 0000 7240 0000 00da 034c  ...r?...r@.....L
+00003e80: 6f67 7242 0000 0072 0e00 0000 720e 0000  ogrB...r....r...
+00003e90: 0072 0e00 0000 720f 0000 0072 0a00 0000  .r....r....r....
+00003ea0: 2200 0000 7386 0000 0008 0104 090e 0500  "...s...........
+00003eb0: 0100 0100 0100 0100 0100 f902 0202 0102  ................
+00003ec0: 0112 0112 0116 0112 0102 0104 f70c 371e  ..............7.
+00003ed0: 2014 0d14 0d18 1002 0004 0002 0104 fe0c   ...............
+00003ee0: 1a02 0004 0004 0002 0104 fe0c 2102 0004  ............!...
+00003ef0: 0002 0104 fe0c 1402 0004 0002 0104 fe0c  ................
+00003f00: 1418 1202 0002 0002 0106 fe0c 1802 0104  ................
+00003f10: 0102 0104 fb0c 1802 0104 0104 0102 0104  ................
+00003f20: fa0c 1f02 0002 0002 0106 fe0c 1514 0d72  ...............r
+00003f30: 0a00 0000 4e29 0dda 0674 7970 696e 6772  ....N)...typingr
+00003f40: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
+00003f50: 0000 0072 0600 0000 da0a 5f67 656e 6572  ...r......_gener
+00003f60: 6174 6564 7208 0000 0072 4700 0000 da00  atedr....rG.....
+00003f70: 7209 0000 0072 1c00 0000 720a 0000 0072  r....r....r....r
+00003f80: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00003f90: 0000 00da 083c 6d6f 6475 6c65 3e1b 0000  .....<module>...
+00003fa0: 0073 0600 0000 1c02 0c02 0c03            .s..........
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/_authentication_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/operations/_authentication_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 
         Instead, you should access the following operations through
         :class:`~kuflow.rest.client.KuFlowRestClient`'s
         :attr:`authentication` attribute.
     """
 
     def __init__(self, kuflow_client: KuFlowRestClientGenerated):
-        self.__kuflow_client = kuflow_client
+        self._kuflow_client = kuflow_client
 
     def create_authentication(self, authentication: _models.Authentication, **kwargs: Any) -> _models.Authentication:
         """Create an authentication for the current principal.
 
         Create an authentication for the current principal.
 
         :param authentication: Authentication to be created. Is either a model type or a IO type. Required.
         :type authentication: ~kuflow.rest.models.Authentication or IO
         :return: Authentication
         :rtype: ~kuflow.rest.models.Authentication
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.authentication.create_authentication(authentication=authentication, **kwargs)
+        return self._kuflow_client.authentication.create_authentication(authentication=authentication, **kwargs)
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/_principal_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/operations/_principal_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         Instead, you should access the following operations through
         :class:`~kuflow.rest.client.KuFlowRestClient`'s
         :attr:`principal` attribute.
     """
 
     def __init__(self, kuflow_client: KuFlowRestClientGenerated):
-        self.__kuflow_client = kuflow_client
+        self._kuflow_client = kuflow_client
 
     def find_principals(
         self,
         size: int = 25,
         page: int = 0,
         sort: Optional[Union[str, List[str]]] = None,
         type: Optional[_models.PrincipalType] = None,
@@ -77,23 +77,23 @@
         """
         if sort is not None and isinstance(sort, str):
             sort = [sort]
 
         if group_id is not None and isinstance(group_id, str):
             group_id = [group_id]
 
-        return self.__kuflow_client.principal.find_principals(
+        return self._kuflow_client.principal.find_principals(
             size=size, page=page, sort=sort, type=type, group_id=group_id, **kwargs
         )
 
     def retrieve_principal(self, id: str, **kwargs: Any) -> _models.Principal:
         """Get a Principal by ID.
 
         Returns the requested Principal when has access to do it.
 
         :param id: The resource ID. Required.
         :type id: str
         :return: Principal
         :rtype: ~kuflow.rest.models.Principal
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.principal.retrieve_principal(id=id, **kwargs)
+        return self._kuflow_client.principal.retrieve_principal(id=id, **kwargs)
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/_process_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/operations/_process_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         Instead, you should access the following operations through
         :class:`~kuflow.rest.client.KuFlowRestClient`'s
         :attr:`process` attribute.
     """
 
     def __init__(self, kuflow_client: KuFlowRestClientGenerated):
-        self.__kuflow_client = kuflow_client
+        self._kuflow_client = kuflow_client
 
     def find_processes(
         self, size: int = 25, page: int = 0, sort: Optional[Union[str, List[str]]] = None, **kwargs: Any
     ) -> _models.ProcessPage:
         """Find all accessible Processes.
 
         List all the Processes that have been created and the credentials has access.
@@ -66,15 +66,15 @@
         :return: ProcessPage
         :rtype: ~kuflow.rest.models.ProcessPage
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         if sort is not None and isinstance(sort, str):
             sort = [sort]
 
-        return self.__kuflow_client.process.find_processes(size=size, page=page, sort=sort, **kwargs)
+        return self._kuflow_client.process.find_processes(size=size, page=page, sort=sort, **kwargs)
 
     def create_process(self, process: _models.Process, **kwargs: Any) -> _models.Process:
         """Create a new process.
 
         Creates a process. This option has direct correspondence to the action of starting a process in
         the Kuflow GUI.
 
@@ -91,28 +91,28 @@
 
         :param process: Process to create. Required.
         :type process: ~kuflow.rest.models.Process
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.create_process(process=process, **kwargs)
+        return self._kuflow_client.process.create_process(process=process, **kwargs)
 
     def retrieve_process(self, id: str, **kwargs: Any) -> _models.Process:
         """Get a Process by ID.
 
         Returns the requested Process when has access to do it.
 
         :param id: The resource ID. Required.
         :type id: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.retrieve_process(id=id, **kwargs)
+        return self._kuflow_client.process.retrieve_process(id=id, **kwargs)
 
     def actions_process_change_initiator(
         self, id: str, command: _models.ProcessChangeInitiatorCommand, **kwargs: Any
     ) -> _models.Process:
         """Change process initiator.
 
         Change the current initiator of a process.
@@ -125,15 +125,15 @@
         :type id: str
         :param command: Command to change the process initiator. Required.
         :type command: ~kuflow.rest.models.ProcessChangeInitiatorCommand
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.actions_process_change_initiator(id=id, command=command, **kwargs)
+        return self._kuflow_client.process.actions_process_change_initiator(id=id, command=command, **kwargs)
 
     def actions_process_save_element(
         self, id: str, command: _models.ProcessSaveElementCommand, **kwargs: Any
     ) -> _models.Process:
         """Save a process element, aka: metadata.
 
         Allow to save an element.
@@ -148,15 +148,15 @@
         :type id: str
         :param command: Command to save an element. Required.
         :type command: ~kuflow.rest.models.ProcessSaveElementCommand
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.actions_process_save_element(id=id, command=command, **kwargs)
+        return self._kuflow_client.process.actions_process_save_element(id=id, command=command, **kwargs)
 
     def actions_process_delete_element(
         self, id: str, command: _models.ProcessDeleteElementCommand, **kwargs: Any
     ) -> _models.Process:
         """Delete an element by code.
 
         Allow to delete a process element by specifying the item definition code.
@@ -167,30 +167,30 @@
         :type id: str
         :param command: Command to delete an element. Required.
         :type command: ~kuflow.rest.models.ProcessDeleteElementCommand
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.actions_process_delete_element(id=id, command=command, **kwargs)
+        return self._kuflow_client.process.actions_process_delete_element(id=id, command=command, **kwargs)
 
     def actions_process_complete(self, id: str, **kwargs: Any) -> _models.Process:
         """Complete a Process.
 
         Complete a Process. The state of Process is set to 'completed'.
 
         If you are already in this state, no action is taken.
 
         :param id: The resource ID. Required.
         :type id: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.actions_process_complete(id=id, **kwargs)
+        return self._kuflow_client.process.actions_process_complete(id=id, **kwargs)
 
     def actions_process_cancel(self, id: str, **kwargs: Any) -> _models.Process:
         """Cancel a Process.
 
         Cancel a Process. The Process state is set to 'cancelled'.
 
         All the active tasks will be marked as cancelled too.
@@ -199,15 +199,15 @@
 
         :param id: The resource ID. Required.
         :type id: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.actions_process_cancel(id=id, **kwargs)
+        return self._kuflow_client.process.actions_process_cancel(id=id, **kwargs)
 
     def actions_process_save_user_action_value_document(
         self, id: str, file: _models.Document, command: _models.ProcessSaveUserActionValueDocumentCommand, **kwargs: Any
     ) -> Optional[_models.Process]:
         """Upload and save a document in a user action.
 
         Allow saving a user action document uploading the content.
@@ -218,15 +218,15 @@
         :type file: _models.Document
         :keyword command: User action info. Required.
         :type command: _models.ProcessSaveUserActionValueDocumentCommand
         :return: Process or None
         :rtype: ~kuflow.rest.models.Process or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.process.actions_process_save_user_action_value_document(
+        return self._kuflow_client.process.actions_process_save_user_action_value_document(
             id=id,
             file=file.file_content,
             file_content_type=file.content_type,
             file_name=file.file_mame,
             user_action_value_id=command.user_action_value_id,
             **kwargs,
         )
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/operations/_task_operations.py` & `kuflow_rest-0.6.1/kuflow_rest/operations/_task_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         Instead, you should access the following operations through
         :class:`~kuflow.rest.client.KuFlowRestClient`'s
         :attr:`task` attribute.
     """
 
     def __init__(self, kuflow_client: KuFlowRestClientGenerated):
-        self.__kuflow_client = kuflow_client
+        self._kuflow_client = kuflow_client
 
     def find_tasks(
         self,
         size: int = 25,
         page: int = 0,
         sort: Optional[Union[str, List[str]]] = None,
         process_id: Optional[Union[str, List[str]]] = None,
@@ -85,15 +85,15 @@
         if process_id is not None and isinstance(process_id, str):
             process_id = [process_id]
         if state is not None and isinstance(state, _models.TaskState):
             state = [state]
         if task_definition_code is not None and isinstance(task_definition_code, str):
             task_definition_code = [task_definition_code]
 
-        return self.__kuflow_client.task.find_tasks(
+        return self._kuflow_client.task.find_tasks(
             size=size,
             page=page,
             sort=sort,
             process_id=process_id,
             state=state,
             task_definition_code=task_definition_code,
             **kwargs,
@@ -125,56 +125,56 @@
          value is required and must be set with the context task token of Temporal.io activity. Default
          value is None.
         :type activity_token: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.create_task(task=task, activity_token=activity_token, **kwargs)
+        return self._kuflow_client.task.create_task(task=task, activity_token=activity_token, **kwargs)
 
     def retrieve_task(self, id: str, **kwargs: Any) -> _models.Task:
         """Get a task given it ID.
 
         Allow to get a task by ID.
 
         :param id: The resource ID. Required.
         :type id: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.retrieve_task(id=id, **kwargs)
+        return self._kuflow_client.task.retrieve_task(id=id, **kwargs)
 
     def actions_task_claim(self, id: str, **kwargs: Any) -> _models.Task:
         """Claim a task.
 
         Allow to claim a task.
 
         :param id: The resource ID. Required.
         :type id: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_claim(id=id, **kwargs)
+        return self._kuflow_client.task.actions_task_claim(id=id, **kwargs)
 
     def actions_task_assign(self, id: str, command: _models.TaskAssignCommand, **kwargs: Any) -> _models.Task:
         """Assign a task.
 
         Allow to assign a task to a user or application. Only one option will be necessary.
 
         :param id: The resource ID. Required.
         :type id: str
         :param command: Command to change the task owner. Required.
         :type command: ~kuflow.rest.models.TaskAssignCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_assign(id=id, command=command, **kwargs)
+        return self._kuflow_client.task.actions_task_assign(id=id, command=command, **kwargs)
 
     def actions_task_save_element(
         self, id: str, command: _models.TaskSaveElementCommand, **kwargs: Any
     ) -> _models.Task:
         """Save an element.
 
         Allow to save an element i.e., a field, a decision, a form, a principal or document.
@@ -191,15 +191,15 @@
         :type id: str
         :param command: Command to save an element. Required.
         :type command: ~kuflow.rest.models.TaskSaveElementCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_save_element(id=id, command=command, **kwargs)
+        return self._kuflow_client.task.actions_task_save_element(id=id, command=command, **kwargs)
 
     def actions_task_save_element_value_document(
         self, id: str, file: _models.Document, command: _models.TaskSaveElementValueDocumentCommand, **kwargs: Any
     ) -> _models.Task:
         """Save an element document.
 
         Allow to save an element document uploading the content.
@@ -214,15 +214,15 @@
         :type file: ~kuflow.rest.models.Document
         :param command: Command info. Required.
         :type command: ~kuflow.rest.models.TaskSaveElementValueDocumentCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_save_element_value_document(
+        return self._kuflow_client.task.actions_task_save_element_value_document(
             id=id,
             file=file.file_content,
             file_content_type=file.content_type,
             file_name=file.file_mame,
             element_definition_code=command.element_definition_code,
             element_value_id=command.element_value_id,
             element_value_valid=command.element_value_valid,
@@ -242,15 +242,15 @@
         :type id: str
         :param command: Command to delete an element. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_delete_element(id=id, command=command, **kwargs)
+        return self._kuflow_client.task.actions_task_delete_element(id=id, command=command, **kwargs)
 
     def actions_task_delete_element_value_document(
         self, id: str, command: _models.TaskDeleteElementValueDocumentCommand, **kwargs: Any
     ) -> _models.Task:
         """Delete an element document value.
 
         Allow to delete a specific document from an element of document type using its id.
@@ -262,30 +262,30 @@
         :type id: str
         :param command: Command to delete a document element value. Required.
         :type command: ~kuflow.rest.models.TaskDeleteElementValueDocumentCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_delete_element_value_document(id=id, command=command, **kwargs)
+        return self._kuflow_client.task.actions_task_delete_element_value_document(id=id, command=command, **kwargs)
 
     def actions_task_download_element_value_document(self, id: str, document_id: str, **kwargs: Any) -> Iterator[bytes]:
         """Download document.
 
         Given a task, download a document from an element of document type.
 
         :param id: The resource ID. Required.
         :type id: str
         :keyword document_id: Document ID to download. Required.
         :type document_id: str
         :return: Iterator of the response bytes
         :rtype: Iterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_download_element_value_document(
+        return self._kuflow_client.task.actions_task_download_element_value_document(
             id=id, document_id=document_id, **kwargs
         )
 
     def actions_task_download_element_value_rendered(
         self, id: str, element_definition_code: str, **kwargs: Any
     ) -> Iterator[bytes]:
         """Download a Form rendered as PDF or Zip of PDFs (when the element is multiple).
@@ -299,15 +299,15 @@
         :type id: str
         :param element_definition_code: Element definition code of a Form Element to download.
         :type element_definition_code: str
         :return: Iterator of the response bytes
         :rtype: Iterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_download_element_value_rendered(
+        return self._kuflow_client.task.actions_task_download_element_value_rendered(
             id=id, element_definition_code=element_definition_code, **kwargs
         )
 
     def actions_task_save_json_forms_value_data(
         self,
         id: str,
         command: _models.TaskSaveJsonFormsValueDataCommand,
@@ -323,15 +323,15 @@
         :type id: str
         :param command: Command to save the JSON value. Required.
         :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_save_json_forms_value_data(id=id, command=command, **kwargs)
+        return self._kuflow_client.task.actions_task_save_json_forms_value_data(id=id, command=command, **kwargs)
 
     def actions_task_save_json_forms_value_document(
         self,
         id: str,
         file: _models.Document,
         command: _models.TaskSaveJsonFormsValueDocumentRequestCommand,
         **kwargs: Any,
@@ -346,15 +346,15 @@
         :type file: ~kuflow.rest.models.Document
         :param command: Command to save the JSON value. Required.
         :type command: ~kuflow.rest.models.TaskSaveJsonFormsValueDataCommand
         :return: TaskSaveJsonFormsValueDocumentResponseCommand
         :rtype: ~kuflow.rest.models.TaskSaveJsonFormsValueDocumentResponseCommand
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_save_json_forms_value_document(
+        return self._kuflow_client.task.actions_task_save_json_forms_value_document(
             id=id,
             file=file.file_content,
             file_content_type=file.content_type,
             file_name=file.file_mame,
             schema_path=command.schema_path,
             **kwargs,
         )
@@ -370,15 +370,15 @@
         :type id: str
         :param document_uri: Document URI to download. Required.
         :type document_uri: str
         :return: Iterator of the response bytes
         :rtype: Iterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_download_json_forms_value_document(
+        return self._kuflow_client.task.actions_task_download_json_forms_value_document(
             id=id,
             document_uri=document_uri,
             **kwargs,
         )
 
     def actions_task_complete(self, id: str, **kwargs: Any) -> _models.Task:
         """Complete a task.
@@ -387,15 +387,15 @@
 
         :param id: The resource ID. Required.
         :type id: str
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_complete(id=id, **kwargs)
+        return self._kuflow_client.task.actions_task_complete(id=id, **kwargs)
 
     def actions_task_append_log(self, id: str, log: _models.Log, **kwargs: Any) -> _models.Task:
         """Append a log to the task.
 
         A log entry is added to the task. If the number of log entries is reached, the oldest log entry
         is removed.
 
@@ -403,8 +403,8 @@
         :type id: str
         :param log: Log to be created. Required.
         :type log: ~kuflow.rest.models.Log
         :return: Task
         :rtype: ~kuflow.rest.models.Task
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self.__kuflow_client.task.actions_task_append_log(id=id, log=log, **kwargs)
+        return self._kuflow_client.task.actions_task_append_log(id=id, log=log, **kwargs)
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/utils/__init__.py` & `kuflow_rest-0.6.1/kuflow_rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 6837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 b51a 0000  U........<.d....
+00000000: 550d 0d0a 0000 0000 9c24 8c64 b51a 0000  U........$.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0048 0000 0040 0000 0073 c801 0000 6400  .H...@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/_element_values.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 41580 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 6ca2 0000  U........<.dl...
+00000000: 550d 0d0a 0000 0000 9c24 8c64 6ca2 0000  U........$.dl...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7a09 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 6404 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc` & `kuflow_rest-0.6.1/kuflow_rest/utils/__pycache__/_json_forms.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun  6 14:03:56 2023 UTC, .py size: 23171 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cc3c 7f64 835a 0000  U........<.d.Z..
+00000000: 550d 0d0a 0000 0000 9c24 8c64 835a 0000  U........$.d.Z..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 e402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c07 5a07 6400  m.Z...d.d.l.Z.d.
 00000060: 6403 6c08 5a08 6404 6405 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-0.6.0/kuflow_rest/utils/_element_values.py` & `kuflow_rest-0.6.1/kuflow_rest/utils/_element_values.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/kuflow_rest/utils/_json_forms.py` & `kuflow_rest-0.6.1/kuflow_rest/utils/_json_forms.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-0.6.0/pyproject.toml` & `kuflow_rest-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-rest"
-version = "0.6.0"
+version = "0.6.1"
 description = "Client for KuFlow Rest Api"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
```

### Comparing `kuflow_rest-0.6.0/setup.py` & `kuflow_rest-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['azure-core>=1.26.4,<2.0.0', 'isodate>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-rest',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Client for KuFlow Rest Api',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n\n# KuFlow Rest\n\nThis is a client for the KuFlow API Rest that allows you to interact with our API in a comfortable way in the creation of your workers and tools.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_rest-0.6.0/PKG-INFO` & `kuflow_rest-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuflow-rest
-Version: 0.6.0
+Version: 0.6.1
 Summary: Client for KuFlow Rest Api
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

