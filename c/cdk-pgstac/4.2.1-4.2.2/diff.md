# Comparing `tmp/cdk-pgstac-4.2.1.tar.gz` & `tmp/cdk-pgstac-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pgstac-4.2.1.tar", last modified: Mon Jun 12 15:40:22 2023, max compression
+gzip compressed data, was "cdk-pgstac-4.2.2.tar", last modified: Fri Jun 16 06:25:00 2023, max compression
```

## Comparing `cdk-pgstac-4.2.1.tar` & `cdk-pgstac-4.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:40:22.708158 cdk-pgstac-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 15:40:22.708158 cdk-pgstac-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:40:22.708158 cdk-pgstac-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:40:22.704158 cdk-pgstac-4.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:40:22.708158 cdk-pgstac-4.2.1/src/cdk_pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)   133159 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/src/cdk_pgstac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:40:22.708158 cdk-pgstac-4.2.1/src/cdk_pgstac/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/src/cdk_pgstac/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   165577 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/src/cdk_pgstac/_jsii/cdk-pgstac@4.2.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:40:12.000000 cdk-pgstac-4.2.1/src/cdk_pgstac/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:40:22.708158 cdk-pgstac-4.2.1/src/cdk_pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 15:40:22.000000 cdk-pgstac-4.2.1/src/cdk_pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-12 15:40:22.000000 cdk-pgstac-4.2.1/src/cdk_pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:40:22.000000 cdk-pgstac-4.2.1/src/cdk_pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 15:40:22.000000 cdk-pgstac-4.2.1/src/cdk_pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 15:40:22.000000 cdk-pgstac-4.2.1/src/cdk_pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/cdk_pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)   136966 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/cdk_pgstac/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172634 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/_jsii/cdk-pgstac@4.2.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:24:49.000000 cdk-pgstac-4.2.2/src/cdk_pgstac/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:25:00.516019 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 06:25:00.000000 cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/top_level.txt
```

### Comparing `cdk-pgstac-4.2.1/LICENSE` & `cdk-pgstac-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.2.1/PKG-INFO` & `cdk-pgstac-4.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.2.1
+Version: 4.2.2
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-pgstac-4.2.1/README.md` & `cdk-pgstac-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.2.1/setup.py` & `cdk-pgstac-4.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pgstac",
-    "version": "4.2.1",
+    "version": "4.2.2",
     "description": "A set of constructs deploying pgSTAC with CDK",
     "license": "ISC",
     "url": "https://github.com/developmentseed/cdk-pgstac.git",
     "long_description_content_type": "text/markdown",
     "author": "Anthony Lukach<anthony@developmentseed.org>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cdk_pgstac",
         "cdk_pgstac._jsii"
     ],
     "package_data": {
         "cdk_pgstac._jsii": [
-            "cdk-pgstac@4.2.1.jsii.tgz"
+            "cdk-pgstac@4.2.2.jsii.tgz"
         ],
         "cdk_pgstac": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.46.0, <3.0.0",
+        "aws-cdk-lib>=2.75.0, <3.0.0",
         "aws-cdk.aws-apigatewayv2-integrations-alpha>=2.47.0.a0, <3.0.0",
         "aws-cdk.aws-lambda-python-alpha>=2.47.0.a0, <3.0.0",
         "constructs>=10.1.113, <11.0.0",
         "jsii>=1.69.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
```

### Comparing `cdk-pgstac-4.2.1/src/cdk_pgstac/__init__.py` & `cdk-pgstac-4.2.2/src/cdk_pgstac/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1044,14 +1044,15 @@
         iam_authentication: typing.Optional[builtins.bool] = None,
         instance_identifier: typing.Optional[builtins.str] = None,
         iops: typing.Optional[jsii.Number] = None,
         max_allocated_storage: typing.Optional[jsii.Number] = None,
         monitoring_interval: typing.Optional[aws_cdk.Duration] = None,
         monitoring_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         multi_az: typing.Optional[builtins.bool] = None,
+        network_type: typing.Optional[aws_cdk.aws_rds.NetworkType] = None,
         option_group: typing.Optional[aws_cdk.aws_rds.IOptionGroup] = None,
         parameter_group: typing.Optional[aws_cdk.aws_rds.IParameterGroup] = None,
         performance_insight_encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         performance_insight_retention: typing.Optional[aws_cdk.aws_rds.PerformanceInsightRetention] = None,
         port: typing.Optional[jsii.Number] = None,
         preferred_backup_window: typing.Optional[builtins.str] = None,
         preferred_maintenance_window: typing.Optional[builtins.str] = None,
@@ -1059,14 +1060,15 @@
         publicly_accessible: typing.Optional[builtins.bool] = None,
         removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
         s3_export_buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
         s3_export_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         s3_import_buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
         s3_import_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        storage_throughput: typing.Optional[jsii.Number] = None,
         storage_type: typing.Optional[aws_cdk.aws_rds.StorageType] = None,
         subnet_group: typing.Optional[aws_cdk.aws_rds.ISubnetGroup] = None,
         vpc_subnets: typing.Optional[typing.Union[aws_cdk.aws_ec2.SubnetSelection, typing.Dict[str, typing.Any]]] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
@@ -1093,38 +1095,40 @@
         :param cloudwatch_logs_exports: The list of log types that need to be enabled for exporting to CloudWatch Logs. Default: - no log exports
         :param cloudwatch_logs_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``Infinity``. Default: - logs never expire
         :param cloudwatch_logs_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - a new role is created.
         :param copy_tags_to_snapshot: Indicates whether to copy all of the user-defined tags from the DB instance to snapshots of the DB instance. Default: true
         :param delete_automated_backups: Indicates whether automated backups should be deleted or retained when you delete a DB instance. Default: false
         :param deletion_protection: Indicates whether the DB instance should have deletion protection enabled. Default: - true if ``removalPolicy`` is RETAIN, false otherwise
         :param domain: The Active Directory directory ID to create the DB instance in. Default: - Do not join domain
-        :param domain_role: The IAM role to be used when making API calls to the Directory Service. The role needs the AWS-managed policy AmazonRDSDirectoryServiceAccess or equivalent. Default: - The role will be created for you if {@link DatabaseInstanceNewProps#domain} is specified
+        :param domain_role: The IAM role to be used when making API calls to the Directory Service. The role needs the AWS-managed policy AmazonRDSDirectoryServiceAccess or equivalent. Default: - The role will be created for you if ``DatabaseInstanceNewProps#domain`` is specified
         :param enable_performance_insights: Whether to enable Performance Insights for the DB instance. Default: - false, unless ``performanceInsightRentention`` or ``performanceInsightEncryptionKey`` is set.
         :param iam_authentication: Whether to enable mapping of AWS Identity and Access Management (IAM) accounts to database accounts. Default: false
         :param instance_identifier: A name for the DB instance. If you specify a name, AWS CloudFormation converts it to lowercase. Default: - a CloudFormation generated name
-        :param iops: The number of I/O operations per second (IOPS) that the database provisions. The value must be equal to or greater than 1000. Default: - no provisioned iops
+        :param iops: The number of I/O operations per second (IOPS) that the database provisions. The value must be equal to or greater than 1000. Default: - no provisioned iops if storage type is not specified. For GP3: 3,000 IOPS if allocated storage is less than 400 GiB for MariaDB, MySQL, and PostgreSQL, less than 200 GiB for Oracle and less than 20 GiB for SQL Server. 12,000 IOPS otherwise (except for SQL Server where the default is always 3,000 IOPS).
         :param max_allocated_storage: Upper limit to which RDS can scale the storage in GiB(Gibibyte). Default: - No autoscaling of RDS instance
         :param monitoring_interval: The interval, in seconds, between points when Amazon RDS collects enhanced monitoring metrics for the DB instance. Default: - no enhanced monitoring
         :param monitoring_role: Role that will be used to manage DB instance monitoring. Default: - A role is automatically created for you
         :param multi_az: Specifies if the database instance is a multiple Availability Zone deployment. Default: false
+        :param network_type: The network type of the DB instance. Default: - IPV4
         :param option_group: The option group to associate with the instance. Default: - no option group
         :param parameter_group: The DB parameter group to associate with the instance. Default: - no parameter group
         :param performance_insight_encryption_key: The AWS KMS key for encryption of Performance Insights data. Default: - default master key
-        :param performance_insight_retention: The amount of time, in days, to retain Performance Insights data. Default: 7
+        :param performance_insight_retention: The amount of time, in days, to retain Performance Insights data. Default: 7 this is the free tier
         :param port: The port for the instance. Default: - the default port for the chosen engine.
         :param preferred_backup_window: The daily time range during which automated backups are performed. Constraints: - Must be in the format ``hh24:mi-hh24:mi``. - Must be in Universal Coordinated Time (UTC). - Must not conflict with the preferred maintenance window. - Must be at least 30 minutes. Default: - a 30-minute window selected at random from an 8-hour block of time for each AWS Region. To see the time blocks available, see https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_WorkingWithAutomatedBackups.html#USER_WorkingWithAutomatedBackups.BackupWindow
         :param preferred_maintenance_window: The weekly time range (in UTC) during which system maintenance can occur. Format: ``ddd:hh24:mi-ddd:hh24:mi`` Constraint: Minimum 30-minute window Default: - a 30-minute window selected at random from an 8-hour block of time for each AWS Region, occurring on a random day of the week. To see the time blocks available, see https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_UpgradeDBInstance.Maintenance.html#Concepts.DBMaintenance
         :param processor_features: The number of CPU cores and the number of threads per core. Default: - the default number of CPU cores and threads per core for the chosen instance class. See https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.DBInstanceClass.html#USER_ConfigureProcessor
         :param publicly_accessible: Indicates whether the DB instance is an internet-facing instance. Default: - ``true`` if ``vpcSubnets`` is ``subnetType: SubnetType.PUBLIC``, ``false`` otherwise
         :param removal_policy: The CloudFormation policy to apply when the instance is removed from the stack or replaced during an update. Default: - RemovalPolicy.SNAPSHOT (remove the resource, but retain a snapshot of the data)
         :param s3_export_buckets: S3 buckets that you want to load data into. This property must not be used if ``s3ExportRole`` is used. For Microsoft SQL Server: Default: - None
         :param s3_export_role: Role that will be associated with this DB instance to enable S3 export. This property must not be used if ``s3ExportBuckets`` is used. For Microsoft SQL Server: Default: - New role is created if ``s3ExportBuckets`` is set, no role is defined otherwise
         :param s3_import_buckets: S3 buckets that you want to load data from. This feature is only supported by the Microsoft SQL Server, Oracle, and PostgreSQL engines. This property must not be used if ``s3ImportRole`` is used. For Microsoft SQL Server: Default: - None
         :param s3_import_role: Role that will be associated with this DB instance to enable S3 import. This feature is only supported by the Microsoft SQL Server, Oracle, and PostgreSQL engines. This property must not be used if ``s3ImportBuckets`` is used. For Microsoft SQL Server: Default: - New role is created if ``s3ImportBuckets`` is set, no role is defined otherwise
         :param security_groups: The security groups to assign to the DB instance. Default: - a new security group is created
+        :param storage_throughput: The storage throughput, specified in mebibytes per second (MiBps). Only applicable for GP3. Default: - 125 MiBps if allocated storage is less than 400 GiB for MariaDB, MySQL, and PostgreSQL, less than 200 GiB for Oracle and less than 20 GiB for SQL Server. 500 MiBps otherwise (except for SQL Server where the default is always 125 MiBps).
         :param storage_type: The storage type. Storage types supported are gp2, io1, standard. Default: GP2
         :param subnet_group: Existing subnet group for the instance. Default: - a new subnet group will be created.
         :param vpc_subnets: The type of subnets to add to the created DB subnet group. Default: - private subnets
 
         :stability: experimental
         '''
         if __debug__:
@@ -1164,14 +1168,15 @@
             iam_authentication=iam_authentication,
             instance_identifier=instance_identifier,
             iops=iops,
             max_allocated_storage=max_allocated_storage,
             monitoring_interval=monitoring_interval,
             monitoring_role=monitoring_role,
             multi_az=multi_az,
+            network_type=network_type,
             option_group=option_group,
             parameter_group=parameter_group,
             performance_insight_encryption_key=performance_insight_encryption_key,
             performance_insight_retention=performance_insight_retention,
             port=port,
             preferred_backup_window=preferred_backup_window,
             preferred_maintenance_window=preferred_maintenance_window,
@@ -1179,14 +1184,15 @@
             publicly_accessible=publicly_accessible,
             removal_policy=removal_policy,
             s3_export_buckets=s3_export_buckets,
             s3_export_role=s3_export_role,
             s3_import_buckets=s3_import_buckets,
             s3_import_role=s3_import_role,
             security_groups=security_groups,
+            storage_throughput=storage_throughput,
             storage_type=storage_type,
             subnet_group=subnet_group,
             vpc_subnets=vpc_subnets,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
@@ -1259,14 +1265,15 @@
         "iam_authentication": "iamAuthentication",
         "instance_identifier": "instanceIdentifier",
         "iops": "iops",
         "max_allocated_storage": "maxAllocatedStorage",
         "monitoring_interval": "monitoringInterval",
         "monitoring_role": "monitoringRole",
         "multi_az": "multiAz",
+        "network_type": "networkType",
         "option_group": "optionGroup",
         "parameter_group": "parameterGroup",
         "performance_insight_encryption_key": "performanceInsightEncryptionKey",
         "performance_insight_retention": "performanceInsightRetention",
         "port": "port",
         "preferred_backup_window": "preferredBackupWindow",
         "preferred_maintenance_window": "preferredMaintenanceWindow",
@@ -1274,14 +1281,15 @@
         "publicly_accessible": "publiclyAccessible",
         "removal_policy": "removalPolicy",
         "s3_export_buckets": "s3ExportBuckets",
         "s3_export_role": "s3ExportRole",
         "s3_import_buckets": "s3ImportBuckets",
         "s3_import_role": "s3ImportRole",
         "security_groups": "securityGroups",
+        "storage_throughput": "storageThroughput",
         "storage_type": "storageType",
         "subnet_group": "subnetGroup",
         "vpc_subnets": "vpcSubnets",
         "engine": "engine",
         "allocated_storage": "allocatedStorage",
         "allow_major_version_upgrade": "allowMajorVersionUpgrade",
         "database_name": "databaseName",
@@ -1319,14 +1327,15 @@
         iam_authentication: typing.Optional[builtins.bool] = None,
         instance_identifier: typing.Optional[builtins.str] = None,
         iops: typing.Optional[jsii.Number] = None,
         max_allocated_storage: typing.Optional[jsii.Number] = None,
         monitoring_interval: typing.Optional[aws_cdk.Duration] = None,
         monitoring_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         multi_az: typing.Optional[builtins.bool] = None,
+        network_type: typing.Optional[aws_cdk.aws_rds.NetworkType] = None,
         option_group: typing.Optional[aws_cdk.aws_rds.IOptionGroup] = None,
         parameter_group: typing.Optional[aws_cdk.aws_rds.IParameterGroup] = None,
         performance_insight_encryption_key: typing.Optional[aws_cdk.aws_kms.IKey] = None,
         performance_insight_retention: typing.Optional[aws_cdk.aws_rds.PerformanceInsightRetention] = None,
         port: typing.Optional[jsii.Number] = None,
         preferred_backup_window: typing.Optional[builtins.str] = None,
         preferred_maintenance_window: typing.Optional[builtins.str] = None,
@@ -1334,14 +1343,15 @@
         publicly_accessible: typing.Optional[builtins.bool] = None,
         removal_policy: typing.Optional[aws_cdk.RemovalPolicy] = None,
         s3_export_buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
         s3_export_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         s3_import_buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
         s3_import_role: typing.Optional[aws_cdk.aws_iam.IRole] = None,
         security_groups: typing.Optional[typing.Sequence[aws_cdk.aws_ec2.ISecurityGroup]] = None,
+        storage_throughput: typing.Optional[jsii.Number] = None,
         storage_type: typing.Optional[aws_cdk.aws_rds.StorageType] = None,
         subnet_group: typing.Optional[aws_cdk.aws_rds.ISubnetGroup] = None,
         vpc_subnets: typing.Optional[typing.Union[aws_cdk.aws_ec2.SubnetSelection, typing.Dict[str, typing.Any]]] = None,
         engine: aws_cdk.aws_rds.IInstanceEngine,
         allocated_storage: typing.Optional[jsii.Number] = None,
         allow_major_version_upgrade: typing.Optional[builtins.bool] = None,
         database_name: typing.Optional[builtins.str] = None,
@@ -1366,38 +1376,40 @@
         :param cloudwatch_logs_exports: The list of log types that need to be enabled for exporting to CloudWatch Logs. Default: - no log exports
         :param cloudwatch_logs_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``Infinity``. Default: - logs never expire
         :param cloudwatch_logs_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - a new role is created.
         :param copy_tags_to_snapshot: Indicates whether to copy all of the user-defined tags from the DB instance to snapshots of the DB instance. Default: true
         :param delete_automated_backups: Indicates whether automated backups should be deleted or retained when you delete a DB instance. Default: false
         :param deletion_protection: Indicates whether the DB instance should have deletion protection enabled. Default: - true if ``removalPolicy`` is RETAIN, false otherwise
         :param domain: The Active Directory directory ID to create the DB instance in. Default: - Do not join domain
-        :param domain_role: The IAM role to be used when making API calls to the Directory Service. The role needs the AWS-managed policy AmazonRDSDirectoryServiceAccess or equivalent. Default: - The role will be created for you if {@link DatabaseInstanceNewProps#domain} is specified
+        :param domain_role: The IAM role to be used when making API calls to the Directory Service. The role needs the AWS-managed policy AmazonRDSDirectoryServiceAccess or equivalent. Default: - The role will be created for you if ``DatabaseInstanceNewProps#domain`` is specified
         :param enable_performance_insights: Whether to enable Performance Insights for the DB instance. Default: - false, unless ``performanceInsightRentention`` or ``performanceInsightEncryptionKey`` is set.
         :param iam_authentication: Whether to enable mapping of AWS Identity and Access Management (IAM) accounts to database accounts. Default: false
         :param instance_identifier: A name for the DB instance. If you specify a name, AWS CloudFormation converts it to lowercase. Default: - a CloudFormation generated name
-        :param iops: The number of I/O operations per second (IOPS) that the database provisions. The value must be equal to or greater than 1000. Default: - no provisioned iops
+        :param iops: The number of I/O operations per second (IOPS) that the database provisions. The value must be equal to or greater than 1000. Default: - no provisioned iops if storage type is not specified. For GP3: 3,000 IOPS if allocated storage is less than 400 GiB for MariaDB, MySQL, and PostgreSQL, less than 200 GiB for Oracle and less than 20 GiB for SQL Server. 12,000 IOPS otherwise (except for SQL Server where the default is always 3,000 IOPS).
         :param max_allocated_storage: Upper limit to which RDS can scale the storage in GiB(Gibibyte). Default: - No autoscaling of RDS instance
         :param monitoring_interval: The interval, in seconds, between points when Amazon RDS collects enhanced monitoring metrics for the DB instance. Default: - no enhanced monitoring
         :param monitoring_role: Role that will be used to manage DB instance monitoring. Default: - A role is automatically created for you
         :param multi_az: Specifies if the database instance is a multiple Availability Zone deployment. Default: false
+        :param network_type: The network type of the DB instance. Default: - IPV4
         :param option_group: The option group to associate with the instance. Default: - no option group
         :param parameter_group: The DB parameter group to associate with the instance. Default: - no parameter group
         :param performance_insight_encryption_key: The AWS KMS key for encryption of Performance Insights data. Default: - default master key
-        :param performance_insight_retention: The amount of time, in days, to retain Performance Insights data. Default: 7
+        :param performance_insight_retention: The amount of time, in days, to retain Performance Insights data. Default: 7 this is the free tier
         :param port: The port for the instance. Default: - the default port for the chosen engine.
         :param preferred_backup_window: The daily time range during which automated backups are performed. Constraints: - Must be in the format ``hh24:mi-hh24:mi``. - Must be in Universal Coordinated Time (UTC). - Must not conflict with the preferred maintenance window. - Must be at least 30 minutes. Default: - a 30-minute window selected at random from an 8-hour block of time for each AWS Region. To see the time blocks available, see https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_WorkingWithAutomatedBackups.html#USER_WorkingWithAutomatedBackups.BackupWindow
         :param preferred_maintenance_window: The weekly time range (in UTC) during which system maintenance can occur. Format: ``ddd:hh24:mi-ddd:hh24:mi`` Constraint: Minimum 30-minute window Default: - a 30-minute window selected at random from an 8-hour block of time for each AWS Region, occurring on a random day of the week. To see the time blocks available, see https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_UpgradeDBInstance.Maintenance.html#Concepts.DBMaintenance
         :param processor_features: The number of CPU cores and the number of threads per core. Default: - the default number of CPU cores and threads per core for the chosen instance class. See https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.DBInstanceClass.html#USER_ConfigureProcessor
         :param publicly_accessible: Indicates whether the DB instance is an internet-facing instance. Default: - ``true`` if ``vpcSubnets`` is ``subnetType: SubnetType.PUBLIC``, ``false`` otherwise
         :param removal_policy: The CloudFormation policy to apply when the instance is removed from the stack or replaced during an update. Default: - RemovalPolicy.SNAPSHOT (remove the resource, but retain a snapshot of the data)
         :param s3_export_buckets: S3 buckets that you want to load data into. This property must not be used if ``s3ExportRole`` is used. For Microsoft SQL Server: Default: - None
         :param s3_export_role: Role that will be associated with this DB instance to enable S3 export. This property must not be used if ``s3ExportBuckets`` is used. For Microsoft SQL Server: Default: - New role is created if ``s3ExportBuckets`` is set, no role is defined otherwise
         :param s3_import_buckets: S3 buckets that you want to load data from. This feature is only supported by the Microsoft SQL Server, Oracle, and PostgreSQL engines. This property must not be used if ``s3ImportRole`` is used. For Microsoft SQL Server: Default: - None
         :param s3_import_role: Role that will be associated with this DB instance to enable S3 import. This feature is only supported by the Microsoft SQL Server, Oracle, and PostgreSQL engines. This property must not be used if ``s3ImportBuckets`` is used. For Microsoft SQL Server: Default: - New role is created if ``s3ImportBuckets`` is set, no role is defined otherwise
         :param security_groups: The security groups to assign to the DB instance. Default: - a new security group is created
+        :param storage_throughput: The storage throughput, specified in mebibytes per second (MiBps). Only applicable for GP3. Default: - 125 MiBps if allocated storage is less than 400 GiB for MariaDB, MySQL, and PostgreSQL, less than 200 GiB for Oracle and less than 20 GiB for SQL Server. 500 MiBps otherwise (except for SQL Server where the default is always 125 MiBps).
         :param storage_type: The storage type. Storage types supported are gp2, io1, standard. Default: GP2
         :param subnet_group: Existing subnet group for the instance. Default: - a new subnet group will be created.
         :param vpc_subnets: The type of subnets to add to the created DB subnet group. Default: - private subnets
         :param engine: The database engine.
         :param allocated_storage: The allocated storage size, specified in gibibytes (GiB). Default: 100
         :param allow_major_version_upgrade: Whether to allow major version upgrades. Default: false
         :param database_name: The name of the database. Default: - no name
@@ -1438,14 +1450,15 @@
             check_type(argname="argument iam_authentication", value=iam_authentication, expected_type=type_hints["iam_authentication"])
             check_type(argname="argument instance_identifier", value=instance_identifier, expected_type=type_hints["instance_identifier"])
             check_type(argname="argument iops", value=iops, expected_type=type_hints["iops"])
             check_type(argname="argument max_allocated_storage", value=max_allocated_storage, expected_type=type_hints["max_allocated_storage"])
             check_type(argname="argument monitoring_interval", value=monitoring_interval, expected_type=type_hints["monitoring_interval"])
             check_type(argname="argument monitoring_role", value=monitoring_role, expected_type=type_hints["monitoring_role"])
             check_type(argname="argument multi_az", value=multi_az, expected_type=type_hints["multi_az"])
+            check_type(argname="argument network_type", value=network_type, expected_type=type_hints["network_type"])
             check_type(argname="argument option_group", value=option_group, expected_type=type_hints["option_group"])
             check_type(argname="argument parameter_group", value=parameter_group, expected_type=type_hints["parameter_group"])
             check_type(argname="argument performance_insight_encryption_key", value=performance_insight_encryption_key, expected_type=type_hints["performance_insight_encryption_key"])
             check_type(argname="argument performance_insight_retention", value=performance_insight_retention, expected_type=type_hints["performance_insight_retention"])
             check_type(argname="argument port", value=port, expected_type=type_hints["port"])
             check_type(argname="argument preferred_backup_window", value=preferred_backup_window, expected_type=type_hints["preferred_backup_window"])
             check_type(argname="argument preferred_maintenance_window", value=preferred_maintenance_window, expected_type=type_hints["preferred_maintenance_window"])
@@ -1453,14 +1466,15 @@
             check_type(argname="argument publicly_accessible", value=publicly_accessible, expected_type=type_hints["publicly_accessible"])
             check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
             check_type(argname="argument s3_export_buckets", value=s3_export_buckets, expected_type=type_hints["s3_export_buckets"])
             check_type(argname="argument s3_export_role", value=s3_export_role, expected_type=type_hints["s3_export_role"])
             check_type(argname="argument s3_import_buckets", value=s3_import_buckets, expected_type=type_hints["s3_import_buckets"])
             check_type(argname="argument s3_import_role", value=s3_import_role, expected_type=type_hints["s3_import_role"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
+            check_type(argname="argument storage_throughput", value=storage_throughput, expected_type=type_hints["storage_throughput"])
             check_type(argname="argument storage_type", value=storage_type, expected_type=type_hints["storage_type"])
             check_type(argname="argument subnet_group", value=subnet_group, expected_type=type_hints["subnet_group"])
             check_type(argname="argument vpc_subnets", value=vpc_subnets, expected_type=type_hints["vpc_subnets"])
             check_type(argname="argument engine", value=engine, expected_type=type_hints["engine"])
             check_type(argname="argument allocated_storage", value=allocated_storage, expected_type=type_hints["allocated_storage"])
             check_type(argname="argument allow_major_version_upgrade", value=allow_major_version_upgrade, expected_type=type_hints["allow_major_version_upgrade"])
             check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
@@ -1514,14 +1528,16 @@
             self._values["max_allocated_storage"] = max_allocated_storage
         if monitoring_interval is not None:
             self._values["monitoring_interval"] = monitoring_interval
         if monitoring_role is not None:
             self._values["monitoring_role"] = monitoring_role
         if multi_az is not None:
             self._values["multi_az"] = multi_az
+        if network_type is not None:
+            self._values["network_type"] = network_type
         if option_group is not None:
             self._values["option_group"] = option_group
         if parameter_group is not None:
             self._values["parameter_group"] = parameter_group
         if performance_insight_encryption_key is not None:
             self._values["performance_insight_encryption_key"] = performance_insight_encryption_key
         if performance_insight_retention is not None:
@@ -1544,14 +1560,16 @@
             self._values["s3_export_role"] = s3_export_role
         if s3_import_buckets is not None:
             self._values["s3_import_buckets"] = s3_import_buckets
         if s3_import_role is not None:
             self._values["s3_import_role"] = s3_import_role
         if security_groups is not None:
             self._values["security_groups"] = security_groups
+        if storage_throughput is not None:
+            self._values["storage_throughput"] = storage_throughput
         if storage_type is not None:
             self._values["storage_type"] = storage_type
         if subnet_group is not None:
             self._values["subnet_group"] = subnet_group
         if vpc_subnets is not None:
             self._values["vpc_subnets"] = vpc_subnets
         if allocated_storage is not None:
@@ -1695,15 +1713,15 @@
     @builtins.property
     def domain_role(self) -> typing.Optional[aws_cdk.aws_iam.IRole]:
         '''The IAM role to be used when making API calls to the Directory Service.
 
         The role needs the AWS-managed policy
         AmazonRDSDirectoryServiceAccess or equivalent.
 
-        :default: - The role will be created for you if {@link DatabaseInstanceNewProps#domain} is specified
+        :default: - The role will be created for you if ``DatabaseInstanceNewProps#domain`` is specified
         '''
         result = self._values.get("domain_role")
         return typing.cast(typing.Optional[aws_cdk.aws_iam.IRole], result)
 
     @builtins.property
     def enable_performance_insights(self) -> typing.Optional[builtins.bool]:
         '''Whether to enable Performance Insights for the DB instance.
@@ -1736,15 +1754,20 @@
 
     @builtins.property
     def iops(self) -> typing.Optional[jsii.Number]:
         '''The number of I/O operations per second (IOPS) that the database provisions.
 
         The value must be equal to or greater than 1000.
 
-        :default: - no provisioned iops
+        :default:
+
+        - no provisioned iops if storage type is not specified. For GP3: 3,000 IOPS if allocated
+        storage is less than 400 GiB for MariaDB, MySQL, and PostgreSQL, less than 200 GiB for Oracle and
+        less than 20 GiB for SQL Server. 12,000 IOPS otherwise (except for SQL Server where the default is
+        always 3,000 IOPS).
         '''
         result = self._values.get("iops")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def max_allocated_storage(self) -> typing.Optional[jsii.Number]:
         '''Upper limit to which RDS can scale the storage in GiB(Gibibyte).
@@ -1780,14 +1803,23 @@
 
         :default: false
         '''
         result = self._values.get("multi_az")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def network_type(self) -> typing.Optional[aws_cdk.aws_rds.NetworkType]:
+        '''The network type of the DB instance.
+
+        :default: - IPV4
+        '''
+        result = self._values.get("network_type")
+        return typing.cast(typing.Optional[aws_cdk.aws_rds.NetworkType], result)
+
+    @builtins.property
     def option_group(self) -> typing.Optional[aws_cdk.aws_rds.IOptionGroup]:
         '''The option group to associate with the instance.
 
         :default: - no option group
         '''
         result = self._values.get("option_group")
         return typing.cast(typing.Optional[aws_cdk.aws_rds.IOptionGroup], result)
@@ -1814,15 +1846,15 @@
 
     @builtins.property
     def performance_insight_retention(
         self,
     ) -> typing.Optional[aws_cdk.aws_rds.PerformanceInsightRetention]:
         '''The amount of time, in days, to retain Performance Insights data.
 
-        :default: 7
+        :default: 7 this is the free tier
         '''
         result = self._values.get("performance_insight_retention")
         return typing.cast(typing.Optional[aws_cdk.aws_rds.PerformanceInsightRetention], result)
 
     @builtins.property
     def port(self) -> typing.Optional[jsii.Number]:
         '''The port for the instance.
@@ -1972,14 +2004,31 @@
 
         :default: - a new security group is created
         '''
         result = self._values.get("security_groups")
         return typing.cast(typing.Optional[typing.List[aws_cdk.aws_ec2.ISecurityGroup]], result)
 
     @builtins.property
+    def storage_throughput(self) -> typing.Optional[jsii.Number]:
+        '''The storage throughput, specified in mebibytes per second (MiBps).
+
+        Only applicable for GP3.
+
+        :default:
+
+        - 125 MiBps if allocated storage is less than 400 GiB for MariaDB, MySQL, and PostgreSQL,
+        less than 200 GiB for Oracle and less than 20 GiB for SQL Server. 500 MiBps otherwise (except for
+        SQL Server where the default is always 125 MiBps).
+
+        :see: https://docs.aws.amazon.com//AmazonRDS/latest/UserGuide/CHAP_Storage.html#gp3-storage
+        '''
+        result = self._values.get("storage_throughput")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def storage_type(self) -> typing.Optional[aws_cdk.aws_rds.StorageType]:
         '''The storage type.
 
         Storage types supported are gp2, io1, standard.
 
         :default: GP2
```

### Comparing `cdk-pgstac-4.2.1/src/cdk_pgstac.egg-info/PKG-INFO` & `cdk-pgstac-4.2.2/src/cdk_pgstac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.2.1
+Version: 4.2.2
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

