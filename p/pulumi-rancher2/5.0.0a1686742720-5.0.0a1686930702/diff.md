# Comparing `tmp/pulumi_rancher2-5.0.0a1686742720.tar.gz` & `tmp/pulumi_rancher2-5.0.0a1686930702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-5.0.0a1686742720.tar", last modified: Wed Jun 14 11:44:51 2023, max compression
+gzip compressed data, was "pulumi_rancher2-5.0.0a1686930702.tar", last modified: Fri Jun 16 15:57:07 2023, max compression
```

## Comparing `pulumi_rancher2-5.0.0a1686742720.tar` & `pulumi_rancher2-5.0.0a1686930702.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1287410 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)   141124 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    31455 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    41552 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    47168 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    82407 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)  1602259 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:07.229950 pulumi_rancher2-5.0.0a1686930702/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-16 15:57:07.229950 pulumi_rancher2-5.0.0a1686930702/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:07.225950 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1287716 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141124 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31455 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41552 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:07.229950 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47168 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82407 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1602525 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:57:07.229950 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-16 15:57:07.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-16 15:57:07.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:57:07.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:57:07.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 15:57:07.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 15:57:07.000000 pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:57:07.229950 pulumi_rancher2-5.0.0a1686930702/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 15:57:06.000000 pulumi_rancher2-5.0.0a1686930702/setup.py
```

### Comparing `pulumi_rancher2-5.0.0a1686742720/PKG-INFO` & `pulumi_rancher2-5.0.0a1686930702/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 5.0.0a1686742720
+Version: 5.0.0a1686930702
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.0.0a1686742720/README.md` & `pulumi_rancher2-5.0.0a1686930702/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/__init__.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23228,71 +23228,73 @@
     def userdata(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "userdata", value)
 
 
 @pulumi.input_type
 class MachineConfigV2HarvesterConfigArgs:
     def __init__(__self__, *,
-                 disk_info: pulumi.Input[str],
-                 network_info: pulumi.Input[str],
                  ssh_user: pulumi.Input[str],
                  vm_namespace: pulumi.Input[str],
                  cpu_count: Optional[pulumi.Input[str]] = None,
                  disk_bus: Optional[pulumi.Input[str]] = None,
+                 disk_info: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[str]] = None,
                  image_name: Optional[pulumi.Input[str]] = None,
                  memory_size: Optional[pulumi.Input[str]] = None,
                  network_data: Optional[pulumi.Input[str]] = None,
+                 network_info: Optional[pulumi.Input[str]] = None,
                  network_model: Optional[pulumi.Input[str]] = None,
                  network_name: Optional[pulumi.Input[str]] = None,
                  ssh_password: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  vm_affinity: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param pulumi.Input[str] network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param pulumi.Input[str] cpu_count: CPU count, Default `2` (string)
         :param pulumi.Input[str] disk_bus: Use `disk_info` instead
+        :param pulumi.Input[str] disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
         :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] image_name: Use `disk_info` instead
         :param pulumi.Input[str] memory_size: Memory size (in GiB), Default `4` (string)
         :param pulumi.Input[str] network_data: NetworkData content of cloud-init, base64 is supported (string)
