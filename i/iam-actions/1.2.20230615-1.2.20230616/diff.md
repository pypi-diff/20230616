# Comparing `tmp/iam_actions-1.2.20230615.tar.gz` & `tmp/iam_actions-1.2.20230616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230615.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230616.tar", max compression
```

## Comparing `iam_actions-1.2.20230615.tar` & `iam_actions-1.2.20230616.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-15 02:34:50.329228 iam_actions-1.2.20230615/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-15 02:34:50.329228 iam_actions-1.2.20230615/README.md
--rw-r--r--   0        0        0      228 2023-06-15 02:34:50.329228 iam_actions-1.2.20230615/iam_actions/__init__.py
--rw-r--r--   0        0        0  4314669 2023-06-15 02:36:27.781775 iam_actions-1.2.20230615/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-15 02:34:50.333228 iam_actions-1.2.20230615/iam_actions/generate/services.py
--rw-r--r--   0        0        0   555034 2023-06-15 02:36:27.781775 iam_actions-1.2.20230615/iam_actions/policies.json
--rw-r--r--   0        0        0   195840 2023-06-15 02:36:27.781775 iam_actions-1.2.20230615/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   538344 2023-06-15 02:36:27.781775 iam_actions-1.2.20230615/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-15 02:36:28.641780 iam_actions-1.2.20230615/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230615/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230615/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/README.md
+-rw-r--r--   0        0        0      228 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4319760 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   555328 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/policies.json
+-rw-r--r--   0        0        0   196366 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   538626 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-16 02:37:33.096760 iam_actions-1.2.20230616/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230616/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230616/PKG-INFO
```

### Comparing `iam_actions-1.2.20230615/LICENSE` & `iam_actions-1.2.20230616/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/README.md` & `iam_actions-1.2.20230616/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/iam_actions/actions.json` & `iam_actions-1.2.20230616/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996509769831773%*

 * *Differences: {"'datasync'": "{'UpdateDiscoveryJob': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *               "'UpdateDiscoveryJob'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *               "AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'drs'": "{'TagResource': {'resources': {insert: [(4, 'SourceNetworkResource')]}}, "*

 * *          "'UntagResource': {'resources': {insert: [(4, 'SourceNetworkResource')]}}, "*

 * *          "'DeleteSourceNetwork': {'access_level': 'Write', 'description':  […]*

```diff
@@ -34670,14 +34670,22 @@
             "condition_keys": [],
             "description": "Grants permission to update the name of an agent",
             "orphan": false,
             "resources": [
                 "agent"
             ]
         },
+        "UpdateDiscoveryJob": {
+            "access_level": "Undocumented",
+            "action": "UpdateDiscoveryJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateLocationHdfs": {
             "access_level": "Write",
             "action": "UpdateLocationHdfs",
             "condition_keys": [],
             "description": "Grants permission to update an HDFS sync Location",
             "orphan": false,
             "resources": [
@@ -40121,20 +40129,25 @@
             "description": "Grants permission to get associate failback client to recovery instance",
             "orphan": false,
             "resources": [
                 "RecoveryInstanceResource"
             ]
         },
         "AssociateSourceNetworkStack": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateSourceNetworkStack",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to associate CloudFormation stack with source network",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "SourceNetworkResource"
+            ]
         },
         "BatchCreateVolumeSnapshotGroupForDrs": {
             "access_level": "Write",
             "action": "BatchCreateVolumeSnapshotGroupForDrs",
             "condition_keys": [],
             "description": "Grants permission to batch create volume snapshot group",
             "orphan": false,
@@ -40207,18 +40220,21 @@
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create replication configuration template",
             "orphan": false,
             "resources": []
         },
         "CreateSourceNetwork": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSourceNetwork",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a source network",
             "orphan": false,
             "resources": []
         },
         "CreateSourceServerForDrs": {
             "access_level": "Write",
             "action": "CreateSourceServerForDrs",
             "condition_keys": [
@@ -40266,20 +40282,22 @@
             "description": "Grants permission to delete replication configuration template",
             "orphan": false,
             "resources": [
                 "ReplicationConfigurationTemplateResource"
             ]
         },
         "DeleteSourceNetwork": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteSourceNetwork",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete source network",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "SourceNetworkResource"
+            ]
         },
         "DeleteSourceServer": {
             "access_level": "Write",
             "action": "DeleteSourceServer",
             "condition_keys": [],
             "description": "Grants permission to delete source server",
             "orphan": false,
@@ -40352,18 +40370,18 @@
             "action": "DescribeSnapshotRequestsForDrs",
             "condition_keys": [],
             "description": "Grants permission to describe snapshot requests",
             "orphan": false,
             "resources": []
         },
         "DescribeSourceNetworks": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeSourceNetworks",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe source networks",
             "orphan": false,
             "resources": []
         },
         "DescribeSourceServers": {
             "access_level": "Read",
             "action": "DescribeSourceServers",
             "condition_keys": [],
@@ -40388,20 +40406,25 @@
             "description": "Grants permission to disconnect source server",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
         "ExportSourceNetworkCfnTemplate": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ExportSourceNetworkCfnTemplate",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to export CloudFormation template which contains source network resources",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "SourceNetworkResource"
+            ]
         },
         "GetAgentCommandForDrs": {
             "access_level": "Read",
             "action": "GetAgentCommandForDrs",
             "condition_keys": [],
             "description": "Grants permission to get agent command",
             "orphan": false,
@@ -40759,28 +40782,35 @@
             "description": "Grants permission to start replication",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
         "StartSourceNetworkRecovery": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartSourceNetworkRecovery",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to start network recovery",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "SourceNetworkResource"
+            ]
         },
         "StartSourceNetworkReplication": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartSourceNetworkReplication",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start network replication",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "SourceNetworkResource"
+            ]
         },
         "StopFailback": {
             "access_level": "Write",
             "action": "StopFailback",
             "condition_keys": [],
             "description": "Grants permission to stop failback",
             "orphan": false,
@@ -40795,20 +40825,22 @@
             "description": "Grants permission to stop replication",
             "orphan": false,
             "resources": [
                 "SourceServerResource"
             ]
         },
         "StopSourceNetworkReplication": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StopSourceNetworkReplication",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to stop network replication",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "SourceNetworkResource"
+            ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
@@ -40817,14 +40849,15 @@
             "description": "Grants permission to assign a resource tag",
             "orphan": false,
             "resources": [
                 "JobResource",
                 "LaunchConfigurationTemplateResource",
                 "RecoveryInstanceResource",
                 "ReplicationConfigurationTemplateResource",
+                "SourceNetworkResource",
                 "SourceServerResource"
             ]
         },
         "TerminateRecoveryInstances": {
             "access_level": "Write",
             "action": "TerminateRecoveryInstances",
             "condition_keys": [
@@ -40846,14 +40879,15 @@
             "description": "Grants permission to untag a resource",
             "orphan": false,
             "resources": [
                 "JobResource",
                 "LaunchConfigurationTemplateResource",
                 "RecoveryInstanceResource",
                 "ReplicationConfigurationTemplateResource",
+                "SourceNetworkResource",
                 "SourceServerResource"
             ]
         },
         "UpdateAgentBacklogForDrs": {
             "access_level": "Write",
             "action": "UpdateAgentBacklogForDrs",
             "condition_keys": [],
@@ -52417,20 +52451,28 @@
             "description": "Grants permission to stop advertising an address range that was provisioned for use in AWS through bring your own IP addresses (BYOIP)",
             "orphan": false,
             "resources": []
         }
     },
     "ec2-instance-connect": {
         "OpenTunnel": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "OpenTunnel",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2-instance-connect:MaxTunnelDuration",
+                "ec2-instance-connect:privateIpAddress",
+                "ec2-instance-connect:remotePort",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to establish SSH connection to an EC2 instance using EC2 Instance Connect Endpoint",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance-connect-endpoint"
+            ]
         },
         "SendSSHPublicKey": {
             "access_level": "Write",
             "action": "SendSSHPublicKey",
             "condition_keys": [
                 "ec2:osuser"
             ],
@@ -74514,18 +74556,18 @@
             "action": "CancelFindingsReport",
             "condition_keys": [],
             "description": "Grants permission to cancel the generation of a findings report",
             "orphan": false,
             "resources": []
         },
         "CancelSbomExport": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelSbomExport",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to cancel the generation of an SBOM report",
             "orphan": false,
             "resources": []
         },
         "CreateFilter": {
             "access_level": "Write",
             "action": "CreateFilter",
             "condition_keys": [
@@ -74543,18 +74585,18 @@
             "action": "CreateFindingsReport",
             "condition_keys": [],
             "description": "Grants permission to request the generation of a findings report",
             "orphan": false,
             "resources": []
         },
         "CreateSbomExport": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSbomExport",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to request the generation of an SBOM report",
             "orphan": false,
             "resources": []
         },
         "DeleteFilter": {
             "access_level": "Write",
             "action": "DeleteFilter",
             "condition_keys": [],
@@ -74633,18 +74675,18 @@
             "action": "GetEc2DeepInspectionConfiguration",
             "condition_keys": [],
             "description": "Grants permission to retrieve ec2 deep inspection configuration for standalone accounts, delegated administrator and member account",
             "orphan": false,
             "resources": []
         },
         "GetEncryptionKey": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetEncryptionKey",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve information about the KMS key used to encrypt code snippets with",
             "orphan": false,
             "resources": []
         },
         "GetFindingsReportStatus": {
             "access_level": "Read",
             "action": "GetFindingsReportStatus",
             "condition_keys": [],
@@ -74657,18 +74699,18 @@
             "action": "GetMember",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about an account that's associated with an Amazon Inspector administrator account",
             "orphan": false,
             "resources": []
         },
         "GetSbomExport": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSbomExport",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a requested SBOM report",
             "orphan": false,
             "resources": []
         },
         "ListAccountPermissions": {
             "access_level": "List",
             "action": "ListAccountPermissions",
             "condition_keys": [],
@@ -74745,18 +74787,18 @@
             "action": "ListUsageTotals",
             "condition_keys": [],
             "description": "Grants permission to retrieve aggregated usage data for an account",
             "orphan": false,
             "resources": []
         },
         "ResetEncryptionKey": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ResetEncryptionKey",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to let a customer reset to use an Amazon-owned KMS key to encrypt code snippets with",
             "orphan": false,
             "resources": []
         },
         "SearchVulnerabilities": {
             "access_level": "Read",
             "action": "SearchVulnerabilities",
             "condition_keys": [],
@@ -74799,18 +74841,18 @@
             "action": "UpdateEc2DeepInspectionConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update ec2 deep inspection configuration by delegated administrator, member and standalone account",
             "orphan": false,
             "resources": []
         },
         "UpdateEncryptionKey": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateEncryptionKey",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to let a customer use a KMS key to encrypt code snippets with",
             "orphan": false,
             "resources": []
         },
         "UpdateFilter": {
             "access_level": "Write",
             "action": "UpdateFilter",
             "condition_keys": [
@@ -90895,17 +90937,15 @@
         },
         "DescribeLogGroups": {
             "access_level": "List",
             "action": "DescribeLogGroups",
             "condition_keys": [],
             "description": "Grants permission to return all the log groups that are associated with the AWS account making the request",
             "orphan": false,
-            "resources": [
-                "log-group"
-            ]
+            "resources": []
         },
         "DescribeLogStreams": {
             "access_level": "List",
             "action": "DescribeLogStreams",
             "condition_keys": [],
             "description": "Grants permission to return all the log streams that are associated with the specified log group",
             "orphan": false,
@@ -111096,14 +111136,22 @@
             "access_level": "Write",
             "action": "ListCustomPermissions",
             "condition_keys": [],
             "description": "Grants permission to list custom permissions resources in QuickSight account",
             "orphan": false,
             "resources": []
         },
+        "ListCustomerManagedKeys": {
+            "access_level": "Undocumented",
+            "action": "ListCustomerManagedKeys",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListDashboardVersions": {
             "access_level": "List",
             "action": "ListDashboardVersions",
             "condition_keys": [],
             "description": "Grants permission to list all versions of a QuickSight Dashboard",
             "orphan": false,
             "resources": [
@@ -111209,14 +111257,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to list all SPICE ingestions on a dataset",
             "orphan": false,
             "resources": []
         },
+        "ListKMSKeysForUser": {
+            "access_level": "Undocumented",
+            "action": "ListKMSKeysForUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListNamespaces": {
             "access_level": "List",
             "action": "ListNamespaces",
             "condition_keys": [],
             "description": "Grants permission to lists all namespaces in a QuickSight account",
             "orphan": false,
             "resources": []
@@ -111386,27 +111442,43 @@
             "condition_keys": [],
             "description": "Grants permission to put dataset refresh properties for a dataset",
             "orphan": false,
             "resources": [
                 "dataset"
             ]
         },
+        "RegisterCustomerManagedKey": {
+            "access_level": "Undocumented",
+            "action": "RegisterCustomerManagedKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RegisterUser": {
             "access_level": "Write",
             "action": "RegisterUser",
             "condition_keys": [
                 "quicksight:IamArn",
                 "quicksight:SessionName"
             ],
             "description": "Grants permission to create a QuickSight user, whose identity is associated with the IAM identity/role specified in the request",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
+        "RemoveCustomerManagedKey": {
+            "access_level": "Undocumented",
+            "action": "RemoveCustomerManagedKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RestoreAnalysis": {
             "access_level": "Write",
             "action": "RestoreAnalysis",
             "condition_keys": [],
             "description": "Grants permission to restore a deleted analysis",
             "orphan": false,
             "resources": [
@@ -116278,14 +116350,22 @@
             "orphan": false,
             "resources": [
                 "route"
             ]
         }
     },
     "rekognition": {
+        "AssociateFaces": {
+            "access_level": "Undocumented",
+            "action": "AssociateFaces",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CompareFaces": {
             "access_level": "Read",
             "action": "CompareFaces",
             "condition_keys": [],
             "description": "Grants permission to compare faces in the source input image with each face detected in the target input image",
             "orphan": false,
             "resources": []
@@ -116365,14 +116445,22 @@
             ],
             "description": "Grants permission to create an Amazon Rekognition stream processor",
             "orphan": false,
             "resources": [
                 "collection"
             ]
         },
+        "CreateUser": {
+            "access_level": "Undocumented",
+            "action": "CreateUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteCollection": {
             "access_level": "Write",
             "action": "DeleteCollection",
             "condition_keys": [],
             "description": "Grants permission to delete the specified collection",
             "orphan": false,
             "resources": [
@@ -116435,14 +116523,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete the specified stream processor",
             "orphan": false,
             "resources": [
                 "streamprocessor"
             ]
         },
+        "DeleteUser": {
+            "access_level": "Undocumented",
+            "action": "DeleteUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeCollection": {
             "access_level": "Read",
             "action": "DescribeCollection",
             "condition_keys": [],
             "description": "Grants permission to read details about a collection",
             "orphan": false,
             "resources": [
@@ -116533,14 +116629,22 @@
             "access_level": "Read",
             "action": "DetectText",
             "condition_keys": [],
             "description": "Grants permission to detect text in the input image and convert it into machine-readable text",
             "orphan": false,
             "resources": []
         },
+        "DisassociateFaces": {
+            "access_level": "Undocumented",
+            "action": "DisassociateFaces",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DistributeDatasetEntries": {
             "access_level": "Write",
             "action": "DistributeDatasetEntries",
             "condition_keys": [],
             "description": "Grants permission to distribute the entries in a training dataset across the training dataset and the test dataset for a project",
             "orphan": false,
             "resources": [
@@ -116703,14 +116807,22 @@
             "condition_keys": [],
             "description": "Grants permission to return a list of tags associated with a resource",
             "orphan": false,
             "resources": [
                 "projectversion"
             ]
         },
+        "ListUsers": {
+            "access_level": "Undocumented",
+            "action": "ListUsers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PutProjectPolicy": {
             "access_level": "Write",
             "action": "PutProjectPolicy",
             "condition_keys": [],
             "description": "Grants permission to attach a resource policy to a project",
             "orphan": false,
             "resources": [
@@ -116741,14 +116853,30 @@
             "condition_keys": [],
             "description": "Grants permission to search the specificed collection for the largest face in the input image",
             "orphan": false,
             "resources": [
                 "collection"
             ]
         },
+        "SearchUsers": {
+            "access_level": "Undocumented",
+            "action": "SearchUsers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "SearchUsersByImage": {
+            "access_level": "Undocumented",
+            "action": "SearchUsersByImage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartCelebrityRecognition": {
             "access_level": "Write",
             "action": "StartCelebrityRecognition",
             "condition_keys": [],
             "description": "Grants permission to start the asynchronous recognition of celebrities in a stored video",
             "orphan": false,
             "resources": []
@@ -124789,15 +124917,16 @@
         },
         "AddTags": {
             "access_level": "Tagging",
             "action": "AddTags",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "sagemaker:TaggingAction"
             ],
             "description": "Grants permission to add or overwrite one or more tags for the specified Amazon SageMaker resource",
             "orphan": false,
             "resources": [
                 "action",
                 "algorithm",
                 "app",
@@ -130239,20 +130368,22 @@
             "description": "Grants permission to accept Security Hub invitations to become a member account",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
         "BatchDeleteAutomationRules": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "BatchDeleteAutomationRules",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete one or more automation rules in Security Hub",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "automation-rule"
+            ]
         },
         "BatchDisableStandards": {
             "access_level": "Write",
             "action": "BatchDisableStandards",
             "condition_keys": [],
             "description": "Grants permission to disable standards in Security Hub",
             "orphan": false,
@@ -130267,20 +130398,22 @@
             "description": "Grants permission to enable standards in Security Hub",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
         "BatchGetAutomationRules": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "BatchGetAutomationRules",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a list of details for automation rules from Security Hub based on rule Amazon Resource Names (ARNs)",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "automation-rule"
+            ]
         },
         "BatchGetControlEvaluations": {
             "access_level": "Read",
             "action": "BatchGetControlEvaluations",
             "condition_keys": [],
             "description": "Grants permission to get the enablement and compliance status of controls, the findings count for controls, and the overall security score for controls on the Security Hub console",
             "orphan": false,
@@ -130313,20 +130446,22 @@
             "description": "Grants permission to import findings into Security Hub from an integrated product",
             "orphan": false,
             "resources": [
                 "product"
             ]
         },
         "BatchUpdateAutomationRules": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "BatchUpdateAutomationRules",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update one or more automation rules from Security Hub based on rule Amazon Resource Names (ARNs) and input parameters",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "automation-rule"
+            ]
         },
         "BatchUpdateFindings": {
             "access_level": "Write",
             "action": "BatchUpdateFindings",
             "condition_keys": [
                 "securityhub:ASFFSyntaxPath/${ASFFSyntaxPath}"
             ],
@@ -130351,18 +130486,21 @@
             "description": "Grants permission to create custom actions in Security Hub",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
         "CreateAutomationRule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateAutomationRule",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create an automation rule based on input parameters",
             "orphan": false,
             "resources": []
         },
         "CreateFindingAggregator": {
             "access_level": "Write",
             "action": "CreateFindingAggregator",
             "condition_keys": [],
@@ -130770,18 +130908,18 @@
             "description": "Grants permission to invite other AWS accounts to become Security Hub member accounts",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
         "ListAutomationRules": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListAutomationRules",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a list of automation rules and their metadata for the calling account from Security Hub",
             "orphan": false,
             "resources": []
         },
         "ListControlEvaluationSummaries": {
             "access_level": "Read",
             "action": "ListControlEvaluationSummaries",
             "condition_keys": [],
@@ -130858,14 +130996,15 @@
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list of tags associated with a resource",
             "orphan": false,
             "resources": [
+                "automation-rule",
                 "hub"
             ]
         },
         "SendFindingEvents": {
             "access_level": "Read",
             "action": "SendFindingEvents",
             "condition_keys": [],
@@ -130888,24 +131027,26 @@
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Grants permission to add tags to a Security Hub resource",
             "orphan": false,
             "resources": [
+                "automation-rule",
                 "hub"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Grants permission to remove tags from a Security Hub resource",
             "orphan": false,
             "resources": [
+                "automation-rule",
                 "hub"
             ]
         },
         "UpdateActionTarget": {
             "access_level": "Write",
             "action": "UpdateActionTarget",
             "condition_keys": [],
@@ -150080,20 +150221,22 @@
             "description": "Grants permission to associate a lens to the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
         "AssociateProfiles": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateProfiles",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to associate a profile to the specified workload",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workload"
+            ]
         },
         "CreateLensShare": {
             "access_level": "Write",
             "action": "CreateLensShare",
             "condition_keys": [],
             "description": "Grants permission to an owner of a lens to share with other AWS accounts and IAM Users",
             "orphan": false,
@@ -150118,28 +150261,33 @@
             "description": "Grants permission to create a new milestone for the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
         "CreateProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateProfile",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a new profile",
             "orphan": false,
             "resources": []
         },
         "CreateProfileShare": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateProfileShare",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to an owner of a profile to share with other AWS accounts and IAM Users",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "profile"
+            ]
         },
         "CreateWorkload": {
             "access_level": "Write",
             "action": "CreateWorkload",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -150175,28 +150323,32 @@
             "description": "Grants permission to delete an existing lens share",
             "orphan": false,
             "resources": [
                 "lens"
             ]
         },
         "DeleteProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteProfile",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a profile",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "profile"
+            ]
         },
         "DeleteProfileShare": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteProfileShare",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete an existing profile share",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "profile"
+            ]
         },
         "DeleteWorkload": {
             "access_level": "Write",
             "action": "DeleteWorkload",
             "condition_keys": [],
             "description": "Grants permission to delete an existing workload",
             "orphan": false,
@@ -150221,20 +150373,22 @@
             "description": "Grants permission to disassociate a lens from the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
         "DisassociateProfiles": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateProfiles",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to disassociate a profile from the specified workload",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workload"
+            ]
         },
         "ExportLens": {
             "access_level": "Read",
             "action": "ExportLens",
             "condition_keys": [],
             "description": "Grants permission to export an existing lens",
             "orphan": false,
@@ -150309,26 +150463,30 @@
             "description": "Grants permission to retrieve the specified milestone of the specified workload",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
         "GetProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetProfile",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to retrieve the specified profile",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "profile"
+            ]
         },
         "GetProfileTemplate": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetProfileTemplate",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve the specified profile template",
             "orphan": false,
             "resources": []
         },
         "GetWorkload": {
             "access_level": "Read",
             "action": "GetWorkload",
             "condition_keys": [
@@ -150434,34 +150592,36 @@
             "action": "ListNotifications",
             "condition_keys": [],
             "description": "Grants permission to list notifications related to the account or specified resource",
             "orphan": false,
             "resources": []
         },
         "ListProfileNotifications": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListProfileNotifications",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list profile notifications related to specified resource",
             "orphan": false,
             "resources": []
         },
         "ListProfileShares": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListProfileShares",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all shares created for a profile",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "profile"
+            ]
         },
         "ListProfiles": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListProfiles",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the profiles available to this account",
             "orphan": false,
             "resources": []
         },
         "ListShareInvitations": {
             "access_level": "List",
             "action": "ListShareInvitations",
             "condition_keys": [],
@@ -150475,14 +150635,15 @@
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to list tags for a Well-Architected resource",
             "orphan": false,
             "resources": [
                 "lens",
+                "profile",
                 "workload"
             ]
         },
         "ListWorkloadShares": {
             "access_level": "List",
             "action": "ListWorkloadShares",
             "condition_keys": [],
@@ -150507,27 +150668,29 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to tag a Well-Architected resource",
             "orphan": false,
             "resources": [
                 "lens",
+                "profile",
                 "workload"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to untag a Well-Architected resource",
             "orphan": false,
             "resources": [
                 "lens",
+                "profile",
                 "workload"
             ]
         },
         "UpdateAnswer": {
             "access_level": "Write",
             "action": "UpdateAnswer",
             "condition_keys": [],
@@ -150552,20 +150715,22 @@
             "description": "Grants permission to update properties of the specified lens review",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
         "UpdateProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateProfile",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update properties of the specified profile",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "profile"
+            ]
         },
         "UpdateShareInvitation": {
             "access_level": "Write",
             "action": "UpdateShareInvitation",
             "condition_keys": [],
             "description": "Grants permission to update status of the specified workload share invitation",
             "orphan": false,
@@ -150598,20 +150763,23 @@
             "description": "Grants permission to upgrade the specified lens review to use the latest version of the associated lens",
             "orphan": false,
             "resources": [
                 "workload"
             ]
         },
         "UpgradeProfileVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpgradeProfileVersion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to upgrade the specified workload to use the latest version of the associated profile",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "profile",
+                "workload"
+            ]
         }
     },
     "wickr": {
         "CreateAdminSession": {
             "access_level": "Write",
             "action": "CreateAdminSession",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230615/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230616/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230616/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/iam_actions/generate/generate.py` & `iam_actions-1.2.20230616/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230616/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230616/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/iam_actions/generate/services.py` & `iam_actions-1.2.20230616/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230615/iam_actions/policies.json` & `iam_actions-1.2.20230616/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999985086839274%*

 * *Differences: {"'serviceMap'": "{'Amazon QuickSight': {'Actions': {insert: [(102, 'ListCustomerManagedKeys'), "*

 * *                 "(114, 'ListKMSKeysForUser'), (132, 'RegisterCustomerManagedKey'), (134, "*

 * *                 "'RemoveCustomerManagedKey')]}}, 'Amazon Rekognition': {'Actions': {insert: [(0, "*

 * *                 "'AssociateFaces'), (9, 'CreateUser'), (17, 'DeleteUser'), (29, "*

 * *                 "'DisassociateFaces'), (49, 'ListUsers'), (54, 'SearchUsers'), (55, "*

 * *                 "'SearchUsersByImage')]}}, 'AWS Dat […]*

```diff
@@ -2610,14 +2610,15 @@
                 "RemoveStorageSystem",
                 "StartDiscoveryJob",
                 "StartTaskExecution",
                 "StopDiscoveryJob",
                 "TagResource",
                 "UntagResource",
                 "UpdateAgent",
+                "UpdateDiscoveryJob",
                 "UpdateLocationHdfs",
                 "UpdateLocationNfs",
                 "UpdateLocationObjectStorage",
                 "UpdateLocationSmb",
                 "UpdateStorageSystem",
                 "UpdateTask",
                 "UpdateTaskExecution"
@@ -16962,25 +16963,27 @@
                 "GetDashboardEmbedUrl",
                 "GetGroupMapping",
                 "GetSessionEmbedUrl",
                 "ListAnalyses",
                 "ListAssetBundleExportJobs",
                 "ListAssetBundleImportJobs",
                 "ListCustomPermissions",
+                "ListCustomerManagedKeys",
                 "ListDashboardVersions",
                 "ListDashboards",
                 "ListDataSets",
                 "ListDataSources",
                 "ListFolderMembers",
                 "ListFolders",
                 "ListGroupMemberships",
                 "ListGroups",
                 "ListIAMPolicyAssignments",
                 "ListIAMPolicyAssignmentsForUser",
                 "ListIngestions",
+                "ListKMSKeysForUser",
                 "ListNamespaces",
                 "ListRefreshSchedules",
                 "ListTagsForResource",
                 "ListTemplateAliases",
                 "ListTemplateVersions",
                 "ListTemplates",
                 "ListThemeAliases",
@@ -16990,15 +16993,17 @@
                 "ListTopics",
                 "ListUserGroups",
                 "ListUsers",
                 "ListVPCConnections",
                 "PassDataSet",
                 "PassDataSource",
                 "PutDataSetRefreshProperties",
+                "RegisterCustomerManagedKey",
                 "RegisterUser",
+                "RemoveCustomerManagedKey",
                 "RestoreAnalysis",
                 "ScopeDownPolicy",
                 "SearchAnalyses",
                 "SearchDashboards",
                 "SearchDataSets",
                 "SearchDataSources",
                 "SearchDirectoryGroups",
@@ -17513,40 +17518,44 @@
                 "redshift-serverless:workgroupId"
             ]
         },
         "Amazon Rekognition": {
             "ARNFormat": "arn:aws:rekognition:${Region}:${Account}:${RelativeId}",
             "ARNRegex": "^arn:aws:rekognition:.+",
             "Actions": [
+                "AssociateFaces",
                 "CompareFaces",
                 "CopyProjectVersion",
                 "CreateCollection",
                 "CreateDataset",
                 "CreateFaceLivenessSession",
                 "CreateProject",
                 "CreateProjectVersion",
                 "CreateStreamProcessor",
+                "CreateUser",
                 "DeleteCollection",
                 "DeleteDataset",
                 "DeleteFaces",
                 "DeleteProject",
                 "DeleteProjectPolicy",
                 "DeleteProjectVersion",
                 "DeleteStreamProcessor",
+                "DeleteUser",
                 "DescribeCollection",
                 "DescribeDataset",
                 "DescribeProjectVersions",
                 "DescribeProjects",
                 "DescribeStreamProcessor",
                 "DetectCustomLabels",
                 "DetectFaces",
                 "DetectLabels",
                 "DetectModerationLabels",
                 "DetectProtectiveEquipment",
                 "DetectText",
+                "DisassociateFaces",
                 "DistributeDatasetEntries",
                 "GetCelebrityInfo",
                 "GetCelebrityRecognition",
                 "GetContentModeration",
                 "GetFaceDetection",
                 "GetFaceLivenessSessionResults",
                 "GetFaceSearch",
@@ -17558,18 +17567,21 @@
                 "ListCollections",
                 "ListDatasetEntries",
                 "ListDatasetLabels",
                 "ListFaces",
                 "ListProjectPolicies",
                 "ListStreamProcessors",
                 "ListTagsForResource",
+                "ListUsers",
                 "PutProjectPolicy",
                 "RecognizeCelebrities",
                 "SearchFaces",
                 "SearchFacesByImage",
+                "SearchUsers",
+                "SearchUsersByImage",
                 "StartCelebrityRecognition",
                 "StartContentModeration",
                 "StartFaceDetection",
                 "StartFaceLivenessSession",
                 "StartFaceSearch",
                 "StartLabelDetection",
                 "StartPersonTracking",
```

### Comparing `iam_actions-1.2.20230615/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230616/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982686980609419%*

 * *Differences: {"'drs'": "{'SourceNetworkResource': OrderedDict([('arn_pattern', "*

 * *          "'arn:*:drs:*:*:source-network/*'), ('condition_keys', 'aws:ResourceTag/${TagKey}')])}",*

 * * "'ec2-instance-connect'": "{'instance-connect-endpoint': OrderedDict([('arn_pattern', "*

 * *                           "'arn:*:ec2:*:*:instance-connect-endpoint/*'), ('condition_keys', "*

 * *                           "'aws:ResourceTag/${TagKey}')])}",*

 * * "'securityhub'": "{'automation-rule': OrderedDict([('arn_pattern', "*

 * *                  "'arn:*:sec […]*

```diff
@@ -1844,14 +1844,18 @@
             "arn_pattern": "arn:*:drs:*:*:recovery-instance/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "ReplicationConfigurationTemplateResource": {
             "arn_pattern": "arn:*:drs:*:*:replication-configuration-template/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "SourceNetworkResource": {
+            "arn_pattern": "arn:*:drs:*:*:source-network/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "SourceServerResource": {
             "arn_pattern": "arn:*:drs:*:*:source-server/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "ds": {
         "directory": {
@@ -2249,14 +2253,18 @@
             "condition_keys": "aws:RequestTag/${TagKey}"
         }
     },
     "ec2-instance-connect": {
         "instance": {
             "arn_pattern": "arn:*:ec2:*:*:instance/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "instance-connect-endpoint": {
+            "arn_pattern": "arn:*:ec2:*:*:instance-connect-endpoint/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "ec2messages": {},
     "ecr": {
         "repository": {
             "arn_pattern": "arn:*:ecr:*:*:repository/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -5797,14 +5805,18 @@
     "secretsmanager": {
         "Secret": {
             "arn_pattern": "arn:*:secretsmanager:*:*:secret:*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         }
     },
     "securityhub": {
+        "automation-rule": {
+            "arn_pattern": "arn:*:securityhub:*:*:automation-rule/*",
+            "condition_keys": null
+        },
         "finding-aggregator": {
             "arn_pattern": "arn:*:securityhub:*:*:finding-aggregator/*",
             "condition_keys": null
         },
         "hub": {
             "arn_pattern": "arn:*:securityhub:*:*:hub/default",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -6537,14 +6549,18 @@
     },
     "wam": {},
     "wellarchitected": {
         "lens": {
             "arn_pattern": "arn:*:wellarchitected:*:*:lens/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "profile": {
+            "arn_pattern": "arn:*:wellarchitected:*:*:profile/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "workload": {
             "arn_pattern": "arn:*:wellarchitected:*:*:workload/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "wickr": {
         "network": {
```

### Comparing `iam_actions-1.2.20230615/iam_actions/services.json` & `iam_actions-1.2.20230616/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999843845574671%*

 * *Differences: {"'datasync'": "{'Actions': {insert: [(49, 'UpdateDiscoveryJob')]}}",*

 * * "'quicksight'": "{'Actions': {insert: [(102, 'ListCustomerManagedKeys'), (114, "*

 * *                 "'ListKMSKeysForUser'), (132, 'RegisterCustomerManagedKey'), (134, "*

 * *                 "'RemoveCustomerManagedKey')]}}",*

 * * "'rekognition'": "{'Actions': {insert: [(0, 'AssociateFaces'), (9, 'CreateUser'), (17, "*

 * *                  "'DeleteUser'), (29, 'DisassociateFaces'), (49, 'ListUsers'), (54, "*

 * *                  "'SearchUsers'), (55, 'Searc […]*

```diff
@@ -5160,14 +5160,15 @@
             "RemoveStorageSystem",
             "StartDiscoveryJob",
             "StartTaskExecution",
             "StopDiscoveryJob",
             "TagResource",
             "UntagResource",
             "UpdateAgent",
+            "UpdateDiscoveryJob",
             "UpdateLocationHdfs",
             "UpdateLocationNfs",
             "UpdateLocationObjectStorage",
             "UpdateLocationSmb",
             "UpdateStorageSystem",
             "UpdateTask",
             "UpdateTaskExecution"
@@ -15573,25 +15574,27 @@
             "GetDashboardEmbedUrl",
             "GetGroupMapping",
             "GetSessionEmbedUrl",
             "ListAnalyses",
             "ListAssetBundleExportJobs",
             "ListAssetBundleImportJobs",
             "ListCustomPermissions",
+            "ListCustomerManagedKeys",
             "ListDashboardVersions",
             "ListDashboards",
             "ListDataSets",
             "ListDataSources",
             "ListFolderMembers",
             "ListFolders",
             "ListGroupMemberships",
             "ListGroups",
             "ListIAMPolicyAssignments",
             "ListIAMPolicyAssignmentsForUser",
             "ListIngestions",
+            "ListKMSKeysForUser",
             "ListNamespaces",
             "ListRefreshSchedules",
             "ListTagsForResource",
             "ListTemplateAliases",
             "ListTemplateVersions",
             "ListTemplates",
             "ListThemeAliases",
@@ -15601,15 +15604,17 @@
             "ListTopics",
             "ListUserGroups",
             "ListUsers",
             "ListVPCConnections",
             "PassDataSet",
             "PassDataSource",
             "PutDataSetRefreshProperties",
+            "RegisterCustomerManagedKey",
             "RegisterUser",
+            "RemoveCustomerManagedKey",
             "RestoreAnalysis",
             "ScopeDownPolicy",
             "SearchAnalyses",
             "SearchDashboards",
             "SearchDataSets",
             "SearchDataSources",
             "SearchDirectoryGroups",
@@ -16300,40 +16305,44 @@
         "ARNFormats": [
             "arn:aws:rekognition:${Region}:${Account}:${RelativeId}"
         ],
         "ARNRegexes": [
             "^arn:aws:rekognition:.+"
         ],
         "Actions": [
+            "AssociateFaces",
             "CompareFaces",
             "CopyProjectVersion",
             "CreateCollection",
             "CreateDataset",
             "CreateFaceLivenessSession",
             "CreateProject",
             "CreateProjectVersion",
             "CreateStreamProcessor",
+            "CreateUser",
             "DeleteCollection",
             "DeleteDataset",
             "DeleteFaces",
             "DeleteProject",
             "DeleteProjectPolicy",
             "DeleteProjectVersion",
             "DeleteStreamProcessor",
+            "DeleteUser",
             "DescribeCollection",
             "DescribeDataset",
             "DescribeProjectVersions",
             "DescribeProjects",
             "DescribeStreamProcessor",
             "DetectCustomLabels",
             "DetectFaces",
             "DetectLabels",
             "DetectModerationLabels",
             "DetectProtectiveEquipment",
             "DetectText",
+            "DisassociateFaces",
             "DistributeDatasetEntries",
             "GetCelebrityInfo",
             "GetCelebrityRecognition",
             "GetContentModeration",
             "GetFaceDetection",
             "GetFaceLivenessSessionResults",
             "GetFaceSearch",
@@ -16345,18 +16354,21 @@
             "ListCollections",
             "ListDatasetEntries",
             "ListDatasetLabels",
             "ListFaces",
             "ListProjectPolicies",
             "ListStreamProcessors",
             "ListTagsForResource",
+            "ListUsers",
             "PutProjectPolicy",
             "RecognizeCelebrities",
             "SearchFaces",
             "SearchFacesByImage",
+            "SearchUsers",
+            "SearchUsersByImage",
             "StartCelebrityRecognition",
             "StartContentModeration",
             "StartFaceDetection",
             "StartFaceLivenessSession",
             "StartFaceSearch",
             "StartLabelDetection",
             "StartPersonTracking",
```

### Comparing `iam_actions-1.2.20230615/pyproject.toml` & `iam_actions-1.2.20230616/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230615"
+version = "1.2.20230616"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230615/setup.py` & `iam_actions-1.2.20230616/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230615',
+    'version': '1.2.20230616',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230615/PKG-INFO` & `iam_actions-1.2.20230616/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230615
+Version: 1.2.20230616
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

