# Comparing `tmp/extremecloudiq-api-23.3.1.15.tar.gz` & `tmp/extremecloudiq-api-23.3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmpmwfnz94c/extremecloudiq-api-23.3.1.15.tar", last modified: Thu Jun  8 17:56:21 2023, max compression
+gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmph7dyjgtd/extremecloudiq-api-23.3.2.1.tar", last modified: Fri Jun 16 04:33:44 2023, max compression
```

## Comparing `extremecloudiq-api-23.3.1.15.tar` & `extremecloudiq-api-23.3.2.1.tar`

### file list

```diff
@@ -1,806 +1,822 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32863 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/account_api.py
--rw-r--r--   0 root         (0) root         (0)    16607 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/alert_api.py
--rw-r--r--   0 root         (0) root         (0)    24696 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/application_api.py
--rw-r--r--   0 root         (0) root         (0)    11075 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    26155 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/authorization_api.py
--rw-r--r--   0 root         (0) root         (0)    47344 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/client_api.py
--rw-r--r--   0 root         (0) root         (0)   171865 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    34020 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)     7036 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)    16188 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)   292853 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)   133458 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)    56032 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)    96669 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)   261168 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/device_api.py
--rw-r--r--   0 root         (0) root         (0)    56015 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/hiq_api.py
--rw-r--r--   0 root         (0) root         (0)    67518 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/location_api.py
--rw-r--r--   0 root         (0) root         (0)    45962 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/log_api.py
--rw-r--r--   0 root         (0) root         (0)    49087 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)    15845 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/notification_api.py
--rw-r--r--   0 root         (0) root         (0)    16819 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/operation_api.py
--rw-r--r--   0 root         (0) root         (0)    59448 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/user_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/
--rw-r--r--   0 root         (0) root         (0)    31442 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3762 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/inline_object.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     7549 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     7117 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     7198 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     7171 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7468 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     7414 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     7684 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     7495 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     7198 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     7171 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7252 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     7468 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     7387 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     7090 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     7090 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     7225 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     7414 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)    14244 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)    30789 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)    21694 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)    10200 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     2914 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     2885 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomalies_count_vo_entity.py
--rw-r--r--   0 root         (0) root         (0)    11942 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)    12035 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2899 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)    11007 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)    11341 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     2983 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     7297 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     4918 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     5034 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assurance_scans_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     6191 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     4744 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     8778 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_entity.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_response.py
--rw-r--r--   0 root         (0) root         (0)     9992 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_sort_field.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     5200 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_data.py
--rw-r--r--   0 root         (0) root         (0)     4360 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_request.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_response.py
--rw-r--r--   0 root         (0) root         (0)     8803 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     9740 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)    10481 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     5521 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     4513 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)    10385 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     9147 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     5160 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     3850 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)    36439 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     3460 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     2981 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)    13090 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3007 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     8602 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)    10453 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     3097 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     8904 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     5501 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6858 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5895 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)    13025 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    11803 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)    11600 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    32293 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    19021 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4577 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5396 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4470 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)    18200 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    15074 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     5736 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    13170 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     7343 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    15880 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     7692 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5113 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7193 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     6441 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     6707 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     7369 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     6913 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     4443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     3465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     8692 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)    29777 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     8199 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     5363 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     4314 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     3237 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)    11915 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_installation_report.py
--rw-r--r--   0 root         (0) root         (0)     5440 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     4958 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_lldp_cdp_info.py
--rw-r--r--   0 root         (0) root         (0)    14407 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     6912 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_null_field.py
--rw-r--r--   0 root         (0) root         (0)     2839 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     5419 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     2957 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)    29253 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_wifi_interface.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_changes_entity.py
--rw-r--r--   0 root         (0) root         (0)     4607 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     5838 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     8070 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_device.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_devices.py
--rw-r--r--   0 root         (0) root         (0)     3026 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_feat_license.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_make.py
--rw-r--r--   0 root         (0) root         (0)     4453 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_model.py
--rw-r--r--   0 root         (0) root         (0)     6350 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_vim_module.py
--rw-r--r--   0 root         (0) root         (0)     5412 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_duplex_data_rate_entity.py
--rw-r--r--   0 root         (0) root         (0)     8666 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)    13081 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)    19289 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     5520 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     2919 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     8960 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     8373 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     3012 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     9136 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)    13976 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)    15643 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     5508 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     6363 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)    15300 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     9830 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     6609 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5022 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     5921 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4704 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     9688 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)    34397 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)    10731 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     9191 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     5807 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     7344 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     2855 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)    18840 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     2916 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)    11043 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     4526 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     5819 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     2854 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     9805 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     3378 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     5598 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)    12064 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     6799 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     8615 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)    10248 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     3938 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     6202 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)    10513 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     9629 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     9871 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     5442 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     7190 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)    24027 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     6104 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    17441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     6149 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     3059 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)    13997 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     6301 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2924 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)    31140 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)    11299 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     8920 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)    12894 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)    50568 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     8501 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     4445 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     3773 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     9306 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)    13069 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)    10197 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)    14921 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)    11003 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)    10607 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_speed_duplex_entity.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     3177 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     3387 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     2881 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     6385 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     5031 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6860 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5907 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5263 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     6261 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)    10733 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10502 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     5313 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10459 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    29855 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    16312 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4264 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)    18046 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6338 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    13979 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6535 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    11163 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)    31687 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     7034 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5657 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    10884 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)    58066 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     5908 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    11172 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    15880 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6941 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5113 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7193 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    14730 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user.py
--rw-r--r--   0 root         (0) root         (0)    19134 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7058 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     7244 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     5800 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     6384 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     7742 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     5243 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     7921 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)    13204 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)    10999 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)    11215 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     3683 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     8403 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     7174 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     7145 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     4028 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     8514 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     5775 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)    13566 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    33383 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26261 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api_client.py
--rw-r--r--   0 root         (0) root         (0)    12886 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/configuration.py
--rw-r--r--   0 root         (0) root         (0)     3802 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12334 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35842 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/test/
--rw-r--r--   0 root         (0) root         (0)     1913 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_account_api.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_alert_api.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_application_api.py
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_authorization_api.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_client_api.py
--rw-r--r--   0 root         (0) root         (0)     6222 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     9451 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)     4802 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)     8486 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_device_api.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_hiq_api.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_inline_object.py
--rw-r--r--   0 root         (0) root         (0)     2473 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_location_api.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_log_api.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)     1226 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_notification_api.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_operation_api.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     4078 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     2063 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     3938 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2321 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     6282 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4819 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     4285 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_user_api.py
--rw-r--r--   0 root         (0) root         (0)     2381 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomalies_count_vo_entity.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)     2372 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assurance_scans_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_entity.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_response.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_data.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_request.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_response.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)     2349 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2609 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     5097 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     2003 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     2081 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     3187 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     3430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_installation_report.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_lldp_cdp_info.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_null_field.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_wifi_interface.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_changes_entity.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_channel_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_count_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_device.py
--rw-r--r--   0 root         (0) root         (0)     2030 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_devices.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_feat_license.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_make.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_model.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_vim_module.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_duplex_data_rate_entity.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2315 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     3768 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)     2505 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     5133 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     5513 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)     2745 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)     3475 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     3059 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3239 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     2957 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     2368 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)     2577 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_speed_duplex_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)     4358 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)     2214 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)     2187 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_speed_duplex_entity.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     1840 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2036 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     3387 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1697 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     9060 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     1796 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     3276 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)     3941 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2044 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     1641 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    68003 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/setup.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32862 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/account_api.py
+-rw-r--r--   0 root         (0) root         (0)    16606 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/alert_api.py
+-rw-r--r--   0 root         (0) root         (0)    24695 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/application_api.py
+-rw-r--r--   0 root         (0) root         (0)    11074 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    26154 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)    47343 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/client_api.py
+-rw-r--r--   0 root         (0) root         (0)   171864 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    34019 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)     7035 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)    16187 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)   292852 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)   133457 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)    79847 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)    96668 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)   261167 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/device_api.py
+-rw-r--r--   0 root         (0) root         (0)    56014 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)    67517 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/location_api.py
+-rw-r--r--   0 root         (0) root         (0)    45961 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/log_api.py
+-rw-r--r--   0 root         (0) root         (0)    49086 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)    15844 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/notification_api.py
+-rw-r--r--   0 root         (0) root         (0)    16818 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/operation_api.py
+-rw-r--r--   0 root         (0) root         (0)    59447 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/user_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/
+-rw-r--r--   0 root         (0) root         (0)    32173 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     7548 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     7116 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     7197 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     7413 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     7683 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     7494 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     7197 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7305 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7305 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7413 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)    14243 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)    30788 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)    21693 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10199 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     5055 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)    10206 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_health_type.py
+-rw-r--r--   0 root         (0) root         (0)    12034 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)    11006 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)    11340 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     5032 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4743 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     8777 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4776 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_response.py
+-rw-r--r--   0 root         (0) root         (0)     9991 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)    15660 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     5199 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     4359 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     5672 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     8802 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     9739 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)    10480 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     5520 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     4512 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     4715 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)    10384 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     9146 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     5159 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)    36438 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     4736 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)    10029 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5121 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)    13089 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     8601 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)    10452 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     8903 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     5500 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6857 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)    13024 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    11802 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)    11599 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    32292 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    19020 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)    18199 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    15073 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     5735 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    13169 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    15879 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7192 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     7368 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     4587 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     5048 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)    29776 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     8198 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     9175 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)    11914 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)    14406 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_null_field.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     5418 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)    10017 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)    29252 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5837 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4872 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     8069 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_device.py
+-rw-r--r--   0 root         (0) root         (0)     3511 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_devices.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_feat_license.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_make.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_model.py
+-rw-r--r--   0 root         (0) root         (0)     6349 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_vim_module.py
+-rw-r--r--   0 root         (0) root         (0)     5411 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     8665 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)    13080 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)    19288 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)    13975 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     6362 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)    15299 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     5813 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     9829 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     6336 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     6608 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     3580 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     5920 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     9687 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)    34396 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)    10730 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     9190 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     7343 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)    18839 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)    11042 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     5818 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     9804 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     5597 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)    12063 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     6798 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     8614 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     3937 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)    10512 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     9628 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     9870 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)    11649 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     5441 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)    24026 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     6103 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    17440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)    13996 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     6300 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)    31139 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     8919 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12893 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    50567 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     8500 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12157 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sessions_data_entity.py
+-rw-r--r--   0 root         (0) root         (0)     9305 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)    13068 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)    14920 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)    11002 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)    10606 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     9632 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     6384 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     5030 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6859 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5262 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     6260 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)    10732 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10501 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     5312 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10458 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    29854 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    16311 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)    18045 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    13978 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    11162 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)    31686 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5656 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    10883 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)    58065 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    15879 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4421 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6940 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7192 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    14729 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)    19133 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5799 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6383 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7741 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     7920 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)    13203 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     8961 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)    10998 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     3863 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_capacity_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_capacity_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_efficiency_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     5723 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     8402 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3853 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     4027 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     8513 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     9193 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)    13565 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3957 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    34113 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26259 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    12883 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12333 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      375 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    36636 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/test/
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_account_api.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_alert_api.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_application_api.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_client_api.py
+-rw-r--r--   0 root         (0) root         (0)     6221 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     9450 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)     8485 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_device_api.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_location_api.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_log_api.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/test/test_notification_api.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/test/test_operation_api.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     3019 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     3937 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     6281 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4284 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/test/test_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_health_type.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_response.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_null_field.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_device.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_feat_license.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_make.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_model.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_vim_module.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4618 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     4357 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sessions_data_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     9059 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_capacity_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_capacity_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_efficiency_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    69227 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)      375 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/PKG-INFO
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/__init__.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/__init__.py`

 * *Files identical despite different names*

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/account_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/alert_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/alert_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/application_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/application_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/authentication_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/authorization_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/authorization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/client_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/client_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___authentication_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___basic_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___basic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___certificate_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___certificate_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___deployment_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___deployment_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___policy_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___user_management_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___user_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___anomalies_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___anomalies_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -1068,14 +1068,498 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_wifi_capacity_client_list(self, device_id, channel, timestamp, **kwargs):  # noqa: E501
+        """get_wifi_capacity_client_list  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_capacity_client_list(device_id, channel, timestamp, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int device_id: The device id (required)
+        :param int channel: The channel (required)
+        :param int timestamp: The timestamp (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqWifiCapacityClientListResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_wifi_capacity_client_list_with_http_info(device_id, channel, timestamp, **kwargs)  # noqa: E501
+
+    def get_wifi_capacity_client_list_with_http_info(self, device_id, channel, timestamp, **kwargs):  # noqa: E501
+        """get_wifi_capacity_client_list  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_capacity_client_list_with_http_info(device_id, channel, timestamp, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int device_id: The device id (required)
+        :param int channel: The channel (required)
+        :param int timestamp: The timestamp (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqWifiCapacityClientListResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'device_id',
+            'channel',
+            'timestamp'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_wifi_capacity_client_list" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'device_id' is set
+        if self.api_client.client_side_validation and ('device_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['device_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `device_id` when calling `get_wifi_capacity_client_list`")  # noqa: E501
+        # verify the required parameter 'channel' is set
+        if self.api_client.client_side_validation and ('channel' not in local_var_params or  # noqa: E501
+                                                        local_var_params['channel'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `channel` when calling `get_wifi_capacity_client_list`")  # noqa: E501
+        # verify the required parameter 'timestamp' is set
+        if self.api_client.client_side_validation and ('timestamp' not in local_var_params or  # noqa: E501
+                                                        local_var_params['timestamp'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `timestamp` when calling `get_wifi_capacity_client_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'device_id' in local_var_params and local_var_params['device_id'] is not None:  # noqa: E501
+            query_params.append(('deviceId', local_var_params['device_id']))  # noqa: E501
+        if 'channel' in local_var_params and local_var_params['channel'] is not None:  # noqa: E501
+            query_params.append(('channel', local_var_params['channel']))  # noqa: E501
+        if 'timestamp' in local_var_params and local_var_params['timestamp'] is not None:  # noqa: E501
+            query_params.append(('timestamp', local_var_params['timestamp']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/copilot/anomalies/wifi-capacity/client-list', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqWifiCapacityClientListResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_wifi_capacity_stats(self, anomaly_id, **kwargs):  # noqa: E501
+        """get_wifi_capacity_stats  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_capacity_stats(anomaly_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str anomaly_id: The anomaly id (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqWifiCapacityStatsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_wifi_capacity_stats_with_http_info(anomaly_id, **kwargs)  # noqa: E501
+
+    def get_wifi_capacity_stats_with_http_info(self, anomaly_id, **kwargs):  # noqa: E501
+        """get_wifi_capacity_stats  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_capacity_stats_with_http_info(anomaly_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str anomaly_id: The anomaly id (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqWifiCapacityStatsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'anomaly_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_wifi_capacity_stats" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'anomaly_id' is set
+        if self.api_client.client_side_validation and ('anomaly_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['anomaly_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `anomaly_id` when calling `get_wifi_capacity_stats`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'anomaly_id' in local_var_params and local_var_params['anomaly_id'] is not None:  # noqa: E501
+            query_params.append(('anomalyId', local_var_params['anomaly_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/copilot/anomalies/wifi-capacity/stats', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqWifiCapacityStatsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_wifi_efficiency_client_list(self, device_id, channel, timestamp, **kwargs):  # noqa: E501
+        """get_wifi_efficiency_client_list  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_efficiency_client_list(device_id, channel, timestamp, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int device_id: The device id (required)
+        :param int channel: The channel number (required)
+        :param int timestamp: The timestamp (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqWifiEfficiencyClientListResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_wifi_efficiency_client_list_with_http_info(device_id, channel, timestamp, **kwargs)  # noqa: E501
+
+    def get_wifi_efficiency_client_list_with_http_info(self, device_id, channel, timestamp, **kwargs):  # noqa: E501
+        """get_wifi_efficiency_client_list  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_efficiency_client_list_with_http_info(device_id, channel, timestamp, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int device_id: The device id (required)
+        :param int channel: The channel number (required)
+        :param int timestamp: The timestamp (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqWifiEfficiencyClientListResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'device_id',
+            'channel',
+            'timestamp'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_wifi_efficiency_client_list" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'device_id' is set
+        if self.api_client.client_side_validation and ('device_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['device_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `device_id` when calling `get_wifi_efficiency_client_list`")  # noqa: E501
+        # verify the required parameter 'channel' is set
+        if self.api_client.client_side_validation and ('channel' not in local_var_params or  # noqa: E501
+                                                        local_var_params['channel'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `channel` when calling `get_wifi_efficiency_client_list`")  # noqa: E501
+        # verify the required parameter 'timestamp' is set
+        if self.api_client.client_side_validation and ('timestamp' not in local_var_params or  # noqa: E501
+                                                        local_var_params['timestamp'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `timestamp` when calling `get_wifi_efficiency_client_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'device_id' in local_var_params and local_var_params['device_id'] is not None:  # noqa: E501
+            query_params.append(('deviceId', local_var_params['device_id']))  # noqa: E501
+        if 'channel' in local_var_params and local_var_params['channel'] is not None:  # noqa: E501
+            query_params.append(('channel', local_var_params['channel']))  # noqa: E501
+        if 'timestamp' in local_var_params and local_var_params['timestamp'] is not None:  # noqa: E501
+            query_params.append(('timestamp', local_var_params['timestamp']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/copilot/anomalies/wifi-efficiency/client-list', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqWifiEfficiencyClientListResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_wifi_efficiency_stats(self, anomaly_id, **kwargs):  # noqa: E501
+        """get_wifi_efficiency_stats  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_efficiency_stats(anomaly_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str anomaly_id: The anomaly id (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqWifiEfficiencyStatsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_wifi_efficiency_stats_with_http_info(anomaly_id, **kwargs)  # noqa: E501
+
+    def get_wifi_efficiency_stats_with_http_info(self, anomaly_id, **kwargs):  # noqa: E501
+        """get_wifi_efficiency_stats  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_wifi_efficiency_stats_with_http_info(anomaly_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str anomaly_id: The anomaly id (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqWifiEfficiencyStatsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'anomaly_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_wifi_efficiency_stats" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'anomaly_id' is set
+        if self.api_client.client_side_validation and ('anomaly_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['anomaly_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `anomaly_id` when calling `get_wifi_efficiency_stats`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'anomaly_id' in local_var_params and local_var_params['anomaly_id'] is not None:  # noqa: E501
+            query_params.append(('anomalyId', local_var_params['anomaly_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/copilot/anomalies/wifi-efficiency/stats', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqWifiEfficiencyStatsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def list_anomaly_locations(self, **kwargs):  # noqa: E501
         """list_anomaly_locations  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_anomaly_locations(async_req=True)
         >>> result = thread.get()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___connectivity_experience_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/device_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/device_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/hiq_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/hiq_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/location_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/location_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/log_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/log_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/network_policy_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/network_policy_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/notification_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/notification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/operation_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/operation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api/user_api.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/__init__.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -63,14 +63,15 @@
 from extremecloudiq.models.xiq_alert_group_query import XiqAlertGroupQuery
 from extremecloudiq.models.xiq_alert_severity import XiqAlertSeverity
 from extremecloudiq.models.xiq_alert_source import XiqAlertSource
 from extremecloudiq.models.xiq_alert_source_type import XiqAlertSourceType
 from extremecloudiq.models.xiq_anomalies_count_vo_entity import XiqAnomaliesCountVoEntity
 from extremecloudiq.models.xiq_anomaly_device_entity import XiqAnomalyDeviceEntity
 from extremecloudiq.models.xiq_anomaly_devices_by_location_response import XiqAnomalyDevicesByLocationResponse
+from extremecloudiq.models.xiq_anomaly_health_type import XiqAnomalyHealthType
 from extremecloudiq.models.xiq_anomaly_location_entity import XiqAnomalyLocationEntity
 from extremecloudiq.models.xiq_anomaly_severity import XiqAnomalySeverity
 from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField
 from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType
 from extremecloudiq.models.xiq_api_token_info import XiqApiTokenInfo
 from extremecloudiq.models.xiq_application import XiqApplication
 from extremecloudiq.models.xiq_application_detection_protocol import XiqApplicationDetectionProtocol
@@ -105,14 +106,15 @@
 from extremecloudiq.models.xiq_classification_rule import XiqClassificationRule
 from extremecloudiq.models.xiq_classification_type import XiqClassificationType
 from extremecloudiq.models.xiq_cli_output import XiqCliOutput
 from extremecloudiq.models.xiq_cli_response_code import XiqCliResponseCode
 from extremecloudiq.models.xiq_client import XiqClient
 from extremecloudiq.models.xiq_client_field import XiqClientField
 from extremecloudiq.models.xiq_client_sort_field import XiqClientSortField
+from extremecloudiq.models.xiq_client_stats_entity import XiqClientStatsEntity
 from extremecloudiq.models.xiq_client_summary import XiqClientSummary
 from extremecloudiq.models.xiq_client_usage import XiqClientUsage
 from extremecloudiq.models.xiq_client_view import XiqClientView
 from extremecloudiq.models.xiq_cloud_config_group import XiqCloudConfigGroup
 from extremecloudiq.models.xiq_connectivity_experience_data import XiqConnectivityExperienceData
 from extremecloudiq.models.xiq_connectivity_experience_view_type import XiqConnectivityExperienceViewType
 from extremecloudiq.models.xiq_copilot_events_wired_sort_field import XiqCopilotEventsWiredSortField
@@ -174,14 +176,15 @@
 from extremecloudiq.models.xiq_device_level_ssid_status import XiqDeviceLevelSsidStatus
 from extremecloudiq.models.xiq_device_lldp_cdp_info import XiqDeviceLldpCdpInfo
 from extremecloudiq.models.xiq_device_location import XiqDeviceLocation
 from extremecloudiq.models.xiq_device_location_assignment import XiqDeviceLocationAssignment
 from extremecloudiq.models.xiq_device_null_field import XiqDeviceNullField
 from extremecloudiq.models.xiq_device_sort_field import XiqDeviceSortField
 from extremecloudiq.models.xiq_device_stats import XiqDeviceStats
+from extremecloudiq.models.xiq_device_stats_entity import XiqDeviceStatsEntity
 from extremecloudiq.models.xiq_device_type import XiqDeviceType
 from extremecloudiq.models.xiq_device_view import XiqDeviceView
 from extremecloudiq.models.xiq_device_wifi_interface import XiqDeviceWifiInterface
 from extremecloudiq.models.xiq_dfs_channel_changes_entity import XiqDfsChannelChangesEntity
 from extremecloudiq.models.xiq_dfs_channel_stats_entity import XiqDfsChannelStatsEntity
 from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
 from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
@@ -289,14 +292,15 @@
 from extremecloudiq.models.xiq_rp_neighborhood_analysis import XiqRpNeighborhoodAnalysis
 from extremecloudiq.models.xiq_rp_radio_usage_optimization import XiqRpRadioUsageOptimization
 from extremecloudiq.models.xiq_rp_sensor_scan_settings import XiqRpSensorScanSettings
 from extremecloudiq.models.xiq_rp_wmm_qos_settings import XiqRpWmmQosSettings
 from extremecloudiq.models.xiq_send_cli_request import XiqSendCliRequest
 from extremecloudiq.models.xiq_send_cli_response import XiqSendCliResponse
 from extremecloudiq.models.xiq_server_role import XiqServerRole
+from extremecloudiq.models.xiq_sessions_data_entity import XiqSessionsDataEntity
 from extremecloudiq.models.xiq_set_ssid_mode_dot1x_request import XiqSetSsidModeDot1xRequest
 from extremecloudiq.models.xiq_set_ssid_mode_ppsk_request import XiqSetSsidModePpskRequest
 from extremecloudiq.models.xiq_set_ssid_mode_psk_request import XiqSetSsidModePskRequest
 from extremecloudiq.models.xiq_set_ssid_mode_wep_request import XiqSetSsidModeWepRequest
 from extremecloudiq.models.xiq_sms_log import XiqSmsLog
 from extremecloudiq.models.xiq_sms_log_status import XiqSmsLogStatus
 from extremecloudiq.models.xiq_sms_template import XiqSmsTemplate
@@ -364,14 +368,18 @@
 from extremecloudiq.models.xiq_viq import XiqViq
 from extremecloudiq.models.xiq_viq_license import XiqViqLicense
 from extremecloudiq.models.xiq_vlan_object_classified_entry import XiqVlanObjectClassifiedEntry
 from extremecloudiq.models.xiq_vlan_profile import XiqVlanProfile
 from extremecloudiq.models.xiq_vlan_profile_filter import XiqVlanProfileFilter
 from extremecloudiq.models.xiq_voss_devices import XiqVossDevices
 from extremecloudiq.models.xiq_webhook_subscription import XiqWebhookSubscription
+from extremecloudiq.models.xiq_wifi_capacity_client_list_response import XiqWifiCapacityClientListResponse
+from extremecloudiq.models.xiq_wifi_capacity_stats_response import XiqWifiCapacityStatsResponse
+from extremecloudiq.models.xiq_wifi_efficiency_client_list_response import XiqWifiEfficiencyClientListResponse
+from extremecloudiq.models.xiq_wifi_efficiency_stats_response import XiqWifiEfficiencyStatsResponse
 from extremecloudiq.models.xiq_wing_devices import XiqWingDevices
 from extremecloudiq.models.xiq_wired_event_entity import XiqWiredEventEntity
 from extremecloudiq.models.xiq_wired_hardware_entity import XiqWiredHardwareEntity
 from extremecloudiq.models.xiq_wired_hardware_response import XiqWiredHardwareResponse
 from extremecloudiq.models.xiq_wired_quality_index_response import XiqWiredQualityIndexResponse
 from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType
 from extremecloudiq.models.xiq_wireless_apps_response import XiqWirelessAppsResponse
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/inline_object.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/inline_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_accounting_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_accounting_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_active_directory_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_alert.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_application.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_audit_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_auth_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_certificate.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_classification_rule.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_client.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cloud_config_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_connectivity_experience_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_credential_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_credential_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cwp.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cwp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device_alarm.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device_alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_digital_twin_products.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_email_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_end_user.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_end_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_user.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ldap_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ldap_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_network_policy.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_network_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radio_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_sms_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_sms_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ssid.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ssid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_group.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_mode.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_accounting_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_category.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_category.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_group_query.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_group_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_severity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomalies_count_vo_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomalies_count_vo_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_device_entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -40,32 +40,38 @@
         'wired': 'bool',
         'anomaly_id': 'str',
         'severity': 'XiqAnomalySeverity',
         'summary': 'str',
         'last_detected_time': 'int',
         'recommended_action': 'str',
         'anomaly_subtypes': 'str',
-        'interface_name': 'str'
+        'interface_name': 'str',
+        'channel_mode': 'str',
+        'channel': 'int',
+        'frequency': 'str'
     }
 
     attribute_map = {
         'device_id': 'device_id',
         'device_name': 'device_name',
         'pinned': 'pinned',
         'wired': 'wired',
         'anomaly_id': 'anomaly_id',
         'severity': 'severity',
         'summary': 'summary',
         'last_detected_time': 'last_detected_time',
         'recommended_action': 'recommended_action',
         'anomaly_subtypes': 'anomaly_subtypes',
-        'interface_name': 'interface_name'
+        'interface_name': 'interface_name',
+        'channel_mode': 'channel_mode',
+        'channel': 'channel',
+        'frequency': 'frequency'
     }
 
-    def __init__(self, device_id=None, device_name=None, pinned=None, wired=None, anomaly_id=None, severity=None, summary=None, last_detected_time=None, recommended_action=None, anomaly_subtypes=None, interface_name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, device_id=None, device_name=None, pinned=None, wired=None, anomaly_id=None, severity=None, summary=None, last_detected_time=None, recommended_action=None, anomaly_subtypes=None, interface_name=None, channel_mode=None, channel=None, frequency=None, local_vars_configuration=None):  # noqa: E501
         """XiqAnomalyDeviceEntity - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._device_id = None
         self._device_name = None
@@ -74,14 +80,17 @@
         self._anomaly_id = None
         self._severity = None
         self._summary = None
         self._last_detected_time = None
         self._recommended_action = None
         self._anomaly_subtypes = None
         self._interface_name = None
+        self._channel_mode = None
+        self._channel = None
+        self._frequency = None
         self.discriminator = None
 
         if device_id is not None:
             self.device_id = device_id
         if device_name is not None:
             self.device_name = device_name
         if pinned is not None:
@@ -98,14 +107,20 @@
             self.last_detected_time = last_detected_time
         if recommended_action is not None:
             self.recommended_action = recommended_action
         if anomaly_subtypes is not None:
             self.anomaly_subtypes = anomaly_subtypes
         if interface_name is not None:
             self.interface_name = interface_name
+        if channel_mode is not None:
+            self.channel_mode = channel_mode
+        if channel is not None:
+            self.channel = channel
+        if frequency is not None:
+            self.frequency = frequency
 
     @property
     def device_id(self):
         """Gets the device_id of this XiqAnomalyDeviceEntity.  # noqa: E501
 
         the device id  # noqa: E501
 
@@ -350,14 +365,83 @@
 
         :param interface_name: The interface_name of this XiqAnomalyDeviceEntity.  # noqa: E501
         :type: str
         """
 
         self._interface_name = interface_name
 
+    @property
+    def channel_mode(self):
+        """Gets the channel_mode of this XiqAnomalyDeviceEntity.  # noqa: E501
+
+        the channel mode : tx or rx  # noqa: E501
+
+        :return: The channel_mode of this XiqAnomalyDeviceEntity.  # noqa: E501
+        :rtype: str
+        """
+        return self._channel_mode
+
+    @channel_mode.setter
+    def channel_mode(self, channel_mode):
+        """Sets the channel_mode of this XiqAnomalyDeviceEntity.
+
+        the channel mode : tx or rx  # noqa: E501
+
+        :param channel_mode: The channel_mode of this XiqAnomalyDeviceEntity.  # noqa: E501
+        :type: str
+        """
+
+        self._channel_mode = channel_mode
+
+    @property
+    def channel(self):
+        """Gets the channel of this XiqAnomalyDeviceEntity.  # noqa: E501
+
+        the channel number  # noqa: E501
+
+        :return: The channel of this XiqAnomalyDeviceEntity.  # noqa: E501
+        :rtype: int
+        """
+        return self._channel
+
+    @channel.setter
+    def channel(self, channel):
+        """Sets the channel of this XiqAnomalyDeviceEntity.
+
+        the channel number  # noqa: E501
+
+        :param channel: The channel of this XiqAnomalyDeviceEntity.  # noqa: E501
+        :type: int
+        """
+
+        self._channel = channel
+
+    @property
+    def frequency(self):
+        """Gets the frequency of this XiqAnomalyDeviceEntity.  # noqa: E501
+
+        the frequency  # noqa: E501
+
+        :return: The frequency of this XiqAnomalyDeviceEntity.  # noqa: E501
+        :rtype: str
+        """
+        return self._frequency
+
+    @frequency.setter
+    def frequency(self, frequency):
+        """Sets the frequency of this XiqAnomalyDeviceEntity.
+
+        the frequency  # noqa: E501
+
+        :param frequency: The frequency of this XiqAnomalyDeviceEntity.  # noqa: E501
+        :type: str
+        """
+
+        self._frequency = frequency
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_location_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_severity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_api_token_info.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_api_token_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_protocol.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_rule.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_top_clients_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_country_code_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assurance_scans_overview_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assurance_scans_overview_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_category.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_auth_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_data.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_operation_result.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_operation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_building.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_ibeacon_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_os_mode_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_rule.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_output.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_response_code.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_response_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_summary.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_usage.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_view.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cloud_config_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_view_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wired_events_score_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_country_code.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_country_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_building_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_building_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_rule_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_end_user_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_floor_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_location_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_organization_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_organization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_group_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_webhook_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_credential_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_credential_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cwp.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cwp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_data_point.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_data_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_unit_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_unit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_default_device_password.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_default_device_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delivery_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delivery_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dell_devices.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dell_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_overview.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_policy.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_admin_state.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_admin_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_alarm.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_cpu_memory_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_filter.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_function.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_ibeacon.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_ibeacon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_installation_report.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_installation_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_lldp_cdp_info.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_lldp_cdp_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location_assignment.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_null_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_db_location.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqDeviceNullField(object):
+class XiqPasswordDbLocation(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    LOCATION_ID = "LOCATION_ID"
-    NETWORK_POLICY_ID = "NETWORK_POLICY_ID"
+    CLOUD = "CLOUD"
+    LOCAL = "LOCAL"
 
-    allowable_values = [LOCATION_ID, NETWORK_POLICY_ID]  # noqa: E501
+    allowable_values = [CLOUD, LOCAL]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqDeviceNullField - a model defined in OpenAPI"""  # noqa: E501
+        """XiqPasswordDbLocation - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqDeviceNullField):
+        if not isinstance(other, XiqPasswordDbLocation):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqDeviceNullField):
+        if not isinstance(other, XiqPasswordDbLocation):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_sort_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_stats.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_view.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_wifi_interface.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_wifi_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_changes_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_changes_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_stats_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_stats_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_device.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_devices.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_feat_license.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_feat_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_make.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_model.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_products.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_vim_module.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_vim_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_duplex_data_rate_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_duplex_data_rate_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_template.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_end_user.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_end_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_entitlement_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_entitlement_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_error.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_exos_devices.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_exos_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_action_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_action_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_account.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_radius_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_extreme_devices.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_extreme_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_activate_option.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_activate_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_upgrade_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_flap_count_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_flap_count_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_floor.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_forensic_bucket.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_forensic_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_get_port_assignment_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_grant_external_user_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_grant_external_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_context.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_initialize_location_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_initialize_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_protocol_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server_verification_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_mode.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_legend.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_measurement_unit.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_measurement_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_view.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_device_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_metadata.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_object.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_character_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_character_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_db_location.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqPasswordDbLocation(object):
+class XiqPasswordType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    CLOUD = "CLOUD"
-    LOCAL = "LOCAL"
+    PPSK = "PPSK"
+    RADIUS = "RADIUS"
 
-    allowable_values = [CLOUD, LOCAL]  # noqa: E501
+    allowable_values = [PPSK, RADIUS]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqPasswordDbLocation - a model defined in OpenAPI"""  # noqa: E501
+        """XiqPasswordType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqPasswordDbLocation):
+        if not isinstance(other, XiqPasswordType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqPasswordDbLocation):
+        if not isinstance(other, XiqPasswordType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqPasswordType(object):
+class XiqSortField(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    PPSK = "PPSK"
-    RADIUS = "RADIUS"
+    NAME = "NAME"
+    QUALITY_INDEX = "QUALITY_INDEX"
 
-    allowable_values = [PPSK, RADIUS]  # noqa: E501
+    allowable_values = [NAME, QUALITY_INDEX]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqPasswordType - a model defined in OpenAPI"""  # noqa: E501
+        """XiqSortField - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqPasswordType):
+        if not isinstance(other, XiqSortField):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqPasswordType):
+        if not isinstance(other, XiqSortField):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_if_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqPcgType(object):
+class XiqWirelessIfName(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    AP_BASED = "AP_BASED"
-    KEY_BASED = "KEY_BASED"
+    WIFI0 = "WIFI0"
+    WIFI1 = "WIFI1"
 
-    allowable_values = [AP_BASED, KEY_BASED]  # noqa: E501
+    allowable_values = [WIFI0, WIFI1]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqPcgType - a model defined in OpenAPI"""  # noqa: E501
+        """XiqWirelessIfName - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqPcgType):
+        if not isinstance(other, XiqWirelessIfName):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqPcgType):
+        if not isinstance(other, XiqWirelessIfName):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_permission.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_poe_flapping_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_stats_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_post_expiration_action.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_post_expiration_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_psk_generation_method.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_psk_generation_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_mode.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_format_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_server_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_server_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_regenerate_end_user_password_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rf_environment_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rf_environment_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_channel_selection.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_channel_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_mac_oui_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_miscellaneous_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_neighborhood_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_radio_usage_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_sensor_scan_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_wmm_qos_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_server_role.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_server_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_template.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_field.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_null_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqSortField(object):
+class XiqDeviceNullField(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    NAME = "NAME"
-    QUALITY_INDEX = "QUALITY_INDEX"
+    LOCATION_ID = "LOCATION_ID"
+    NETWORK_POLICY_ID = "NETWORK_POLICY_ID"
 
-    allowable_values = [NAME, QUALITY_INDEX]  # noqa: E501
+    allowable_values = [LOCATION_ID, NETWORK_POLICY_ID]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqSortField - a model defined in OpenAPI"""  # noqa: E501
+        """XiqDeviceNullField - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqSortField):
+        if not isinstance(other, XiqDeviceNullField):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqSortField):
+        if not isinstance(other, XiqDeviceNullField):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_order.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_speed_duplex_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_speed_duplex_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_key_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_key_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_key_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_ppsk_key_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_encryption_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_sae_group.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_sae_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_authentication_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_default_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_encryption_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_data_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_data_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_message_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_message_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_top_applications_usage.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_top_applications_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_trend_indicator.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_trend_indicator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_building_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_building_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_rule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_cloud_config_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_device_level_ssid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_end_user_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_user_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_floor_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_floor_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_location_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_channel_selection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_group_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_profile_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_group.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_role.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_daily_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_daily_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_during_date_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_for_time_period_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_first_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq_license.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_object_classified_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_voss_devices.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_voss_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_webhook_subscription.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_webhook_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wing_devices.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wing_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_event_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_quality_index_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_view_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_view_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_apps_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_apps_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_event_retries_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_if_name.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_health_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqWirelessIfName(object):
+class XiqAnomalyHealthType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    WIFI0 = "WIFI0"
-    WIFI1 = "WIFI1"
+    NONE = "NONE"
+    GOOD = "GOOD"
+    MEDIUM = "MEDIUM"
+    POOR = "POOR"
 
-    allowable_values = [WIFI0, WIFI1]  # noqa: E501
+    allowable_values = [NONE, GOOD, MEDIUM, POOR]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +46,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqWirelessIfName - a model defined in OpenAPI"""  # noqa: E501
+        """XiqAnomalyHealthType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqWirelessIfName):
+        if not isinstance(other, XiqAnomalyHealthType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqWirelessIfName):
+        if not isinstance(other, XiqAnomalyHealthType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_retries_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_quality_index_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_list_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_type_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/__init__.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "23.3.1.15"
+__version__ = "23.3.2.1"
 
 # import apis into sdk package
 from extremecloudiq.api.account_api import AccountApi
 from extremecloudiq.api.alert_api import AlertApi
 from extremecloudiq.api.application_api import ApplicationApi
 from extremecloudiq.api.authentication_api import AuthenticationApi
 from extremecloudiq.api.authorization_api import AuthorizationApi
@@ -98,14 +98,15 @@
 from extremecloudiq.models.xiq_alert_group_query import XiqAlertGroupQuery
 from extremecloudiq.models.xiq_alert_severity import XiqAlertSeverity
 from extremecloudiq.models.xiq_alert_source import XiqAlertSource
 from extremecloudiq.models.xiq_alert_source_type import XiqAlertSourceType
 from extremecloudiq.models.xiq_anomalies_count_vo_entity import XiqAnomaliesCountVoEntity
 from extremecloudiq.models.xiq_anomaly_device_entity import XiqAnomalyDeviceEntity
 from extremecloudiq.models.xiq_anomaly_devices_by_location_response import XiqAnomalyDevicesByLocationResponse
+from extremecloudiq.models.xiq_anomaly_health_type import XiqAnomalyHealthType
 from extremecloudiq.models.xiq_anomaly_location_entity import XiqAnomalyLocationEntity
 from extremecloudiq.models.xiq_anomaly_severity import XiqAnomalySeverity
 from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField
 from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType
 from extremecloudiq.models.xiq_api_token_info import XiqApiTokenInfo
 from extremecloudiq.models.xiq_application import XiqApplication
 from extremecloudiq.models.xiq_application_detection_protocol import XiqApplicationDetectionProtocol
@@ -140,14 +141,15 @@
 from extremecloudiq.models.xiq_classification_rule import XiqClassificationRule
 from extremecloudiq.models.xiq_classification_type import XiqClassificationType
 from extremecloudiq.models.xiq_cli_output import XiqCliOutput
 from extremecloudiq.models.xiq_cli_response_code import XiqCliResponseCode
 from extremecloudiq.models.xiq_client import XiqClient
 from extremecloudiq.models.xiq_client_field import XiqClientField
 from extremecloudiq.models.xiq_client_sort_field import XiqClientSortField
+from extremecloudiq.models.xiq_client_stats_entity import XiqClientStatsEntity
 from extremecloudiq.models.xiq_client_summary import XiqClientSummary
 from extremecloudiq.models.xiq_client_usage import XiqClientUsage
 from extremecloudiq.models.xiq_client_view import XiqClientView
 from extremecloudiq.models.xiq_cloud_config_group import XiqCloudConfigGroup
 from extremecloudiq.models.xiq_connectivity_experience_data import XiqConnectivityExperienceData
 from extremecloudiq.models.xiq_connectivity_experience_view_type import XiqConnectivityExperienceViewType
 from extremecloudiq.models.xiq_copilot_events_wired_sort_field import XiqCopilotEventsWiredSortField
@@ -209,14 +211,15 @@
 from extremecloudiq.models.xiq_device_level_ssid_status import XiqDeviceLevelSsidStatus
 from extremecloudiq.models.xiq_device_lldp_cdp_info import XiqDeviceLldpCdpInfo
 from extremecloudiq.models.xiq_device_location import XiqDeviceLocation
 from extremecloudiq.models.xiq_device_location_assignment import XiqDeviceLocationAssignment
 from extremecloudiq.models.xiq_device_null_field import XiqDeviceNullField
 from extremecloudiq.models.xiq_device_sort_field import XiqDeviceSortField
 from extremecloudiq.models.xiq_device_stats import XiqDeviceStats
+from extremecloudiq.models.xiq_device_stats_entity import XiqDeviceStatsEntity
 from extremecloudiq.models.xiq_device_type import XiqDeviceType
 from extremecloudiq.models.xiq_device_view import XiqDeviceView
 from extremecloudiq.models.xiq_device_wifi_interface import XiqDeviceWifiInterface
 from extremecloudiq.models.xiq_dfs_channel_changes_entity import XiqDfsChannelChangesEntity
 from extremecloudiq.models.xiq_dfs_channel_stats_entity import XiqDfsChannelStatsEntity
 from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
 from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
@@ -324,14 +327,15 @@
 from extremecloudiq.models.xiq_rp_neighborhood_analysis import XiqRpNeighborhoodAnalysis
 from extremecloudiq.models.xiq_rp_radio_usage_optimization import XiqRpRadioUsageOptimization
 from extremecloudiq.models.xiq_rp_sensor_scan_settings import XiqRpSensorScanSettings
 from extremecloudiq.models.xiq_rp_wmm_qos_settings import XiqRpWmmQosSettings
 from extremecloudiq.models.xiq_send_cli_request import XiqSendCliRequest
 from extremecloudiq.models.xiq_send_cli_response import XiqSendCliResponse
 from extremecloudiq.models.xiq_server_role import XiqServerRole
+from extremecloudiq.models.xiq_sessions_data_entity import XiqSessionsDataEntity
 from extremecloudiq.models.xiq_set_ssid_mode_dot1x_request import XiqSetSsidModeDot1xRequest
 from extremecloudiq.models.xiq_set_ssid_mode_ppsk_request import XiqSetSsidModePpskRequest
 from extremecloudiq.models.xiq_set_ssid_mode_psk_request import XiqSetSsidModePskRequest
 from extremecloudiq.models.xiq_set_ssid_mode_wep_request import XiqSetSsidModeWepRequest
 from extremecloudiq.models.xiq_sms_log import XiqSmsLog
 from extremecloudiq.models.xiq_sms_log_status import XiqSmsLogStatus
 from extremecloudiq.models.xiq_sms_template import XiqSmsTemplate
@@ -399,14 +403,18 @@
 from extremecloudiq.models.xiq_viq import XiqViq
 from extremecloudiq.models.xiq_viq_license import XiqViqLicense
 from extremecloudiq.models.xiq_vlan_object_classified_entry import XiqVlanObjectClassifiedEntry
 from extremecloudiq.models.xiq_vlan_profile import XiqVlanProfile
 from extremecloudiq.models.xiq_vlan_profile_filter import XiqVlanProfileFilter
 from extremecloudiq.models.xiq_voss_devices import XiqVossDevices
 from extremecloudiq.models.xiq_webhook_subscription import XiqWebhookSubscription
+from extremecloudiq.models.xiq_wifi_capacity_client_list_response import XiqWifiCapacityClientListResponse
+from extremecloudiq.models.xiq_wifi_capacity_stats_response import XiqWifiCapacityStatsResponse
+from extremecloudiq.models.xiq_wifi_efficiency_client_list_response import XiqWifiEfficiencyClientListResponse
+from extremecloudiq.models.xiq_wifi_efficiency_stats_response import XiqWifiEfficiencyStatsResponse
 from extremecloudiq.models.xiq_wing_devices import XiqWingDevices
 from extremecloudiq.models.xiq_wired_event_entity import XiqWiredEventEntity
 from extremecloudiq.models.xiq_wired_hardware_entity import XiqWiredHardwareEntity
 from extremecloudiq.models.xiq_wired_hardware_response import XiqWiredHardwareResponse
 from extremecloudiq.models.xiq_wired_quality_index_response import XiqWiredQualityIndexResponse
 from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType
 from extremecloudiq.models.xiq_wireless_apps_response import XiqWirelessAppsResponse
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/api_client.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/23.3.1.15/python'
+        self.user_agent = 'OpenAPI-Generator/23.3.2.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/configuration.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -333,16 +333,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.3.1.15\n"\
-               "SDK Package Version: 23.3.1.15".\
+               "Version of the API: 23.3.2.1\n"\
+               "SDK Package Version: 23.3.2.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/exceptions.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq/rest.py` & `extremecloudiq-api-23.3.2.1/extremecloudiq/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/SOURCES.txt` & `extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 extremecloudiq/models/xiq_alert_group_query.py
 extremecloudiq/models/xiq_alert_severity.py
 extremecloudiq/models/xiq_alert_source.py
 extremecloudiq/models/xiq_alert_source_type.py
 extremecloudiq/models/xiq_anomalies_count_vo_entity.py
 extremecloudiq/models/xiq_anomaly_device_entity.py
 extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
+extremecloudiq/models/xiq_anomaly_health_type.py
 extremecloudiq/models/xiq_anomaly_location_entity.py
 extremecloudiq/models/xiq_anomaly_severity.py
 extremecloudiq/models/xiq_anomaly_sort_field.py
 extremecloudiq/models/xiq_anomaly_type.py
 extremecloudiq/models/xiq_api_token_info.py
 extremecloudiq/models/xiq_application.py
 extremecloudiq/models/xiq_application_detection_protocol.py
@@ -120,14 +121,15 @@
 extremecloudiq/models/xiq_classification_rule.py
 extremecloudiq/models/xiq_classification_type.py
 extremecloudiq/models/xiq_cli_output.py
 extremecloudiq/models/xiq_cli_response_code.py
 extremecloudiq/models/xiq_client.py
 extremecloudiq/models/xiq_client_field.py
 extremecloudiq/models/xiq_client_sort_field.py
+extremecloudiq/models/xiq_client_stats_entity.py
 extremecloudiq/models/xiq_client_summary.py
 extremecloudiq/models/xiq_client_usage.py
 extremecloudiq/models/xiq_client_view.py
 extremecloudiq/models/xiq_cloud_config_group.py
 extremecloudiq/models/xiq_connectivity_experience_data.py
 extremecloudiq/models/xiq_connectivity_experience_view_type.py
 extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
@@ -189,14 +191,15 @@
 extremecloudiq/models/xiq_device_level_ssid_status.py
 extremecloudiq/models/xiq_device_lldp_cdp_info.py
 extremecloudiq/models/xiq_device_location.py
 extremecloudiq/models/xiq_device_location_assignment.py
 extremecloudiq/models/xiq_device_null_field.py
 extremecloudiq/models/xiq_device_sort_field.py
 extremecloudiq/models/xiq_device_stats.py
+extremecloudiq/models/xiq_device_stats_entity.py
 extremecloudiq/models/xiq_device_type.py
 extremecloudiq/models/xiq_device_view.py
 extremecloudiq/models/xiq_device_wifi_interface.py
 extremecloudiq/models/xiq_dfs_channel_changes_entity.py
 extremecloudiq/models/xiq_dfs_channel_stats_entity.py
 extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
 extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
@@ -304,14 +307,15 @@
 extremecloudiq/models/xiq_rp_neighborhood_analysis.py
 extremecloudiq/models/xiq_rp_radio_usage_optimization.py
 extremecloudiq/models/xiq_rp_sensor_scan_settings.py
 extremecloudiq/models/xiq_rp_wmm_qos_settings.py
 extremecloudiq/models/xiq_send_cli_request.py
 extremecloudiq/models/xiq_send_cli_response.py
 extremecloudiq/models/xiq_server_role.py
+extremecloudiq/models/xiq_sessions_data_entity.py
 extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
 extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
 extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
 extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
 extremecloudiq/models/xiq_sms_log.py
 extremecloudiq/models/xiq_sms_log_status.py
 extremecloudiq/models/xiq_sms_template.py
@@ -379,14 +383,18 @@
 extremecloudiq/models/xiq_viq.py
 extremecloudiq/models/xiq_viq_license.py
 extremecloudiq/models/xiq_vlan_object_classified_entry.py
 extremecloudiq/models/xiq_vlan_profile.py
 extremecloudiq/models/xiq_vlan_profile_filter.py
 extremecloudiq/models/xiq_voss_devices.py
 extremecloudiq/models/xiq_webhook_subscription.py
+extremecloudiq/models/xiq_wifi_capacity_client_list_response.py
+extremecloudiq/models/xiq_wifi_capacity_stats_response.py
+extremecloudiq/models/xiq_wifi_efficiency_client_list_response.py
+extremecloudiq/models/xiq_wifi_efficiency_stats_response.py
 extremecloudiq/models/xiq_wing_devices.py
 extremecloudiq/models/xiq_wired_event_entity.py
 extremecloudiq/models/xiq_wired_hardware_entity.py
 extremecloudiq/models/xiq_wired_hardware_response.py
 extremecloudiq/models/xiq_wired_quality_index_response.py
 extremecloudiq/models/xiq_wired_view_type.py
 extremecloudiq/models/xiq_wireless_apps_response.py
@@ -475,14 +483,15 @@
 test/test_xiq_alert_group_query.py
 test/test_xiq_alert_severity.py
 test/test_xiq_alert_source.py
 test/test_xiq_alert_source_type.py
 test/test_xiq_anomalies_count_vo_entity.py
 test/test_xiq_anomaly_device_entity.py
 test/test_xiq_anomaly_devices_by_location_response.py
+test/test_xiq_anomaly_health_type.py
 test/test_xiq_anomaly_location_entity.py
 test/test_xiq_anomaly_severity.py
 test/test_xiq_anomaly_sort_field.py
 test/test_xiq_anomaly_type.py
 test/test_xiq_api_token_info.py
 test/test_xiq_application.py
 test/test_xiq_application_detection_protocol.py
@@ -517,14 +526,15 @@
 test/test_xiq_classification_rule.py
 test/test_xiq_classification_type.py
 test/test_xiq_cli_output.py
 test/test_xiq_cli_response_code.py
 test/test_xiq_client.py
 test/test_xiq_client_field.py
 test/test_xiq_client_sort_field.py
+test/test_xiq_client_stats_entity.py
 test/test_xiq_client_summary.py
 test/test_xiq_client_usage.py
 test/test_xiq_client_view.py
 test/test_xiq_cloud_config_group.py
 test/test_xiq_connectivity_experience_data.py
 test/test_xiq_connectivity_experience_view_type.py
 test/test_xiq_copilot_events_wired_sort_field.py
@@ -586,14 +596,15 @@
 test/test_xiq_device_level_ssid_status.py
 test/test_xiq_device_lldp_cdp_info.py
 test/test_xiq_device_location.py
 test/test_xiq_device_location_assignment.py
 test/test_xiq_device_null_field.py
 test/test_xiq_device_sort_field.py
 test/test_xiq_device_stats.py
+test/test_xiq_device_stats_entity.py
 test/test_xiq_device_type.py
 test/test_xiq_device_view.py
 test/test_xiq_device_wifi_interface.py
 test/test_xiq_dfs_channel_changes_entity.py
 test/test_xiq_dfs_channel_stats_entity.py
 test/test_xiq_dfs_recurence_channel_stats_response.py
 test/test_xiq_dfs_recurence_count_stats_response.py
@@ -701,14 +712,15 @@
 test/test_xiq_rp_neighborhood_analysis.py
 test/test_xiq_rp_radio_usage_optimization.py
 test/test_xiq_rp_sensor_scan_settings.py
 test/test_xiq_rp_wmm_qos_settings.py
 test/test_xiq_send_cli_request.py
 test/test_xiq_send_cli_response.py
 test/test_xiq_server_role.py
+test/test_xiq_sessions_data_entity.py
 test/test_xiq_set_ssid_mode_dot1x_request.py
 test/test_xiq_set_ssid_mode_ppsk_request.py
 test/test_xiq_set_ssid_mode_psk_request.py
 test/test_xiq_set_ssid_mode_wep_request.py
 test/test_xiq_sms_log.py
 test/test_xiq_sms_log_status.py
 test/test_xiq_sms_template.py
@@ -776,14 +788,18 @@
 test/test_xiq_viq.py
 test/test_xiq_viq_license.py
 test/test_xiq_vlan_object_classified_entry.py
 test/test_xiq_vlan_profile.py
 test/test_xiq_vlan_profile_filter.py
 test/test_xiq_voss_devices.py
 test/test_xiq_webhook_subscription.py
+test/test_xiq_wifi_capacity_client_list_response.py
+test/test_xiq_wifi_capacity_stats_response.py
+test/test_xiq_wifi_efficiency_client_list_response.py
+test/test_xiq_wifi_efficiency_stats_response.py
 test/test_xiq_wing_devices.py
 test/test_xiq_wired_event_entity.py
 test/test_xiq_wired_hardware_entity.py
 test/test_xiq_wired_hardware_response.py
 test/test_xiq_wired_quality_index_response.py
 test/test_xiq_wired_view_type.py
 test/test_xiq_wireless_apps_response.py
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_account_api.py` & `extremecloudiq-api-23.3.2.1/test/test_account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_alert_api.py` & `extremecloudiq-api-23.3.2.1/test/test_alert_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_application_api.py` & `extremecloudiq-api-23.3.2.1/test/test_application_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_authentication_api.py` & `extremecloudiq-api-23.3.2.1/test/test_authentication_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_authorization_api.py` & `extremecloudiq-api-23.3.2.1/test/test_authorization_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_client_api.py` & `extremecloudiq-api-23.3.2.1/test/test_client_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_configuration___authentication_api.py` & `extremecloudiq-api-23.3.2.1/test/test_configuration___authentication_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_configuration___basic_api.py` & `extremecloudiq-api-23.3.2.1/test/test_configuration___basic_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_configuration___certificate_api.py` & `extremecloudiq-api-23.3.2.1/test/test_configuration___certificate_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_configuration___deployment_api.py` & `extremecloudiq-api-23.3.2.1/test/test_configuration___deployment_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_configuration___policy_api.py` & `extremecloudiq-api-23.3.2.1/test/test_configuration___policy_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_configuration___user_management_api.py` & `extremecloudiq-api-23.3.2.1/test/test_configuration___user_management_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_copilot___anomalies_api.py` & `extremecloudiq-api-23.3.2.1/test/test_copilot___anomalies_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -79,14 +79,38 @@
 
     def test_get_port_efficiency_stats(self):
         """Test case for get_port_efficiency_stats
 
         """
         pass
 
+    def test_get_wifi_capacity_client_list(self):
+        """Test case for get_wifi_capacity_client_list
+
+        """
+        pass
+
+    def test_get_wifi_capacity_stats(self):
+        """Test case for get_wifi_capacity_stats
+
+        """
+        pass
+
+    def test_get_wifi_efficiency_client_list(self):
+        """Test case for get_wifi_efficiency_client_list
+
+        """
+        pass
+
+    def test_get_wifi_efficiency_stats(self):
+        """Test case for get_wifi_efficiency_stats
+
+        """
+        pass
+
     def test_list_anomaly_locations(self):
         """Test case for list_anomaly_locations
 
         """
         pass
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.3.2.1/test/test_copilot___connectivity_experience_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_device_api.py` & `extremecloudiq-api-23.3.2.1/test/test_device_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_hiq_api.py` & `extremecloudiq-api-23.3.2.1/test/test_hiq_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_inline_object.py` & `extremecloudiq-api-23.3.2.1/test/test_inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_location_api.py` & `extremecloudiq-api-23.3.2.1/test/test_location_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_log_api.py` & `extremecloudiq-api-23.3.2.1/test/test_log_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_network_policy_api.py` & `extremecloudiq-api-23.3.2.1/test/test_network_policy_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_notification_api.py` & `extremecloudiq-api-23.3.2.1/test/test_notification_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_operation_api.py` & `extremecloudiq-api-23.3.2.1/test/test_operation_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_accounting_log.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_active_directory_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_alert.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_application.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_audit_log.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_audit_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_auth_log.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_auth_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_certificate.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_classification_rule.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_client.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cloud_config_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_connectivity_experience_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_credential_log.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_credential_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cwp.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cwp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device_alarm.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device_alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_digital_twin_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_email_log.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_email_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_end_user.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_end_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_radius_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_user.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ldap_server.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ldap_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_network_policy.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_network_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radio_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radio_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_client_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_rp_mac_oui_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_sms_log.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ssid.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ssid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_group.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_user_api.py` & `extremecloudiq-api-23.3.2.1/test/test_user_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_account.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_account_mode.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_account_mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_account_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_account_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_accounting_log.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_accounting_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_alert.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_alert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_category.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_category.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_group_query.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_group_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_severity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_severity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_anomalies_count_vo_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_anomalies_count_vo_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_device_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -43,15 +43,18 @@
                 wired = True, 
                 anomaly_id = '0', 
                 severity = 'NONE', 
                 summary = '0', 
                 last_detected_time = 56, 
                 recommended_action = '0', 
                 anomaly_subtypes = '0', 
-                interface_name = '0'
+                interface_name = '0', 
+                channel_mode = '0', 
+                channel = 56, 
+                frequency = '0'
             )
         else :
             return XiqAnomalyDeviceEntity(
         )
 
     def testXiqAnomalyDeviceEntity(self):
         """Test XiqAnomalyDeviceEntity"""
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_devices_by_location_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -57,15 +57,18 @@
                         wired = True, 
                         anomaly_id = '0', 
                         severity = 'NONE', 
                         summary = '0', 
                         last_detected_time = 56, 
                         recommended_action = '0', 
                         anomaly_subtypes = '0', 
-                        interface_name = '0', )
+                        interface_name = '0', 
+                        channel_mode = '0', 
+                        channel = 56, 
+                        frequency = '0', )
                     ]
             )
         else :
             return XiqAnomalyDevicesByLocationResponse(
         )
 
     def testXiqAnomalyDevicesByLocationResponse(self):
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_location_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_severity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_sort_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_api_token_info.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_api_token_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_application.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_protocol.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_rule.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_application_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_application_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_application_top_clients_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_country_code_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_location_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_network_policy_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_assurance_scans_overview_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_assurance_scans_overview_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_category.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_category.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_auth_log.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_auth_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_data.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_operation_result.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_operation_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_building.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_building.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_certificate.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_certificate_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_certificate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_ibeacon_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_os_mode_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_classification.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_classification_rule.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_classification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_classification_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_classification_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_cli_output.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_cli_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_cli_response_code.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_cli_response_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_client.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_client_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_client_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_client_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_client_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_client_summary.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_client_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_client_usage.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_client_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_client_view.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_client_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_view_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wired_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wireless_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wired_events_score_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_events_score_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_country_code.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_country_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_building_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_building_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_rule_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_cloud_config_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_end_user_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_end_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_external_radius_server_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_floor_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_floor_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_internal_radius_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_key_based_pcg_users_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_ldap_server_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_location_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_location_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_organization_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_organization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client_object_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_rp_mac_oui_profile_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_group_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_profile_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_object_classified_entry_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_profile_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_create_webhook_subscription_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_credential_log.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_credential_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_cwp.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_cwp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_data_point.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_data_point.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_unit_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_unit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_default_device_password.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_default_device_password.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_delete_key_based_pcg_users_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_delivery_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_delivery_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_dell_devices.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_dell_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_overview.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_policy.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_admin_state.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_admin_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_alarm.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_alarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_cpu_memory_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_filter.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_function.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_ibeacon.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_ibeacon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_installation_report.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_installation_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_lldp_cdp_info.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_lldp_cdp_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_location.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_location_assignment.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_location_assignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_null_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_null_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_stats.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_view.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_device_wifi_interface.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_device_wifi_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_changes_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_changes_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_stats_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_stats_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_channel_stats_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_channel_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_count_stats_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_count_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_device.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_devices.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_feat_license.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_feat_license.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_make.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_make.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_model.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_products.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_vim_module.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_vim_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_duplex_data_rate_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_duplex_data_rate_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_email_log.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_email_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_email_template.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_email_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_end_user.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_end_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_entitlement_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_entitlement_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_error.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_exos_devices.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_exos_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_action_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_action_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_external_account.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_external_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_external_radius_server.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_extreme_devices.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_extreme_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_activate_option.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_activate_option.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_upgrade_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_flap_count_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_flap_count_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_floor.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_floor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_forensic_bucket.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_forensic_bucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_get_port_assignment_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_grant_external_user_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_grant_external_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_context.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_init_key_based_pcg_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_initialize_location_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_initialize_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user_base_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_protocol_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server_verification_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_license_mode.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_license_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_license_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_license_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_location.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_location_legend.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_location_legend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_location_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_location_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_login_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_login_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_login_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_measurement_unit.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_measurement_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_view.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_device_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_key_based_pcg_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_operation_metadata.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_operation_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_operation_object.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_operation_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_operation_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_organization.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_organization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_organization_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_organization_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_password_character_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_password_character_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_password_db_location.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_password_db_location.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_password_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_password_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_password_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_password_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_permission.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_poe_flapping_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_speed_duplex_stats_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_speed_duplex_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_stats_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_post_expiration_action.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_post_expiration_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_psk_generation_method.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_psk_generation_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radio_mode.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radio_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radio_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radio_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_format_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_server_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_server_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_regenerate_end_user_password_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rf_environment_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rf_environment_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_channel_selection.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_channel_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_mac_oui_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_miscellaneous_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_neighborhood_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_radio_usage_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_sensor_scan_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_wmm_qos_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_server_role.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_server_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_dot1x_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_ppsk_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_psk_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_wep_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_sms_template.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_sms_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_sort_field.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_sort_order.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_sort_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_speed_duplex_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_speed_duplex_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_key_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_key_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_ppsk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_sae_group.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_sae_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_default_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_encryption_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_key_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_data_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_data_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_message_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_message_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_top_applications_usage.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_top_applications_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_trend_indicator.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_trend_indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_building_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_building_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_rule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_device_level_ssid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_end_user_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_radius_server_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_user_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_floor_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_key_based_pcg_users_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_ldap_server_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_location_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_network_policy_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radio_profile_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client_object_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_channel_selection_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_mac_oui_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_group_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_profile_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_object_classified_entry_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_user.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_user_group.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_user_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_user_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_user_role.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_user_role.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_daily_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_daily_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_during_date_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_for_time_period_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_first_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_id_creation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_viq.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_viq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_viq_license.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_viq_license.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_object_classified_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_voss_devices.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_voss_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_webhook_subscription.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_webhook_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wing_devices.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wing_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_quality_index_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_view_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_view_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_apps_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_apps_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_connectivity_performance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_event_retries_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_if_name.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_if_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_retries_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_quality_index_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_list_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_type_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.1.15/README.md` & `extremecloudiq-api-23.3.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # extremecloudiq-api
 ExtremeCloud IQ RESTful API for external and internal applications.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 23.3.1.15
-- Package version: 23.3.1.15
+- API version: 23.3.2.1
+- Package version: 23.3.2.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.extremenetworks.com/support](https://www.extremenetworks.com/support)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -233,14 +233,18 @@
 *CopilotAnomaliesApi* | [**get_atp_packet_counts**](docs/CopilotAnomaliesApi.md#get_atp_packet_counts) | **GET** /copilot/anomalies/adverse-traffic/packet-counts | 
 *CopilotAnomaliesApi* | [**get_devices_by_location**](docs/CopilotAnomaliesApi.md#get_devices_by_location) | **GET** /copilot/anomalies/devices-by-location | 
 *CopilotAnomaliesApi* | [**get_dfs_recurrence_channel_stats**](docs/CopilotAnomaliesApi.md#get_dfs_recurrence_channel_stats) | **GET** /copilot/anomalies/dfs-recurrence/channel-stats | 
 *CopilotAnomaliesApi* | [**get_dfs_recurrence_count_stats**](docs/CopilotAnomaliesApi.md#get_dfs_recurrence_count_stats) | **GET** /copilot/anomalies/dfs-recurrence/count-stats | 
 *CopilotAnomaliesApi* | [**get_poe_flapping_stats**](docs/CopilotAnomaliesApi.md#get_poe_flapping_stats) | **GET** /copilot/anomalies/poeflapping/stats | 
 *CopilotAnomaliesApi* | [**get_port_efficiency_speed_duplex_stats**](docs/CopilotAnomaliesApi.md#get_port_efficiency_speed_duplex_stats) | **GET** /copilot/anomalies/port-efficiency/speed-duplex-stats | 
 *CopilotAnomaliesApi* | [**get_port_efficiency_stats**](docs/CopilotAnomaliesApi.md#get_port_efficiency_stats) | **GET** /copilot/anomalies/port-efficiency/stats | 
+*CopilotAnomaliesApi* | [**get_wifi_capacity_client_list**](docs/CopilotAnomaliesApi.md#get_wifi_capacity_client_list) | **GET** /copilot/anomalies/wifi-capacity/client-list | 
+*CopilotAnomaliesApi* | [**get_wifi_capacity_stats**](docs/CopilotAnomaliesApi.md#get_wifi_capacity_stats) | **GET** /copilot/anomalies/wifi-capacity/stats | 
+*CopilotAnomaliesApi* | [**get_wifi_efficiency_client_list**](docs/CopilotAnomaliesApi.md#get_wifi_efficiency_client_list) | **GET** /copilot/anomalies/wifi-efficiency/client-list | 
+*CopilotAnomaliesApi* | [**get_wifi_efficiency_stats**](docs/CopilotAnomaliesApi.md#get_wifi_efficiency_stats) | **GET** /copilot/anomalies/wifi-efficiency/stats | 
 *CopilotAnomaliesApi* | [**list_anomaly_locations**](docs/CopilotAnomaliesApi.md#list_anomaly_locations) | **GET** /copilot/anomalies/locations | 
 *CopilotConnectivityExperienceApi* | [**get_wired_connectivity_experience**](docs/CopilotConnectivityExperienceApi.md#get_wired_connectivity_experience) | **GET** /copilot/connectivity/wired/experience | 
 *CopilotConnectivityExperienceApi* | [**get_wired_events**](docs/CopilotConnectivityExperienceApi.md#get_wired_events) | **GET** /copilot/connectivity/wired/events | 
 *CopilotConnectivityExperienceApi* | [**get_wired_hardware**](docs/CopilotConnectivityExperienceApi.md#get_wired_hardware) | **GET** /copilot/connectivity/wired/hardware | 
 *CopilotConnectivityExperienceApi* | [**get_wired_quality_index**](docs/CopilotConnectivityExperienceApi.md#get_wired_quality_index) | **GET** /copilot/connectivity/wired/quality-index | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_apps**](docs/CopilotConnectivityExperienceApi.md#get_wireless_apps) | **GET** /copilot/connectivity/wireless/apps | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_connectivity_experience**](docs/CopilotConnectivityExperienceApi.md#get_wireless_connectivity_experience) | **GET** /copilot/connectivity/wireless/experience | 
@@ -400,14 +404,15 @@
  - [XiqAlertGroupQuery](docs/XiqAlertGroupQuery.md)
  - [XiqAlertSeverity](docs/XiqAlertSeverity.md)
  - [XiqAlertSource](docs/XiqAlertSource.md)
  - [XiqAlertSourceType](docs/XiqAlertSourceType.md)
  - [XiqAnomaliesCountVoEntity](docs/XiqAnomaliesCountVoEntity.md)
  - [XiqAnomalyDeviceEntity](docs/XiqAnomalyDeviceEntity.md)
  - [XiqAnomalyDevicesByLocationResponse](docs/XiqAnomalyDevicesByLocationResponse.md)
+ - [XiqAnomalyHealthType](docs/XiqAnomalyHealthType.md)
  - [XiqAnomalyLocationEntity](docs/XiqAnomalyLocationEntity.md)
  - [XiqAnomalySeverity](docs/XiqAnomalySeverity.md)
  - [XiqAnomalySortField](docs/XiqAnomalySortField.md)
  - [XiqAnomalyType](docs/XiqAnomalyType.md)
  - [XiqApiTokenInfo](docs/XiqApiTokenInfo.md)
  - [XiqApplication](docs/XiqApplication.md)
  - [XiqApplicationDetectionProtocol](docs/XiqApplicationDetectionProtocol.md)
@@ -442,14 +447,15 @@
  - [XiqClassificationRule](docs/XiqClassificationRule.md)
  - [XiqClassificationType](docs/XiqClassificationType.md)
  - [XiqCliOutput](docs/XiqCliOutput.md)
  - [XiqCliResponseCode](docs/XiqCliResponseCode.md)
  - [XiqClient](docs/XiqClient.md)
  - [XiqClientField](docs/XiqClientField.md)
  - [XiqClientSortField](docs/XiqClientSortField.md)
+ - [XiqClientStatsEntity](docs/XiqClientStatsEntity.md)
  - [XiqClientSummary](docs/XiqClientSummary.md)
  - [XiqClientUsage](docs/XiqClientUsage.md)
  - [XiqClientView](docs/XiqClientView.md)
  - [XiqCloudConfigGroup](docs/XiqCloudConfigGroup.md)
  - [XiqConnectivityExperienceData](docs/XiqConnectivityExperienceData.md)
  - [XiqConnectivityExperienceViewType](docs/XiqConnectivityExperienceViewType.md)
  - [XiqCopilotEventsWiredSortField](docs/XiqCopilotEventsWiredSortField.md)
@@ -511,14 +517,15 @@
  - [XiqDeviceLevelSsidStatus](docs/XiqDeviceLevelSsidStatus.md)
  - [XiqDeviceLldpCdpInfo](docs/XiqDeviceLldpCdpInfo.md)
  - [XiqDeviceLocation](docs/XiqDeviceLocation.md)
  - [XiqDeviceLocationAssignment](docs/XiqDeviceLocationAssignment.md)
  - [XiqDeviceNullField](docs/XiqDeviceNullField.md)
  - [XiqDeviceSortField](docs/XiqDeviceSortField.md)
  - [XiqDeviceStats](docs/XiqDeviceStats.md)
+ - [XiqDeviceStatsEntity](docs/XiqDeviceStatsEntity.md)
  - [XiqDeviceType](docs/XiqDeviceType.md)
  - [XiqDeviceView](docs/XiqDeviceView.md)
  - [XiqDeviceWifiInterface](docs/XiqDeviceWifiInterface.md)
  - [XiqDfsChannelChangesEntity](docs/XiqDfsChannelChangesEntity.md)
  - [XiqDfsChannelStatsEntity](docs/XiqDfsChannelStatsEntity.md)
  - [XiqDfsRecurenceChannelStatsResponse](docs/XiqDfsRecurenceChannelStatsResponse.md)
  - [XiqDfsRecurenceCountStatsResponse](docs/XiqDfsRecurenceCountStatsResponse.md)
@@ -626,14 +633,15 @@
  - [XiqRpNeighborhoodAnalysis](docs/XiqRpNeighborhoodAnalysis.md)
  - [XiqRpRadioUsageOptimization](docs/XiqRpRadioUsageOptimization.md)
  - [XiqRpSensorScanSettings](docs/XiqRpSensorScanSettings.md)
  - [XiqRpWmmQosSettings](docs/XiqRpWmmQosSettings.md)
  - [XiqSendCliRequest](docs/XiqSendCliRequest.md)
  - [XiqSendCliResponse](docs/XiqSendCliResponse.md)
  - [XiqServerRole](docs/XiqServerRole.md)
+ - [XiqSessionsDataEntity](docs/XiqSessionsDataEntity.md)
  - [XiqSetSsidModeDot1xRequest](docs/XiqSetSsidModeDot1xRequest.md)
  - [XiqSetSsidModePpskRequest](docs/XiqSetSsidModePpskRequest.md)
  - [XiqSetSsidModePskRequest](docs/XiqSetSsidModePskRequest.md)
  - [XiqSetSsidModeWepRequest](docs/XiqSetSsidModeWepRequest.md)
  - [XiqSmsLog](docs/XiqSmsLog.md)
  - [XiqSmsLogStatus](docs/XiqSmsLogStatus.md)
  - [XiqSmsTemplate](docs/XiqSmsTemplate.md)
@@ -701,14 +709,18 @@
  - [XiqViq](docs/XiqViq.md)
  - [XiqViqLicense](docs/XiqViqLicense.md)
  - [XiqVlanObjectClassifiedEntry](docs/XiqVlanObjectClassifiedEntry.md)
  - [XiqVlanProfile](docs/XiqVlanProfile.md)
  - [XiqVlanProfileFilter](docs/XiqVlanProfileFilter.md)
  - [XiqVossDevices](docs/XiqVossDevices.md)
  - [XiqWebhookSubscription](docs/XiqWebhookSubscription.md)
+ - [XiqWifiCapacityClientListResponse](docs/XiqWifiCapacityClientListResponse.md)
+ - [XiqWifiCapacityStatsResponse](docs/XiqWifiCapacityStatsResponse.md)
+ - [XiqWifiEfficiencyClientListResponse](docs/XiqWifiEfficiencyClientListResponse.md)
+ - [XiqWifiEfficiencyStatsResponse](docs/XiqWifiEfficiencyStatsResponse.md)
  - [XiqWingDevices](docs/XiqWingDevices.md)
  - [XiqWiredEventEntity](docs/XiqWiredEventEntity.md)
  - [XiqWiredHardwareEntity](docs/XiqWiredHardwareEntity.md)
  - [XiqWiredHardwareResponse](docs/XiqWiredHardwareResponse.md)
  - [XiqWiredQualityIndexResponse](docs/XiqWiredQualityIndexResponse.md)
  - [XiqWiredViewType](docs/XiqWiredViewType.md)
  - [XiqWirelessAppsResponse](docs/XiqWirelessAppsResponse.md)
```

### Comparing `extremecloudiq-api-23.3.1.15/setup.py` & `extremecloudiq-api-23.3.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.1.15
+    The version of the OpenAPI document: 23.3.2.1
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "extremecloudiq-api"
-VERSION = "23.3.1.15"
+VERSION = "23.3.2.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