+        :param pulumi.Input[str] network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param pulumi.Input[str] network_model: Use `network_info` instead
         :param pulumi.Input[str] network_name: Use `network_info` instead
         :param pulumi.Input[str] ssh_password: SSH password (string)
         :param pulumi.Input[str] user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
         :param pulumi.Input[str] vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
         """
-        pulumi.set(__self__, "disk_info", disk_info)
-        pulumi.set(__self__, "network_info", network_info)
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
             pulumi.log.warn("""disk_bus is deprecated: Use disk_info instead""")
         if disk_bus is not None:
             pulumi.set(__self__, "disk_bus", disk_bus)
+        if disk_info is not None:
+            pulumi.set(__self__, "disk_info", disk_info)
         if disk_size is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
             pulumi.log.warn("""disk_size is deprecated: Use disk_info instead""")
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
         if image_name is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
             pulumi.log.warn("""image_name is deprecated: Use disk_info instead""")
         if image_name is not None:
             pulumi.set(__self__, "image_name", image_name)
         if memory_size is not None:
             pulumi.set(__self__, "memory_size", memory_size)
         if network_data is not None:
             pulumi.set(__self__, "network_data", network_data)
+        if network_info is not None:
+            pulumi.set(__self__, "network_info", network_info)
         if network_model is not None:
             warnings.warn("""Use network_info instead""", DeprecationWarning)
             pulumi.log.warn("""network_model is deprecated: Use network_info instead""")
         if network_model is not None:
             pulumi.set(__self__, "network_model", network_model)
         if network_name is not None:
             warnings.warn("""Use network_info instead""", DeprecationWarning)
@@ -23303,38 +23305,14 @@
             pulumi.set(__self__, "ssh_password", ssh_password)
         if user_data is not None:
             pulumi.set(__self__, "user_data", user_data)
         if vm_affinity is not None:
             pulumi.set(__self__, "vm_affinity", vm_affinity)
 
     @property
-    @pulumi.getter(name="diskInfo")
-    def disk_info(self) -> pulumi.Input[str]:
-        """
-        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        """
-        return pulumi.get(self, "disk_info")
-
-    @disk_info.setter
-    def disk_info(self, value: pulumi.Input[str]):
-        pulumi.set(self, "disk_info", value)
-
-    @property
-    @pulumi.getter(name="networkInfo")
-    def network_info(self) -> pulumi.Input[str]:
-        """
-        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
-        """
-        return pulumi.get(self, "network_info")
-
-    @network_info.setter
-    def network_info(self, value: pulumi.Input[str]):
-        pulumi.set(self, "network_info", value)
-
-    @property
     @pulumi.getter(name="sshUser")
     def ssh_user(self) -> pulumi.Input[str]:
         """
         Set the name of the ssh user (string)
         """
         return pulumi.get(self, "ssh_user")
 
@@ -23375,14 +23353,26 @@
         return pulumi.get(self, "disk_bus")
 
     @disk_bus.setter
     def disk_bus(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_bus", value)
 
     @property
+    @pulumi.getter(name="diskInfo")
+    def disk_info(self) -> Optional[pulumi.Input[str]]:
+        """
+        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
+        """
+        return pulumi.get(self, "disk_info")
+
+    @disk_info.setter
+    def disk_info(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "disk_info", value)
+
+    @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
         Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
@@ -23423,14 +23413,26 @@
         return pulumi.get(self, "network_data")
 
     @network_data.setter
     def network_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_data", value)
 
     @property
+    @pulumi.getter(name="networkInfo")
+    def network_info(self) -> Optional[pulumi.Input[str]]:
+        """
+        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
+        """
+        return pulumi.get(self, "network_info")
+
+    @network_info.setter
+    def network_info(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_info", value)
+
+    @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[pulumi.Input[str]]:
         """
         Use `network_info` instead
         """
         return pulumi.get(self, "network_model")
 
@@ -26858,71 +26860,73 @@
     def userdata(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "userdata", value)
 
 
 @pulumi.input_type
 class NodeTemplateHarvesterConfigArgs:
     def __init__(__self__, *,
-                 disk_info: pulumi.Input[str],
-                 network_info: pulumi.Input[str],
                  ssh_user: pulumi.Input[str],
                  vm_namespace: pulumi.Input[str],
                  cpu_count: Optional[pulumi.Input[str]] = None,
                  disk_bus: Optional[pulumi.Input[str]] = None,
+                 disk_info: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[str]] = None,
                  image_name: Optional[pulumi.Input[str]] = None,
                  memory_size: Optional[pulumi.Input[str]] = None,
                  network_data: Optional[pulumi.Input[str]] = None,
+                 network_info: Optional[pulumi.Input[str]] = None,
                  network_model: Optional[pulumi.Input[str]] = None,
                  network_name: Optional[pulumi.Input[str]] = None,
                  ssh_password: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  vm_affinity: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param pulumi.Input[str] network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param pulumi.Input[str] ssh_user: Set the name of the ssh user (string)
         :param pulumi.Input[str] vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param pulumi.Input[str] cpu_count: CPU count, Default `2` (string)
         :param pulumi.Input[str] disk_bus: Use `disk_info` instead
+        :param pulumi.Input[str] disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
         :param pulumi.Input[str] disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         :param pulumi.Input[str] image_name: Use `disk_info` instead
         :param pulumi.Input[str] memory_size: Memory size (in GiB), Default `4` (string)
         :param pulumi.Input[str] network_data: NetworkData content of cloud-init, base64 is supported (string)
+        :param pulumi.Input[str] network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param pulumi.Input[str] network_model: Use `network_info` instead
         :param pulumi.Input[str] network_name: Use `network_info` instead
         :param pulumi.Input[str] ssh_password: SSH password (string)
         :param pulumi.Input[str] user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
         :param pulumi.Input[str] vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
         """
