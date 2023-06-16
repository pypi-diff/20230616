# Comparing `tmp/simple_aws_rds-0.2.1.tar.gz` & `tmp/simple_aws_rds-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_rds-0.2.1.tar", last modified: Thu Jun 15 19:39:49 2023, max compression
+gzip compressed data, was "simple_aws_rds-0.3.1.tar", last modified: Fri Jun 16 01:03:04 2023, max compression
```

## Comparing `simple_aws_rds-0.2.1.tar` & `simple_aws_rds-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.945490 simple_aws_rds-0.2.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:21.000000 simple_aws_rds-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-15 19:39:49.945330 simple_aws_rds-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3833 2023-06-15 18:43:35.000000 simple_aws_rds-0.2.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1048 2023-06-15 18:59:50.000000 simple_aws_rds-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-15 16:48:33.000000 simple_aws_rds-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-15 16:48:10.000000 simple_aws_rds-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-15 19:39:49.945536 simple_aws_rds-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7563 2023-06-15 18:42:44.000000 simple_aws_rds-0.2.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.943403 simple_aws_rds-0.2.1/simple_aws_rds/
--rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.2.1/simple_aws_rds/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 19:01:48.000000 simple_aws_rds-0.2.1/simple_aws_rds/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      122 2023-05-03 16:11:07.000000 simple_aws_rds-0.2.1/simple_aws_rds/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.944151 simple_aws_rds-0.2.1/simple_aws_rds/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/simple_aws_rds/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    22301 2023-06-15 19:01:15.000000 simple_aws_rds-0.2.1/simple_aws_rds/rds.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.944564 simple_aws_rds-0.2.1/simple_aws_rds/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_rds-0.2.1/simple_aws_rds/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_rds-0.2.1/simple_aws_rds/vendor/waiter.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.944031 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      577 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.945010 simple_aws_rds-0.2.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-03 16:11:52.000000 simple_aws_rds-0.2.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3343 2023-06-15 19:00:20.000000 simple_aws_rds-0.2.1/tests/test_rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.896461 simple_aws_rds-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:21.000000 simple_aws_rds-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-16 01:03:04.896308 simple_aws_rds-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3833 2023-06-15 18:43:35.000000 simple_aws_rds-0.3.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1302 2023-06-16 00:51:56.000000 simple_aws_rds-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-15 16:48:33.000000 simple_aws_rds-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-15 16:48:10.000000 simple_aws_rds-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 01:03:04.896506 simple_aws_rds-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7563 2023-06-15 18:42:44.000000 simple_aws_rds-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.894204 simple_aws_rds-0.3.1/simple_aws_rds/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.3.1/simple_aws_rds/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 00:50:28.000000 simple_aws_rds-0.3.1/simple_aws_rds/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      201 2023-06-15 22:04:45.000000 simple_aws_rds-0.3.1/simple_aws_rds/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.894991 simple_aws_rds-0.3.1/simple_aws_rds/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/simple_aws_rds/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_rds-0.3.1/simple_aws_rds/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    27497 2023-06-16 00:55:46.000000 simple_aws_rds-0.3.1/simple_aws_rds/rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.895506 simple_aws_rds-0.3.1/simple_aws_rds/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_rds-0.3.1/simple_aws_rds/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_rds-0.3.1/simple_aws_rds/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.894877 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.895970 simple_aws_rds-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-03 16:11:52.000000 simple_aws_rds-0.3.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3957 2023-06-15 22:06:25.000000 simple_aws_rds-0.3.1/tests/test_rds.py
```

### Comparing `simple_aws_rds-0.2.1/AUTHORS.rst` & `simple_aws_rds-0.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.2.1/LICENSE.txt` & `simple_aws_rds-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.2.1/PKG-INFO` & `simple_aws_rds-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_rds
-Version: 0.2.1
+Version: 0.3.1
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_rds-0.2.1/README.rst` & `simple_aws_rds-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.2.1/release-history.rst` & `simple_aws_rds-0.3.1/release-history.rst`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,23 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2023-06-15)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``RDSDBInstanceStatusGroupEnum``
+- add ``RDSDBInstance.wait_for_available``
+- add ``RDSDBInstance.wait_for_stopped``
+
+
 0.2.1 (2023-06-15)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``RDSDBInstnace.wait_for_status`` method
 
 **Minor Improvements**
```

