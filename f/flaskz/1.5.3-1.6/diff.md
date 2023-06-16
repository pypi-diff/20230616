# Comparing `tmp/flaskz-1.5.3.tar.gz` & `tmp/flaskz-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.5.3.tar", last modified: Thu Jun  1 02:01:12 2023, max compression
+gzip compressed data, was "flaskz-1.6.tar", last modified: Fri Jun 16 02:00:30 2023, max compression
```

## Comparing `flaskz-1.5.3.tar` & `flaskz-1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.719781 flaskz-1.5.3/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.5.3/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     6475 2023-06-01 02:01:12.720056 flaskz-1.5.3/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     6038 2023-06-01 01:51:10.000000 flaskz-1.5.3/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.5.3/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      704 2023-06-01 02:01:12.721183 flaskz-1.5.3/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.683712 flaskz-1.5.3/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.688234 flaskz-1.5.3/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-06-01 01:51:53.000000 flaskz-1.5.3/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.693620 flaskz-1.5.3/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.5.3/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.5.3/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.697041 flaskz-1.5.3/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.5.3/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.5.3/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)     9693 2023-04-26 10:31:33.000000 flaskz-1.5.3/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.698109 flaskz-1.5.3/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2256 2023-05-15 03:14:20.000000 flaskz-1.5.3/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.703009 flaskz-1.5.3/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5488 2023-05-17 02:06:29.000000 flaskz-1.5.3/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    26672 2023-05-17 02:34:00.000000 flaskz-1.5.3/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.5.3/src/flaskz/models/_model.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6450 2023-05-27 16:43:07.000000 flaskz-1.5.3/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.5.3/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.706321 flaskz-1.5.3/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    19354 2023-04-27 11:45:35.000000 flaskz-1.5.3/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.5.3/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.5.3/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.718852 flaskz-1.5.3/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-05-10 07:01:15.000000 flaskz-1.5.3/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.5.3/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.5.3/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.5.3/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.5.3/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.5.3/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.5.3/src/flaskz/utils/_magic.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6497 2023-05-30 05:37:32.000000 flaskz-1.5.3/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7742 2023-05-16 02:51:46.000000 flaskz-1.5.3/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.5.3/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.5.3/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-01 02:01:12.691937 flaskz-1.5.3/src/flaskz.egg-info/
--rwxrwxrwx   0 taozh      (501) staff       (20)     6475 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-06-01 02:01:12.000000 flaskz-1.5.3/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.283067 flaskz-1.6/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.6/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     6853 2023-06-16 02:00:30.283321 flaskz-1.6/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6424 2023-06-15 11:25:44.000000 flaskz-1.6/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.6/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      702 2023-06-16 02:00:30.284472 flaskz-1.6/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.246590 flaskz-1.6/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.252130 flaskz-1.6/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       21 2023-06-15 02:00:26.000000 flaskz-1.6/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.257568 flaskz-1.6/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.6/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.6/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.260418 flaskz-1.6/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.6/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.6/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    12268 2023-06-15 11:27:27.000000 flaskz-1.6/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.261459 flaskz-1.6/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2256 2023-05-15 03:14:20.000000 flaskz-1.6/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.266429 flaskz-1.6/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5488 2023-05-17 02:06:29.000000 flaskz-1.6/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    29199 2023-06-15 11:27:27.000000 flaskz-1.6/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.6/src/flaskz/models/_model.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6450 2023-05-27 16:43:07.000000 flaskz-1.6/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.6/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.270163 flaskz-1.6/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    19434 2023-06-15 03:31:44.000000 flaskz-1.6/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.6/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.6/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.282134 flaskz-1.6/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-05-10 07:01:15.000000 flaskz-1.6/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.6/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.6/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.6/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.6/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.6/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.6/src/flaskz/utils/_magic.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6497 2023-05-30 05:37:32.000000 flaskz-1.6/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     9086 2023-06-15 11:19:30.000000 flaskz-1.6/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.6/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.6/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.255860 flaskz-1.6/src/flaskz.egg-info/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6853 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.5.3/LICENSE` & `flaskz-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/PKG-INFO` & `flaskz-1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.5.3
+Version: 1.6
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,37 +24,43 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6** `2023/06/16`
+    - [A] `BaseModelMixin`添加`count`方法，用于数量查询(全量/条件)
+    - [A] `BaseModelMixin`添加`clear_db`方法，用于清空数据
+    - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
+    - [A] `flaskz.ext.ssh`添加对Paramiko>=3.0.0版本的支持
+    - [A] `flaskz.ext.ssh`添加`secondary_password`和`recv_endswith`参数
 - **1.5.3** `2023/06/01`
     - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
     - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