-        pulumi.set(__self__, "disk_info", disk_info)
-        pulumi.set(__self__, "network_info", network_info)
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
             pulumi.log.warn("""disk_bus is deprecated: Use disk_info instead""")
         if disk_bus is not None:
             pulumi.set(__self__, "disk_bus", disk_bus)
+        if disk_info is not None:
+            pulumi.set(__self__, "disk_info", disk_info)
         if disk_size is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
             pulumi.log.warn("""disk_size is deprecated: Use disk_info instead""")
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
         if image_name is not None:
             warnings.warn("""Use disk_info instead""", DeprecationWarning)
             pulumi.log.warn("""image_name is deprecated: Use disk_info instead""")
         if image_name is not None:
             pulumi.set(__self__, "image_name", image_name)
         if memory_size is not None:
             pulumi.set(__self__, "memory_size", memory_size)
         if network_data is not None:
             pulumi.set(__self__, "network_data", network_data)
+        if network_info is not None:
+            pulumi.set(__self__, "network_info", network_info)
         if network_model is not None:
             warnings.warn("""Use network_info instead""", DeprecationWarning)
             pulumi.log.warn("""network_model is deprecated: Use network_info instead""")
         if network_model is not None:
             pulumi.set(__self__, "network_model", network_model)
         if network_name is not None:
             warnings.warn("""Use network_info instead""", DeprecationWarning)
@@ -26933,38 +26937,14 @@
             pulumi.set(__self__, "ssh_password", ssh_password)
         if user_data is not None:
             pulumi.set(__self__, "user_data", user_data)
         if vm_affinity is not None:
             pulumi.set(__self__, "vm_affinity", vm_affinity)
 
     @property
-    @pulumi.getter(name="diskInfo")
-    def disk_info(self) -> pulumi.Input[str]:
-        """
-        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        """
-        return pulumi.get(self, "disk_info")
-
-    @disk_info.setter
-    def disk_info(self, value: pulumi.Input[str]):
-        pulumi.set(self, "disk_info", value)
-
-    @property
-    @pulumi.getter(name="networkInfo")
-    def network_info(self) -> pulumi.Input[str]:
-        """
-        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
-        """
-        return pulumi.get(self, "network_info")
-
-    @network_info.setter
-    def network_info(self, value: pulumi.Input[str]):
-        pulumi.set(self, "network_info", value)
-
-    @property
     @pulumi.getter(name="sshUser")
     def ssh_user(self) -> pulumi.Input[str]:
         """
         Set the name of the ssh user (string)
         """
         return pulumi.get(self, "ssh_user")
 
