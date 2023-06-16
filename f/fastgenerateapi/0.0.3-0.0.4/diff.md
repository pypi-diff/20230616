# Comparing `tmp/fastgenerateapi-0.0.3.tar.gz` & `tmp/fastgenerateapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgenerateapi-0.0.3.tar", last modified: Thu Jun 15 06:54:42 2023, max compression
+gzip compressed data, was "fastgenerateapi-0.0.4.tar", last modified: Fri Jun 16 06:33:07 2023, max compression
```

## Comparing `fastgenerateapi-0.0.3.tar` & `fastgenerateapi-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/
--rw-rw-rw-   0        0        0    35821 2023-06-15 06:34:41.000000 fastgenerateapi-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      664 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.339232 fastgenerateapi-0.0.3/fastgenerateapi/
--rw-rw-rw-   0        0        0      826 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/__init__.py
--rw-rw-rw-   0        0        0      496 2023-06-15 06:54:39.000000 fastgenerateapi-0.0.3/fastgenerateapi/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.370474 fastgenerateapi-0.0.3/fastgenerateapi/api_view/
--rw-rw-rw-   0        0        0       14 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/api_view.py
--rw-rw-rw-   0        0        0     9311 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/base_view.py
--rw-rw-rw-   0        0        0     4192 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/create_view.py
--rw-rw-rw-   0        0        0     3829 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/delete_tree_view.py
--rw-rw-rw-   0        0        0     3225 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/delete_view.py
--rw-rw-rw-   0        0        0     7585 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_all_view.py
--rw-rw-rw-   0        0        0     3077 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_one_view.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.370474 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/
--rw-rw-rw-   0        0        0        0 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/__init__.py
--rw-rw-rw-   0        0        0     3529 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/base_mixin.py
--rw-rw-rw-   0        0        0     3826 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
--rw-rw-rw-   0        0        0      266 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/get_mixin.py
--rw-rw-rw-   0        0        0     2221 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/response_mixin.py
--rw-rw-rw-   0        0        0      317 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/save_mixin.py
--rw-rw-rw-   0        0        0    13029 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/tool_mixin.py
--rw-rw-rw-   0        0        0     3279 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/switch_view.py
--rw-rw-rw-   0        0        0     4152 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/api_view/update_view.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.370474 fastgenerateapi-0.0.3/fastgenerateapi/controller/
--rw-rw-rw-   0        0        0      316 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/__init__.py
--rw-rw-rw-   0        0        0     3391 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/filter_controller.py
--rw-rw-rw-   0        0        0     2385 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/router_controller.py
--rw-rw-rw-   0        0        0     2298 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/rpc_controller.py
--rw-rw-rw-   0        0        0      873 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/controller/search_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/data_type/__init__.py
--rw-rw-rw-   0        0        0      727 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/data_type/data_type.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/deps/
--rw-rw-rw-   0        0        0      160 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/deps/__init__.py
--rw-rw-rw-   0        0        0     1581 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/deps/filter_params_deps.py
--rw-rw-rw-   0        0        0     3171 2023-06-15 06:34:06.000000 fastgenerateapi-0.0.3/fastgenerateapi/deps/paginator_deps.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/
--rw-rw-rw-   0        0        0        0 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/base_model.py
--rw-rw-rw-   0        0        0     2814 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/json_encoders.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.386096 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/
--rw-rw-rw-   0        0        0      472 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/__init__.py
--rw-rw-rw-   0        0        0     4305 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/common_function.py
--rw-rw-rw-   0        0        0     1856 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/create_schema_factory.py
--rw-rw-rw-   0        0        0     3102 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_all_schema_factory.py
--rw-rw-rw-   0        0        0     1763 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_one_schema_factory.py
--rw-rw-rw-   0        0        0     1251 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/response_factory.py
--rw-rw-rw-   0        0        0     1856 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/update_schema_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/fastgenerateapi/settings/
--rw-rw-rw-   0        0        0        6 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/settings/__init__.py
--rw-rw-rw-   0        0        0      232 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/settings/register_settings.py
--rw-rw-rw-   0        0        0     3083 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/settings/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/fastgenerateapi/utils/
--rw-rw-rw-   0        0        0        0 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/utils/__init__.py
--rw-rw-rw-   0        0        0      121 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/utils/exception.py
--rw-rw-rw-   0        0        0      670 2023-06-15 06:34:07.000000 fastgenerateapi-0.0.3/fastgenerateapi/utils/parse_str.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:54:42.354853 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/
--rw-rw-rw-   0        0        0      664 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2106 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 06:54:42.000000 fastgenerateapi-0.0.3/fastgenerateapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 06:54:42.401717 fastgenerateapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3832 2023-06-15 06:34:41.000000 fastgenerateapi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.830804 fastgenerateapi-0.0.4/
+-rw-rw-rw-   0        0        0    35821 2023-06-15 11:33:13.000000 fastgenerateapi-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-06-16 06:33:07.830138 fastgenerateapi-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.773770 fastgenerateapi-0.0.4/fastgenerateapi/
+-rw-rw-rw-   0        0        0      883 2023-06-16 01:37:51.000000 fastgenerateapi-0.0.4/fastgenerateapi/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-16 06:28:03.000000 fastgenerateapi-0.0.4/fastgenerateapi/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.790723 fastgenerateapi-0.0.4/fastgenerateapi/api_view/
+-rw-rw-rw-   0        0        0       14 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/api_view.py
+-rw-rw-rw-   0        0        0     9189 2023-06-16 03:02:52.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/base_view.py
+-rw-rw-rw-   0        0        0     4177 2023-06-16 00:58:02.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/create_view.py
+-rw-rw-rw-   0        0        0     3634 2023-06-16 01:26:57.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_tree_view.py
+-rw-rw-rw-   0        0        0     3061 2023-06-16 01:18:56.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_view.py
+-rw-rw-rw-   0        0        0     7426 2023-06-16 01:29:40.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_all_view.py
+-rw-rw-rw-   0        0        0     3062 2023-06-16 01:03:06.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_one_view.py
+-rw-rw-rw-   0        0        0     7235 2023-06-16 04:52:13.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.798222 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-16 04:46:20.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/base_mixin.py
+-rw-rw-rw-   0        0        0     3826 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
+-rw-rw-rw-   0        0        0      266 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/get_mixin.py
+-rw-rw-rw-   0        0        0     2290 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/response_mixin.py
+-rw-rw-rw-   0        0        0      317 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/save_mixin.py
+-rw-rw-rw-   0        0        0    13029 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/tool_mixin.py
+-rw-rw-rw-   0        0        0     3070 2023-06-16 01:29:40.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/switch_view.py
+-rw-rw-rw-   0        0        0     4006 2023-06-16 03:02:52.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/update_view.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.802213 fastgenerateapi-0.0.4/fastgenerateapi/controller/
+-rw-rw-rw-   0        0        0      316 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3391 2023-06-16 00:44:07.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/filter_controller.py
+-rw-rw-rw-   0        0        0     2385 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/router_controller.py
+-rw-rw-rw-   0        0        0     2298 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/rpc_controller.py
+-rw-rw-rw-   0        0        0      873 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/search_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.804208 fastgenerateapi-0.0.4/fastgenerateapi/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/data_type/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/data_type/data_type.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.808197 fastgenerateapi-0.0.4/fastgenerateapi/deps/
+-rw-rw-rw-   0        0        0      160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-06-16 02:41:05.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/filter_params_deps.py
+-rw-rw-rw-   0        0        0     3171 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/paginator_deps.py
+-rw-rw-rw-   0        0        0     1061 2023-06-16 02:55:25.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/tree_params_deps.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.811194 fastgenerateapi-0.0.4/fastgenerateapi/example/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-06-16 05:36:12.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/models.py
+-rw-rw-rw-   0        0        0      195 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/routers.py
+-rw-rw-rw-   0        0        0      400 2023-06-16 05:42:12.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/views.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.814186 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/__init__.py
+-rw-rw-rw-   0        0        0      694 2023-06-16 00:57:41.000000 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/base_model.py
+-rw-rw-rw-   0        0        0     2814 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/json_encoders.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.823157 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/
+-rw-rw-rw-   0        0        0      472 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-16 00:44:35.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/common_function.py
+-rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/create_schema_factory.py
+-rw-rw-rw-   0        0        0     1284 2023-06-16 02:48:31.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/filter_schema_factory.py
+-rw-rw-rw-   0        0        0     3303 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_all_schema_factory.py
+-rw-rw-rw-   0        0        0     2194 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_one_schema_factory.py
+-rw-rw-rw-   0        0        0     3187 2023-06-16 06:21:06.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
+-rw-rw-rw-   0        0        0     1647 2023-06-16 00:43:56.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/response_factory.py
+-rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/update_schema_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.826149 fastgenerateapi-0.0.4/fastgenerateapi/settings/
+-rw-rw-rw-   0        0        0        6 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/settings/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-16 00:40:41.000000 fastgenerateapi-0.0.4/fastgenerateapi/settings/register_settings.py
+-rw-rw-rw-   0        0        0     3952 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.4/fastgenerateapi/settings/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.829141 fastgenerateapi-0.0.4/fastgenerateapi/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/utils/exception.py
+-rw-rw-rw-   0        0        0      670 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/utils/parse_str.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.779753 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2443 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:33:07.830804 fastgenerateapi-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2023-06-15 11:33:14.000000 fastgenerateapi-0.0.4/setup.py
```

### Comparing `fastgenerateapi-0.0.3/LICENSE` & `fastgenerateapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/PKG-INFO` & `fastgenerateapi-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/__init__.py` & `fastgenerateapi-0.0.4/fastgenerateapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 #  Y8ooooo. 88'  `88 88   88 88 88'  `88 88'  `88 88'  `88
 #        88 88    88 88   88 88 88.  .88 88    88 88.  .88
 #  `88888P' dP    dP dP   dP dP `88888P8 dP    dP `8888P88
 #                                                      .88
 #                                                  d8888P
 
 