-    - [A] 重构`flaskz.rest`路由生成模块*
+    - [A] 扩展`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
         - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
         - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
         - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
         - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
         - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
         - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
     - [A] `ModelMixin.query_pss`方法支持多列排序*
     - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
     - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
     - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
     - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
-    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决<2.2.3版本的Flask不会将结尾不带`/`的请求重定向到带`/`路由的问题
+    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决Flask<2.2.3版本不会将结尾不带`/`的请求重定向到带`/`路由的问题
 - **1.3** `2023/03/01`
     - [A] `init_model_rest_blueprint`函数生成的query路由, 添加对单个数据的查询功能(`[GET]url_prefix/did/`)
     - [A] `init_model_rest_blueprint`函数生成的update路由, 添加URL主键支持(`[PATCH]url_prefix/did/`)
     - [C] `init_model_rest_blueprint`函数生成的delete路由, 结尾添加`/`, 用于支持以`/`结尾的URL删除请求(`[DELETE]url_prefix/did/`)
     - [A] 添加`FLASKZ_DATABASE_ENGINE_KWARGS`参数, 用于自定义engine参数
 - **1.2** `2023/02/01`
     - [A] 添加`FLASKZ_DATABASE_POOL_PRE_PING`参数, 用于设置engine的`pool_pre_ping`参数
```

### Comparing `flaskz-1.5.3/README.md` & `flaskz-1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,37 +9,43 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6** `2023/06/16`
+    - [A] `BaseModelMixin`添加`count`方法，用于数量查询(全量/条件)
+    - [A] `BaseModelMixin`添加`clear_db`方法，用于清空数据
+    - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
+    - [A] `flaskz.ext.ssh`添加对Paramiko>=3.0.0版本的支持
+    - [A] `flaskz.ext.ssh`添加`secondary_password`和`recv_endswith`参数
 - **1.5.3** `2023/06/01`
     - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
     - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
-    - [A] 重构`flaskz.rest`路由生成模块*
+    - [A] 扩展`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
         - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
         - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
         - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
         - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
         - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
         - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
     - [A] `ModelMixin.query_pss`方法支持多列排序*
     - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
     - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
     - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
     - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
-    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决<2.2.3版本的Flask不会将结尾不带`/`的请求重定向到带`/`路由的问题
+    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决Flask<2.2.3版本不会将结尾不带`/`的请求重定向到带`/`路由的问题
 - **1.3** `2023/03/01`
     - [A] `init_model_rest_blueprint`函数生成的query路由, 添加对单个数据的查询功能(`[GET]url_prefix/did/`)
     - [A] `init_model_rest_blueprint`函数生成的update路由, 添加URL主键支持(`[PATCH]url_prefix/did/`)
     - [C] `init_model_rest_blueprint`函数生成的delete路由, 结尾添加`/`, 用于支持以`/`结尾的URL删除请求(`[DELETE]url_prefix/did/`)
     - [A] 添加`FLASKZ_DATABASE_ENGINE_KWARGS`参数, 用于自定义engine参数
 - **1.2** `2023/02/01`
     - [A] 添加`FLASKZ_DATABASE_POOL_PRE_PING`参数, 用于设置engine的`pool_pre_ping`参数
```

### Comparing `flaskz-1.5.3/src/flaskz/auth/_jws.py` & `flaskz-1.6/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/ext/cypher.py` & `flaskz-1.6/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/ext/ssh.py` & `flaskz-1.6/src/flaskz/ext/ssh.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,51 +4,79 @@
 import errno
 import os
 import re
 import socket
 import stat
 import time
 from contextlib import contextmanager