### Comparing `simple_aws_rds-0.2.1/requirements-doc.txt` & `simple_aws_rds-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.2.1/setup.py` & `simple_aws_rds-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.2.1/simple_aws_rds/rds.py` & `simple_aws_rds-0.3.1/simple_aws_rds/rds.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,37 +9,41 @@
 import dataclasses
 from datetime import datetime
 
 from iterproxy import IterProxy
 from func_args import resolve_kwargs, NOTHING
 
 from .vendor.waiter import Waiter
+from .exc import StatusError
 
 
 class RDSDBInstanceStatusEnum(str, enum.Enum):
     """
     RDS DB instance status enum. The official document doesn't mention the exact
     string. But I found it is all lower case slugified.
 
     Reference:
 
     - https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/accessing-monitoring.html#Overview.DBInstance.Status
     """
+
     available = "available"
     backing_up = "backing-up"
     configuring_enhanced_monitoring = "configuring-enhanced-monitoring"
     configuring_iam_database_auth = "configuring-iam-database-auth"
     configuring_log_exports = "configuring-log-exports"
     converting_to_vpc = "converting-to-vpc"
     creating = "creating"
     delete_precheck = "delete-precheck"
     deleting = "deleting"
     failed = "failed"
     inaccessible_encryption_credentials = "inaccessible-encryption-credentials"
-    inaccessible_encryption_credentials_recoverable = "inaccessible-encryption-credentials-recoverable"
+    inaccessible_encryption_credentials_recoverable = (
+        "inaccessible-encryption-credentials-recoverable"
+    )
     incompatible_network = "incompatible-network"
     incompatible_option_group = "incompatible-option-group"
     incompatible_parameters = "incompatible-parameters"
     incompatible_restore = "incompatible-restore"
     insufficient_capacity = "insufficient-capacity"
     maintenance = "maintenance"
     modifying = "modifying"
@@ -52,14 +56,84 @@
     stopped = "stopped"
     stopping = "stopping"
     storage_full = "storage-full"
     storage_optimization = "storage-optimization"
     upgrading = "upgrading"
 
 