+from fastgenerateapi.settings.register_settings import settings
 from fastgenerateapi.api_view.api_view import APIView, CreateView, GetOneView, GetAllView, UpdateView, DeleteView, \
     SwitchView
+from fastgenerateapi.api_view.get_tree_view import GetTreeView
 from fastgenerateapi.api_view.delete_tree_view import DeleteTreeView
 from fastgenerateapi.api_view.base_view import BaseView
 from fastgenerateapi.settings.settings import SettingsModel
-from fastgenerateapi.settings.register_settings import register_settings
+
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/api_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/api_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/base_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/base_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional, Type, List, Union, Sequence
 from urllib.parse import parse_qs
 
 from fastapi import params
 from pydantic import create_model
 from starlette.requests import Request
 from tortoise import Model
+from tortoise.expressions import Q
 
 from fastgenerateapi.api_view.mixin.base_mixin import BaseMixin
 from fastgenerateapi.api_view.mixin.dbmodel_mixin import DBModelMixin
 from fastgenerateapi.api_view.mixin.response_mixin import ResponseMixin
 from fastgenerateapi.api_view.mixin.tool_mixin import ToolMixin
 from fastgenerateapi.controller import RouterController
 from fastgenerateapi.pydantic_utils.base_model import BaseModel
@@ -71,17 +72,15 @@
         if self.model_class:
             for route_field in self._get_routes(is_controller_field=True):
                 route_field_func = f"_handler_{route_field.rsplit('_', 1)[0]}_settings"
                 if hasattr(self, route_field) and getattr(self, route_field) and hasattr(self, route_field_func):
                     getattr(self, route_field_func)()
 
     async def get_object(self, pk):