-from datetime import datetime
 
 import paramiko
 from paramiko.ssh_exception import SSHException
-from paramiko.util import retry_on_signal
 
 
 @contextmanager
 def ssh_session(hostname, username, password=None, port=22, **kwargs):
     """
     SSH contextmanager.
 
     Example:
         with ssh_session(host, username, password, timeout=20) as ssh:
-            ssh.run_command("ls -l")
+            ssh.run_command('ls -l')
+
+        with ssh_session(host, username, password, timeout=20) as ssh:
+            ssh.run_command_list(['show version', 'show running-config'])
+
+        with ssh_session(host, username, password, timeout=20, secondary_password=enable_pwd, recv_endswith=['# ', '$ ', ': ', '? ', '#']) as ssh:
+            ssh.run_command_list(['enable', 'show run'])
 
     """
     ssh_client = SSH(hostname=hostname, username=username, password=password, port=port, **kwargs)
     yield ssh_client
     ssh_client.close()
 
 
 class SSH(object):
     def __init__(self, hostname, username, password=None, port=22, **kwargs):
         """
         Create a SSH instance.
 
+        .. versionupdated:: 1.6 - add secondary_password and recv_endswith kwargs
+
         Example:
             ssh = SSH(host, username, password, timeout=20)
+            ssh.run_command('ls -l')
+
+            ssh = SSH(host, username, password, timeout=20)
+            ssh.run_command_list(['enable', enable_pwd, 'show run'])
+
+            ssh = SSH(host, username, password, timeout=20, secondary_password=enable_pwd, recv_endswith=['# ', '$ ', ': ', '? ', '#'])
+            ssh.run_command_list(['enable', 'show run'])
+
+
+        :param hostname: the host(address) to ssh
+        :param username: the username of the host
+        :param password: the password of the host
+        :param port: the ssh port, default is 22
+        :param kwargs:
+                - secondary_password: use for enable/sudo action, if None, the password needs to be sent through the command
+                - recv_endswith: use for stop receiving, default is ['# ', '$ ', ': ', '? ']
+                - timeout: timeout on blocking read/write operations & socket timer, default is 0
+                - connect_kwargs: kwargs for Transport.connect()
         """
         self._username = username
         self._password = password
-
+        self._secondary_password = kwargs.pop('secondary_password', None)  # for enable/sudo
+        # recv_endswith = kwargs.pop('recv_endswith', None)  # for stop receiving
+        self.recv_endswith = tuple(kwargs.pop('recv_endswith', None) or ['# ', '$ ', ': ', '? '])  # for stop receiving
         self._timeout = kwargs.pop('timeout', 0)
-        self.transport = paramiko.Transport(_create_socket(hostname=hostname, port=port, timeout=self._timeout))
+
         # self.transport = paramiko.Transport((hostname, port))
-        self.transport.connect(username=username, password=password, **kwargs)
+        self.transport = paramiko.Transport(_create_socket(hostname=hostname, port=port, timeout=self._timeout))
+        _connect_kwargs = kwargs.pop('connect_kwargs', None) or {}  # kwargs for Transport.connect()
+        self.transport.connect(username=username, password=password, **_connect_kwargs)
 
         self.ssh = paramiko.SSHClient()
         self.ssh._transport = self.transport
         self.ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     @property
     def sftp(self):
@@ -65,23 +93,28 @@
         return self._channel
 
     def run_command(self, command):
         """
         Run the command.
 
         Example:
-            ssh.run_command("ls -l")
+            ssh.run_command('ls -l')
+            ssh.run_command('show run')
         """
         command = command.strip()
         self.channel.send(command + '\n')
         output = self._get_output(command)