+T_STATUS_ENUM_SET = T.Set[RDSDBInstanceStatusEnum]
+
+
+class RDSDBInstanceStatusGroupEnum:
+    """
+    Group RDS DB instance status enum by semantic.
+
+    :param ended: The status that the instance can be considered as "stopped", "won't change".
+    :param in_transition: The status that the instance can be considered as "changing".
+    :param impossible_to_become_available: as the name
+    :param impossible_to_become_stopped: as the name
+    """
+
+    ended: T_STATUS_ENUM_SET = {
+        RDSDBInstanceStatusEnum.available,
+        RDSDBInstanceStatusEnum.failed,
+        RDSDBInstanceStatusEnum.stopped,
+        RDSDBInstanceStatusEnum.inaccessible_encryption_credentials,
+        RDSDBInstanceStatusEnum.inaccessible_encryption_credentials_recoverable,
+        RDSDBInstanceStatusEnum.incompatible_network,
+        RDSDBInstanceStatusEnum.incompatible_option_group,
+        RDSDBInstanceStatusEnum.incompatible_parameters,
+        RDSDBInstanceStatusEnum.incompatible_restore,
+        RDSDBInstanceStatusEnum.insufficient_capacity,
+        RDSDBInstanceStatusEnum.restore_error,
+    }
+
+    in_transition: T_STATUS_ENUM_SET = {
+        RDSDBInstanceStatusEnum.backing_up,
+        RDSDBInstanceStatusEnum.configuring_enhanced_monitoring,
+        RDSDBInstanceStatusEnum.configuring_iam_database_auth,
+        RDSDBInstanceStatusEnum.configuring_log_exports,
+        RDSDBInstanceStatusEnum.converting_to_vpc,
+        RDSDBInstanceStatusEnum.creating,
+        RDSDBInstanceStatusEnum.deleting,
+        RDSDBInstanceStatusEnum.maintenance,
+        RDSDBInstanceStatusEnum.modifying,
+        RDSDBInstanceStatusEnum.moving_to_vpc,
+        RDSDBInstanceStatusEnum.rebooting,
+        RDSDBInstanceStatusEnum.resetting_master_credentials,
+        RDSDBInstanceStatusEnum.renaming,
+        RDSDBInstanceStatusEnum.starting,
+        RDSDBInstanceStatusEnum.stopping,
+        RDSDBInstanceStatusEnum.storage_optimization,
+        RDSDBInstanceStatusEnum.upgrading,
+    }
+
+    impossible_to_become_available: T_STATUS_ENUM_SET = (
+        {
+            RDSDBInstanceStatusEnum.deleting,
+            RDSDBInstanceStatusEnum.stopping,
+        }
+        .union(ended)
+        .difference(
+            {
+                RDSDBInstanceStatusEnum.available,
+            }
+        )
+    )
+
+    impossible_to_become_stopped: T_STATUS_ENUM_SET = in_transition.union(
+        ended
+    ).difference(
+        {
+            RDSDBInstanceStatusEnum.stopping,
+            RDSDBInstanceStatusEnum.stopped,
+        }
+    )
+
+
 @dataclasses.dataclass
 class RDSDBInstance:
     """
     Represent an RDS DB instance.
 
     See attributes explanation at:
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb/client/describe_db_instances.html
@@ -99,36 +173,48 @@
     copy_tags_to_snapshot: T.Optional[bool] = dataclasses.field(default=None)
     monitoring_interval: T.Optional[int] = dataclasses.field(default=None)
     enhanced_monitoring_resource_arn: T.Optional[str] = dataclasses.field(default=None)
     monitoring_role_arn: T.Optional[str] = dataclasses.field(default=None)
     promotion_tier: T.Optional[int] = dataclasses.field(default=None)
     db_instance_arn: T.Optional[str] = dataclasses.field(default=None)
     timezone: T.Optional[str] = dataclasses.field(default=None)
-    iam_database_authentication_enabled: T.Optional[bool] = dataclasses.field(default=None)
+    iam_database_authentication_enabled: T.Optional[bool] = dataclasses.field(
+        default=None
+    )
     performance_insights_enabled: T.Optional[bool] = dataclasses.field(default=None)
     performance_insights_kms_key_id: T.Optional[str] = dataclasses.field(default=None)
-    performance_insights_retention_period: T.Optional[int] = dataclasses.field(default=None)
+    performance_insights_retention_period: T.Optional[int] = dataclasses.field(
+        default=None
+    )
     deletion_protection: T.Optional[bool] = dataclasses.field(default=None)
     max_allocated_storage: T.Optional[int] = dataclasses.field(default=None)
     customer_owned_ip_enabled: T.Optional[bool] = dataclasses.field(default=None)
     aws_backup_recovery_point_arn: T.Optional[str] = dataclasses.field(default=None)
     activity_stream_status: T.Optional[str] = dataclasses.field(default=None)
     activity_stream_kms_key_id: T.Optional[str] = dataclasses.field(default=None)
-    activity_stream_kinesis_stream_name: T.Optional[str] = dataclasses.field(default=None)
+    activity_stream_kinesis_stream_name: T.Optional[str] = dataclasses.field(
+        default=None
+    )
     activity_stream_mode: T.Optional[str] = dataclasses.field(default=None)
-    activity_stream_engine_native_audit_fields_included: T.Optional[bool] = dataclasses.field(default=None)
+    activity_stream_engine_native_audit_fields_included: T.Optional[
+        bool
+    ] = dataclasses.field(default=None)
     automation_mode: T.Optional[str] = dataclasses.field(default=None)
-    resume_full_automation_mode_time: T.Optional[datetime] = dataclasses.field(default=None)
+    resume_full_automation_mode_time: T.Optional[datetime] = dataclasses.field(
+        default=None
+    )
     custom_iam_instance_profile: T.Optional[str] = dataclasses.field(default=None)
     backup_target: T.Optional[str] = dataclasses.field(default=None)
     network_type: T.Optional[str] = dataclasses.field(default=None)
     activity_stream_policy_status: T.Optional[str] = dataclasses.field(default=None)
     storage_throughput: T.Optional[int] = dataclasses.field(default=None)
     db_system_id: T.Optional[str] = dataclasses.field(default=None)
-    read_replica_source_db_cluster_identifier: T.Optional[str] = dataclasses.field(default=None)
+    read_replica_source_db_cluster_identifier: T.Optional[str] = dataclasses.field(
+        default=None
+    )
     vpc_id: T.Optional[str] = dataclasses.field(default=None)
     subnet_ids: T.List[str] = dataclasses.field(default_factory=list)
     subnet_group_name: T.Optional[str] = dataclasses.field(default=None)
     subnet_group_description: T.Optional[str] = dataclasses.field(default=None)
     subnet_group_arn: T.Optional[str] = dataclasses.field(default=None)
     subnet_group_status: T.Optional[str] = dataclasses.field(default=None)
     security_groups: T.List[T.Dict[str, str]] = dataclasses.field(default_factory=list)
@@ -176,229 +262,252 @@
             copy_tags_to_snapshot=dct.get("CopyTagsToSnapshot"),
             monitoring_interval=dct.get("MonitoringInterval"),
             enhanced_monitoring_resource_arn=dct.get("EnhancedMonitoringResourceArn"),
             monitoring_role_arn=dct.get("MonitoringRoleArn"),
             promotion_tier=dct.get("PromotionTier"),
             db_instance_arn=dct.get("DBInstanceArn"),
             timezone=dct.get("Timezone"),
-            iam_database_authentication_enabled=dct.get("IAMDatabaseAuthenticationEnabled"),
+            iam_database_authentication_enabled=dct.get(
+                "IAMDatabaseAuthenticationEnabled"
+            ),
             performance_insights_enabled=dct.get("PerformanceInsightsEnabled"),
             performance_insights_kms_key_id=dct.get("PerformanceInsightsKMSKeyId"),
-            performance_insights_retention_period=dct.get("PerformanceInsightsRetentionPeriod"),
+            performance_insights_retention_period=dct.get(
+                "PerformanceInsightsRetentionPeriod"
+            ),
             deletion_protection=dct.get("DeletionProtection"),
             max_allocated_storage=dct.get("MaxAllocatedStorage"),
             customer_owned_ip_enabled=dct.get("CustomerOwnedIpEnabled"),
             aws_backup_recovery_point_arn=dct.get("AwsBackupRecoveryPointArn"),
             activity_stream_status=dct.get("ActivityStreamStatus"),
             activity_stream_kms_key_id=dct.get("ActivityStreamKmsKeyId"),
-            activity_stream_kinesis_stream_name=dct.get("ActivityStreamKinesisStreamName"),
+            activity_stream_kinesis_stream_name=dct.get(
+                "ActivityStreamKinesisStreamName"
+            ),
             activity_stream_mode=dct.get("ActivityStreamMode"),
-            activity_stream_engine_native_audit_fields_included=dct.get("ActivityStreamEngineNativeAuditFieldsIncluded"),
+            activity_stream_engine_native_audit_fields_included=dct.get(
+                "ActivityStreamEngineNativeAuditFieldsIncluded"
+            ),
             automation_mode=dct.get("AutomationMode"),
             resume_full_automation_mode_time=dct.get("ResumeFullAutomationModeTime"),
             custom_iam_instance_profile=dct.get("CustomIamInstanceProfile"),
             backup_target=dct.get("BackupTarget"),
             network_type=dct.get("NetworkType"),
             activity_stream_policy_status=dct.get("ActivityStreamPolicyStatus"),
             storage_throughput=dct.get("StorageThroughput"),
             db_system_id=dct.get("DBSystemId"),
-            read_replica_source_db_cluster_identifier=dct.get("ReadReplicaSourceDBClusterIdentifier"),
+            read_replica_source_db_cluster_identifier=dct.get(
+                "ReadReplicaSourceDBClusterIdentifier"
+            ),
             vpc_id=dct.get("DBSubnetGroup", {}).get("VpcId"),
             subnet_ids=[
                 kv["SubnetIdentifier"]
                 for kv in dct.get("DBSubnetGroup", {}).get("Subnets", [])
             ],
             subnet_group_name=dct.get("DBSubnetGroup", {}).get("DBSubnetGroupName"),
-            subnet_group_description=dct.get("DBSubnetGroup", {}).get("DBSubnetGroupDescription"),
+            subnet_group_description=dct.get("DBSubnetGroup", {}).get(
+                "DBSubnetGroupDescription"
+            ),
             subnet_group_arn=dct.get("DBSubnetGroup", {}).get("DBSubnetGroupArn"),
             subnet_group_status=dct.get("DBSubnetGroup", {}).get("SubnetGroupStatus"),
             security_groups=dct.get("DBSecurityGroups", []),
             availability_zone=dct.get("AvailabilityZone"),
             tags={d["Key"]: d["Value"] for d in dct.get("TagList", [])},
             data=dct,
         )
 
     # status checking methods human intuitive status check
     def is_available(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.available.value
 
     def is_backing_up(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.backing_up.value
 
     def is_configuring_enhanced_monitoring(self) -> bool:  # pragma: no cover
-        """
-        """
-        return self.status == RDSDBInstanceStatusEnum.configuring_enhanced_monitoring.value
+        """ """
+        return (
+            self.status == RDSDBInstanceStatusEnum.configuring_enhanced_monitoring.value
+        )
 
     def is_configuring_iam_database_auth(self) -> bool:  # pragma: no cover
-        """
-        """
-        return self.status == RDSDBInstanceStatusEnum.configuring_iam_database_auth.value
+        """ """
+        return (
+            self.status == RDSDBInstanceStatusEnum.configuring_iam_database_auth.value
+        )
 
     def is_configuring_log_exports(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.configuring_log_exports.value
 
     def is_converting_to_vpc(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.converting_to_vpc.value
 
     def is_creating(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.creating.value
 
     def is_delete_precheck(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.delete_precheck.value
 
     def is_deleting(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.deleting.value
 
     def is_failed(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.failed.value
 
     def is_inaccessible_encryption_credentials(self) -> bool:  # pragma: no cover
-        """
-        """
-        return self.status == RDSDBInstanceStatusEnum.inaccessible_encryption_credentials.value
+        """ """
+        return (
+            self.status
+            == RDSDBInstanceStatusEnum.inaccessible_encryption_credentials.value
+        )
 
-    def is_inaccessible_encryption_credentials_recoverable(self) -> bool:  # pragma: no cover
-        """
-        """
-        return self.status == RDSDBInstanceStatusEnum.inaccessible_encryption_credentials_recoverable.value
+    def is_inaccessible_encryption_credentials_recoverable(
+        self,
+    ) -> bool:  # pragma: no cover
+        """ """
+        return (
+            self.status
+            == RDSDBInstanceStatusEnum.inaccessible_encryption_credentials_recoverable.value
+        )
 
     def is_incompatible_network(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.incompatible_network.value
 
     def is_incompatible_option_group(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.incompatible_option_group.value
 
     def is_incompatible_parameters(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.incompatible_parameters.value
 
     def is_incompatible_restore(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.incompatible_restore.value
 
     def is_insufficient_capacity(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.insufficient_capacity.value
 
     def is_maintenance(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.maintenance.value
 
     def is_modifying(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.modifying.value
 
     def is_moving_to_vpc(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.moving_to_vpc.value
 
     def is_rebooting(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.rebooting.value
 
     def is_resetting_master_credentials(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.resetting_master_credentials.value
 
     def is_renaming(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.renaming.value
 
     def is_restore_error(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.restore_error.value
 
     def is_starting(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.starting.value
 
     def is_stopped(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.stopped.value
 
     def is_stopping(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.stopping.value
 
     def is_storage_full(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.storage_full.value
 
     def is_storage_optimization(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.storage_optimization.value
 
     def is_upgrading(self) -> bool:  # pragma: no cover
-        """
-        """
+        """ """
         return self.status == RDSDBInstanceStatusEnum.upgrading.value
 
     # more human intuitive status check
     def is_ready_to_start(self) -> bool:
         """ """
         return self.is_stopped()
 
     def is_ready_to_stop(self) -> bool:
         """ """
         return self.is_available()
 
+    def is_end(self) -> bool:
+        """ """
+        return self.status in {
+            status.value for status in RDSDBInstanceStatusGroupEnum.ended
+        }
+
+    def is_in_transition(self) -> bool:
+        """ """
+        return self.status in {
+            status.value for status in RDSDBInstanceStatusGroupEnum.in_transition
+        }
+
     def start_db_instance(self, rds_client) -> dict:
         """ """
         return rds_client.start_db_instance(DBInstanceIdentifier=self.id)
 
     def stop_db_instance(self, rds_client) -> dict:
         """ """
         return rds_client.stop_db_instance(DBInstanceIdentifier=self.id)
 
     def wait_for_status(
         self,
         rds_client,
         stop_status: T.Union[RDSDBInstanceStatusEnum, T.List[RDSDBInstanceStatusEnum]],
         delays: T.Union[int, float] = 10,
         timeout: T.Union[int, float] = 300,
-        error_status: T.Optional[T.Union[RDSDBInstanceStatusEnum, T.List[RDSDBInstanceStatusEnum]]] = None,
+        error_status: T.Optional[
+            T.Union[RDSDBInstanceStatusEnum, T.List[RDSDBInstanceStatusEnum]]
+        ] = None,
         indent: int = 0,
         verbose: bool = True,
-    ) -> "RDSDBInstance": # pragma: no cover
+    ) -> "RDSDBInstance":  # pragma: no cover
+        """
+        wait until the DB instance reaches the specified status defined in
+        ``stop_status``. If reaches any of ``error_status ``, raise error.
+
+        :param rds_client:
+        :param stop_status: status to stop waiting
+        :param delays: delay between each check
+        :param timeout: timeout in seconds
+        :param error_status: status to raise error
+        :param indent: indent level for logging
+        :param verbose: whether to print log
+
+        :return: the :class:`RDSDBInstance` representing the latest status
+            of DB instance.
+        """
         if isinstance(stop_status, RDSDBInstanceStatusEnum):
             stop_status_set = {stop_status.value}
         else:
             stop_status_set = {status.value for status in RDSDBInstanceStatusEnum}
         if error_status is None:
             error_status_set = set()
         elif isinstance(error_status, RDSDBInstanceStatusEnum):
@@ -412,18 +521,66 @@
             indent=indent,
             verbose=verbose,
         ):
             db_inst = self.from_id(rds_client, self.id)
             if db_inst.status in stop_status_set:
                 return db_inst
             elif db_inst.status in error_status_set:
-                raise ValueError(f"stop because status reaches {db_inst.status!r}")
+                raise StatusError(f"stop because status reaches {db_inst.status!r}")
             else:
                 pass
 
+    def wait_for_available(
+        self,
+        rds_client,
+        delays: T.Union[int, float] = 10,
+        timeout: T.Union[int, float] = 300,
+        indent: int = 0,
+        verbose: bool = True,
+    ) -> "RDSDBInstance":  # pragma: no cover
+        """
+        Similar to :meth:`RDSDBInstance.wait_for_status`, but wait for
+        DB instance to reach "available" status.
+        """
+        return self.wait_for_status(
+            rds_client=rds_client,
+            stop_status=RDSDBInstanceStatusEnum.available,
+            delays=delays,
+            timeout=timeout,
+            error_status=list(
+                RDSDBInstanceStatusGroupEnum.impossible_to_become_available
+            ),
+            indent=indent,
+            verbose=verbose,
+        )
+
+    def wait_for_stopped(
+        self,
+        rds_client,
+        delays: T.Union[int, float] = 10,
+        timeout: T.Union[int, float] = 300,
+        indent: int = 0,
+        verbose: bool = True,
+    ) -> "RDSDBInstance":  # pragma: no cover
+        """
+        Similar to :meth:`RDSDBInstance.wait_for_status`, but wait for
+        DB instance to reach "stopped" status.
+        """
+        return self.wait_for_status(
+            rds_client=rds_client,
+            stop_status=RDSDBInstanceStatusEnum.stopped,
+            delays=delays,
+            timeout=timeout,
+            error_status=list(
+                RDSDBInstanceStatusGroupEnum.impossible_to_become_stopped
+            ),
+            indent=indent,
+            verbose=verbose,
+        )
+
     # --------------------------------------------------------------------------
     # more constructor methods
     # --------------------------------------------------------------------------
     @classmethod
     def _yield_dict_from_describe_db_instances_response(
         cls,
         res: dict,
@@ -442,14 +599,15 @@
     ) -> "RDSDBInstanceIterProxy":
         """
         A wrapper around ``rds_client.describe_db_instances``.
 
         Multiple filters join with logic "AND", multiple values in a filter
         join with logic "OR".
         """
+
         def run():
             paginator = rds_client.get_paginator("describe_db_instances")
             kwargs = resolve_kwargs(
                 DBInstanceIdentifier=db_instance_identifier,
                 Filters=filters,
                 PaginationConfig={
                     "MaxItems": 9999,
@@ -489,14 +647,15 @@
         Query RDS DB Instance by tag key and value. This function only support
         single key, value pair filtering, if you want more advanced filtering,
         you can use the ``query`` method and do in-memory filtering.
 
         :param key: tag key
         :param value: tag value
         """