-        queryset = self.model_class.filter(
-            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
-        model = await queryset.filter(id=pk).prefetch_related(
+        model = await self.queryset.filter(pk=pk).prefetch_related(
             *self.prefetch_related_fields.keys()).first()
         if model:
             return model
         else:
             raise NOT_FOUND
 
     @staticmethod
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/create_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/create_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         model = await self.model_class.filter(id=model.id).prefetch_related(
             *self.prefetch_related_fields.keys()).first()
 
         await self.setattr_model(model, prefetch_related_fields=self.prefetch_related_fields)
 
         # await self.setattr_model_rpc(self.rpc_class, model, self.rpc_param)
 
-        return await self.get_one_schema.from_tortoise_orm(model)
+        return self.get_one_schema.from_orm(model)
 
     async def set_create_fields(self, request_data, *args, **kwargs):
         """
         添加属性: request_data.user_id = current_user.id
         """
 
         return self.model_class(**request_data.dict())
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/delete_tree_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_tree_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import time
 from typing import Optional, Type, Any, Union
 
 from fastapi.types import DecoratedCallable
 from starlette.requests import Request
 from starlette.responses import JSONResponse
-from tortoise import Model
 from tortoise.transactions import atomic
 
 from fastgenerateapi.api_view.base_view import BaseView
 from fastgenerateapi.data_type.data_type import CALLABLE, DEPENDENCIES
 from fastgenerateapi.pydantic_utils.base_model import BaseModel, IDList
 from fastgenerateapi.schemas_factory import response_factory
 from fastgenerateapi.settings.register_settings import settings
@@ -24,15 +23,15 @@
     """
 
     @atomic()
     async def destroy_tree(self, request_data, request, *args, **kwargs):
         delete_id_list = request_data.id_list
         parent_id_list = delete_id_list
         while parent_id_list:
-            children_id_list = await self.model_class.filter(parent_id__in=parent_id_list).values_list(self._get_pk_field(self.model_class), flat=True)
+            children_id_list = await self.queryset.filter(parent_id__in=parent_id_list).values_list(self._get_pk_field(self.model_class), flat=True)
             if children_id_list:
                 delete_id_list += children_id_list
                 parent_id_list = delete_id_list
             else:
                 break
 
         request_data.id_list = delete_id_list
@@ -47,30 +46,28 @@
                         setattr(model, field, getattr(model, field) + f"__{int(time.time() * 1000)}")
                 await model.save()
         else:
             await queryset.update(is_active=False)
         return
 
     async def get_del_tree_queryset(self, request_data, *args, **kwargs):
-        queryset = self.model_class.filter(
-            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
-        queryset = queryset.filter(id__in=request_data.id_list)
+        queryset = self.queryset.filter(id__in=request_data.id_list)
         return queryset
 
     def _delete_tree_decorator(self, *args: Any, **kwargs: Any) -> DecoratedCallable:
         async def route(
                 request_data: self.delete_tree_schema,  # type: ignore
                 request: Request,
         ) -> JSONResponse:
             await self.destroy_tree(
                 request_data=request_data,
                 request=request,
                 *args, **kwargs
             )
-            return await self.success(msg="删除成功")
+            return self.success(msg="删除成功")
         return route
 
     def _handler_delete_tree_settings(self):
         if not hasattr(self, "get_one_response_schema"):
             self.get_one_response_schema = response_factory(None, name="GetOne")
         if self.delete_tree_route:
             doc = self.destroy_tree.__doc__
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/delete_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,30 +36,28 @@
                         setattr(model, field, getattr(model, field) + f"__{int(time.time() * 1000)}")
                 await model.save()
         else:
             await queryset.update(is_active=False)
         return
 
     async def get_del_queryset(self, request_data, *args, **kwargs):
-        queryset = self.model_class.filter(
-            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
-        queryset = queryset.filter(id__in=request_data.id_list)
+        queryset = self.queryset.filter(id__in=request_data.id_list)
         return queryset
 
     def _delete_decorator(self, *args: Any, **kwargs: Any) -> DecoratedCallable:
         async def route(
                 request_data: self.delete_schema,  # type: ignore
                 request: Request,
         ) -> JSONResponse:
             await self.destroy(
                 request_data=request_data,
                 request=request,
                 *args, **kwargs
             )
-            return await self.success(msg="删除成功")
+            return self.success(msg="删除成功")
         return route
 
     def _handler_delete_settings(self):
         if not hasattr(self, "get_one_response_schema"):
             self.get_one_response_schema = response_factory(None, name="GetOne")
         if self.delete_route:
             doc = self.destroy.__doc__
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_all_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_all_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 
         return await self.pagination_data(queryset=queryset, request=request, fields=None, *args, **kwargs)
 
     async def get_queryset(self, search: str, filters: dict, *args, **kwargs) -> QuerySet:
         """
         处理search搜索；处理筛选字段；处理外键预加载；处理排序
         """
-        queryset = self.model_class.filter(eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
-        queryset = self.search_controller.query(queryset=queryset, value=search)
+        queryset = self.search_controller.query(queryset=self.queryset, value=search)
         queryset = self.filter_queryset(queryset, filters)
         queryset = self.filter_controller.query(queryset=queryset, values=filters).prefetch_related(
             *self.prefetch_related_fields.keys()).order_by(*self.order_by_fields or [])
 
         return queryset
 
     def filter_queryset(self, queryset: QuerySet, filters: dict) -> QuerySet:
@@ -96,15 +95,15 @@
             # await self.setattr_model_rpc(self.rpc_class, model, self.rpc_param)
             await self.set_get_model(model)
             await self.set_get_all_model(model)
 
             if fields:
                 data_list.append(await self.getattr_model(model=model, fields=fields))
             else:
-                data_list.append(await self.get_all_schema.from_tortoise_orm(model))
+                data_list.append(self.get_all_schema.from_orm(model))
 
         if getattr(paginator, settings.app_settings.DETERMINE_WHETHER_PAGE_FIELD):
             return self.get_list_schema(**{
                 settings.app_settings.LIST_RESPONSE_FIELD: data_list,
             })
 
         return self.get_page_schema(**{
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/get_one_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_one_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         model = await self.get_object(pk)
 
         await self.setattr_model(model, prefetch_related_fields=self.prefetch_related_fields, *args, **kwargs)
 
         # await self.setattr_model_rpc(self.rpc_class, model, self.rpc_param)
         await self.set_get_model(model)
 
-        return await self.get_one_schema.from_tortoise_orm(model)
+        return self.get_one_schema.from_orm(model)
 
     def _get_one_decorator(self, *args: Any, **kwargs: Any) -> DecoratedCallable:
         async def route(
                 pk: str,
                 request: Request,
         ) -> JSONResponse:
             data = await self.get_one(
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/base_mixin.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/base_mixin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 import inspect
 from abc import ABC
 from typing import List, Callable, Any, Union, Optional, Generic, Type
 
 from fastapi import APIRouter
 from fastapi.types import DecoratedCallable
+from tortoise.expressions import Q
+from tortoise.queryset import QuerySet
+
+from fastgenerateapi.settings.register_settings import settings
 from starlette.exceptions import HTTPException
-from tortoise import Model
 
 from fastgenerateapi.data_type.data_type import DEPENDENCIES, T
 
 
 class BaseMixin(Generic[T], APIRouter, ABC):
 
+    @property
+    def queryset(self) -> QuerySet:
+        if not self.model_class:
+            return self.error(msg="model_class not allow None")
+        queryset = self.model_class.filter(
+            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
+        return queryset
+
     @staticmethod
     def _get_routes(is_controller_field: bool = False) -> List[str]:
         if is_controller_field:
-            return ["get_one_route", "get_all_route", "create_route",
+            return ["get_one_route", "get_all_route", "get_tree_route", "create_route",
                     "update_route", "delete_route", "delete_tree_route", "switch_route_fields"]
-        return ["get_one", "get_all", "create",  "update", "destroy", "delete_tree", "switch"]
+        return ["get_one", "get_all", "get_tree", "create",  "update", "destroy", "destroy_tree", "switch"]
 
     @classmethod
     def _get_cls_func(cls):
         func_list = inspect.getmembers(cls, inspect.isfunction)
         return [func[0] for func in func_list if func[0].startswith("view_")]
 
     def _add_api_route(
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/dbmodel_mixin.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/dbmodel_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/response_mixin.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/response_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Union, Optional, Dict, Any
 
 from fastapi import HTTPException
 from fastapi.encoders import jsonable_encoder
 from starlette.background import BackgroundTask
 from starlette.responses import JSONResponse
 
-from fastgenerateapi.pydantic_utils.base_model import JSON_ENCODERS, BaseModel
+from fastgenerateapi.pydantic_utils.base_model import JSON_ENCODERS
+from fastgenerateapi.schemas_factory import response_factory
 
 
-class CommonResponse(BaseModel):
-    success: bool = True
-    code: int = 200
-    message: str = "请求成功"
-    data: Union[dict, str, BaseModel] = {}
+# class CommonResponse(BaseModel):
+#     success: bool = True
+#     code: int = 200
+#     message: str = "请求成功"
+#     data: Union[dict, str, BaseModel] = {}
 
 
 class ResponseMixin:
 
     @staticmethod
     def success(msg: str = "请求成功",
                 status_code: int = 200,
@@ -25,15 +26,15 @@
                 background: Optional[BackgroundTask] = None,
                 *args,
                 **kwargs):
         if data is None:
             json_compatible_data = {}
         else:
             json_compatible_data = jsonable_encoder(data, custom_encoder=JSON_ENCODERS)
-        resp = CommonResponse(success=True, code=code, message=msg, data=json_compatible_data)
+        resp = response_factory()(success=True, code=code, message=msg, data=json_compatible_data)
         kwargs.update(resp.dict())
         return JSONResponse(kwargs, status_code=status_code, background=background)
 
     @staticmethod
     def fail(msg: str = "请求失败",
              status_code: int = 200,
              code: int = -1,
@@ -43,15 +44,15 @@
              *args,
              **kwargs):
 
         if data is None:
             json_compatible_data = {}
         else:
             json_compatible_data = jsonable_encoder(data, custom_encoder=JSON_ENCODERS)
-        resp = CommonResponse(success=success, code=code, message=msg, data=json_compatible_data)
+        resp = response_factory()(success=success, code=code, message=msg, data=json_compatible_data)
         kwargs.update(resp.dict())
         return JSONResponse(kwargs, status_code=status_code, background=background)
 
     @staticmethod
     def error(msg: str = "系统繁忙，请稍后再试...",
               status_code: int = 400,
               headers: Optional[Dict[str, Any]] = None,
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/mixin/tool_mixin.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/tool_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/switch_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/switch_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Optional, Type, Union, List, Any
+from typing import List, Any
 
 from fastapi.types import DecoratedCallable
 from starlette.requests import Request
 from starlette.responses import JSONResponse
-from tortoise import Model
 
 from fastgenerateapi.api_view.base_view import BaseView
 from fastgenerateapi.schemas_factory import response_factory, get_one_schema_factory
 from fastgenerateapi.settings.register_settings import settings
 from fastgenerateapi.utils.exception import NOT_FOUND
 from fastgenerateapi.utils.parse_str import parse_str_to_bool
 
@@ -23,17 +22,15 @@
 
     async def switch(self, pk, request, filed, *args, **kwargs):
         try:
             request_data = await request.json()
         except Exception:
             request_data = {}
 
-        queryset = self.model_class.filter(
-            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
-        model = await queryset.filter(id=pk).first()
+        model = await self.queryset.filter(id=pk).first()
         if not model:
             raise NOT_FOUND
 
         setattr(
             model,
             filed,
             not getattr(model, filed) if request_data.get(filed) is None else parse_str_to_bool(request_data.get(filed))
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/api_view/update_view.py` & `fastgenerateapi-0.0.4/fastgenerateapi/api_view/update_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional, Type, Union, Any
 
 from fastapi.types import DecoratedCallable
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 from tortoise import Model
+from tortoise.expressions import Q
 from tortoise.transactions import atomic
 
 from fastgenerateapi.api_view.base_view import BaseView
 from fastgenerateapi.api_view.mixin.save_mixin import SaveMixin
 from fastgenerateapi.data_type.data_type import DEPENDENCIES, CALLABLE
 from fastgenerateapi.pydantic_utils.base_model import BaseModel
 from fastgenerateapi.schemas_factory import update_schema_factory, get_one_schema_factory, response_factory
@@ -22,17 +23,15 @@
     """
     update_schema: 修改请求模型
     update_route: 修改路由开关，可以放依赖函数列表
     """
 
     @atomic()
     async def update(self, pk: str, request_data, *args, **kwargs):
-        queryset = self.model_class.filter(
-            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
-        model = await queryset.filter(id=pk).first()
+        model = await self.get_object(pk)
         if not model:
             raise NOT_FOUND
 
         request_data = await self.set_update_fields(request_data=request_data, *args, **kwargs)
 
         await self.check_unique_field(request_data, model_class=self.model_class, model=model)
 
@@ -42,15 +41,15 @@
 
         await model.update_from_dict(request_data.dict(exclude_none=True)).save()
 
         await self.setattr_model(model, prefetch_related_fields=self.prefetch_related_fields, *args, **kwargs)
 
         # await self.setattr_model_rpc(self.rpc_class, model, self.rpc_param)
 
-        return await self.schema.from_tortoise_orm(model)
+        return self.update_schema.from_orm(model)
 
     @staticmethod
     async def set_update_fields(request_data, *args, **kwargs):
         """
         修改属性: request_data.user_id = current_user.id
         """
         return request_data
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/controller/filter_controller.py` & `fastgenerateapi-0.0.4/fastgenerateapi/controller/filter_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/controller/router_controller.py` & `fastgenerateapi-0.0.4/fastgenerateapi/controller/router_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/controller/rpc_controller.py` & `fastgenerateapi-0.0.4/fastgenerateapi/controller/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/controller/search_controller.py` & `fastgenerateapi-0.0.4/fastgenerateapi/controller/search_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/data_type/data_type.py` & `fastgenerateapi-0.0.4/fastgenerateapi/data_type/data_type.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/deps/filter_params_deps.py` & `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/filter_schema_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Type, Union, Any
+from typing import Type, Union
 
-from fastapi import Query, Depends
-from pydantic import create_model
+from fastapi import Query
+from fastgenerateapi.pydantic_utils.base_model import QueryConfig
+from pydantic import BaseModel, create_model
 from pydantic.fields import FieldInfo
-from tortoise import Model
 
 from fastgenerateapi.api_view.mixin.dbmodel_mixin import DBModelMixin
 from fastgenerateapi.controller.filter_controller import BaseFilter
-from fastgenerateapi.pydantic_utils.base_model import BaseModel, QueryConfig
+from tortoise import Model
 
 
-def filter_params_deps(model_class: Type[Model], fields: list[str, tuple[str, Type], BaseFilter] = None):
+def filter_schema_factory(model_class: Type[Model], fields: list[str, tuple[str, Type], BaseFilter] = None):
     """
-        生成filter依赖
+        generate filter schema
     """
     model_fields = {}
 
     for field_info in fields or []:
         if not isinstance(field_info, BaseFilter):
             field_info = BaseFilter(field_info)
         f = field_info.filter_field
@@ -30,17 +30,11 @@
                     default=Query(""),
                     description=f"{DBModelMixin.get_field_description(model_class, field_info.model_field)}"
                 ))
         })
 
     filter_params_model: Type[BaseModel] = create_model(__model_name="CommonFilterParams", **model_fields, __config__=QueryConfig)
 
-    def filter_query(filter_params: filter_params_model = Depends(filter_params_model)) -> dict[str, Any]:
-        """
-            filter 筛选字段依赖
-        :param filter_params:
-        :return:
-        """
-        result = filter_params.dict(exclude_none=True)
-        return result
+    return filter_params_model
+
+
 
-    return filter_query
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/deps/paginator_deps.py` & `fastgenerateapi-0.0.4/fastgenerateapi/deps/paginator_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/pydantic_utils/json_encoders.py` & `fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/json_encoders.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/common_function.py` & `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/common_function.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/create_schema_factory.py` & `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/create_schema_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Type
 
+from fastgenerateapi.settings.register_settings import settings
+
+from fastgenerateapi.pydantic_utils.base_model import Config
 from pydantic import create_model
 from tortoise import Model
 
 from fastgenerateapi.data_type.data_type import T
 from fastgenerateapi.schemas_factory.common_function import get_dict_from_model_fields, get_dict_from_pydanticmeta
 
 
@@ -26,19 +29,27 @@
             get_one_include_fields_dict = get_dict_from_pydanticmeta(model_class, model_class.PydanticMeta.create_include)
             all_fields_info.update(get_one_include_fields_dict)
             include_fields.update(get_one_include_fields_dict.keys())
         if hasattr(model_class.PydanticMeta, "exclude"):
             exclude_fields.update(model_class.PydanticMeta.exclude)
         if hasattr(model_class.PydanticMeta, "create_exclude"):
             exclude_fields.update(model_class.PydanticMeta.create_exclude)
+    else:
+        include_fields.update(all_fields_info.keys())
 
     all_fields = include_fields.difference(exclude_fields)
     try:
+        if settings.app_settings.CREATE_EXCLUDE_ACTIVE_VALUE:
+            try:
+                all_fields.remove(settings.app_settings.WHETHER_DELETE_FIELD)
+            except Exception:
+                ...
         all_fields.remove(model_class._meta.pk_attr)
     except Exception:
         ...
 
     name = model_class.__name__ + "CreateSchema"
-    schema: Type[T] = create_model(__model_name=name, **{field: all_fields_info[field] for field in all_fields})
+    schema: Type[T] = create_model(
+        __model_name=name, **{field: all_fields_info[field] for field in all_fields}, __config__=Config)
     return schema
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_all_schema_factory.py` & `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_all_schema_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,52 +21,58 @@
 
     all_fields_info = get_dict_from_model_fields(model_class)
 
     include_fields = set()
     exclude_fields = set()
 
     get_all_include_fields_dict = get_dict_from_pydanticmeta(model_class, model_class.PydanticMeta.get_all_include)
-    all_fields_info = get_all_include_fields_dict.update(all_fields_info)
+    all_fields_info.update(get_all_include_fields_dict)
     include_fields.update(get_all_include_fields_dict.keys())
     if hasattr(model_class.PydanticMeta, "include"):
         include_fields_dict = get_dict_from_pydanticmeta(model_class, model_class.PydanticMeta.include)
-        all_fields_info = include_fields_dict.update(all_fields_info)
+        all_fields_info.update(include_fields_dict)
         include_fields.update(include_fields_dict.keys())
     else:
         include_fields.update(all_fields_info.keys())
 
     exclude_fields.update(model_class.PydanticMeta.get_all_exclude)
     if hasattr(model_class.PydanticMeta, "exclude"):
         exclude_fields.update(model_class.PydanticMeta.exclude)
 
     all_fields = include_fields.difference(exclude_fields)
+    if settings.app_settings.GET_EXCLUDE_ACTIVE_VALUE:
+        try:
+            all_fields.remove(settings.app_settings.WHETHER_DELETE_FIELD)
+        except Exception:
+            ...
 
     name = model_class.__name__ + "GetAllSchema"
-    schema: Type[T] = create_model(__model_name=name, **{field: all_fields_info[field] for field in all_fields}, __config__=Config)
+    schema: Type[T] = create_model(
+        __model_name=name, **{field: all_fields_info[field] for field in all_fields}, __config__=Config)
     return schema
 
 
 def get_list_schema_factory(schema_cls: Type[T]) -> Type[T]:
     fields = {
         settings.app_settings.LIST_RESPONSE_FIELD: (Optional[List[schema_cls]], FieldInfo(default=[], description="数据返回")),
     }
     name = schema_cls.__name__ + "GetListSchema"
-    schema: Type[T] = create_model(__model_name=name, **fields)
+    schema: Type[T] = create_model(__model_name=name, **fields, __config__=Config)
     return schema
 
 
 def get_page_schema_factory(schema_cls: Type[T]) -> Type[T]:
     fields = {
         settings.app_settings.CURRENT_PAGE_FIELD: (Optional[int], FieldInfo(default=1, description="当前页")),
         settings.app_settings.PAGE_SIZE_FIELD: (Optional[int], FieldInfo(default=settings.app_settings.DEFAULT_PAGE_SIZE, description="每页数量")),
         settings.app_settings.TOTAL_SIZE_FIELD: (Optional[int], FieldInfo(default=0, description="数量总计")),
         settings.app_settings.LIST_RESPONSE_FIELD: (Optional[List[schema_cls]], FieldInfo(default=[], description="数据返回")),
     }
     name = schema_cls.__name__ + "GetPageSchema"
-    schema: Type[T] = create_model(__model_name=name, **fields)
+    schema: Type[T] = create_model(__model_name=name, **fields, __config__=Config)
     return schema
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/get_one_schema_factory.py` & `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_one_schema_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from typing import Type
+from typing import Type, Optional
 
+from fastgenerateapi.settings.register_settings import settings
+
+from fastgenerateapi.pydantic_utils.base_model import Config
 from pydantic import create_model
 from tortoise import Model
 
 from fastgenerateapi.data_type.data_type import T
 from fastgenerateapi.schemas_factory.common_function import get_dict_from_model_fields, get_dict_from_pydanticmeta
 
 
 def get_one_schema_factory(model_class: Type[Model]) -> Type[T]:
     """
     Is used to create a GetOneSchema
     """
-    all_fields_info = get_dict_from_model_fields(model_class)
+    all_fields_info: dict = get_dict_from_model_fields(model_class)
 
     include_fields = set()
     exclude_fields = set()
     if hasattr(model_class, "PydanticMeta"):
         if hasattr(model_class.PydanticMeta, "include"):
             include_fields_dict = get_dict_from_pydanticmeta(model_class, model_class.PydanticMeta.include)
             all_fields_info.update(include_fields_dict)
@@ -26,16 +29,25 @@
             get_one_include_fields_dict = get_dict_from_pydanticmeta(model_class, model_class.PydanticMeta.get_one_include)
             all_fields_info.update(get_one_include_fields_dict)
             include_fields.update(get_one_include_fields_dict.keys())
         if hasattr(model_class.PydanticMeta, "exclude"):
             exclude_fields.update(model_class.PydanticMeta.exclude)
         if hasattr(model_class.PydanticMeta, "get_one_exclude"):
             exclude_fields.update(model_class.PydanticMeta.get_one_exclude)
+    else:
+        include_fields.update(all_fields_info.keys())
 
     all_fields = include_fields.difference(exclude_fields)
 
+    if settings.app_settings.GET_EXCLUDE_ACTIVE_VALUE:
+        try:
+            all_fields.remove(settings.app_settings.WHETHER_DELETE_FIELD)
+        except Exception:
+            ...
+
     name = model_class.__name__ + "GetOneSchema"
-    schema: Type[T] = create_model(__model_name=name, **{field: all_fields_info[field] for field in all_fields})
+    schema: Type[T] = create_model(
+        __model_name=name, **{field: all_fields_info[field] for field in all_fields}, __config__=Config)
     return schema
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/response_factory.py` & `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/response_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 from typing import Type, Union, Optional
 
 from pydantic import create_model
 from pydantic.fields import FieldInfo
 
 from fastgenerateapi.data_type.data_type import T
-from fastgenerateapi.pydantic_utils.base_model import BaseModel
+from fastgenerateapi.pydantic_utils.base_model import BaseModel, Config
 from fastgenerateapi.settings.register_settings import settings
 
 
-def response_factory(schema_cls: Union[Type[T], BaseModel, None], name: str = "") -> Type[T]:
-    fields = {
-        settings.app_settings.MESSAGE_RESPONSE_FIELD: (str, FieldInfo(default="请求成功", description="返回消息")),
-        settings.app_settings.DATA_RESPONSE_FIELD: (schema_cls or dict, FieldInfo(default={}, description="数据内容")),
-    }
+def response_factory(schema_cls: Union[Type[T], BaseModel, None] = None, name: str = "") -> Type[T]:
+    fields = {}
     if settings.app_settings.CODE_RESPONSE_FIELD:
         default_code_field = FieldInfo(default=200, description="编码")
         fields.setdefault("code", (Optional[int], default_code_field))
     if settings.app_settings.SUCCESS_RESPONSE_FIELD:
         default_success_field = FieldInfo(default=True, description="是否请求成功")
         fields.setdefault("success", (Optional[bool], default_success_field))
-
-    name = schema_cls.__name__ + name + "Response"
-    schema: Type[T] = create_model(__model_name=name, **fields)
+    fields.setdefault(
+        settings.app_settings.MESSAGE_RESPONSE_FIELD,
+        (str, FieldInfo(default="请求成功", description="返回消息")),
+    )
+    if schema_cls:
+        fields.setdefault(
+            settings.app_settings.DATA_RESPONSE_FIELD,
+            (Optional[schema_cls], FieldInfo(default={}, description="数据内容"))
+        )
+    else:
+        fields.setdefault(
+            settings.app_settings.DATA_RESPONSE_FIELD,
+            (Union[dict, str, None], FieldInfo(default={}, description="数据内容"))
+        )
+
+    try:
+        name = schema_cls.__name__ + name + "Response"
+    except:
+        name = "CommonResponse"
+    schema: Type[T] = create_model(__model_name=name, **fields, __config__=Config)
 
     return schema
 
 
 
 
 
 
-
-
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/schemas_factory/update_schema_factory.py` & `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/update_schema_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Type
 
+from fastgenerateapi.settings.register_settings import settings
+
+from fastgenerateapi.pydantic_utils.base_model import Config
 from pydantic import create_model
 from tortoise import Model
 
 from fastgenerateapi.data_type.data_type import T
 from fastgenerateapi.schemas_factory.common_function import get_dict_from_model_fields, get_dict_from_pydanticmeta
 
 
@@ -26,19 +29,27 @@
             get_one_include_fields_dict = get_dict_from_pydanticmeta(model_class, model_class.PydanticMeta.update_include)
             all_fields_info.update(get_one_include_fields_dict)
             include_fields.update(get_one_include_fields_dict.keys())
         if hasattr(model_class.PydanticMeta, "exclude"):
             exclude_fields.update(model_class.PydanticMeta.exclude)
         if hasattr(model_class.PydanticMeta, "update_exclude"):
             exclude_fields.update(model_class.PydanticMeta.update_exclude)
+    else:
+        include_fields.update(all_fields_info.keys())
 
     all_fields = include_fields.difference(exclude_fields)
     try:
+        if settings.app_settings.UPDATE_EXCLUDE_ACTIVE_VALUE:
+            try:
+                all_fields.remove(settings.app_settings.WHETHER_DELETE_FIELD)
+            except Exception:
+                ...
         all_fields.remove(model_class._meta.pk_attr)
     except Exception:
         ...
 
     name = model_class.__name__ + "UpdateSchema"
-    schema: Type[T] = create_model(__model_name=name, **{field: all_fields_info[field] for field in all_fields})
+    schema: Type[T] = create_model(
+        __model_name=name, **{field: all_fields_info[field] for field in all_fields}, __config__=Config)
     return schema
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/settings/settings.py` & `fastgenerateapi-0.0.4/fastgenerateapi/settings/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 from typing import Optional
 
-from pydantic import BaseSettings as PydanticSettings, Field, BaseModel
+from pydantic import BaseSettings, Field, BaseModel
 
 
-class AppSettings(PydanticSettings):
+class AppSettings(BaseSettings):
     # 分页对应字段以及配置默认值
     CURRENT_PAGE_FIELD: Optional[str] = Field(default='page', description="当前页字段")
     PAGE_SIZE_FIELD: Optional[str] = Field(default='page_size', description="每页数量字段")
     TOTAL_SIZE_FIELD: Optional[str] = Field(default='total', description="统计数量字段")
     DETERMINE_WHETHER_PAGE_FIELD: Optional[str] = Field(default='no_page', description="判断是否分页字段")
     DEFAULT_PAGE_SIZE: Optional[int] = Field(default=10, description="默认每页数量")
     DEFAULT_WHETHER_PAGE: Optional[bool] = Field(default=False, description="默认是否分页")
     DEFAULT_MAX_PAGE_SIZE: Optional[int] = Field(default=200, description="默认最大每页数量")
 
     # 路由后缀字段是否添加以及配置默认值
     ROUTER_WHETHER_ADD_SUFFIX: Optional[bool] = Field(default=True, description="增删改查路由是否添加后缀")
-    ROUTER_CREATE_SUFFIX_FIELD: Optional[str] = Field(default='create', description="创建后缀字段")
-    ROUTER_GET_ONE_SUFFIX_FIELD: Optional[str] = Field(default='get-one', description="获取一个后缀字段")
-    ROUTER_GET_ALL_SUFFIX_FIELD: Optional[str] = Field(default='get-all', description="获取列表后缀字段")
-    ROUTER_UPDATE_SUFFIX_FIELD: Optional[str] = Field(default='update', description="修改后缀字段")
-    ROUTER_DELETE_SUFFIX_FIELD: Optional[str] = Field(default='delete', description="删除后缀字段")
-    ROUTER_RECURSION_DELETE_SUFFIX_FIELD: Optional[str] = Field(default='delete-tree', description="递归删除后缀字段")
+    ROUTER_CREATE_SUFFIX_FIELD: Optional[str] = Field(default='create', description="创建路由后缀字段")
+    ROUTER_GET_ONE_SUFFIX_FIELD: Optional[str] = Field(default='get-one', description="获取一个路由后缀字段")
+    ROUTER_GET_ALL_SUFFIX_FIELD: Optional[str] = Field(default='get-all', description="获取列表路由后缀字段")
+    ROUTER_GET_TREE_SUFFIX_FIELD: Optional[str] = Field(default='get-tree', description="获取树状数据路由后缀字段")
+    ROUTER_UPDATE_SUFFIX_FIELD: Optional[str] = Field(default='update', description="修改路由后缀字段")
+    ROUTER_DELETE_SUFFIX_FIELD: Optional[str] = Field(default='delete', description="删除路由后缀字段")
+    ROUTER_RECURSION_DELETE_SUFFIX_FIELD: Optional[str] = Field(default='delete-tree', description="递归删除路由后缀字段")
 
     # 数据库字段默认值
     WHETHER_DELETE_FIELD: Optional[str] = Field(default="is_active", description="是否删除字段")
-    ACTIVE_DEFAULT_VALUE: Optional[bool] = Field(default=True, description="有效的默认值值")
+    ACTIVE_DEFAULT_VALUE: Optional[bool] = Field(default=True, description="有效的默认值")
+    GET_EXCLUDE_ACTIVE_VALUE: Optional[bool] = Field(default=True, description="查询结果是否排除有效字段")
+    CREATE_EXCLUDE_ACTIVE_VALUE: Optional[bool] = Field(default=True, description="创建是否排除有效字段")
+    UPDATE_EXCLUDE_ACTIVE_VALUE: Optional[bool] = Field(default=True, description="修改是否排除有效字段")
+    DEFAULT_TREE_PARENT_FIELD: Optional[str] = Field(default="parent", description="默认递归父级字段")
+    DEFAULT_TREE_CHILDREN_FIELD: Optional[str] = Field(default="children", description="默认递归子级字段")
+    DEFAULT_TREE_FILTER_FIELD: Optional[str] = Field(default="begin_id", description="默认递归起点筛选字段")
 
     # 返回格式字段配置默认值
     CODE_RESPONSE_FIELD: Optional[bool] = Field(default=True, description="code返回字段")
     SUCCESS_RESPONSE_FIELD: Optional[bool] = Field(default=True, description="success返回字段")
     MESSAGE_RESPONSE_FIELD: Optional[str] = Field(default="message", description="消息返回字段")
     DATA_RESPONSE_FIELD: Optional[str] = Field(default="data", description="数据返回字段")
     LIST_RESPONSE_FIELD: Optional[str] = Field(default='list', description="列表页返回字段")
 
     # GetAll 筛选是否双下划线转单下划线
     FILTER_UNDERLINE_WHETHER_DOUBLE_TO_SINGLE: Optional[bool] = Field(default=True, description="筛选是否双下划线转单下划线")
     SCHEMAS_UNDERLINE_WHETHER_DOUBLE_TO_SINGLE: Optional[bool] = Field(default=True, description="序列化字段是否双下划线转单下划线")
 
     class Config:
         env_prefix = 'APP_'
+        env_file = "./.env"
         case_sensitive = True
 
 
 class SettingsModel(BaseModel):
     # 系统配置
     app_settings: AppSettings = AppSettings()
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi/utils/parse_str.py` & `fastgenerateapi-0.0.4/fastgenerateapi/utils/parse_str.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi.egg-info/PKG-INFO` & `fastgenerateapi-0.0.4/fastgenerateapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.3/fastgenerateapi.egg-info/SOURCES.txt` & `fastgenerateapi-0.0.4/fastgenerateapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 fastgenerateapi/api_view/api_view.py
 fastgenerateapi/api_view/base_view.py
 fastgenerateapi/api_view/create_view.py
 fastgenerateapi/api_view/delete_tree_view.py
 fastgenerateapi/api_view/delete_view.py
 fastgenerateapi/api_view/get_all_view.py
 fastgenerateapi/api_view/get_one_view.py
+fastgenerateapi/api_view/get_tree_view.py
 fastgenerateapi/api_view/switch_view.py
 fastgenerateapi/api_view/update_view.py
 fastgenerateapi/api_view/mixin/__init__.py
 fastgenerateapi/api_view/mixin/base_mixin.py
 fastgenerateapi/api_view/mixin/dbmodel_mixin.py
 fastgenerateapi/api_view/mixin/get_mixin.py
 fastgenerateapi/api_view/mixin/response_mixin.py
@@ -29,22 +30,29 @@
 fastgenerateapi/controller/rpc_controller.py
 fastgenerateapi/controller/search_controller.py
 fastgenerateapi/data_type/__init__.py
 fastgenerateapi/data_type/data_type.py
 fastgenerateapi/deps/__init__.py
 fastgenerateapi/deps/filter_params_deps.py
 fastgenerateapi/deps/paginator_deps.py
+fastgenerateapi/deps/tree_params_deps.py
+fastgenerateapi/example/__init__.py
+fastgenerateapi/example/models.py
+fastgenerateapi/example/routers.py
+fastgenerateapi/example/views.py
 fastgenerateapi/pydantic_utils/__init__.py
 fastgenerateapi/pydantic_utils/base_model.py
 fastgenerateapi/pydantic_utils/json_encoders.py
 fastgenerateapi/schemas_factory/__init__.py
 fastgenerateapi/schemas_factory/common_function.py
 fastgenerateapi/schemas_factory/create_schema_factory.py
+fastgenerateapi/schemas_factory/filter_schema_factory.py
 fastgenerateapi/schemas_factory/get_all_schema_factory.py
 fastgenerateapi/schemas_factory/get_one_schema_factory.py
+fastgenerateapi/schemas_factory/get_tree_schema_factory.py
 fastgenerateapi/schemas_factory/response_factory.py
 fastgenerateapi/schemas_factory/update_schema_factory.py
 fastgenerateapi/settings/__init__.py
 fastgenerateapi/settings/register_settings.py
 fastgenerateapi/settings/settings.py
 fastgenerateapi/utils/__init__.py
 fastgenerateapi/utils/exception.py
```

### Comparing `fastgenerateapi-0.0.3/setup.py` & `fastgenerateapi-0.0.4/setup.py`

 * *Files identical despite different names*