@@ -27005,14 +26985,26 @@
         return pulumi.get(self, "disk_bus")
 
     @disk_bus.setter
     def disk_bus(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_bus", value)
 
     @property
+    @pulumi.getter(name="diskInfo")
+    def disk_info(self) -> Optional[pulumi.Input[str]]:
+        """
+        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
+        """
+        return pulumi.get(self, "disk_info")
+
+    @disk_info.setter
+    def disk_info(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "disk_info", value)
+
+    @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[pulumi.Input[str]]:
         """
         Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
@@ -27053,14 +27045,26 @@
         return pulumi.get(self, "network_data")
 
     @network_data.setter
     def network_data(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_data", value)
 
     @property
+    @pulumi.getter(name="networkInfo")
+    def network_info(self) -> Optional[pulumi.Input[str]]:
+        """
+        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
+        """
+        return pulumi.get(self, "network_info")
+
+    @network_info.setter
+    def network_info(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_info", value)
+
+    @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[pulumi.Input[str]]:
         """
         Use `network_info` instead
         """
         return pulumi.get(self, "network_model")
```

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/active_directory.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/app_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/auth_config_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/certificate.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_group.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alter_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_rule.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_alter_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_sync.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/feature.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_app.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alter_rule.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_alter_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_namespace.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
     foo = rancher2.get_namespace(name="foo",
-        project_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+        project_id=rancher2_cluster["foo-custom"]["default_project_id"])
     ```
 
 
     :param str name: The name of the namespace (string)
     :param str project_id: The project id where namespace is assigned (string)
     """
     __args__ = dict()
@@ -170,15 +170,15 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
     foo = rancher2.get_namespace(name="foo",
-        project_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+        project_id=rancher2_cluster["foo-custom"]["default_project_id"])
     ```
 
 
     :param str name: The name of the namespace (string)
     :param str project_id: The project id where namespace is assigned (string)
     """
     ...
```

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_node_pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_node_pool(cluster_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    foo = rancher2.get_node_pool(cluster_id=rancher2_cluster["foo-custom"]["id"],
         name="foo")
     ```
 
 
     :param str cluster_id: The RKE cluster id to use Node Pool (string)
     :param str name: The name of the Node Pool (string)
     :param str node_template_id: The Node Template ID to use for node creation (string)
@@ -235,15 +235,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_node_pool(cluster_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    foo = rancher2.get_node_pool(cluster_id=rancher2_cluster["foo-custom"]["id"],
         name="foo")
     ```
 
 
     :param str cluster_id: The RKE cluster id to use Node Pool (string)
     :param str name: The name of the Node Pool (string)
     :param str node_template_id: The Node Template ID to use for node creation (string)
```

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_tempalte.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_role_tempalte.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_user.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/machine_config_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/namespace.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/notifier.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/outputs.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22047,34 +22047,34 @@
 
 
 @pulumi.output_type
 class MachineConfigV2HarvesterConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "diskInfo":
-            suggest = "disk_info"
-        elif key == "networkInfo":
-            suggest = "network_info"
-        elif key == "sshUser":
+        if key == "sshUser":
             suggest = "ssh_user"
         elif key == "vmNamespace":
             suggest = "vm_namespace"
         elif key == "cpuCount":
             suggest = "cpu_count"
         elif key == "diskBus":
             suggest = "disk_bus"
+        elif key == "diskInfo":
+            suggest = "disk_info"
         elif key == "diskSize":
             suggest = "disk_size"
         elif key == "imageName":
             suggest = "image_name"
         elif key == "memorySize":
             suggest = "memory_size"
         elif key == "networkData":
             suggest = "network_data"
+        elif key == "networkInfo":
+            suggest = "network_info"
         elif key == "networkModel":
             suggest = "network_model"
         elif key == "networkName":
             suggest = "network_name"
         elif key == "sshPassword":
             suggest = "ssh_password"
         elif key == "userData":
@@ -22090,90 +22090,76 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         MachineConfigV2HarvesterConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 disk_info: str,
-                 network_info: str,
                  ssh_user: str,
                  vm_namespace: str,
                  cpu_count: Optional[str] = None,
                  disk_bus: Optional[str] = None,
+                 disk_info: Optional[str] = None,
                  disk_size: Optional[str] = None,
                  image_name: Optional[str] = None,
                  memory_size: Optional[str] = None,
                  network_data: Optional[str] = None,
+                 network_info: Optional[str] = None,
                  network_model: Optional[str] = None,
                  network_name: Optional[str] = None,
                  ssh_password: Optional[str] = None,
                  user_data: Optional[str] = None,
                  vm_affinity: Optional[str] = None):
         """
-        :param str disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param str network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param str ssh_user: Set the name of the ssh user (string)
         :param str vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param str cpu_count: CPU count, Default `2` (string)
         :param str disk_bus: Use `disk_info` instead
+        :param str disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
         :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         :param str image_name: Use `disk_info` instead
         :param str memory_size: Memory size (in GiB), Default `4` (string)
         :param str network_data: NetworkData content of cloud-init, base64 is supported (string)
+        :param str network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param str network_model: Use `network_info` instead
         :param str network_name: Use `network_info` instead
         :param str ssh_password: SSH password (string)
         :param str user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
         :param str vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
         """
-        pulumi.set(__self__, "disk_info", disk_info)
-        pulumi.set(__self__, "network_info", network_info)
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             pulumi.set(__self__, "disk_bus", disk_bus)
+        if disk_info is not None:
+            pulumi.set(__self__, "disk_info", disk_info)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
         if image_name is not None:
             pulumi.set(__self__, "image_name", image_name)
         if memory_size is not None:
             pulumi.set(__self__, "memory_size", memory_size)
         if network_data is not None:
             pulumi.set(__self__, "network_data", network_data)
+        if network_info is not None:
+            pulumi.set(__self__, "network_info", network_info)
         if network_model is not None:
             pulumi.set(__self__, "network_model", network_model)
         if network_name is not None:
             pulumi.set(__self__, "network_name", network_name)
         if ssh_password is not None:
             pulumi.set(__self__, "ssh_password", ssh_password)
         if user_data is not None:
             pulumi.set(__self__, "user_data", user_data)
         if vm_affinity is not None:
             pulumi.set(__self__, "vm_affinity", vm_affinity)
 
     @property
-    @pulumi.getter(name="diskInfo")
-    def disk_info(self) -> str:
-        """
-        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        """
-        return pulumi.get(self, "disk_info")
-
-    @property
-    @pulumi.getter(name="networkInfo")
-    def network_info(self) -> str:
-        """
-        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
-        """
-        return pulumi.get(self, "network_info")
-
-    @property
     @pulumi.getter(name="sshUser")
     def ssh_user(self) -> str:
         """
         Set the name of the ssh user (string)
         """
         return pulumi.get(self, "ssh_user")
 
@@ -22198,14 +22184,22 @@
     def disk_bus(self) -> Optional[str]:
         """
         Use `disk_info` instead
         """
         return pulumi.get(self, "disk_bus")
 
     @property
+    @pulumi.getter(name="diskInfo")
+    def disk_info(self) -> Optional[str]:
+        """
+        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
+        """
+        return pulumi.get(self, "disk_info")
+
+    @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
         Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
@@ -22230,14 +22224,22 @@
     def network_data(self) -> Optional[str]:
         """
         NetworkData content of cloud-init, base64 is supported (string)
         """
         return pulumi.get(self, "network_data")
 
     @property
+    @pulumi.getter(name="networkInfo")
+    def network_info(self) -> Optional[str]:
+        """
+        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
+        """
+        return pulumi.get(self, "network_info")
+
+    @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[str]:
         """
         Use `network_info` instead
         """
         return pulumi.get(self, "network_model")
 
@@ -25329,34 +25331,34 @@
 
 
 @pulumi.output_type
 class NodeTemplateHarvesterConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "diskInfo":
-            suggest = "disk_info"
-        elif key == "networkInfo":
-            suggest = "network_info"
-        elif key == "sshUser":
+        if key == "sshUser":
             suggest = "ssh_user"
         elif key == "vmNamespace":
             suggest = "vm_namespace"
         elif key == "cpuCount":
             suggest = "cpu_count"
         elif key == "diskBus":
             suggest = "disk_bus"
+        elif key == "diskInfo":
+            suggest = "disk_info"
         elif key == "diskSize":
             suggest = "disk_size"
         elif key == "imageName":
             suggest = "image_name"
         elif key == "memorySize":
             suggest = "memory_size"
         elif key == "networkData":
             suggest = "network_data"
+        elif key == "networkInfo":
+            suggest = "network_info"
         elif key == "networkModel":
             suggest = "network_model"
         elif key == "networkName":
             suggest = "network_name"
         elif key == "sshPassword":
             suggest = "ssh_password"
         elif key == "userData":
@@ -25372,90 +25374,76 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         NodeTemplateHarvesterConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 disk_info: str,
-                 network_info: str,
                  ssh_user: str,
                  vm_namespace: str,
                  cpu_count: Optional[str] = None,
                  disk_bus: Optional[str] = None,
+                 disk_info: Optional[str] = None,
                  disk_size: Optional[str] = None,
                  image_name: Optional[str] = None,
                  memory_size: Optional[str] = None,
                  network_data: Optional[str] = None,
+                 network_info: Optional[str] = None,
                  network_model: Optional[str] = None,
                  network_name: Optional[str] = None,
                  ssh_password: Optional[str] = None,
                  user_data: Optional[str] = None,
                  vm_affinity: Optional[str] = None):
         """
-        :param str disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        :param str network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param str ssh_user: Set the name of the ssh user (string)
         :param str vm_namespace: Virtual machine namespace e.g. `default` (string)
         :param str cpu_count: CPU count, Default `2` (string)
         :param str disk_bus: Use `disk_info` instead
+        :param str disk_info: A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
         :param str disk_size: Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         :param str image_name: Use `disk_info` instead
         :param str memory_size: Memory size (in GiB), Default `4` (string)
         :param str network_data: NetworkData content of cloud-init, base64 is supported (string)
+        :param str network_info: A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
         :param str network_model: Use `network_info` instead
         :param str network_name: Use `network_info` instead
         :param str ssh_password: SSH password (string)
         :param str user_data: UserData content of cloud-init, base64 is supported. If the image does not contain the qemu-guest-agent package, you must install and start qemu-guest-agent using userdata (string)
         :param str vm_affinity: Virtual machine affinity, only base64 format is supported. For Rancher v2.6.7 or above (string)
         """
-        pulumi.set(__self__, "disk_info", disk_info)
-        pulumi.set(__self__, "network_info", network_info)
         pulumi.set(__self__, "ssh_user", ssh_user)
         pulumi.set(__self__, "vm_namespace", vm_namespace)
         if cpu_count is not None:
             pulumi.set(__self__, "cpu_count", cpu_count)
         if disk_bus is not None:
             pulumi.set(__self__, "disk_bus", disk_bus)
+        if disk_info is not None:
+            pulumi.set(__self__, "disk_info", disk_info)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
         if image_name is not None:
             pulumi.set(__self__, "image_name", image_name)
         if memory_size is not None:
             pulumi.set(__self__, "memory_size", memory_size)
         if network_data is not None:
             pulumi.set(__self__, "network_data", network_data)
+        if network_info is not None:
+            pulumi.set(__self__, "network_info", network_info)
         if network_model is not None:
             pulumi.set(__self__, "network_model", network_model)
         if network_name is not None:
             pulumi.set(__self__, "network_name", network_name)
         if ssh_password is not None:
             pulumi.set(__self__, "ssh_password", ssh_password)
         if user_data is not None:
             pulumi.set(__self__, "user_data", user_data)
         if vm_affinity is not None:
             pulumi.set(__self__, "vm_affinity", vm_affinity)
 
     @property
-    @pulumi.getter(name="diskInfo")
-    def disk_info(self) -> str:
-        """
-        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
-        """
-        return pulumi.get(self, "disk_info")
-
-    @property
-    @pulumi.getter(name="networkInfo")
-    def network_info(self) -> str:
-        """
-        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
-        """
-        return pulumi.get(self, "network_info")
-
-    @property
     @pulumi.getter(name="sshUser")
     def ssh_user(self) -> str:
         """
         Set the name of the ssh user (string)
         """
         return pulumi.get(self, "ssh_user")
 
@@ -25480,14 +25468,22 @@
     def disk_bus(self) -> Optional[str]:
         """
         Use `disk_info` instead
         """
         return pulumi.get(self, "disk_bus")
 
     @property
+    @pulumi.getter(name="diskInfo")
+    def disk_info(self) -> Optional[str]:
+        """
+        A JSON string specifying info for the disks e.g. `{\\"disks\\":[{\\"imageName\\":\\"harvester-public/image-57hzg\\",\\"bootOrder\\":1,\\"size\\":40},{\\"storageClassName\\":\\"node-driver-test\\",\\"bootOrder\\":2,\\"size\\":1}]}` (string)
+        """
+        return pulumi.get(self, "disk_info")
+
+    @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> Optional[str]:
         """
         Disk size if using managed disk. Just for Rancher v2.3.x and above. Default `30` (string)
         """
         return pulumi.get(self, "disk_size")
 
@@ -25512,14 +25508,22 @@
     def network_data(self) -> Optional[str]:
         """
         NetworkData content of cloud-init, base64 is supported (string)
         """
         return pulumi.get(self, "network_data")
 
     @property
+    @pulumi.getter(name="networkInfo")
+    def network_info(self) -> Optional[str]:
+        """
+        A JSON string specifying info for the networks e.g. `{\\"interfaces\\":[{\\"networkName\\":\\"harvester-public/vlan1\\"},{\\"networkName\\":\\"harvester-public/vlan2\\"}]}` (string)
+        """
+        return pulumi.get(self, "network_info")
+
+    @property
     @pulumi.getter(name="networkModel")
     def network_model(self) -> Optional[str]:
         """
         Use `network_info` instead
         """
         return pulumi.get(self, "network_model")
```

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/provider.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/registry.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_tempalte.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/role_tempalte.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_template.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/setting.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/token.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/user.py` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rancher2
-Version: 5.0.0a1686742720
+Version: 5.0.0a1686930702
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-5.0.0a1686930702/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0a1686742720/setup.py` & `pulumi_rancher2-5.0.0a1686930702/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.0.0a1686742720"
-PLUGIN_VERSION = "5.0.0-alpha.1686742720+75dbe1d1"
+VERSION = "5.0.0a1686930702"
+PLUGIN_VERSION = "5.0.0-alpha.1686930702+53b894ea"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rancher2', PLUGIN_VERSION])
         except OSError as error:
```