+
         def run():
             for db_inst in cls.query(rds_client):
                 if db_inst.tags.get(key, "THIS_IS_IMPOSSIBLE_TO_MATCH") == value:
                     yield db_inst
 
         return RDSDBInstanceIterProxy(run())
```

### Comparing `simple_aws_rds-0.2.1/simple_aws_rds/vendor/waiter.py` & `simple_aws_rds-0.3.1/simple_aws_rds/vendor/waiter.py`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.2.1/simple_aws_rds.egg-info/PKG-INFO` & `simple_aws_rds-0.3.1/simple_aws_rds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-rds
-Version: 0.2.1
+Version: 0.3.1
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_rds-0.2.1/simple_aws_rds.egg-info/SOURCES.txt` & `simple_aws_rds-0.3.1/simple_aws_rds.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 simple_aws_rds/__init__.py
 simple_aws_rds/_version.py
 simple_aws_rds/api.py
+simple_aws_rds/exc.py
 simple_aws_rds/rds.py
 simple_aws_rds.egg-info/PKG-INFO
 simple_aws_rds.egg-info/SOURCES.txt
 simple_aws_rds.egg-info/dependency_links.txt
 simple_aws_rds.egg-info/requires.txt
 simple_aws_rds.egg-info/top_level.txt
 simple_aws_rds/docs/__init__.py
```