-
-        if self._password and command.lower().startswith('sudo') and 'assword' in output:  # input password
-            pwd_output = self.run_command(self._password)
-            if 'assword' in pwd_output:
+        enable_commands = ('sudo', 'enable')
+        secondary_password = self._secondary_password  # or self._password
+        if secondary_password and \
+                command.lower().startswith(enable_commands) and \
+                'assword' in output:  # input password
+            pwd_output = self.run_command(secondary_password)
+            # if 'assword' in pwd_output:
+            if pwd_output == output:
                 return output
             return self.run_command(command)
 
         return output
 
     def run_command_list(self, command_list, last_result=False):
         """
@@ -105,15 +138,15 @@
 
     def sftp_get_dir(self, remote_dir, local_dir):
         """
         Download remote direction to local.
         Return the local files list.
 
         Example:
-            ssh.sftp_get_dir("/usr/projects/git/srte/src/", "/Users/taozh/Work/Codes/ssh_test/sftp")
+            ssh.sftp_get_dir('/usr/projects/git/srte/src/', '/Users/taozh/Work/Codes/ssh_test/sftp')
         """
         if not self._path_exists(remote_dir):
             return False
         remote_dir = _remove_end_slash(remote_dir)
         local_dir = _remove_end_slash(local_dir)
         if not os.path.exists(local_dir):
             os.mkdir(local_dir)
@@ -129,15 +162,15 @@
         return local_files
 
     def listdir(self, path, recursion=False):
         """
         List all files in the given path.
 
         Example:
-            ssh.listdir("/usr/projects/git/srte/src/")
+            ssh.listdir('/usr/projects/git/srte/src/')
         """
         all_files = []
         path = _remove_end_slash(path)
         if path[-1] == '/':
             path = path[0:-1]
         files = self.sftp.listdir_attr(path)
         for f in files:
@@ -173,21 +206,22 @@
     def _recv_data(self):
         """Receive the command output"""
         while not self.channel.recv_ready():
             time.sleep(0.01)
         res_list = []
         time.sleep(0.2)  # Solve the problem of incomplete data
         # cmd_pattern = re.compile('.*[#$] ' + command) # Does not work with password entry
+
         while True:
             data = self.channel.recv(1024)
             info = data.decode()
             res = info.replace(' \r', '')
             res_list.append(res)
             if len(info) < 1024:  # read speed > write speed
-                if info.endswith(('# ', '$ ', ': ', '? ')):
+                if info.endswith(self.recv_endswith):  # Cisco C9300:# /
                     break
 
         return ''.join(res_list)
 
 
 def _create_socket(hostname, port, timeout=0):
     """
@@ -195,32 +229,32 @@
     If timeout>0, set the timeout of the instance, otherwise use the default timeout(maybe 75s).
 
     :param hostname:
     :param port:
     :param timeout:
     :return:
     """
-    reason = "No suitable address family"
+
+    reason = 'No suitable address family'
     addrinfos = socket.getaddrinfo(hostname, port, socket.AF_UNSPEC, socket.SOCK_STREAM)
     for family, socktype, proto, canonname, sockaddr in addrinfos:
         if socktype == socket.SOCK_STREAM:
             sock = socket.socket(family, socket.SOCK_STREAM)
             if timeout > 0:
                 sock.settimeout(timeout)
-            now = datetime.now()
             try:
-                retry_on_signal(lambda: sock.connect((hostname, port)))
+                # retry_on_signal(lambda: sock.connect((hostname, port))) # @2023-06-09 change, remove paramiko.util.retry_on_signal(Paramiko3.0.0 2023-01-20)
+                sock.connect((hostname, port))
             except socket.error as e:
                 reason = str(e)
-                print(datetime.now() - now)
             else:
                 break
     else:
         raise SSHException(
-            "Unable to connect to {}: {}".format(hostname, reason)
+            'Unable to connect to {}: {}'.format(hostname, reason)
         )
     return sock
 
 
 def _clear_redundant(txt, command):
     """
     Clear the redundant information.
