# Comparing `tmp/karuoflow-1.31.tar.gz` & `tmp/karuoflow-1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karuoflow-1.31.tar", last modified: Thu Jun  1 00:38:56 2023, max compression
+gzip compressed data, was "karuoflow-1.32.tar", last modified: Fri Jun 16 02:38:41 2023, max compression
```

## Comparing `karuoflow-1.31.tar` & `karuoflow-1.32.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.248937 karuoflow-1.31/
--rw-rw-r--   0 work      (1001) work      (1001)     1063 2023-05-12 05:20:22.000000 karuoflow-1.31/LICENSE
--rw-rw-r--   0 work      (1001) work      (1001)      287 2023-06-01 00:38:56.247937 karuoflow-1.31/PKG-INFO
--rw-rw-r--   0 work      (1001) work      (1001)       38 2023-05-12 05:20:22.000000 karuoflow-1.31/README.md
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.246937 karuoflow-1.31/karuoflow/
--rw-rw-r--   0 work      (1001) work      (1001)     2269 2023-06-01 00:29:09.000000 karuoflow-1.31/karuoflow/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)     2558 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/datadef.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.247937 karuoflow-1.31/karuoflow/db/
--rw-rw-r--   0 work      (1001) work      (1001)      151 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/db/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)      764 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/db/session.py
--rw-rw-r--   0 work      (1001) work      (1001)     7251 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/db/tables.py
--rw-rw-r--   0 work      (1001) work      (1001)     2510 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/error_code.py
--rw-rw-r--   0 work      (1001) work      (1001)    30685 2023-06-01 00:26:07.000000 karuoflow-1.31/karuoflow/flowapp.py
--rw-rw-r--   0 work      (1001) work      (1001)    19421 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/flowmodelagent.py
--rw-rw-r--   0 work      (1001) work      (1001)     6854 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/initflow.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.247937 karuoflow-1.31/karuoflow/test/
--rw-rw-r--   0 work      (1001) work      (1001)        0 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/test/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)    11800 2023-05-12 05:49:21.000000 karuoflow-1.31/karuoflow/test/test_initenvironment.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.246937 karuoflow-1.31/karuoflow.egg-info/
--rw-rw-r--   0 work      (1001) work      (1001)      287 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/PKG-INFO
--rw-rw-r--   0 work      (1001) work      (1001)      466 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/SOURCES.txt
--rw-rw-r--   0 work      (1001) work      (1001)        1 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/dependency_links.txt
--rw-rw-r--   0 work      (1001) work      (1001)       26 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/requires.txt
--rw-rw-r--   0 work      (1001) work      (1001)       10 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/top_level.txt
--rw-rw-r--   0 work      (1001) work      (1001)       38 2023-06-01 00:38:56.248937 karuoflow-1.31/setup.cfg
--rw-rw-r--   0 work      (1001) work      (1001)      685 2023-05-12 05:20:22.000000 karuoflow-1.31/setup.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-16 02:38:41.253472 karuoflow-1.32/
+-rw-rw-r--   0 work      (1001) work      (1001)     1063 2023-05-12 05:20:22.000000 karuoflow-1.32/LICENSE
+-rw-rw-r--   0 work      (1001) work      (1001)      287 2023-06-16 02:38:41.253472 karuoflow-1.32/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)       38 2023-05-12 05:20:22.000000 karuoflow-1.32/README.md
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-16 02:38:41.251472 karuoflow-1.32/karuoflow/
+-rw-rw-r--   0 work      (1001) work      (1001)     2339 2023-06-16 02:36:38.000000 karuoflow-1.32/karuoflow/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2558 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/datadef.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-16 02:38:41.252472 karuoflow-1.32/karuoflow/db/
+-rw-rw-r--   0 work      (1001) work      (1001)      151 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/db/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)      764 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/db/session.py
+-rw-rw-r--   0 work      (1001) work      (1001)     7251 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/db/tables.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2510 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/error_code.py
+-rw-rw-r--   0 work      (1001) work      (1001)    31134 2023-06-16 02:19:33.000000 karuoflow-1.32/karuoflow/flowapp.py
+-rw-rw-r--   0 work      (1001) work      (1001)    19421 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/flowmodelagent.py
+-rw-rw-r--   0 work      (1001) work      (1001)     6854 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/initflow.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-16 02:38:41.253472 karuoflow-1.32/karuoflow/test/
+-rw-rw-r--   0 work      (1001) work      (1001)        0 2023-05-12 05:20:22.000000 karuoflow-1.32/karuoflow/test/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)    12030 2023-06-16 02:35:43.000000 karuoflow-1.32/karuoflow/test/test_initenvironment.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-16 02:38:41.252472 karuoflow-1.32/karuoflow.egg-info/
+-rw-rw-r--   0 work      (1001) work      (1001)      287 2023-06-16 02:38:41.000000 karuoflow-1.32/karuoflow.egg-info/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)      466 2023-06-16 02:38:41.000000 karuoflow-1.32/karuoflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 work      (1001) work      (1001)        1 2023-06-16 02:38:41.000000 karuoflow-1.32/karuoflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       26 2023-06-16 02:38:41.000000 karuoflow-1.32/karuoflow.egg-info/requires.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       10 2023-06-16 02:38:41.000000 karuoflow-1.32/karuoflow.egg-info/top_level.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       38 2023-06-16 02:38:41.253472 karuoflow-1.32/setup.cfg
+-rw-rw-r--   0 work      (1001) work      (1001)      685 2023-05-12 05:20:22.000000 karuoflow-1.32/setup.py
```

### Comparing `karuoflow-1.31/LICENSE` & `karuoflow-1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `karuoflow-1.31/karuoflow/__init__.py` & `karuoflow-1.32/karuoflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,10 +29,11 @@
 @version 1.25 [2022-03-10] 增加AppendSign 接口，供批量追加审核节点，（多能上会申请定制化场景需求）
 @version 1.26 [2022-03-14] 修正了查询已审核申请列表数据问题，该问题由关联查询引起，但模糊匹配仍然存在问题
 @version 1.27 [2022-03-14] 修正了1.26版本中join查询的条件bug
 @version 1.28 [2022-11-06] 针对sqlalchemy的缓存问题，对db操作包裹db_session.begin()事务上下文
 @version 1.29 [2022-11-06] 针对sqlalchemy的缓存问题，对db操作包裹db_session.begin()事务上下文，该机制因为在外部系统中传入了session，并在传入前开启了事务，因此会报错，先退回。
 @version 1.30 [2023-05-12] 增加更新ext_data字段的函数
 @version 1.31 [2023-06-01] 修改AddSign函数的签名，增加传入name和node_label两个参数
+@version 1.32 [2023-06-16] 在审批流查询中增加观察员角色
 '''
 
-__version__ = 1.31
+__version__ = 1.32
```

