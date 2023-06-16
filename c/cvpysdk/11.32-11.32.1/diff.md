# Comparing `tmp/cvpysdk-11.32.tar.gz` & `tmp/cvpysdk-11.32.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvpysdk-11.32.tar", last modified: Thu Jun 15 08:11:27 2023, max compression
+gzip compressed data, was "cvpysdk-11.32.1.tar", last modified: Fri Jun 16 06:45:13 2023, max compression
```

## Comparing `cvpysdk-11.32.tar` & `cvpysdk-11.32.1.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.220131 cvpysdk-11.32/
--rw-rw-rw-   0        0        0    11531 2023-06-15 06:13:11.000000 cvpysdk-11.32/LICENSE.txt
--rw-rw-rw-   0        0        0       71 2023-06-15 06:13:11.000000 cvpysdk-11.32/MANIFEST.in
--rw-rw-rw-   0        0        0     7649 2023-06-15 08:11:27.204508 cvpysdk-11.32/PKG-INFO
--rw-rw-rw-   0        0        0     7082 2023-06-15 08:11:08.000000 cvpysdk-11.32/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:25.980871 cvpysdk-11.32/cvpysdk/
--rw-rw-rw-   0        0        0     1347 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/__init__.py
--rw-rw-rw-   0        0        0     6845 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activate.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.090238 cvpysdk-11.32/cvpysdk/activateapps/
--rw-rw-rw-   0        0        0      866 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/__init__.py
--rw-rw-rw-   0        0        0    33458 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/constants.py
--rw-rw-rw-   0        0        0   136470 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/ediscovery_utils.py
--rw-rw-rw-   0        0        0   101465 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/entity_manager.py
--rw-rw-rw-   0        0        0    36915 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/file_storage_optimization.py
--rw-rw-rw-   0        0        0    45588 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/inventory_manager.py
--rw-rw-rw-   0        0        0    34226 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/request_manager.py
--rw-rw-rw-   0        0        0    20756 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activateapps/sensitive_data_governance.py
--rw-rw-rw-   0        0        0    10277 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/activitycontrol.py
--rw-rw-rw-   0        0        0    35180 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/agent.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.090238 cvpysdk-11.32/cvpysdk/agents/
--rw-rw-rw-   0        0        0      863 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/agents/__init__.py
--rw-rw-rw-   0        0        0     7472 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/agents/exchange_database_agent.py
--rw-rw-rw-   0        0        0    47512 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/alert.py
--rw-rw-rw-   0        0        0    26553 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/array_management.py
--rw-rw-rw-   0        0        0    10120 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/backup_network_pairs.py
--rw-rw-rw-   0        0        0    92668 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/backupset.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.152765 cvpysdk-11.32/cvpysdk/backupsets/
--rw-rw-rw-   0        0        0      863 2023-06-15 06:19:04.000000 cvpysdk-11.32/cvpysdk/backupsets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.168368 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/
--rw-rw-rw-   0        0        0      876 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/__init__.py
--rw-rw-rw-   0        0        0     2501 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/kubernetes.py
--rw-rw-rw-   0        0        0    10718 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/vmware.py
--rw-rw-rw-   0        0        0    18407 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/aadbackupset.py
--rw-rw-rw-   0        0        0     3275 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/adbackupset.py
--rw-rw-rw-   0        0        0     2695 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/cabackupset.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.168368 cvpysdk-11.32/cvpysdk/backupsets/cloudapps/
--rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/cloudapps/__init__.py
--rw-rw-rw-   0        0        0     9083 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/cloudapps/salesforce_backupset.py
--rw-rw-rw-   0        0        0    11908 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/db2backupset.py
--rw-rw-rw-   0        0        0    72677 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/fsbackupset.py
--rw-rw-rw-   0        0        0     4615 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/hanabackupset.py
--rw-rw-rw-   0        0        0     3639 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/nasbackupset.py
--rw-rw-rw-   0        0        0    11438 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/postgresbackupset.py
--rw-rw-rw-   0        0        0     3721 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/sharepointbackupset.py
--rw-rw-rw-   0        0        0    12986 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/backupsets/vsbackupset.py
--rw-rw-rw-   0        0        0     6246 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/certificates.py
--rw-rw-rw-   0        0        0   270983 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/client.py
--rw-rw-rw-   0        0        0    76883 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clientgroup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.183988 cvpysdk-11.32/cvpysdk/clients/
--rw-rw-rw-   0        0        0      860 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clients/__init__.py
--rw-rw-rw-   0        0        0     6864 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clients/onedrive_client.py
--rw-rw-rw-   0        0        0     9029 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/clients/vmclient.py
--rw-rw-rw-   0        0        0   146330 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/commcell.py
--rw-rw-rw-   0        0        0    24026 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/commcell_migration.py
--rw-rw-rw-   0        0        0    32624 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/constants.py
--rw-rw-rw-   0        0        0    16567 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/content_analyzer.py
--rw-rw-rw-   0        0        0    30092 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/credential_manager.py
--rw-rw-rw-   0        0        0    17286 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/cvpysdk.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.230869 cvpysdk-11.32/cvpysdk/datacube/
--rw-rw-rw-   0        0        0      879 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/__init__.py
--rw-rw-rw-   0        0        0     3294 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/constants.py
--rw-rw-rw-   0        0        0     6634 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/datacube.py
--rw-rw-rw-   0        0        0    36258 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/datasource.py
--rw-rw-rw-   0        0        0    18093 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/handler.py
--rw-rw-rw-   0        0        0     1997 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/datacube/sedstype.py
--rw-rw-rw-   0        0        0    54808 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/deduplication_engines.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.262118 cvpysdk-11.32/cvpysdk/deployment/
--rw-rw-rw-   0        0        0      863 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/__init__.py
--rw-rw-rw-   0        0        0    17053 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/cache_config.py
--rw-rw-rw-   0        0        0     3650 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/deployment/deploymentconstants.py
--rw-rw-rw-   0        0        0    19233 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/download.py
--rw-rw-rw-   0        0        0    30374 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/install.py
--rw-rw-rw-   0        0        0     6862 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/deployment/uninstall.py
--rw-rw-rw-   0        0        0     6091 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/dev_test_group.py
--rw-rw-rw-   0        0        0    42515 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/disasterrecovery.py
--rw-rw-rw-   0        0        0    23493 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/domains.py
--rw-rw-rw-   0        0        0    51805 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/download_center.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.308996 cvpysdk-11.32/cvpysdk/drorchestration/
--rw-rw-rw-   0        0        0      882 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/__init__.py
--rw-rw-rw-   0        0        0    48119 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/blr_pairs.py
--rw-rw-rw-   0        0        0     3808 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/dr_orchestration_job_phase.py
--rw-rw-rw-   0        0        0     7099 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/drjob.py
--rw-rw-rw-   0        0        0    33528 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/drorchestrationoperations.py
--rw-rw-rw-   0        0        0    20998 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/failovergroups.py
--rw-rw-rw-   0        0        0    29317 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/replication_groups.py
--rw-rw-rw-   0        0        0    12423 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/replication_pairs.py
--rw-rw-rw-   0        0        0    13215 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/drorchestration/replicationmonitor.py
--rw-rw-rw-   0        0        0     8905 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/eventviewer.py
--rw-rw-rw-   0        0        0    25244 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/exception.py
--rw-rw-rw-   0        0        0     9765 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/globalfilter.py
--rw-rw-rw-   0        0        0    19921 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/hac_clusters.py
--rw-rw-rw-   0        0        0    38514 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/identity_management.py
--rw-rw-rw-   0        0        0    19706 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/index_pools.py
--rw-rw-rw-   0        0        0    56990 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/index_server.py
--rw-rw-rw-   0        0        0   131423 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/instance.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.425388 cvpysdk-11.32/cvpysdk/instances/
--rw-rw-rw-   0        0        0      862 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/__init__.py
--rw-rw-rw-   0        0        0     2399 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/aadinstance.py
--rw-rw-rw-   0        0        0     2827 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/bigdataappsinstance.py
--rw-rw-rw-   0        0        0     4702 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cainstance.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.466717 cvpysdk-11.32/cvpysdk/instances/cloudapps/
--rw-rw-rw-   0        0        0      873 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/__init__.py
--rw-rw-rw-   0        0        0    23441 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/amazon_instance.py
--rw-rw-rw-   0        0        0     8534 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_database_instance.py
--rw-rw-rw-   0        0        0    32465 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_storage_instance.py
--rw-rw-rw-   0        0        0     6414 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/dynamics365_instance.py
--rw-rw-rw-   0        0        0    17755 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/google_instance.py
--rw-rw-rw-   0        0        0    33100 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/salesforce_instance.py
--rw-rw-rw-   0        0        0     5195 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/spanner_instance.py
--rw-rw-rw-   0        0        0    13394 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/cloudapps/teams_instance.py
--rw-rw-rw-   0        0        0    24491 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/db2instance.py
--rw-rw-rw-   0        0        0     4930 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/dbinstance.py
--rw-rw-rw-   0        0        0    18464 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/instances/hanainstance.py
--rw-rw-rw-   0        0        0    15761 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/informixinstance.py
--rw-rw-rw-   0        0        0    16033 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lndbinstance.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.497966 cvpysdk-11.32/cvpysdk/instances/lotusnotes/
--rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/__init__.py
--rw-rw-rw-   0        0        0    15182 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndbinstance.py
--rw-rw-rw-   0        0        0     8851 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndminstance.py
--rw-rw-rw-   0        0        0     9268 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndocinstance.py
--rw-rw-rw-   0        0        0     7983 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/lotusnotes/lninstance.py
--rw-rw-rw-   0        0        0    24121 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/mysqlinstance.py
--rw-rw-rw-   0        0        0    53422 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/oracleinstance.py
--rw-rw-rw-   0        0        0    26338 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/postgresinstance.py
--rw-rw-rw-   0        0        0    18937 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/saporacleinstance.py
--rw-rw-rw-   0        0        0     9192 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/sharepointinstance.py
--rw-rw-rw-   0        0        0     4584 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/splunkinstance.py
--rw-rw-rw-   0        0        0    61965 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/sqlinstance.py
--rw-rw-rw-   0        0        0    43205 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/sybaseinstance.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.669842 cvpysdk-11.32/cvpysdk/instances/virtualserver/
--rw-rw-rw-   0        0        0      862 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/__init__.py
--rw-rw-rw-   0        0        0     5325 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/alibaba_cloud.py
--rw-rw-rw-   0        0        0     5419 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/amazon_web_services.py
--rw-rw-rw-   0        0        0     4316 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/azure.py
--rw-rw-rw-   0        0        0     4810 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_resource_manager.py
--rw-rw-rw-   0        0        0     4861 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_stack.py
--rw-rw-rw-   0        0        0     4883 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/fusioncompute.py
--rw-rw-rw-   0        0        0     3647 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/google_cloud_platform.py
--rw-rw-rw-   0        0        0     4645 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/hyperv.py
--rw-rw-rw-   0        0        0     4430 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/kubernetes.py
--rw-rw-rw-   0        0        0     1177 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/null.py
--rw-rw-rw-   0        0        0     4943 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/nutanix_ahv.py
--rw-rw-rw-   0        0        0     4554 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/openstack.py
--rw-rw-rw-   0        0        0     5320 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud.py
--rw-rw-rw-   0        0        0     4125 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py
--rw-rw-rw-   0        0        0     4225 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/oraclevm.py
--rw-rw-rw-   0        0        0     4333 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/red_hat_virtualization.py
--rw-rw-rw-   0        0        0     4488 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/vcloud_director.py
--rw-rw-rw-   0        0        0     4401 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/vmware.py
--rw-rw-rw-   0        0        0     4371 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/virtualserver/xen.py
--rw-rw-rw-   0        0        0     2007 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/vminstance.py
--rw-rw-rw-   0        0        0    13055 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/instances/vsinstance.py
--rw-rw-rw-   0        0        0     7827 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/internetoptions.py
--rw-rw-rw-   0        0        0   119599 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/job.py
--rw-rw-rw-   0        0        0    33588 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/key_management_server.py
--rw-rw-rw-   0        0        0    13533 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/license.py
--rw-rw-rw-   0        0        0    20426 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/metallic.py
--rw-rw-rw-   0        0        0    27461 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/metricsreport.py
--rw-rw-rw-   0        0        0    28226 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/monitoring.py
--rw-rw-rw-   0        0        0    23387 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/name_change.py
--rw-rw-rw-   0        0        0    34060 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/network.py
--rw-rw-rw-   0        0        0    13795 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/network_throttle.py
--rw-rw-rw-   0        0        0    36142 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/network_topology.py
--rw-rw-rw-   0        0        0    48129 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/operation_window.py
--rw-rw-rw-   0        0        0   138787 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/organization.py
--rw-rw-rw-   0        0        0   106777 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/plan.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.701106 cvpysdk-11.32/cvpysdk/policies/
--rw-rw-rw-   0        0        0      879 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/__init__.py
--rw-rw-rw-   0        0        0    74032 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/configuration_policies.py
--rw-rw-rw-   0        0        0     8072 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/schedule_options.py
--rw-rw-rw-   0        0        0    44091 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policies/schedule_policies.py
--rw-rw-rw-   0        0        0   184554 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/policies/storage_policies.py
--rw-rw-rw-   0        0        0     3033 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/policy.py
--rw-rw-rw-   0        0        0    26335 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/recovery_targets.py
--rw-rw-rw-   0        0        0    11526 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/regions.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.716709 cvpysdk-11.32/cvpysdk/reports/
--rw-rw-rw-   0        0        0      860 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/reports/__init__.py
--rw-rw-rw-   0        0        0    19808 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/reports/report.py
--rw-rw-rw-   0        0        0   108687 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/schedules.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.747964 cvpysdk-11.32/cvpysdk/security/
--rw-rw-rw-   0        0        0      869 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/__init__.py
--rw-rw-rw-   0        0        0    29798 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/role.py
--rw-rw-rw-   0        0        0    16846 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/security/security_association.py
--rw-rw-rw-   0        0        0     8966 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/two_factor_authentication.py
--rw-rw-rw-   0        0        0    42885 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/security/user.py
--rw-rw-rw-   0        0        0    38467 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/security/usergroup.py
--rw-rw-rw-   0        0        0    30539 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/services.py
--rw-rw-rw-   0        0        0   104242 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/storage.py
--rw-rw-rw-   0        0        0    37723 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/storage_pool.py
--rw-rw-rw-   0        0        0   126396 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclient.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.910173 cvpysdk-11.32/cvpysdk/subclients/
--rw-rw-rw-   0        0        0      863 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/__init__.py
--rw-rw-rw-   0        0        0     1952 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/aadsubclient.py
--rw-rw-rw-   0        0        0     4182 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/adsubclient.py
--rw-rw-rw-   0        0        0     4110 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/bigdataappssubclient.py
--rw-rw-rw-   0        0        0    11760 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/casesubclient.py
--rw-rw-rw-   0        0        0     3650 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/casubclient.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.970136 cvpysdk-11.32/cvpysdk/subclients/cloudapps/
--rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/__init__.py
--rw-rw-rw-   0        0        0     7660 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_database_subclient.py
--rw-rw-rw-   0        0        0    15228 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py
--rw-rw-rw-   0        0        0    42053 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/dynamics365_subclient.py
--rw-rw-rw-   0        0        0    29846 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/google_subclient.py
--rw-rw-rw-   0        0        0    51907 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/salesforce_subclient.py
--rw-rw-rw-   0        0        0     3329 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/spanner_subclient.py
--rw-rw-rw-   0        0        0     3704 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/teams_constants.py
--rw-rw-rw-   0        0        0    47765 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/cloudapps/teams_subclient.py
--rw-rw-rw-   0        0        0    13162 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/db2subclient.py
--rw-rw-rw-   0        0        0     3424 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/dbsubclient.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.001402 cvpysdk-11.32/cvpysdk/subclients/exchange/
--rw-rw-rw-   0        0        0      872 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/__init__.py
--rw-rw-rw-   0        0        0    13470 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py
--rw-rw-rw-   0        0        0    16906 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/exchange_database_subclient.py
--rw-rw-rw-   0        0        0    17764 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/journalmailbox_subclient.py
--rw-rw-rw-   0        0        0    73265 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchange/usermailbox_subclient.py
--rw-rw-rw-   0        0        0    32624 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/exchsubclient.py
--rw-rw-rw-   0        0        0    99425 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/fssubclient.py
--rw-rw-rw-   0        0        0     6083 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/hanasubclient.py
--rw-rw-rw-   0        0        0    15274 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/index_server_subclient.py
--rw-rw-rw-   0        0        0     4834 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/informixsubclient.py
--rw-rw-rw-   0        0        0    16884 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lndbsubclient.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.032812 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/
--rw-rw-rw-   0        0        0      875 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/__init__.py
--rw-rw-rw-   0        0        0    13018 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndbsubclient.py
--rw-rw-rw-   0        0        0     7184 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndmsubclient.py
--rw-rw-rw-   0        0        0     7947 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndocsubclient.py
--rw-rw-rw-   0        0        0     9183 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lnsubclient.py
--rw-rw-rw-   0        0        0    19522 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/mysqlsubclient.py
--rw-rw-rw-   0        0        0    15585 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/nassubclient.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/o365apps_subclient.py
--rw-rw-rw-   0        0        0    20278 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/oraclesubclient.py
--rw-rw-rw-   0        0        0    15895 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/postgressubclient.py
--rw-rw-rw-   0        0        0     5244 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/saporaclesubclient.py
--rw-rw-rw-   0        0        0    56653 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/sharepointsubclient.py
--rw-rw-rw-   0        0        0     4493 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/splunksubclient.py
--rw-rw-rw-   0        0        0    15757 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/sqlsubclient.py
--rw-rw-rw-   0        0        0    21028 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/sybasesubclient.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.157634 cvpysdk-11.32/cvpysdk/subclients/virtualserver/
--rw-rw-rw-   0        0        0      877 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/__init__.py
--rw-rw-rw-   0        0        0     6624 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/alibaba_cloud.py
--rw-rw-rw-   0        0        0    24113 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/amazon_web_services.py
--rw-rw-rw-   0        0        0     7647 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure.py
--rw-rw-rw-   0        0        0    28032 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_resource_manager.py
--rw-rw-rw-   0        0        0     7341 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_stack.py
--rw-rw-rw-   0        0        0    10508 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/fusioncompute.py
--rw-rw-rw-   0        0        0     9892 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/google_cloud_platform.py
--rw-rw-rw-   0        0        0    29479 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/hyperv.py
--rw-rw-rw-   0        0        0    72691 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/kubernetes.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.204508 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/
--rw-rw-rw-   0        0        0      819 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/__init__.py
--rw-rw-rw-   0        0        0     8233 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py
--rw-rw-rw-   0        0        0     8315 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py
--rw-rw-rw-   0        0        0     6974 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py
--rw-rw-rw-   0        0        0     6628 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vmware_live_sync.py
--rw-rw-rw-   0        0        0    30597 2023-06-15 06:19:05.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py
--rw-rw-rw-   0        0        0     1231 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/null.py
--rw-rw-rw-   0        0        0    14517 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/nutanix_ahv.py
--rw-rw-rw-   0        0        0    22011 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/openstack.py
--rw-rw-rw-   0        0        0     5112 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud.py
--rw-rw-rw-   0        0        0    13363 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py
--rw-rw-rw-   0        0        0    11967 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/oraclevm.py
--rw-rw-rw-   0        0        0     1812 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_openshift.py
--rw-rw-rw-   0        0        0    11336 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_virtualization.py
--rw-rw-rw-   0        0        0     2606 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/vcloud_director.py
--rw-rw-rw-   0        0        0    43570 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/vmware.py
--rw-rw-rw-   0        0        0     9081 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/virtualserver/xen.py
--rw-rw-rw-   0        0        0    12599 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/subclients/vminstancesubclient.py
--rw-rw-rw-   0        0        0   129743 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/subclients/vssubclient.py
--rw-rw-rw-   0        0        0     1933 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/system.py
--rw-rw-rw-   0        0        0    72522 2023-06-15 06:19:06.000000 cvpysdk-11.32/cvpysdk/virtualmachinepolicies.py
--rw-rw-rw-   0        0        0    57808 2023-06-15 06:21:20.000000 cvpysdk-11.32/cvpysdk/workflow.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.027746 cvpysdk-11.32/cvpysdk.egg-info/
--rw-rw-rw-   0        0        0     7649 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9443 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 06:48:49.000000 cvpysdk-11.32/cvpysdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 08:11:25.000000 cvpysdk-11.32/cvpysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 08:11:27.220131 cvpysdk-11.32/setup.cfg
--rw-rw-rw-   0        0        0     2301 2023-06-15 06:13:13.000000 cvpysdk-11.32/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:13.258964 cvpysdk-11.32.1/
+-rw-rw-rw-   0        0        0    11531 2023-06-15 06:13:11.000000 cvpysdk-11.32.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       71 2023-06-15 06:13:11.000000 cvpysdk-11.32.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7651 2023-06-16 06:45:13.258964 cvpysdk-11.32.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7082 2023-06-15 08:11:08.000000 cvpysdk-11.32.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:11.829693 cvpysdk-11.32.1/cvpysdk/
+-rw-rw-rw-   0        0        0     1349 2023-06-16 06:43:48.000000 cvpysdk-11.32.1/cvpysdk/__init__.py
+-rw-rw-rw-   0        0        0     6845 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activate.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:11.923433 cvpysdk-11.32.1/cvpysdk/activateapps/
+-rw-rw-rw-   0        0        0      866 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/__init__.py
+-rw-rw-rw-   0        0        0    33458 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/constants.py
+-rw-rw-rw-   0        0        0   136470 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/ediscovery_utils.py
+-rw-rw-rw-   0        0        0   101465 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/entity_manager.py
+-rw-rw-rw-   0        0        0    36915 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/file_storage_optimization.py
+-rw-rw-rw-   0        0        0    45588 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/inventory_manager.py
+-rw-rw-rw-   0        0        0    34226 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/request_manager.py
+-rw-rw-rw-   0        0        0    20756 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activateapps/sensitive_data_governance.py
+-rw-rw-rw-   0        0        0    10277 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/activitycontrol.py
+-rw-rw-rw-   0        0        0    35180 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/agent.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:11.940141 cvpysdk-11.32.1/cvpysdk/agents/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/agents/__init__.py
+-rw-rw-rw-   0        0        0     7472 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/agents/exchange_database_agent.py
+-rw-rw-rw-   0        0        0    47512 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/alert.py
+-rw-rw-rw-   0        0        0    26553 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/array_management.py
+-rw-rw-rw-   0        0        0    10120 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/backup_network_pairs.py
+-rw-rw-rw-   0        0        0    92668 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/backupset.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.017183 cvpysdk-11.32.1/cvpysdk/backupsets/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:04.000000 cvpysdk-11.32.1/cvpysdk/backupsets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.032812 cvpysdk-11.32.1/cvpysdk/backupsets/_virtual_server/
+-rw-rw-rw-   0        0        0      876 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/_virtual_server/__init__.py
+-rw-rw-rw-   0        0        0     2501 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/_virtual_server/kubernetes.py
+-rw-rw-rw-   0        0        0    10718 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/_virtual_server/vmware.py
+-rw-rw-rw-   0        0        0    18407 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/aadbackupset.py
+-rw-rw-rw-   0        0        0     3275 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/adbackupset.py
+-rw-rw-rw-   0        0        0     2695 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/cabackupset.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.048434 cvpysdk-11.32.1/cvpysdk/backupsets/cloudapps/
+-rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/cloudapps/__init__.py
+-rw-rw-rw-   0        0        0     9083 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/cloudapps/salesforce_backupset.py
+-rw-rw-rw-   0        0        0    11908 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/db2backupset.py
+-rw-rw-rw-   0        0        0    72677 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/fsbackupset.py
+-rw-rw-rw-   0        0        0     4615 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/hanabackupset.py
+-rw-rw-rw-   0        0        0     3639 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/nasbackupset.py
+-rw-rw-rw-   0        0        0    11438 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/postgresbackupset.py
+-rw-rw-rw-   0        0        0     3721 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/sharepointbackupset.py
+-rw-rw-rw-   0        0        0    12986 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/backupsets/vsbackupset.py
+-rw-rw-rw-   0        0        0     6246 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/certificates.py
+-rw-rw-rw-   0        0        0   270983 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/client.py
+-rw-rw-rw-   0        0        0    76883 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/clientgroup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.064066 cvpysdk-11.32.1/cvpysdk/clients/
+-rw-rw-rw-   0        0        0      860 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/clients/__init__.py
+-rw-rw-rw-   0        0        0     6864 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/clients/onedrive_client.py
+-rw-rw-rw-   0        0        0     9029 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/clients/vmclient.py
+-rw-rw-rw-   0        0        0   146330 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/commcell.py
+-rw-rw-rw-   0        0        0    24026 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/commcell_migration.py
+-rw-rw-rw-   0        0        0    32624 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/constants.py
+-rw-rw-rw-   0        0        0    16567 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/content_analyzer.py
+-rw-rw-rw-   0        0        0    30092 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/credential_manager.py
+-rw-rw-rw-   0        0        0    17286 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/cvpysdk.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.113607 cvpysdk-11.32.1/cvpysdk/datacube/
+-rw-rw-rw-   0        0        0      879 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/datacube/__init__.py
+-rw-rw-rw-   0        0        0     3294 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/datacube/constants.py
+-rw-rw-rw-   0        0        0     6634 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/datacube/datacube.py
+-rw-rw-rw-   0        0        0    36258 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/datacube/datasource.py
+-rw-rw-rw-   0        0        0    18093 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/datacube/handler.py
+-rw-rw-rw-   0        0        0     1997 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/datacube/sedstype.py
+-rw-rw-rw-   0        0        0    54808 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/deduplication_engines.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.159514 cvpysdk-11.32.1/cvpysdk/deployment/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/deployment/__init__.py
+-rw-rw-rw-   0        0        0    17053 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/deployment/cache_config.py
+-rw-rw-rw-   0        0        0     3650 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/deployment/deploymentconstants.py
+-rw-rw-rw-   0        0        0    19233 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/deployment/download.py
+-rw-rw-rw-   0        0        0    30374 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/deployment/install.py
+-rw-rw-rw-   0        0        0     6862 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/deployment/uninstall.py
+-rw-rw-rw-   0        0        0     6091 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/dev_test_group.py
+-rw-rw-rw-   0        0        0    42515 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/disasterrecovery.py
+-rw-rw-rw-   0        0        0    23493 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/domains.py
+-rw-rw-rw-   0        0        0    51805 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/download_center.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.206389 cvpysdk-11.32.1/cvpysdk/drorchestration/
+-rw-rw-rw-   0        0        0      882 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/__init__.py
+-rw-rw-rw-   0        0        0    48119 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/blr_pairs.py
+-rw-rw-rw-   0        0        0     3808 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/dr_orchestration_job_phase.py
+-rw-rw-rw-   0        0        0     7099 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/drjob.py
+-rw-rw-rw-   0        0        0    33528 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/drorchestrationoperations.py
+-rw-rw-rw-   0        0        0    20998 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/failovergroups.py
+-rw-rw-rw-   0        0        0    29317 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/replication_groups.py
+-rw-rw-rw-   0        0        0    12423 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/replication_pairs.py
+-rw-rw-rw-   0        0        0    13215 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/drorchestration/replicationmonitor.py
+-rw-rw-rw-   0        0        0     8905 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/eventviewer.py
+-rw-rw-rw-   0        0        0    25244 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/exception.py
+-rw-rw-rw-   0        0        0     9765 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/globalfilter.py
+-rw-rw-rw-   0        0        0    19921 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/hac_clusters.py
+-rw-rw-rw-   0        0        0    38514 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/identity_management.py
+-rw-rw-rw-   0        0        0    19706 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/index_pools.py
+-rw-rw-rw-   0        0        0    56990 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/index_server.py
+-rw-rw-rw-   0        0        0   131423 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/instance.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.331469 cvpysdk-11.32.1/cvpysdk/instances/
+-rw-rw-rw-   0        0        0      862 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/__init__.py
+-rw-rw-rw-   0        0        0     2399 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/aadinstance.py
+-rw-rw-rw-   0        0        0     2827 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/bigdataappsinstance.py
+-rw-rw-rw-   0        0        0     4702 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cainstance.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.425145 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/
+-rw-rw-rw-   0        0        0      873 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/__init__.py
+-rw-rw-rw-   0        0        0    23441 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/amazon_instance.py
+-rw-rw-rw-   0        0        0     8534 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/cloud_database_instance.py
+-rw-rw-rw-   0        0        0    32465 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/cloud_storage_instance.py
+-rw-rw-rw-   0        0        0     6414 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/dynamics365_instance.py
+-rw-rw-rw-   0        0        0    17755 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/google_instance.py
+-rw-rw-rw-   0        0        0    33100 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/salesforce_instance.py
+-rw-rw-rw-   0        0        0     5195 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/spanner_instance.py
+-rw-rw-rw-   0        0        0    13394 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/cloudapps/teams_instance.py
+-rw-rw-rw-   0        0        0    24491 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/db2instance.py
+-rw-rw-rw-   0        0        0     4930 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/dbinstance.py
+-rw-rw-rw-   0        0        0    18883 2023-06-16 06:42:48.000000 cvpysdk-11.32.1/cvpysdk/instances/hanainstance.py
+-rw-rw-rw-   0        0        0    15761 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/informixinstance.py
+-rw-rw-rw-   0        0        0    16033 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/lndbinstance.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.458824 cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/
+-rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/__init__.py
+-rw-rw-rw-   0        0        0    15182 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lndbinstance.py
+-rw-rw-rw-   0        0        0     8851 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lndminstance.py
+-rw-rw-rw-   0        0        0     9268 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lndocinstance.py
+-rw-rw-rw-   0        0        0     7983 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lninstance.py
+-rw-rw-rw-   0        0        0    24121 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/mysqlinstance.py
+-rw-rw-rw-   0        0        0    53422 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/oracleinstance.py
+-rw-rw-rw-   0        0        0    26338 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/postgresinstance.py
+-rw-rw-rw-   0        0        0    18937 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/saporacleinstance.py
+-rw-rw-rw-   0        0        0     9192 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/sharepointinstance.py
+-rw-rw-rw-   0        0        0     4584 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/splunkinstance.py
+-rw-rw-rw-   0        0        0    61965 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/sqlinstance.py
+-rw-rw-rw-   0        0        0    43205 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/sybaseinstance.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.565765 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/
+-rw-rw-rw-   0        0        0      862 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/__init__.py
+-rw-rw-rw-   0        0        0     5325 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/alibaba_cloud.py
+-rw-rw-rw-   0        0        0     5419 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/amazon_web_services.py
+-rw-rw-rw-   0        0        0     4316 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/azure.py
+-rw-rw-rw-   0        0        0     4810 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/azure_resource_manager.py
+-rw-rw-rw-   0        0        0     4861 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/azure_stack.py
+-rw-rw-rw-   0        0        0     4883 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/fusioncompute.py
+-rw-rw-rw-   0        0        0     3647 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/google_cloud_platform.py
+-rw-rw-rw-   0        0        0     4645 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/hyperv.py
+-rw-rw-rw-   0        0        0     4430 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/kubernetes.py
+-rw-rw-rw-   0        0        0     1177 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/null.py
+-rw-rw-rw-   0        0        0     4943 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/nutanix_ahv.py
+-rw-rw-rw-   0        0        0     4554 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/openstack.py
+-rw-rw-rw-   0        0        0     5320 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/oracle_cloud.py
+-rw-rw-rw-   0        0        0     4125 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py
+-rw-rw-rw-   0        0        0     4225 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/oraclevm.py
+-rw-rw-rw-   0        0        0     4333 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/red_hat_virtualization.py
+-rw-rw-rw-   0        0        0     4488 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/vcloud_director.py
+-rw-rw-rw-   0        0        0     4401 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/vmware.py
+-rw-rw-rw-   0        0        0     4371 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/virtualserver/xen.py
+-rw-rw-rw-   0        0        0     2007 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/vminstance.py
+-rw-rw-rw-   0        0        0    13055 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/instances/vsinstance.py
+-rw-rw-rw-   0        0        0     7827 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/internetoptions.py
+-rw-rw-rw-   0        0        0   119599 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/job.py
+-rw-rw-rw-   0        0        0    33588 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/key_management_server.py
+-rw-rw-rw-   0        0        0    13533 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/license.py
+-rw-rw-rw-   0        0        0    20426 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/metallic.py
+-rw-rw-rw-   0        0        0    27461 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/metricsreport.py
+-rw-rw-rw-   0        0        0    28226 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/monitoring.py
+-rw-rw-rw-   0        0        0    23387 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/name_change.py
+-rw-rw-rw-   0        0        0    34060 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/network.py
+-rw-rw-rw-   0        0        0    13795 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/network_throttle.py
+-rw-rw-rw-   0        0        0    36142 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/network_topology.py
+-rw-rw-rw-   0        0        0    48129 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/operation_window.py
+-rw-rw-rw-   0        0        0   138787 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/organization.py
+-rw-rw-rw-   0        0        0   106777 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/plan.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.617398 cvpysdk-11.32.1/cvpysdk/policies/
+-rw-rw-rw-   0        0        0      879 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/policies/__init__.py
+-rw-rw-rw-   0        0        0    74032 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/policies/configuration_policies.py
+-rw-rw-rw-   0        0        0     8072 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/policies/schedule_options.py
+-rw-rw-rw-   0        0        0    44091 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/policies/schedule_policies.py
+-rw-rw-rw-   0        0        0   184554 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/policies/storage_policies.py
+-rw-rw-rw-   0        0        0     3033 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/policy.py
+-rw-rw-rw-   0        0        0    26335 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/recovery_targets.py
+-rw-rw-rw-   0        0        0    11526 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/regions.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.631396 cvpysdk-11.32.1/cvpysdk/reports/
+-rw-rw-rw-   0        0        0      860 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/reports/__init__.py
+-rw-rw-rw-   0        0        0    19808 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/reports/report.py
+-rw-rw-rw-   0        0        0   108687 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/schedules.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.662898 cvpysdk-11.32.1/cvpysdk/security/
+-rw-rw-rw-   0        0        0      869 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/security/__init__.py
+-rw-rw-rw-   0        0        0    29798 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/security/role.py
+-rw-rw-rw-   0        0        0    16846 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/security/security_association.py
+-rw-rw-rw-   0        0        0     8966 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/security/two_factor_authentication.py
+-rw-rw-rw-   0        0        0    42885 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/security/user.py
+-rw-rw-rw-   0        0        0    38467 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/security/usergroup.py
+-rw-rw-rw-   0        0        0    30539 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/services.py
+-rw-rw-rw-   0        0        0   104242 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/storage.py
+-rw-rw-rw-   0        0        0    37723 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/storage_pool.py
+-rw-rw-rw-   0        0        0   126396 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/subclient.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.867114 cvpysdk-11.32.1/cvpysdk/subclients/
+-rw-rw-rw-   0        0        0      863 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/__init__.py
+-rw-rw-rw-   0        0        0     1952 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/aadsubclient.py
+-rw-rw-rw-   0        0        0     4182 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/adsubclient.py
+-rw-rw-rw-   0        0        0     4110 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/bigdataappssubclient.py
+-rw-rw-rw-   0        0        0    11760 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/casesubclient.py
+-rw-rw-rw-   0        0        0     3650 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/casubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.959774 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/
+-rw-rw-rw-   0        0        0      874 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/__init__.py
+-rw-rw-rw-   0        0        0     7660 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/cloud_database_subclient.py
+-rw-rw-rw-   0        0        0    15228 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py
+-rw-rw-rw-   0        0        0    42053 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/dynamics365_subclient.py
+-rw-rw-rw-   0        0        0    29846 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/google_subclient.py
+-rw-rw-rw-   0        0        0    51907 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/salesforce_subclient.py
+-rw-rw-rw-   0        0        0     3329 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/spanner_subclient.py
+-rw-rw-rw-   0        0        0     3704 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/teams_constants.py
+-rw-rw-rw-   0        0        0    47765 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/teams_subclient.py
+-rw-rw-rw-   0        0        0    13162 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/db2subclient.py
+-rw-rw-rw-   0        0        0     3424 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/dbsubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:12.991027 cvpysdk-11.32.1/cvpysdk/subclients/exchange/
+-rw-rw-rw-   0        0        0      872 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/exchange/__init__.py
+-rw-rw-rw-   0        0        0    13470 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py
+-rw-rw-rw-   0        0        0    16906 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/exchange/exchange_database_subclient.py
+-rw-rw-rw-   0        0        0    17764 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/exchange/journalmailbox_subclient.py
+-rw-rw-rw-   0        0        0    73265 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/exchange/usermailbox_subclient.py
+-rw-rw-rw-   0        0        0    32624 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/exchsubclient.py
+-rw-rw-rw-   0        0        0    99425 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/fssubclient.py
+-rw-rw-rw-   0        0        0     6083 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/hanasubclient.py
+-rw-rw-rw-   0        0        0    15274 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/subclients/index_server_subclient.py
+-rw-rw-rw-   0        0        0     4834 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/informixsubclient.py
+-rw-rw-rw-   0        0        0    16884 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/lndbsubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:13.037903 cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/
+-rw-rw-rw-   0        0        0      875 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/__init__.py
+-rw-rw-rw-   0        0        0    13018 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lndbsubclient.py
+-rw-rw-rw-   0        0        0     7184 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lndmsubclient.py
+-rw-rw-rw-   0        0        0     7947 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lndocsubclient.py
+-rw-rw-rw-   0        0        0     9183 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lnsubclient.py
+-rw-rw-rw-   0        0        0    19522 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/mysqlsubclient.py
+-rw-rw-rw-   0        0        0    15585 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/nassubclient.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/o365apps_subclient.py
+-rw-rw-rw-   0        0        0    20278 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/oraclesubclient.py
+-rw-rw-rw-   0        0        0    15895 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/postgressubclient.py
+-rw-rw-rw-   0        0        0     5244 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/saporaclesubclient.py
+-rw-rw-rw-   0        0        0    56653 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/sharepointsubclient.py
+-rw-rw-rw-   0        0        0     4493 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/splunksubclient.py
+-rw-rw-rw-   0        0        0    15757 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/sqlsubclient.py
+-rw-rw-rw-   0        0        0    21028 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/sybasesubclient.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:13.196462 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/
+-rw-rw-rw-   0        0        0      877 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/__init__.py
+-rw-rw-rw-   0        0        0     6624 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/alibaba_cloud.py
+-rw-rw-rw-   0        0        0    24113 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/amazon_web_services.py
+-rw-rw-rw-   0        0        0     7647 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/azure.py
+-rw-rw-rw-   0        0        0    28032 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/azure_resource_manager.py
+-rw-rw-rw-   0        0        0     7341 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/azure_stack.py
+-rw-rw-rw-   0        0        0    10508 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/fusioncompute.py
+-rw-rw-rw-   0        0        0     9892 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/google_cloud_platform.py
+-rw-rw-rw-   0        0        0    29479 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/hyperv.py
+-rw-rw-rw-   0        0        0    72691 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/kubernetes.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:13.243345 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/
+-rw-rw-rw-   0        0        0      819 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/__init__.py
+-rw-rw-rw-   0        0        0     8233 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py
+-rw-rw-rw-   0        0        0     8315 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py
+-rw-rw-rw-   0        0        0     6974 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py
+-rw-rw-rw-   0        0        0     6628 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/vmware_live_sync.py
+-rw-rw-rw-   0        0        0    30597 2023-06-15 06:19:05.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py
+-rw-rw-rw-   0        0        0     1231 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/null.py
+-rw-rw-rw-   0        0        0    14517 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/nutanix_ahv.py
+-rw-rw-rw-   0        0        0    22011 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/openstack.py
+-rw-rw-rw-   0        0        0     5112 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/oracle_cloud.py
+-rw-rw-rw-   0        0        0    13363 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py
+-rw-rw-rw-   0        0        0    11967 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/oraclevm.py
+-rw-rw-rw-   0        0        0     1812 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/red_hat_openshift.py
+-rw-rw-rw-   0        0        0    11336 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/red_hat_virtualization.py
+-rw-rw-rw-   0        0        0     2606 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/vcloud_director.py
+-rw-rw-rw-   0        0        0    43570 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/vmware.py
+-rw-rw-rw-   0        0        0     9081 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/xen.py
+-rw-rw-rw-   0        0        0    12599 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/subclients/vminstancesubclient.py
+-rw-rw-rw-   0        0        0   129743 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/subclients/vssubclient.py
+-rw-rw-rw-   0        0        0     1933 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/system.py
+-rw-rw-rw-   0        0        0    72522 2023-06-15 06:19:06.000000 cvpysdk-11.32.1/cvpysdk/virtualmachinepolicies.py
+-rw-rw-rw-   0        0        0    57808 2023-06-15 06:21:20.000000 cvpysdk-11.32.1/cvpysdk/workflow.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:45:11.860934 cvpysdk-11.32.1/cvpysdk.egg-info/
+-rw-rw-rw-   0        0        0     7651 2023-06-16 06:45:11.000000 cvpysdk-11.32.1/cvpysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9443 2023-06-16 06:45:11.000000 cvpysdk-11.32.1/cvpysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:45:11.000000 cvpysdk-11.32.1/cvpysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 06:48:49.000000 cvpysdk-11.32.1/cvpysdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-16 06:45:11.000000 cvpysdk-11.32.1/cvpysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 06:45:11.000000 cvpysdk-11.32.1/cvpysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:45:13.258964 cvpysdk-11.32.1/setup.cfg
+-rw-rw-rw-   0        0        0     2301 2023-06-15 06:13:13.000000 cvpysdk-11.32.1/setup.py
```

### Comparing `cvpysdk-11.32/LICENSE.txt` & `cvpysdk-11.32.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/PKG-INFO` & `cvpysdk-11.32.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvpysdk
-Version: 11.32
+Version: 11.32.1
 Summary: Commvault SDK for Python
 Home-page: https://github.com/Commvault/cvpysdk
 Author: Commvault Systems Inc.
 Author-email: Dev-PythonSDK@commvault.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Commvault/cvpysdk/issues
 Project-URL: Documentation, https://commvault.github.io/cvpysdk/