@@ -231,15 +265,15 @@
 
     """
     # remove the start command  ex) ls -l
     if txt.startswith(command):
         txt = txt[len(command):].lstrip()
 
     # remove text before command ex) [root@localhost ~]# ls -l
-    cmd_pattern = re.compile('.*([#$])?( )*' + re.escape(command))
+    cmd_pattern = re.compile('.*([#$])( )*' + re.escape(command))  # @2023-06-07 change ([#$])? --> ([#$])
     last_match = None
     for match in cmd_pattern.finditer(txt):
         last_match = match
     if last_match:
         txt = txt[last_match.end():]
     path_pattern = re.compile('.*[#$] ')
     txt = path_pattern.sub('', txt)  # remove the path info
@@ -252,51 +286,61 @@
     if path[-1] == '/':
         return path[0:-1]
     return path
 
 
 if __name__ == '__main__':
     servers = [
-        {  # Centos
-            'host': '10.124.4.21',
-            'username': 'admin1',
-            'password': 'Cisco@123',
-            'commands': ['show int eth3/1']
-        },
+        # {  # C9300
+        #     'host': '10.75.37.165',
+        #     'username': 'admin',
+        #     'password': 'Cisco123',
+        #     # 'secondary_password': 'Cisco123',
+        #     'recv_endswith': ['# ', '$ ', ': ', '? ', '#'],
+        #     'commands': ['enable', 'Cisco123', 'show run']
+        # },
+        # {  # Centos
+        #     'host': '10.124.4.21',
+        #     'username': 'admin1',
+        #     'password': 'Cisco@123',
+        #     'commands': ['show int eth3/1']
+        # },
         # {  # Centos
         #     'host': '10.124.5.222',
         #     'username': 'root',
         #     'password': 'cisco123',
         #     'commands': ['ls -l', 'cd ../opt', '\cp a.txt b.txt']
         # },
         # {  # Ubuntu
         #     'host': '10.124.5.198',
         #     'username': 'root',
         #     'password': 'Cisco@123',
         #     'commands': ['ls -l']
         # },
-        # {  # Ubuntu, test input password
-        #     'host': '10.124.205.216',
-        #     'username': 'cisco',
-        #     'password': 'cisco123',
-        #     'commands': ['sudo ls -l']
-        # },
+        {  # Ubuntu, test input password
+            'host': '10.124.5.216',
+            'username': 'cisco',
+            'password': 'cisco123',
+            'secondary_password': 'cisco123',
+            'commands': ['sudo ls -l']
+        },
         # {  # NX-OS
         #     'host': '10.124.11.134',
         #     'username': 'admin',
         #     'password': 'Cisco@123',
         #     'commands': ['show version', 'show running-config']
         # },
         # {  # NX-OS
         #     'host': '10.66.94.62',
         #     'username': 'admin',
         #     'password': 'cisco!123',
         #     'commands': ['show version', 'show running-config']
         # }
     ]
     for item in servers:
-        print((item.get('host') + " : " + str(item.get("commands"))).center(100, '*'))
-        with ssh_session(item.get('host'), item.get('username'), item.get('password'), timeout=10) as ssh:
+        print((item.get('host') + ' : ' + str(item.get('commands'))).center(100, '*'))
+        with ssh_session(item.get('host'), item.get('username'), item.get('password'), timeout=10, recv_endswith=item.get('recv_endswith'),
+                         secondary_password=item.get('secondary_password')) as ssh:
             print(ssh.run_command_list(item.get('commands'), True))
 
-    # ssh.sftp_get_dir("/usr/projects/git/srte/src/", "/Users/taozh/Work/Codes/ssh_test/sftp")
+    # ssh.sftp_get_dir('/usr/projects/git/srte/src/', '/Users/taozh/Work/Codes/ssh_test/sftp')
     print('\n', 'end'.center(100, '-'))
```

### Comparing `flaskz-1.5.3/src/flaskz/log/__init__.py` & `flaskz-1.6/src/flaskz/log/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/models/__init__.py` & `flaskz-1.6/src/flaskz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/models/_base.py` & `flaskz-1.6/src/flaskz/models/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -469,33 +469,50 @@
         .. versionupdated:: 1.0
 
         Example:
             User.bulk_delete([1,2,3])   # pk list
             User.bulk_delete([{'id': 1}, {'id': 2}, {'id': 3}]) # dict list
 
         :param items:
-        :return:
+        :return: the deleted count
         """
         if len(items) == 0:
             return
         pk = cls.get_primary_field()