### Comparing `karuoflow-1.31/karuoflow/datadef.py` & `karuoflow-1.32/karuoflow/datadef.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.31/karuoflow/db/session.py` & `karuoflow-1.32/karuoflow/db/session.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.31/karuoflow/db/tables.py` & `karuoflow-1.32/karuoflow/db/tables.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.31/karuoflow/error_code.py` & `karuoflow-1.32/karuoflow/error_code.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.31/karuoflow/flowapp.py` & `karuoflow-1.32/karuoflow/flowapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 '''
 @文件    :flowapp.py
 @说明    :
 @时间    :2020/09/02 14:27:13
 @作者    :caimmy@hotmail.com
 @版本    :0.1
 '''
+from typing import List
 import copy
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 from sqlalchemy.orm.attributes import flag_modified
 from sqlalchemy.exc import SQLAlchemyError
 from datetime import datetime
-from sqlalchemy import and_
+from sqlalchemy import and_, or_
 from .db.session import createDbSession
 from .db.tables import TblFlowRule, TblFlowJob, TblFlowRecords
 from .flowmodelagent import FlowModelsAgent
 from .datadef import DbConfig, OperResult, QueryParams
 from .error_code import KaruoFlowErrors
 from .db.tables import InitKaruoflowTables
 from .initflow import InitializeFlowsFromConfigure
@@ -86,27 +87,32 @@
             TblFlowRule.prev_id==0,
             TblFlowRule.status=='1',
         )).all()
         return [_flow.property2Dict() for _flow in flow_rules] if flow_rules else []
 
     # ======================= querys
 
-    def _QueryApplySets(self, user_id: str, catalog:str = None, subflow:str=None, closed_label: str=None, result=None, page=1, size=30):
+    def _QueryApplySets(self, user_id: str, catalog:str = None, subflow:str=None, closed_label: str=None, result=None, page=1, size=30, supervisor_users: List=[]):
         """
         根据close字段来查询某个ID作为发起人的审核流程
         catalog: 审批类别
         close_label: 关闭字段内容, ['0', '1']
         result: 审核结果, 0审核驳回；1审核通过；
         page: int 当前页
         size: int 分页大小
         """
         # 对分区参数做安全性校验
         if page < 1: page = 1
         if size < 1: size = 30
-        _common_query = self.db_session.query(TblFlowJob).filter(TblFlowJob.apply_user==user_id)
+        if not isinstance(supervisor_users, list):
+            supervisor_users = []
+        if user_id in supervisor_users:
+            _common_query = self.db_session.query(TblFlowJob)
+        else:
+            _common_query = self.db_session.query(TblFlowJob).filter(TblFlowJob.apply_user==user_id)
         if catalog:
             _common_query = _common_query.filter(TblFlowJob.catalog==catalog)
         if subflow:
             _common_query = _common_query.filter(TblFlowJob.subflow==subflow)
         if closed_label and closed_label in ['0', '1']:
             _common_query = _common_query.filter(TblFlowJob.closed==closed_label)
         if result and result in ['0', '1']:
@@ -179,41 +185,41 @@
             "total": _total,
             "page": page,
             "size": size,
             "sets": [_mi.property2Dict() for _mi in match_items] if match_items else []
         }
         
 
-    def QueryApplyListInDoing(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0):
+    def QueryApplyListInDoing(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0, supervisor_users: List = []):
         """
         查询用户发起的正在进行中的审批记录
         """
-        return self._QueryApplySets(user_id, catalog, subflow, '0', None, page, size)
+        return self._QueryApplySets(user_id, catalog, subflow, '0', None, page, size, supervisor_users)
 
-    def QueryApplyListClosed(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0):
+    def QueryApplyListClosed(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0, supervisor_users: List = []):
         """
         查询用户发起的已经结束的审批记录
         """
-        return self._QueryApplySets(user_id, catalog, subflow, '1', None, page, size)
+        return self._QueryApplySets(user_id, catalog, subflow, '1', None, page, size, supervisor_users)
 
-    def QueryApplyListSuccessed(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0):
+    def QueryApplyListSuccessed(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0, supervisor_users: List = []):
         """
         查询用户发起的已经流转完成，并审核批准的申请记录
         :param user_id 申请人编号
         :param catalog 申请类别
         """
-        return self._QueryApplySets(user_id, catalog, subflow, '1', '1', page, size)
+        return self._QueryApplySets(user_id, catalog, subflow, '1', '1', page, size, supervisor_users)
 
-    def QueryApplyListRefused(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0):
+    def QueryApplyListRefused(self, user_id, catalog: str=None, subflow: str=None, page=0, size=0, supervisor_users: List = []):
         """
         查询用户发起的已经流转完成，并审核拒绝的申请记录
         :param user_id 申请人编号
         :param catalog 申请类别
         """
-        return self._QueryApplySets(user_id, catalog, subflow, '1', '0', page, size)
+        return self._QueryApplySets(user_id, catalog, subflow, '1', '0', page, size, supervisor_users)
 
 
     def QueryReviewTodoList(self, user_id, catalog:str=None, subflow:str=None):
         """
         查询用户正在审批的记录
         """
         _common_query = self.db_session.query(TblFlowJob).filter(and_(
```

### Comparing `karuoflow-1.31/karuoflow/flowmodelagent.py` & `karuoflow-1.32/karuoflow/flowmodelagent.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.31/karuoflow/initflow.py` & `karuoflow-1.32/karuoflow/initflow.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.31/karuoflow/test/test_initenvironment.py` & `karuoflow-1.32/karuoflow/test/test_initenvironment.py`

 * *Files 3% similar despite different names*

```diff
@@ -278,9 +278,16 @@
             _ext_data = _item.data["job"]["ext_data"]
             print(_ext_data)
             if isinstance(_ext_data, dict):
                 _ext_data.update({"inuse": 1})
             res = self.flow_app.UpdateJobExtdata(_jobid, _ext_data)
             print(res.toDict)
 
+    def testQueryFlowClosed(self):
+        """
+        测试查询已完成的工单
+        """
+        _item_list = self.flow_app.QueryApplyListSuccessed("long", supervisor_users=["caimmy", "long"])
+        pprint(_item_list)
+
 if "__main__" == __name__:
     unittest.main()
```

### Comparing `karuoflow-1.31/setup.py` & `karuoflow-1.32/setup.py`

 * *Files identical despite different names*