```

### Comparing `cvpysdk-11.32/README.rst` & `cvpysdk-11.32.1/README.rst`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/__init__.py` & `cvpysdk-11.32.1/cvpysdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     -   **xmltodict**
 
 And Commvault Software v11 SP7 or later release with WebConsole installed
 
 """
 
 __author__ = 'Commvault Systems Inc.'
-__version__ = '11.32'
+__version__ = '11.32.1'
```

### Comparing `cvpysdk-11.32/cvpysdk/activate.py` & `cvpysdk-11.32.1/cvpysdk/activate.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/__init__.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/constants.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/constants.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/ediscovery_utils.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/ediscovery_utils.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/entity_manager.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/entity_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/file_storage_optimization.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/file_storage_optimization.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/inventory_manager.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/inventory_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/request_manager.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/request_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activateapps/sensitive_data_governance.py` & `cvpysdk-11.32.1/cvpysdk/activateapps/sensitive_data_governance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/activitycontrol.py` & `cvpysdk-11.32.1/cvpysdk/activitycontrol.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/agent.py` & `cvpysdk-11.32.1/cvpysdk/agent.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/agents/__init__.py` & `cvpysdk-11.32.1/cvpysdk/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/agents/exchange_database_agent.py` & `cvpysdk-11.32.1/cvpysdk/agents/exchange_database_agent.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/alert.py` & `cvpysdk-11.32.1/cvpysdk/alert.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/array_management.py` & `cvpysdk-11.32.1/cvpysdk/array_management.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backup_network_pairs.py` & `cvpysdk-11.32.1/cvpysdk/backup_network_pairs.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupset.py` & `cvpysdk-11.32.1/cvpysdk/backupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/__init__.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/__init__.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/_virtual_server/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/kubernetes.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/_virtual_server/kubernetes.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/_virtual_server/vmware.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/_virtual_server/vmware.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/aadbackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/aadbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/adbackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/adbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/cabackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/cabackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/cloudapps/__init__.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/cloudapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/cloudapps/salesforce_backupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/cloudapps/salesforce_backupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/db2backupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/db2backupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/fsbackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/fsbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/hanabackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/hanabackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/nasbackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/nasbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/postgresbackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/postgresbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/sharepointbackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/sharepointbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/backupsets/vsbackupset.py` & `cvpysdk-11.32.1/cvpysdk/backupsets/vsbackupset.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/certificates.py` & `cvpysdk-11.32.1/cvpysdk/certificates.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/client.py` & `cvpysdk-11.32.1/cvpysdk/client.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/clientgroup.py` & `cvpysdk-11.32.1/cvpysdk/clientgroup.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/clients/__init__.py` & `cvpysdk-11.32.1/cvpysdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/clients/onedrive_client.py` & `cvpysdk-11.32.1/cvpysdk/clients/onedrive_client.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/clients/vmclient.py` & `cvpysdk-11.32.1/cvpysdk/clients/vmclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/commcell.py` & `cvpysdk-11.32.1/cvpysdk/commcell.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/commcell_migration.py` & `cvpysdk-11.32.1/cvpysdk/commcell_migration.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/constants.py` & `cvpysdk-11.32.1/cvpysdk/constants.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/content_analyzer.py` & `cvpysdk-11.32.1/cvpysdk/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/credential_manager.py` & `cvpysdk-11.32.1/cvpysdk/credential_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/cvpysdk.py` & `cvpysdk-11.32.1/cvpysdk/cvpysdk.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/datacube/__init__.py` & `cvpysdk-11.32.1/cvpysdk/datacube/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/datacube/constants.py` & `cvpysdk-11.32.1/cvpysdk/datacube/constants.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/datacube/datacube.py` & `cvpysdk-11.32.1/cvpysdk/datacube/datacube.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/datacube/datasource.py` & `cvpysdk-11.32.1/cvpysdk/datacube/datasource.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/datacube/handler.py` & `cvpysdk-11.32.1/cvpysdk/datacube/handler.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/datacube/sedstype.py` & `cvpysdk-11.32.1/cvpysdk/datacube/sedstype.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/deduplication_engines.py` & `cvpysdk-11.32.1/cvpysdk/deduplication_engines.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/deployment/__init__.py` & `cvpysdk-11.32.1/cvpysdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/deployment/cache_config.py` & `cvpysdk-11.32.1/cvpysdk/deployment/cache_config.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/deployment/deploymentconstants.py` & `cvpysdk-11.32.1/cvpysdk/deployment/deploymentconstants.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/deployment/download.py` & `cvpysdk-11.32.1/cvpysdk/deployment/download.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/deployment/install.py` & `cvpysdk-11.32.1/cvpysdk/deployment/install.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/deployment/uninstall.py` & `cvpysdk-11.32.1/cvpysdk/deployment/uninstall.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/dev_test_group.py` & `cvpysdk-11.32.1/cvpysdk/dev_test_group.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/disasterrecovery.py` & `cvpysdk-11.32.1/cvpysdk/disasterrecovery.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/domains.py` & `cvpysdk-11.32.1/cvpysdk/domains.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/download_center.py` & `cvpysdk-11.32.1/cvpysdk/download_center.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/__init__.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/blr_pairs.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/blr_pairs.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/dr_orchestration_job_phase.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/dr_orchestration_job_phase.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/drjob.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/drjob.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/drorchestrationoperations.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/drorchestrationoperations.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/failovergroups.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/failovergroups.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/replication_groups.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/replication_groups.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/replication_pairs.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/replication_pairs.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/drorchestration/replicationmonitor.py` & `cvpysdk-11.32.1/cvpysdk/drorchestration/replicationmonitor.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/eventviewer.py` & `cvpysdk-11.32.1/cvpysdk/eventviewer.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/exception.py` & `cvpysdk-11.32.1/cvpysdk/exception.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/globalfilter.py` & `cvpysdk-11.32.1/cvpysdk/globalfilter.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/hac_clusters.py` & `cvpysdk-11.32.1/cvpysdk/hac_clusters.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/identity_management.py` & `cvpysdk-11.32.1/cvpysdk/identity_management.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/index_pools.py` & `cvpysdk-11.32.1/cvpysdk/index_pools.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/index_server.py` & `cvpysdk-11.32.1/cvpysdk/index_server.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instance.py` & `cvpysdk-11.32.1/cvpysdk/instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/__init__.py` & `cvpysdk-11.32.1/cvpysdk/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/aadinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/aadinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/bigdataappsinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/bigdataappsinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cainstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cainstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/__init__.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/amazon_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/amazon_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_database_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/cloud_database_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/cloud_storage_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/cloud_storage_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/dynamics365_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/dynamics365_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/google_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/google_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/salesforce_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/salesforce_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/spanner_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/spanner_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/cloudapps/teams_instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/cloudapps/teams_instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/db2instance.py` & `cvpysdk-11.32.1/cvpysdk/instances/db2instance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/dbinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/dbinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/hanainstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/hanainstance.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,16 @@
             backup_prefix=None,
             point_in_time=None,
             initialize_log_area=False,
             use_hardware_revert=False,
             clone_env=False,
             check_access=False,
             destination_instance_dir=None,