+        count = 0
         with db_session() as session:
             pk_list = []
             for item in items:
                 if is_dict(item):
                     # instance = session.query(cls).filter_by(**item).limit(1).first()
                     # if instance:
                     #     pk_list.append(getattr(instance, pk))
                     for instance in session.query(cls).filter_by(**item):  # @2023-03-27 first to all, ex)delete all items with same name
                         pk_list.append(getattr(instance, pk))
                 else:
                     pk_list.append(item)
             # @2022-11-03: Use 'where' and 'in' to rewrite bulk delete to avoid partial delete scenarios
             if len(pk_list) > 0:
-                session.query(cls).filter(getattr(cls, pk).in_(pk_list)).delete()
+                count = session.query(cls).filter(getattr(cls, pk).in_(pk_list)).delete()
+        return count
+
+    @classmethod
+    def clear_db(cls):
+        """
+        Clear all the data.
+
+        .. versionadded:: 1.6
+
+        Example:
+            SysActionLog.clear_db()
+
+        :return: the deleted count
+        """
+        with db_session() as session:
+            return session.query(cls).delete()
 
     # -------------------------------------------query-------------------------------------------
 
     @classmethod
     def query(cls):
         """
         Return a 'Query' object corresponding to this class.
@@ -657,39 +674,94 @@
             AND (country='America' OR country='Canada')
         ORDER BY templates.name ASC
         LIMIT ? OFFSET ? (20, 0)
 
         :param pss_option:
         :return:
         """
+        return cls._query_pss(pss_option)
+
+    @classmethod
+    def count(cls, search=None):
+        """
+        Return the count of the specified search, if search option is None, return the count of all data.
+
+        .. versionadded:: 1.6
+
+        Example:
+            SysActionLog.count()
+            SysActionLog.count(get_pss(   # use flaskz.utils.get_pss to format condition
+                TemplateModel, {   # FROM templates
+                    "search": {                         # WHERE
+                        "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
+                        "age": {                        # AND (age>1 AND age<20)
+                            ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
+                            "<": 20
+                        },
+                        "email": "taozh@focus-ui.com",  # AND (email='taozh@focus-ui.com')
+                        "_ors": {                       # AND (country='America' OR country='Canada')
+                            "country": "America||Canada"
+                        },
+                        "_ands": {                      # AND (grade>1 AND grade<5)
+                            "grade": {
+                                ">": 1,
+                                "<": 5
+                            }
+                        }
+                    }
+                }))
+        :param search: the search option
+        :return: the count number
+        """
+        return cls._query_pss(search, True)
+
+    @classmethod
+    def _query_pss(cls, pss_option, return_count=False):
+        pss_option = pss_option or {}
         filter_likes = pss_option.get('filter_likes', [])
         filter_ands = pss_option.get('filter_ands', [])
         filter_ors = pss_option.get('filter_ors', [])
+
+        group = pss_option.get('group', [])
+
         offset = max(get_dict_value_by_type(pss_option, 'offset', int, 0), 0)  # @2023-01-09 update, add type check
         limit = max(get_dict_value_by_type(pss_option, 'limit', int, 0), 0)
+        # distinct = pss_option.get('distinct', [])
 
         orders = pss_option.get('order')
         if orders is None:
             orders = []
         elif not is_list(orders):  # asc/desc
             orders = [orders]
 
         if len(orders) == 0:  # @2023-05-04 fix
             orders = [cls.get_query_default_order()]  # default order
         orders = [item for item in orders if item is not None]
 
         with db_session(do_commit=False) as session:
             query = session.query(cls)
+
             if len(filter_likes) > 0:
                 query = query.filter(text('(' + (' OR '.join(filter_likes)) + ')'))
             if len(filter_ands) > 0:
                 query = query.filter(text('(' + (' AND '.join(filter_ands)) + ')'))
             if len(filter_ors) > 0:
                 query = query.filter(text('(' + (' OR '.join(filter_ors)) + ')'))
+
+            # if len(distinct) > 0:
+            #     query.distinct(*distinct)
+
+            if len(group) > 0:  # @2023-06-07 add
+                query = query.group_by(*group)
+
             count = query.count()