### Comparing `simple_aws_rds-0.2.1/tests/test_rds.py` & `simple_aws_rds-0.3.1/tests/test_rds.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 # -*- coding: utf-8 -*-
 
 import os
 import pytest
 import moto
 from boto_session_manager import BotoSesManager
 
-from simple_aws_rds.rds import RDSDBInstanceStatusEnum, RDSDBInstance
+from simple_aws_rds.rds import (
+    RDSDBInstanceStatusEnum,
+    RDSDBInstanceStatusGroupEnum,
+    RDSDBInstance,
+    StatusError,
+)
+
+
+class TestRDSDBInstanceStatusGroupEnum:
+    def test(self):
+        _ = RDSDBInstanceStatusGroupEnum.impossible_to_become_available
+        _ = RDSDBInstanceStatusGroupEnum.impossible_to_become_stopped
 
 
 class TestRds:
     mock_rds = None
     bsm: BotoSesManager = None
 
     @classmethod
@@ -79,22 +90,32 @@
             self.bsm.rds_client, key="Env", value="sandbox"
         ).all()
         assert len(db_inst_list) == 0
 
     def _test_wait_for_status(self):
         db_inst = RDSDBInstance.from_id(self.bsm.rds_client, self.inst_id_1)
         assert db_inst.is_available() is True
+        with pytest.raises(StatusError):
+            db_inst.wait_for_stopped(
+                rds_client=self.bsm.rds_client,
+                verbose=False,
+            )
 
         db_inst.stop_db_instance(self.bsm.rds_client)
         new_db_inst = db_inst.wait_for_status(
             rds_client=self.bsm.rds_client,
             stop_status=RDSDBInstanceStatusEnum.stopped,
             verbose=False,
         )
         assert new_db_inst.is_stopped() is True
+        with pytest.raises(StatusError):
+            db_inst.wait_for_available(
+                rds_client=self.bsm.rds_client,
+                verbose=False,
+            )
 
     def test(self):
         self._test()
         self._test_wait_for_status()
 
 
 if __name__ == "__main__":
```