-            ignore_delta_backups=False):
+            ignore_delta_backups=False,
+            no_of_streams=2):
         """Returns the JSON request to pass to the API as per the options selected by the user.
 
             Args:
                 destination_client          (str)   --  HANA client to restore the database at
 
                 destination_instance        (str)   --  destination instance to restore the db at
 
@@ -184,14 +185,18 @@
                                                             restore or cross machine restores
                     default: None
 
                 ignore_delta_backups        (bool)  --  whether to ignore delta backups during
                                                             restore or not
                     default: True
 
+                no_of_streams               (int)   --  number of streams to be used for restore
+
+                    default: 2
+
             Returns:
                 dict    -   JSON request to pass to the API
 
         """
         self._get_hana_restore_options(destination_client)
 
         if destination_instance is None:
@@ -265,15 +270,16 @@
                                 "destinationInstance": {
                                     "clientName": destination_client,
                                     "appName": self._agent_object.agent_name,
                                     "instanceName": destination_instance
                                 },
                                 "destClient": {
                                     "clientName": destination_hana_client
-                                }
+                                },
+                                "noOfStreams": no_of_streams
                             },
                             "browseOption": {
                                 "backupset": {
                                     "clientName": self._agent_object._client_object.client_name
                                 }
                             }
                         }
@@ -384,15 +390,16 @@
             backup_prefix=None,
             point_in_time=None,
             initialize_log_area=False,
             use_hardware_revert=False,
             clone_env=False,
             check_access=True,
             destination_instance_dir=None,