+
+            if return_count is True:
+                return count
+
             if count > 0 and offset < count:
                 # for order in orders:
                 #     if order is not None:
                 #         query = query.order_by(order)
                 if len(orders) > 0:
                     query = query.order_by(*orders)
```

### Comparing `flaskz-1.5.3/src/flaskz/models/_model.py` & `flaskz-1.6/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/models/_util.py` & `flaskz-1.6/src/flaskz/models/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/res_status_codes.py` & `flaskz-1.6/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/rest/__init__.py` & `flaskz-1.6/src/flaskz/rest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from flask import request
 from flaskz import res_status_codes
 
 from ..log import flaskz_logger, get_log_data
 from ..models import model_to_dict, query_all_models, ModelMixin
-from ..utils import get_list, is_dict, create_response, get_pss
+from ..utils import get_list, is_dict, create_response, get_pss, get_request_json
 
 
 def init_model_rest_blueprint(model_cls, api_blueprint, url_prefix, module, routers=None, to_json_option=None, multiple_option=None):
     """
     ** Deprecated, please use register_model_route **
 
     Append rest api route to the api blueprint for the specified model class.
@@ -332,15 +332,15 @@
     methods = methods or ['GET', 'POST']
     rule, pss_rule = _get_route_rule(rule, strict_slash, rule_suffix)
 
     @app.route(pss_rule, methods=methods)
     @rest_permission_required(module, action)
     @gen_route_method('query_pss', rule)
     def query_pss():
-        request_json = request.json
+        request_json = get_request_json({})  # @2023-06-15, request.json --> get_request_json({})
         req_log_data = json.dumps(request_json)
 
         success, data = model.query_pss(get_pss(model, request_json))
         if success is True:
             data['data'] = model_to_dict(data.get('data', []), to_json_option)
 
         flaskz_logger.debug(get_rest_log_msg('Query pss {} data'.format(model.get_class_name()), req_log_data, success, data))
```

### Comparing `flaskz-1.5.3/src/flaskz/rest/_mgmt.py` & `flaskz-1.6/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/rest/_util.py` & `flaskz-1.6/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_app.py` & `flaskz-1.6/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_cache.py` & `flaskz-1.6/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_cls.py` & `flaskz-1.6/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_common.py` & `flaskz-1.6/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_func.py` & `flaskz-1.6/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_magic.py` & `flaskz-1.6/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_request_api.py` & `flaskz-1.6/src/flaskz/utils/_request_api.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_request_args.py` & `flaskz-1.6/src/flaskz/utils/_request_args.py`

 * *Files 15% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     :return:
     """
     pss_config = get_dict(pss_config)
     # --------------------search--------------------
     search = pss_config.get('search') or {}
     ands = []
     ors = []
+
+    # select
     search_like = search.pop('like', None)
     like_columns = getattr(cls, 'like_columns', None)
     likes = []
     if search_like and like_columns is not None:
         search_like = str(search_like).strip()
         if search_like != '':
             for col in like_columns:
@@ -117,14 +119,39 @@
     _ors = search.pop('_ors', None)
     if _ors:
         for key in _ors:
             _append_item(ors, key, _ors[key], columns_fields)
 
     for key in search:
         _append_item(ands, key, search[key], columns_fields)
+
+    # distinct = []  # @2023-06-07 add
+    # _distinct = search.pop('_distinct', None)
+    # if _distinct:
+    #     if is_str(_distinct):
+    #         _distinct = [_distinct]
+    #
+    #     if is_list(_distinct):
+    #         for distinct_item in _distinct:
+    #             distinct_column = cls.get_column_by_field(distinct_item)
+    #             if distinct_column is not None:
+    #                 distinct.append(distinct_column)
+
+    # --------------------group--------------------
+    groups = []  # @2023-06-07 add
+    _groups = pss_config.get('group', None)
+    if _groups:
+        if is_str(_groups):
+            _groups = [_groups]
+        if is_list(_groups):
+            for group_item in _groups:
+                group_column = cls.get_column_by_field(group_item)
+                if group_column is not None:
+                    groups.append(group_column)
+
     # --------------------page--------------------
     page = pss_config.get('page') or {}
     offset = page.get('offset') or page.get('skip') or 0
     limit = page.get('limit') or page.get('size') or 100000
 
     # --------------------sort--------------------
     # @2022-04-10 fix exception subs2 = relationship('PerfTestSubModel2', cascade='all,delete-orphan', lazy='joined') ->
