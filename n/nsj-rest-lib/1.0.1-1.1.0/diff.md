# Comparing `tmp/nsj_rest_lib-1.0.1.tar.gz` & `tmp/nsj_rest_lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.0.1.tar", last modified: Wed Jun 14 17:51:03 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.1.0.tar", last modified: Thu Jun 15 22:55:12 2023, max compression
```

## Comparing `nsj_rest_lib-1.0.1.tar` & `nsj_rest_lib-1.1.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-1.0.1/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.480347 nsj_rest_lib-1.0.1/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.488348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    16780 2023-06-14 17:50:21.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9827 2023-06-14 17:50:21.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.492348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    23264 2023-05-30 22:01:35.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.496348 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-14 17:51:03.488348 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1609 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-06-14 17:51:03.000000 nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-1.1.0/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-06-15 22:55:12.323049 nsj_rest_lib-1.1.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.307049 nsj_rest_lib-1.1.0/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.311049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4104 2023-06-15 22:54:32.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16780 2023-06-14 17:50:21.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9827 2023-06-14 17:50:21.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-05-30 22:01:35.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    23263 2023-06-15 22:54:32.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1652 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.0.1/PKG-INFO` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj_rest_lib
-Version: 1.0.1
+Name: nsj-rest-lib
+Version: 1.1.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.0.1/setup.cfg` & `nsj_rest_lib-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 1.0.1
+version = 1.1.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/service_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,22 +294,24 @@
             id=id,
             aditional_filters=aditional_filters
         )
 
     def partial_update(
         self,
         dto: DTOBase,
-        id: Any
+        id: Any,
+        aditional_filters: Dict[str, Any] = None
     ) -> DTOBase:
         return self._save(
             insert=False,
             dto=dto,
             manage_transaction=True,
             partial_update=True,
-            id=id
+            id=id,
+            aditional_filters=aditional_filters
         )
 
     def _save(
         self,
         insert: bool,
         dto: DTOBase,
         manage_transaction: bool,
@@ -486,16 +488,14 @@
 
             # Salvando cada DTO detalhe
             for detail_dto in detail_list:
 
                 # Recuperando o ID da entidade relacionada
                 detail_pk_field = detail_dto.__class__.pk_field
                 detail_pk = getattr(detail_dto, detail_pk_field)
-                if isinstance(detail_pk, uuid.UUID):
-                    detail_pk = str(detail_pk)
 
                 # Verificando se é um update ou insert
                 is_detail_insert = True
                 if old_detail_ids is not None and detail_pk in old_detail_ids:
                     is_detail_insert = False
                     old_detail_ids.remove(detail_pk)
```

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj-rest-lib
-Version: 1.0.1
+Name: nsj_rest_lib
+Version: 1.1.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.0.1/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/nsj_rest_lib.egg-info/top_level.txt
 src/nsj_rest_lib/controller/__init__.py
 src/nsj_rest_lib/controller/controller_util.py
 src/nsj_rest_lib/controller/delete_route.py
 src/nsj_rest_lib/controller/funtion_route_wrapper.py
 src/nsj_rest_lib/controller/get_route.py
 src/nsj_rest_lib/controller/list_route.py
+src/nsj_rest_lib/controller/patch_route.py
 src/nsj_rest_lib/controller/post_route.py
 src/nsj_rest_lib/controller/put_route.py
 src/nsj_rest_lib/controller/route_base.py
 src/nsj_rest_lib/dao/__init__.py
 src/nsj_rest_lib/dao/dao_base.py
 src/nsj_rest_lib/decorator/__init__.py
 src/nsj_rest_lib/decorator/dto.py
```

