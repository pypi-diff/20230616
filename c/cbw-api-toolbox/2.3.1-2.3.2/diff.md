# Comparing `tmp/cbw-api-toolbox-2.3.1.tar.gz` & `tmp/cbw-api-toolbox-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cbw-api-toolbox-2.3.1.tar", last modified: Thu Dec 22 15:43:59 2022, max compression
+gzip compressed data, was "dist/cbw-api-toolbox-2.3.2.tar", last modified: Fri Jun 16 13:11:48 2023, max compression
```

## Comparing `cbw-api-toolbox-2.3.1.tar` & `cbw-api-toolbox-2.3.2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3525 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3156 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/bin/
--rw-r--r--   0 runner    (1001) docker     (116)     1272 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/bin/cyberwatch-cli
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox/
--rw-r--r--   0 runner    (1001) docker     (116)      371 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      966 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox/__routes__.py
--rw-r--r--   0 runner    (1001) docker     (116)    34940 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox/cbw_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     2055 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox/cbw_auth.py
--rw-r--r--   0 runner    (1001) docker     (116)     3780 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox/cbw_file_xlsx.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3525 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3361 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       89 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       50 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cli/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cli/airgap/
--rw-r--r--   0 runner    (1001) docker     (116)     1365 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/airgap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3919 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/airgap/download_compliance_scripts.py
--rw-r--r--   0 runner    (1001) docker     (116)     4550 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/airgap/download_scripts.py
--rw-r--r--   0 runner    (1001) docker     (116)     1900 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/airgap/upload.py
--rw-r--r--   0 runner    (1001) docker     (116)     2010 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/airgap/upload_compliance.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cli/docker_image/
--rw-r--r--   0 runner    (1001) docker     (116)     1417 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/docker_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1738 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/docker_image/create.py
--rw-r--r--   0 runner    (1001) docker     (116)     1301 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/docker_image/list_images.py
--rw-r--r--   0 runner    (1001) docker     (116)     2363 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/docker_image/scan.py
--rw-r--r--   0 runner    (1001) docker     (116)     5128 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/docker_image/show.py
--rw-r--r--   0 runner    (1001) docker     (116)     1287 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/docker_image/update.py
--rw-r--r--   0 runner    (1001) docker     (116)      567 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/docker_image/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/cli/os/
--rw-r--r--   0 runner    (1001) docker     (116)      802 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      946 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/cli/os/list_os.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1678 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/affect_group_by_hostname.py
--rw-r--r--   0 runner    (1001) docker     (116)     1373 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/affect_group_os.py
--rw-r--r--   0 runner    (1001) docker     (116)     1857 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/affect_repository_to_group.py
--rw-r--r--   0 runner    (1001) docker     (116)      389 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/agent.py
--rw-r--r--   0 runner    (1001) docker     (116)      386 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/agent_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)      363 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/agents.py
--rw-r--r--   0 runner    (1001) docker     (116)      600 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/agents_by_last_communication.py
--rw-r--r--   0 runner    (1001) docker     (116)      459 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/applicative_scan.py
--rw-r--r--   0 runner    (1001) docker     (116)      381 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/applicative_scans.py
--rw-r--r--   0 runner    (1001) docker     (116)      389 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/asset.py
--rw-r--r--   0 runner    (1001) docker     (116)      426 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/asset_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)      362 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/assets.py
--rw-r--r--   0 runner    (1001) docker     (116)     2783 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/clean_discovered_docker.py
--rw-r--r--   0 runner    (1001) docker     (116)     2070 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/cleanup_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (116)     7346 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/cleanup_initialization_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (116)     2335 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/cleanup_lost_com_filters.py
--rw-r--r--   0 runner    (1001) docker     (116)      607 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/create_applicative_scan.py
--rw-r--r--   0 runner    (1001) docker     (116)      706 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/create_host.py
--rw-r--r--   0 runner    (1001) docker     (116)     4394 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/create_multiple_remote_accesses.py
--rw-r--r--   0 runner    (1001) docker     (116)     4891 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/create_remote_by_host.py
--rw-r--r--   0 runner    (1001) docker     (116)      500 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/cve_announcement.py
--rw-r--r--   0 runner    (1001) docker     (116)      483 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/cve_announcements_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     5713 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/cve_published_last_month_export_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (116)      460 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/delete_applicative_scan.py
--rw-r--r--   0 runner    (1001) docker     (116)      436 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/delete_cve_announcement.py
--rw-r--r--   0 runner    (1001) docker     (116)     2829 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/detail_servers.py
--rw-r--r--   0 runner    (1001) docker     (116)      424 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/discoveries.py
--rw-r--r--   0 runner    (1001) docker     (116)      439 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (116)      801 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/docker_image_add.py
--rw-r--r--   0 runner    (1001) docker     (116)      440 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/docker_image_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)      532 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/docker_image_update.py
--rw-r--r--   0 runner    (1001) docker     (116)      373 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/docker_images.py
--rw-r--r--   0 runner    (1001) docker     (116)     2701 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/email_report.py
--rw-r--r--   0 runner    (1001) docker     (116)    11056 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/email_report_filters.py
--rw-r--r--   0 runner    (1001) docker     (116)     4062 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/fetch_daily_cves_to_redmine.py
--rw-r--r--   0 runner    (1001) docker     (116)     3856 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/find_outdated_last_detection.py
--rw-r--r--   0 runner    (1001) docker     (116)     2010 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/get_all_subnets.py
--rw-r--r--   0 runner    (1001) docker     (116)      562 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/group_create.py
--rw-r--r--   0 runner    (1001) docker     (116)      411 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/groups.py
--rw-r--r--   0 runner    (1001) docker     (116)     2506 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/groups_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (116)     2320 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/host_detail_export_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (116)      360 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/hosts.py
--rw-r--r--   0 runner    (1001) docker     (116)     1971 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/ignore_spooler_cves_after_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (116)      788 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/import_file_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (116)      357 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/nodes.py
--rw-r--r--   0 runner    (1001) docker     (116)      355 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/ping.py
--rw-r--r--   0 runner    (1001) docker     (116)      403 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/remote_access.py
--rw-r--r--   0 runner    (1001) docker     (116)     1197 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/remote_access_create.py
--rw-r--r--   0 runner    (1001) docker     (116)      417 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/remote_access_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     1056 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/remote_access_update.py
--rw-r--r--   0 runner    (1001) docker     (116)      381 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/remote_accesses.py
--rw-r--r--   0 runner    (1001) docker     (116)      547 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/remote_accesses_test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (116)      448 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/remote_accesses_to_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (116)      423 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/security_issue.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/security_issue_create.py
--rw-r--r--   0 runner    (1001) docker     (116)      422 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/security_issue_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)      855 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/security_issue_update.py
--rw-r--r--   0 runner    (1001) docker     (116)      381 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/security_issues.py
--rw-r--r--   0 runner    (1001) docker     (116)      393 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/server.py
--rw-r--r--   0 runner    (1001) docker     (116)      704 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/server_affect_ignoring_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1470 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/server_creation_date_to_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/server_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     2300 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/server_to_qradar.py
--rw-r--r--   0 runner    (1001) docker     (116)     1169 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/server_to_splunk.py
--rw-r--r--   0 runner    (1001) docker     (116)      936 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/server_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     1257 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/servers_by_group.py
--rw-r--r--   0 runner    (1001) docker     (116)     2252 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/servers_cves_csv.py
--rw-r--r--   0 runner    (1001) docker     (116)     7510 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/servers_detail_export_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (116)      437 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/stored_credential.py
--rw-r--r--   0 runner    (1001) docker     (116)     1331 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/stored_credential_create.py
--rw-r--r--   0 runner    (1001) docker     (116)      447 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/stored_credential_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     1360 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/stored_credential_update.py
--rw-r--r--   0 runner    (1001) docker     (116)      387 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/stored_credentials.py
--rw-r--r--   0 runner    (1001) docker     (116)      701 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/update_applicative_scan.py
--rw-r--r--   0 runner    (1001) docker     (116)      716 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/update_cve_announcement.py
--rw-r--r--   0 runner    (1001) docker     (116)      556 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/update_server_cve.py
--rw-r--r--   0 runner    (1001) docker     (116)      499 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/users.py
--rw-r--r--   0 runner    (1001) docker     (116)     2319 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/view_dashboard_indicator.py
--rw-r--r--   0 runner    (1001) docker     (116)      951 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/examples/view_server_patch.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      860 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:59.000000 cbw-api-toolbox-2.3.1/spec/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    42337 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/spec/test_cbw_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     3252 2022-12-22 15:43:41.000000 cbw-api-toolbox-2.3.1/spec/test_cbw_files_xlsx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/bin/cyberwatch-cli
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox/__routes__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34940 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox/cbw_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox/cbw_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox/cbw_file_xlsx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cli/airgap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/airgap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/airgap/download_compliance_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/airgap/download_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/airgap/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/airgap/upload_compliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cli/docker_image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/docker_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/docker_image/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/docker_image/list_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/docker_image/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/docker_image/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/docker_image/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/docker_image/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/cli/os/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/cli/os/list_os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/affect_group_by_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/affect_group_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/affect_repository_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/agent_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/agents_by_last_communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/applicative_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/applicative_scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/asset_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/clean_discovered_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/cleanup_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/cleanup_initialization_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/cleanup_lost_com_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/create_applicative_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/create_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/create_multiple_remote_accesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/create_remote_by_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/cve_announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/cve_announcements_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/cve_published_last_month_export_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/delete_applicative_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/delete_cve_announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/detail_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/discoveries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/docker_image_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/docker_image_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/docker_image_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/docker_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/email_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/email_report_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/fetch_daily_cves_to_redmine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/find_outdated_last_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/get_all_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/group_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/groups_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/host_detail_export_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/ignore_spooler_cves_after_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/import_file_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/remote_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/remote_access_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/remote_access_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/remote_access_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/remote_accesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/remote_accesses_test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/remote_accesses_to_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/security_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/security_issue_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/security_issue_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/security_issue_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/security_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/server_affect_ignoring_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/server_creation_date_to_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/server_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/server_to_qradar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/server_to_splunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/server_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/servers_by_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/servers_cves_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/servers_detail_export_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/stored_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/stored_credential_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/stored_credential_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/stored_credential_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/stored_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/update_applicative_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/update_cve_announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/update_server_cve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/view_dashboard_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/examples/view_server_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:48.000000 cbw-api-toolbox-2.3.2/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42337 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/spec/test_cbw_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-16 13:11:39.000000 cbw-api-toolbox-2.3.2/spec/test_cbw_files_xlsx.py
```

### Comparing `cbw-api-toolbox-2.3.1/LICENSE` & `cbw-api-toolbox-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/PKG-INFO` & `cbw-api-toolbox-2.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: cbw-api-toolbox
-Version: 2.3.1
+Version: 2.3.2
 Summary: CyberWatch Api Tools.
 Home-page: https://github.com/Cyberwatch/cyberwatch_api_toolbox
 Author: CyberWatch SAS
 Author-email: support-it+api@cyberwatch.fr
 License: MIT
 Project-URL: Documentation, https://docs.cyberwatch.fr/api/#introduction
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cyberwatch API toolbox
+# \[DEPRECATED\]
+
+## New Api Client
+This module has been deprecated. Please consider using [cyberwatch_api](https://github.com/Cyberwatch/cyberwatch_api).
+
+Please contact Cyberwatch support if you need help to migrate your existing scripts to the new client.
+
+## Cyberwatch API toolbox
 
 A simple interface for your Cyberwatch instance API composed of a python library
 and a command line program.
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-
-- [Cyberwatch API toolbox](#cyberwatch-api-toolbox)
-  - [Installation](#installation)
-    - [Prerequisites](#prerequisites)
-    - [Install the package](#install-the-package)
-    - [Test your installation](#test-your-installation)
-  - [Configuration](#configuration)
-  - [Usage](#usage)
-  - [API Documentation](#api-documentation)
-  - [Command line Documentation](#command-line-documentation)
+- [Installation](#installation)
+  - [Prerequisites](#prerequisites)
+  - [Install the latest package](#install-the-latest-package)
+  - [Install an older package version](#install-an-older-package-version)
+  - [Test your installation](#test-your-installation)
+- [Configuration](#configuration)
+- [Usage](#usage)
+- [API Documentation](#api-documentation)
+- [Command line Documentation](#command-line-documentation)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Installation
 
 ### Prerequisites
 - [ ] [Python 3](https://www.python.org/)
```

### Comparing `cbw-api-toolbox-2.3.1/README.md` & `cbw-api-toolbox-2.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-# Cyberwatch API toolbox
+# \[DEPRECATED\]
+
+## New Api Client
+This module has been deprecated. Please consider using [cyberwatch_api](https://github.com/Cyberwatch/cyberwatch_api).
+
+Please contact Cyberwatch support if you need help to migrate your existing scripts to the new client.
+
+## Cyberwatch API toolbox
 
 A simple interface for your Cyberwatch instance API composed of a python library
 and a command line program.
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-
-- [Cyberwatch API toolbox](#cyberwatch-api-toolbox)
-  - [Installation](#installation)
-    - [Prerequisites](#prerequisites)
-    - [Install the package](#install-the-package)
-    - [Test your installation](#test-your-installation)
-  - [Configuration](#configuration)
-  - [Usage](#usage)
-  - [API Documentation](#api-documentation)
-  - [Command line Documentation](#command-line-documentation)
+- [Installation](#installation)
+  - [Prerequisites](#prerequisites)
+  - [Install the latest package](#install-the-latest-package)
+  - [Install an older package version](#install-an-older-package-version)
+  - [Test your installation](#test-your-installation)
+- [Configuration](#configuration)
+- [Usage](#usage)
+- [API Documentation](#api-documentation)
+- [Command line Documentation](#command-line-documentation)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Installation
 
 ### Prerequisites
 - [ ] [Python 3](https://www.python.org/)
```

### Comparing `cbw-api-toolbox-2.3.1/bin/cyberwatch-cli` & `cbw-api-toolbox-2.3.2/bin/cyberwatch-cli`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cbw_api_toolbox/__routes__.py` & `cbw-api-toolbox-2.3.2/cbw_api_toolbox/__routes__.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cbw_api_toolbox/cbw_api.py` & `cbw-api-toolbox-2.3.2/cbw_api_toolbox/cbw_api.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cbw_api_toolbox/cbw_auth.py` & `cbw-api-toolbox-2.3.2/cbw_api_toolbox/cbw_auth.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cbw_api_toolbox/cbw_file_xlsx.py` & `cbw-api-toolbox-2.3.2/cbw_api_toolbox/cbw_file_xlsx.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/PKG-INFO` & `cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: cbw-api-toolbox
-Version: 2.3.1
+Version: 2.3.2
 Summary: CyberWatch Api Tools.
 Home-page: https://github.com/Cyberwatch/cyberwatch_api_toolbox
 Author: CyberWatch SAS
 Author-email: support-it+api@cyberwatch.fr
 License: MIT
 Project-URL: Documentation, https://docs.cyberwatch.fr/api/#introduction
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cyberwatch API toolbox
+# \[DEPRECATED\]
+
+## New Api Client
+This module has been deprecated. Please consider using [cyberwatch_api](https://github.com/Cyberwatch/cyberwatch_api).
+
+Please contact Cyberwatch support if you need help to migrate your existing scripts to the new client.
+
+## Cyberwatch API toolbox
 
 A simple interface for your Cyberwatch instance API composed of a python library
 and a command line program.
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-
-- [Cyberwatch API toolbox](#cyberwatch-api-toolbox)
-  - [Installation](#installation)
-    - [Prerequisites](#prerequisites)
-    - [Install the package](#install-the-package)
-    - [Test your installation](#test-your-installation)
-  - [Configuration](#configuration)
-  - [Usage](#usage)
-  - [API Documentation](#api-documentation)
-  - [Command line Documentation](#command-line-documentation)
+- [Installation](#installation)
+  - [Prerequisites](#prerequisites)
+  - [Install the latest package](#install-the-latest-package)
+  - [Install an older package version](#install-an-older-package-version)
+  - [Test your installation](#test-your-installation)
+- [Configuration](#configuration)
+- [Usage](#usage)
+- [API Documentation](#api-documentation)
+- [Command line Documentation](#command-line-documentation)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Installation
 
 ### Prerequisites
 - [ ] [Python 3](https://www.python.org/)
```

### Comparing `cbw-api-toolbox-2.3.1/cbw_api_toolbox.egg-info/SOURCES.txt` & `cbw-api-toolbox-2.3.2/cbw_api_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/airgap/__init__.py` & `cbw-api-toolbox-2.3.2/cli/airgap/__init__.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/airgap/download_scripts.py` & `cbw-api-toolbox-2.3.2/cli/airgap/download_scripts.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/airgap/upload.py` & `cbw-api-toolbox-2.3.2/cli/airgap/upload.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/airgap/upload_compliance.py` & `cbw-api-toolbox-2.3.2/cli/airgap/upload_compliance.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/docker_image/__init__.py` & `cbw-api-toolbox-2.3.2/cli/docker_image/__init__.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/docker_image/create.py` & `cbw-api-toolbox-2.3.2/cli/docker_image/create.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/docker_image/list_images.py` & `cbw-api-toolbox-2.3.2/cli/docker_image/list_images.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/docker_image/scan.py` & `cbw-api-toolbox-2.3.2/cli/docker_image/scan.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/docker_image/show.py` & `cbw-api-toolbox-2.3.2/cli/docker_image/show.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/docker_image/update.py` & `cbw-api-toolbox-2.3.2/cli/docker_image/update.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/docker_image/utils.py` & `cbw-api-toolbox-2.3.2/cli/docker_image/utils.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/os/__init__.py` & `cbw-api-toolbox-2.3.2/cli/os/__init__.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/cli/os/list_os.py` & `cbw-api-toolbox-2.3.2/cli/os/list_os.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/affect_group_by_hostname.py` & `cbw-api-toolbox-2.3.2/examples/affect_group_by_hostname.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/affect_group_os.py` & `cbw-api-toolbox-2.3.2/examples/affect_group_os.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/affect_repository_to_group.py` & `cbw-api-toolbox-2.3.2/examples/affect_repository_to_group.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/agents_by_last_communication.py` & `cbw-api-toolbox-2.3.2/examples/agents_by_last_communication.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/clean_discovered_docker.py` & `cbw-api-toolbox-2.3.2/examples/clean_discovered_docker.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/cleanup_duplicates.py` & `cbw-api-toolbox-2.3.2/examples/cleanup_duplicates.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/cleanup_initialization_duplicates.py` & `cbw-api-toolbox-2.3.2/examples/cleanup_initialization_duplicates.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/cleanup_lost_com_filters.py` & `cbw-api-toolbox-2.3.2/examples/cleanup_lost_com_filters.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/create_applicative_scan.py` & `cbw-api-toolbox-2.3.2/examples/create_applicative_scan.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/create_host.py` & `cbw-api-toolbox-2.3.2/examples/create_host.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/create_multiple_remote_accesses.py` & `cbw-api-toolbox-2.3.2/examples/create_multiple_remote_accesses.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/create_remote_by_host.py` & `cbw-api-toolbox-2.3.2/examples/create_remote_by_host.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/cve_published_last_month_export_xlsx.py` & `cbw-api-toolbox-2.3.2/examples/cve_published_last_month_export_xlsx.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/detail_servers.py` & `cbw-api-toolbox-2.3.2/examples/detail_servers.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/docker_image_add.py` & `cbw-api-toolbox-2.3.2/examples/docker_image_add.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/docker_image_update.py` & `cbw-api-toolbox-2.3.2/examples/docker_image_update.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/email_report.py` & `cbw-api-toolbox-2.3.2/examples/email_report.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/email_report_filters.py` & `cbw-api-toolbox-2.3.2/examples/email_report_filters.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/fetch_daily_cves_to_redmine.py` & `cbw-api-toolbox-2.3.2/examples/fetch_daily_cves_to_redmine.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/find_outdated_last_detection.py` & `cbw-api-toolbox-2.3.2/examples/find_outdated_last_detection.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/get_all_subnets.py` & `cbw-api-toolbox-2.3.2/examples/get_all_subnets.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/group_create.py` & `cbw-api-toolbox-2.3.2/examples/group_create.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/groups_from_csv.py` & `cbw-api-toolbox-2.3.2/examples/groups_from_csv.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/host_detail_export_xlsx.py` & `cbw-api-toolbox-2.3.2/examples/host_detail_export_xlsx.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/ignore_spooler_cves_after_mitigation.py` & `cbw-api-toolbox-2.3.2/examples/ignore_spooler_cves_after_mitigation.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/import_file_xlsx.py` & `cbw-api-toolbox-2.3.2/examples/import_file_xlsx.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/remote_access_create.py` & `cbw-api-toolbox-2.3.2/examples/remote_access_create.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/remote_access_update.py` & `cbw-api-toolbox-2.3.2/examples/remote_access_update.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/remote_accesses_test_deploy.py` & `cbw-api-toolbox-2.3.2/examples/remote_accesses_test_deploy.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/security_issue_create.py` & `cbw-api-toolbox-2.3.2/examples/security_issue_create.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/security_issue_update.py` & `cbw-api-toolbox-2.3.2/examples/security_issue_update.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/server_affect_ignoring_policy.py` & `cbw-api-toolbox-2.3.2/examples/server_affect_ignoring_policy.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/server_creation_date_to_xlsx.py` & `cbw-api-toolbox-2.3.2/examples/server_creation_date_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/server_delete.py` & `cbw-api-toolbox-2.3.2/examples/server_delete.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/server_to_qradar.py` & `cbw-api-toolbox-2.3.2/examples/server_to_qradar.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/server_to_splunk.py` & `cbw-api-toolbox-2.3.2/examples/server_to_splunk.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/server_update.py` & `cbw-api-toolbox-2.3.2/examples/server_update.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/servers_by_group.py` & `cbw-api-toolbox-2.3.2/examples/servers_by_group.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/servers_cves_csv.py` & `cbw-api-toolbox-2.3.2/examples/servers_cves_csv.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/servers_detail_export_xlsx.py` & `cbw-api-toolbox-2.3.2/examples/servers_detail_export_xlsx.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/stored_credential_create.py` & `cbw-api-toolbox-2.3.2/examples/stored_credential_create.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/stored_credential_update.py` & `cbw-api-toolbox-2.3.2/examples/stored_credential_update.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/update_applicative_scan.py` & `cbw-api-toolbox-2.3.2/examples/update_applicative_scan.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/update_cve_announcement.py` & `cbw-api-toolbox-2.3.2/examples/update_cve_announcement.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/update_server_cve.py` & `cbw-api-toolbox-2.3.2/examples/update_server_cve.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/view_dashboard_indicator.py` & `cbw-api-toolbox-2.3.2/examples/view_dashboard_indicator.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/examples/view_server_patch.py` & `cbw-api-toolbox-2.3.2/examples/view_server_patch.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/setup.py` & `cbw-api-toolbox-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cbw-api-toolbox',
     description='CyberWatch Api Tools.',
     long_description=open('README.md').read().strip(),
     long_description_content_type="text/markdown",
-    version='2.3.1',
+    version='2.3.2',
     author='CyberWatch SAS',
     author_email='support-it+api@cyberwatch.fr',
     license='MIT',
     url='https://github.com/Cyberwatch/cyberwatch_api_toolbox',
     project_urls={
         "Documentation": "https://docs.cyberwatch.fr/api/#introduction",
     },
```

### Comparing `cbw-api-toolbox-2.3.1/spec/test_cbw_api.py` & `cbw-api-toolbox-2.3.2/spec/test_cbw_api.py`

 * *Files identical despite different names*

### Comparing `cbw-api-toolbox-2.3.1/spec/test_cbw_files_xlsx.py` & `cbw-api-toolbox-2.3.2/spec/test_cbw_files_xlsx.py`

 * *Files identical despite different names*