@@ -182,27 +209,45 @@
     return {
         'filter_ands': ands,
         'filter_ors': ors,
         'filter_likes': likes,
         'offset': offset,
         'limit': limit,
         'order': orders,
+        'group': groups
+        # 'distinct': distinct
     }
 
 
 def _append_item(items, key, value, columns_fields):  # @2023-02-06 add columns_fields args to fix "Unknown column 'col' in 'where clause'"
+    """
+    Create sql text
+    - if need '' in sql, add in value ex) "'abc'"
+
+    :param items:
+    :param key:
+    :param value:
+    :param columns_fields:
+    :return:
+
+    :param items:
+    :param key:
+    :param value:
+    :param columns_fields:
+    :return:
+    """
     if columns_fields and (key not in columns_fields):
         return items
 
     if value is not None:
         if is_str(value):
             value = value.strip()
             if value != '':
                 val_arr = value.split('||')
                 for op_v in val_arr:
-                    items.append(key + "='" + op_v + "'")
+                    items.append(key + " = '" + op_v + "'")
         elif is_dict(value):
             for operator, op_v in value.items():
-                items.append(key + operator + str(op_v))
+                items.append(key + ' ' + operator + ' ' + str(op_v))  # @2023-06-15 add blank, "in":"('a','b','c')"/ "like":"'%a'"
         else:
-            items.append(key + '=' + str(value))
+            items.append(key + ' = ' + str(value))
     return items
```

### Comparing `flaskz-1.5.3/src/flaskz/utils/_response.py` & `flaskz-1.6/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz/utils/_timer.py` & `flaskz-1.6/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.5.3/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.6/src/flaskz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.5.3
+Version: 1.6
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,37 +24,43 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6** `2023/06/16`
+    - [A] `BaseModelMixin`添加`count`方法，用于数量查询(全量/条件)
+    - [A] `BaseModelMixin`添加`clear_db`方法，用于清空数据
+    - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
+    - [A] `flaskz.ext.ssh`添加对Paramiko>=3.0.0版本的支持
+    - [A] `flaskz.ext.ssh`添加`secondary_password`和`recv_endswith`参数
 - **1.5.3** `2023/06/01`
     - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
     - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
-    - [A] 重构`flaskz.rest`路由生成模块*
+    - [A] 扩展`flaskz.rest`路由生成模块*
         - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
         - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
         - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
         - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
         - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
         - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
         - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
         - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
     - [A] `ModelMixin.query_pss`方法支持多列排序*
     - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
     - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
     - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
     - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
-    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决<2.2.3版本的Flask不会将结尾不带`/`的请求重定向到带`/`路由的问题
+    - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决Flask<2.2.3版本不会将结尾不带`/`的请求重定向到带`/`路由的问题
 - **1.3** `2023/03/01`
     - [A] `init_model_rest_blueprint`函数生成的query路由, 添加对单个数据的查询功能(`[GET]url_prefix/did/`)
     - [A] `init_model_rest_blueprint`函数生成的update路由, 添加URL主键支持(`[PATCH]url_prefix/did/`)
     - [C] `init_model_rest_blueprint`函数生成的delete路由, 结尾添加`/`, 用于支持以`/`结尾的URL删除请求(`[DELETE]url_prefix/did/`)
     - [A] 添加`FLASKZ_DATABASE_ENGINE_KWARGS`参数, 用于自定义engine参数
 - **1.2** `2023/02/01`
     - [A] 添加`FLASKZ_DATABASE_POOL_PRE_PING`参数, 用于设置engine的`pool_pre_ping`参数
```

### Comparing `flaskz-1.5.3/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.6/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