-            ignore_delta_backups=True):
+            ignore_delta_backups=True,
+            no_of_streams=2):
         """Restores the databases specified in the input paths list.
 
             Args:
                 pseudo_client               (str)   --  HANA client to restore the database at
 
                 instance                    (str)   --  destination instance to restore the db at
 
@@ -427,14 +434,18 @@
                                                             restore or cross machine restores
                     default: None
 
                 ignore_delta_backups        (bool)  --  whether to ignore delta backups during
                                                             restore or not
                     default: True
 
+                no_of_streams               (int)   --  number of streams to be used for restore
+
+                    default: 2
+
             Returns:
                 object  -   instance of the Job class for this restore job
 
             Raises:
                 SDKException:
                     if instance is not a string or object
 
@@ -453,11 +464,12 @@
             backup_prefix,
             point_in_time,
             initialize_log_area,
             use_hardware_revert,
             clone_env,
             check_access,
             destination_instance_dir,
-            ignore_delta_backups
+            ignore_delta_backups,
+            no_of_streams
         )
 
         return self._process_restore_response(request_json)
```

### Comparing `cvpysdk-11.32/cvpysdk/instances/informixinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/informixinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/lndbinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/lndbinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/lotusnotes/__init__.py` & `cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndbinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lndbinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndminstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lndminstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lndocinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lndocinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/lotusnotes/lninstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/lotusnotes/lninstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/mysqlinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/mysqlinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/oracleinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/oracleinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/postgresinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/postgresinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/saporacleinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/saporacleinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/sharepointinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/sharepointinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/splunkinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/splunkinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/sqlinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/sqlinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/sybaseinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/sybaseinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/__init__.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/alibaba_cloud.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/alibaba_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/amazon_web_services.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/azure.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/azure.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_resource_manager.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/azure_resource_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/azure_stack.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/azure_stack.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/fusioncompute.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/fusioncompute.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/google_cloud_platform.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/google_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/hyperv.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/hyperv.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/kubernetes.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/kubernetes.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/null.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/null.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/nutanix_ahv.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/nutanix_ahv.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/openstack.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/openstack.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/oracle_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/oracle_cloud_infrastructure.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/oraclevm.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/oraclevm.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/red_hat_virtualization.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/red_hat_virtualization.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/vcloud_director.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/vcloud_director.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/vmware.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/vmware.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/virtualserver/xen.py` & `cvpysdk-11.32.1/cvpysdk/instances/virtualserver/xen.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/vminstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/vminstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/instances/vsinstance.py` & `cvpysdk-11.32.1/cvpysdk/instances/vsinstance.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/internetoptions.py` & `cvpysdk-11.32.1/cvpysdk/internetoptions.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/job.py` & `cvpysdk-11.32.1/cvpysdk/job.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/key_management_server.py` & `cvpysdk-11.32.1/cvpysdk/key_management_server.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/license.py` & `cvpysdk-11.32.1/cvpysdk/license.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/metallic.py` & `cvpysdk-11.32.1/cvpysdk/metallic.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/metricsreport.py` & `cvpysdk-11.32.1/cvpysdk/metricsreport.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/monitoring.py` & `cvpysdk-11.32.1/cvpysdk/monitoring.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/name_change.py` & `cvpysdk-11.32.1/cvpysdk/name_change.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/network.py` & `cvpysdk-11.32.1/cvpysdk/network.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/network_throttle.py` & `cvpysdk-11.32.1/cvpysdk/network_throttle.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/network_topology.py` & `cvpysdk-11.32.1/cvpysdk/network_topology.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/operation_window.py` & `cvpysdk-11.32.1/cvpysdk/operation_window.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/organization.py` & `cvpysdk-11.32.1/cvpysdk/organization.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/plan.py` & `cvpysdk-11.32.1/cvpysdk/plan.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/policies/__init__.py` & `cvpysdk-11.32.1/cvpysdk/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/policies/configuration_policies.py` & `cvpysdk-11.32.1/cvpysdk/policies/configuration_policies.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/policies/schedule_options.py` & `cvpysdk-11.32.1/cvpysdk/policies/schedule_options.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/policies/schedule_policies.py` & `cvpysdk-11.32.1/cvpysdk/policies/schedule_policies.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/policies/storage_policies.py` & `cvpysdk-11.32.1/cvpysdk/policies/storage_policies.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/policy.py` & `cvpysdk-11.32.1/cvpysdk/policy.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/recovery_targets.py` & `cvpysdk-11.32.1/cvpysdk/recovery_targets.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/regions.py` & `cvpysdk-11.32.1/cvpysdk/regions.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/reports/__init__.py` & `cvpysdk-11.32.1/cvpysdk/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/reports/report.py` & `cvpysdk-11.32.1/cvpysdk/reports/report.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/schedules.py` & `cvpysdk-11.32.1/cvpysdk/schedules.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/security/__init__.py` & `cvpysdk-11.32.1/cvpysdk/security/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/security/role.py` & `cvpysdk-11.32.1/cvpysdk/security/role.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/security/security_association.py` & `cvpysdk-11.32.1/cvpysdk/security/security_association.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/security/two_factor_authentication.py` & `cvpysdk-11.32.1/cvpysdk/security/two_factor_authentication.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/security/user.py` & `cvpysdk-11.32.1/cvpysdk/security/user.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/security/usergroup.py` & `cvpysdk-11.32.1/cvpysdk/security/usergroup.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/services.py` & `cvpysdk-11.32.1/cvpysdk/services.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/storage.py` & `cvpysdk-11.32.1/cvpysdk/storage.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/storage_pool.py` & `cvpysdk-11.32.1/cvpysdk/storage_pool.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/__init__.py` & `cvpysdk-11.32.1/cvpysdk/subclients/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/aadsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/aadsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/adsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/adsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/bigdataappssubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/bigdataappssubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/casesubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/casesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/casubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/casubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/__init__.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_database_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/cloud_database_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/cloud_storage_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/dynamics365_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/dynamics365_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/google_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/google_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/salesforce_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/salesforce_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/spanner_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/spanner_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/teams_constants.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/teams_constants.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/cloudapps/teams_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/cloudapps/teams_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/db2subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/db2subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/dbsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/dbsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/exchange/__init__.py` & `cvpysdk-11.32.1/cvpysdk/subclients/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/exchange/contentstoremailbox_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/exchange/exchange_database_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/exchange/exchange_database_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/exchange/journalmailbox_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/exchange/journalmailbox_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/exchange/usermailbox_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/exchange/usermailbox_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/exchsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/exchsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/fssubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/fssubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/hanasubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/hanasubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/index_server_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/index_server_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/informixsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/informixsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/lndbsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/lndbsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/__init__.py` & `cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndbsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lndbsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndmsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lndmsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lndocsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lndocsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/lotusnotes/lnsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/lotusnotes/lnsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/mysqlsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/mysqlsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/nassubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/nassubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/o365apps_subclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/o365apps_subclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/oraclesubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/oraclesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/postgressubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/postgressubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/saporaclesubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/saporaclesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/sharepointsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/sharepointsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/splunksubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/splunksubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/sqlsubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/sqlsubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/sybasesubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/sybasesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/__init__.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/alibaba_cloud.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/alibaba_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/amazon_web_services.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/azure.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_resource_manager.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/azure_resource_manager.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/azure_stack.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/azure_stack.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/fusioncompute.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/fusioncompute.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/google_cloud_platform.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/google_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/hyperv.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/hyperv.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/kubernetes.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/kubernetes.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/__init__.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/__init__.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/amazon_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/azure_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/hyperv_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vmware_live_sync.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/vmware_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/livesync/vsa_live_sync.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/null.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/null.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/nutanix_ahv.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/nutanix_ahv.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/openstack.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/openstack.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/oracle_cloud.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/oracle_cloud_infrastructure.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/oraclevm.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/oraclevm.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_openshift.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/red_hat_openshift.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/red_hat_virtualization.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/red_hat_virtualization.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/vcloud_director.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/vcloud_director.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/vmware.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/vmware.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/virtualserver/xen.py` & `cvpysdk-11.32.1/cvpysdk/subclients/virtualserver/xen.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/vminstancesubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/vminstancesubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/subclients/vssubclient.py` & `cvpysdk-11.32.1/cvpysdk/subclients/vssubclient.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/system.py` & `cvpysdk-11.32.1/cvpysdk/system.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/virtualmachinepolicies.py` & `cvpysdk-11.32.1/cvpysdk/virtualmachinepolicies.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk/workflow.py` & `cvpysdk-11.32.1/cvpysdk/workflow.py`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/cvpysdk.egg-info/PKG-INFO` & `cvpysdk-11.32.1/cvpysdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvpysdk
-Version: 11.32
+Version: 11.32.1
 Summary: Commvault SDK for Python
 Home-page: https://github.com/Commvault/cvpysdk
 Author: Commvault Systems Inc.
 Author-email: Dev-PythonSDK@commvault.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Commvault/cvpysdk/issues
 Project-URL: Documentation, https://commvault.github.io/cvpysdk/
```

### Comparing `cvpysdk-11.32/cvpysdk.egg-info/SOURCES.txt` & `cvpysdk-11.32.1/cvpysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvpysdk-11.32/setup.py` & `cvpysdk-11.32.1/setup.py`

 * *Files identical despite different names*

