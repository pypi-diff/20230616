# Comparing `tmp/alibabacloud_dingtalk-2.0.20.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.20.tar", last modified: Tue Jun 13 08:58:19 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.21.tar", last modified: Fri Jun 16 07:09:03 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.20.tar` & `alibabacloud_dingtalk-2.0.21.tar`

### file list

```diff
@@ -1,369 +1,373 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/
--rw-r--r--   0 root         (0) root         (0)    19947 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139370 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   341471 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90334 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   117347 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19674 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27526 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52941 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    71864 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9368 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12542 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   146899 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   175146 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12151 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 08:58:19.000000 alibabacloud_dingtalk-2.0.20/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-06-13 08:58:18.000000 alibabacloud_dingtalk-2.0.20/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/
+-rw-r--r--   0 root         (0) root         (0)    20012 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   202090 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   571964 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139370 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   341471 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108908 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152805 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19674 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27526 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52941 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    71864 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269351 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472940 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731141 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21540 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146899 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   175146 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   418571 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12294 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-16 07:09:03.000000 alibabacloud_dingtalk-2.0.21/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-06-16 07:09:02.000000 alibabacloud_dingtalk-2.0.21/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.20/ChangeLog.md` & `alibabacloud_dingtalk-2.0.21/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-13 Version: 2.0.20
+- Update AddOfficialAccountFollower.
+
 2023-06-09 Version: 2.0.19
 - Update AddOfficialAccountFollower.
 
 2023-05-31 Version: 2.0.18
 - Update AddOfficialAccountFollower.
 
 2023-05-26 Version: 2.0.17
```

### Comparing `alibabacloud_dingtalk-2.0.20/LICENSE` & `alibabacloud_dingtalk-2.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/PKG-INFO` & `alibabacloud_dingtalk-2.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.20
+Version: 2.0.21
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.20/README-CN.md` & `alibabacloud_dingtalk-2.0.21/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/README.md` & `alibabacloud_dingtalk-2.0.21/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2503,14 +2503,16 @@
         headers: dingtalkbizfinance__1__0_models.QueryReceiptForInvoiceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__1__0_models.QueryReceiptForInvoiceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.apply_status_list):
             body['applyStatusList'] = request.apply_status_list
+        if not UtilClient.is_unset(request.biz_status_list):
+            body['bizStatusList'] = request.biz_status_list
         if not UtilClient.is_unset(request.end_time):
             body['endTime'] = request.end_time
         if not UtilClient.is_unset(request.page_number):
             body['pageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             body['pageSize'] = request.page_size
         if not UtilClient.is_unset(request.receipt_status_list):
@@ -2550,14 +2552,16 @@
         headers: dingtalkbizfinance__1__0_models.QueryReceiptForInvoiceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__1__0_models.QueryReceiptForInvoiceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.apply_status_list):
             body['applyStatusList'] = request.apply_status_list
+        if not UtilClient.is_unset(request.biz_status_list):
+            body['bizStatusList'] = request.biz_status_list
         if not UtilClient.is_unset(request.end_time):
             body['endTime'] = request.end_time
         if not UtilClient.is_unset(request.page_number):
             body['pageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             body['pageSize'] = request.page_size
         if not UtilClient.is_unset(request.receipt_status_list):
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,14 +546,15 @@
         purchaser_address: str = None,
         purchaser_bank_account: str = None,
         purchaser_bank_name_account: str = None,
         purchaser_name: str = None,
         purchaser_tax_no: str = None,
         purchaser_tel: str = None,
         remark: str = None,
+        reviewer: str = None,
         second_hand_car_invoice_detail_list: List[BatchAddInvoiceRequestGeneralInvoiceVOListSecondHandCarInvoiceDetailList] = None,
         seller_address: str = None,
         seller_bank_account: str = None,
         seller_bank_name_account: str = None,
         seller_name: str = None,
         seller_tax_no: str = None,
         seller_tel: str = None,
@@ -589,14 +590,15 @@
         self.purchaser_address = purchaser_address
         self.purchaser_bank_account = purchaser_bank_account
         self.purchaser_bank_name_account = purchaser_bank_name_account
         self.purchaser_name = purchaser_name
         self.purchaser_tax_no = purchaser_tax_no
         self.purchaser_tel = purchaser_tel
         self.remark = remark
+        self.reviewer = reviewer
         self.second_hand_car_invoice_detail_list = second_hand_car_invoice_detail_list
         self.seller_address = seller_address
         self.seller_bank_account = seller_bank_account
         self.seller_bank_name_account = seller_bank_name_account
         self.seller_name = seller_name
         self.seller_tax_no = seller_tax_no
         self.seller_tel = seller_tel
@@ -686,14 +688,16 @@
             result['purchaserName'] = self.purchaser_name
         if self.purchaser_tax_no is not None:
             result['purchaserTaxNo'] = self.purchaser_tax_no
         if self.purchaser_tel is not None:
             result['purchaserTel'] = self.purchaser_tel
         if self.remark is not None:
             result['remark'] = self.remark
+        if self.reviewer is not None:
+            result['reviewer'] = self.reviewer
         result['secondHandCarInvoiceDetailList'] = []
         if self.second_hand_car_invoice_detail_list is not None:
             for k in self.second_hand_car_invoice_detail_list:
                 result['secondHandCarInvoiceDetailList'].append(k.to_map() if k else None)
         if self.seller_address is not None:
             result['sellerAddress'] = self.seller_address
         if self.seller_bank_account is not None:
@@ -783,14 +787,16 @@
             self.purchaser_name = m.get('purchaserName')
         if m.get('purchaserTaxNo') is not None:
             self.purchaser_tax_no = m.get('purchaserTaxNo')
         if m.get('purchaserTel') is not None:
             self.purchaser_tel = m.get('purchaserTel')
         if m.get('remark') is not None:
             self.remark = m.get('remark')
+        if m.get('reviewer') is not None:
+            self.reviewer = m.get('reviewer')
         self.second_hand_car_invoice_detail_list = []
         if m.get('secondHandCarInvoiceDetailList') is not None:
             for k in m.get('secondHandCarInvoiceDetailList'):
                 temp_model = BatchAddInvoiceRequestGeneralInvoiceVOListSecondHandCarInvoiceDetailList()
                 self.second_hand_car_invoice_detail_list.append(temp_model.from_map(k))
         if m.get('sellerAddress') is not None:
             self.seller_address = m.get('sellerAddress')
@@ -6774,78 +6780,97 @@
         return self
 
 
 class QueryReceiptDetailForInvoiceResponseBodyResultProductInfoList(TeaModel):
     def __init__(
         self,
         amount_with_tax: str = None,
+        amount_without_tax: str = None,
         name: str = None,
         quantity: str = None,
         specification: str = None,
         tax_rate: str = None,
         unit: str = None,
         unit_price_with_tax: str = None,
+        unit_price_without_tax: str = None,
+        with_tax: bool = None,
     ):
         self.amount_with_tax = amount_with_tax
+        self.amount_without_tax = amount_without_tax
         self.name = name
         self.quantity = quantity
         self.specification = specification
         self.tax_rate = tax_rate
         self.unit = unit
         self.unit_price_with_tax = unit_price_with_tax
+        self.unit_price_without_tax = unit_price_without_tax
+        self.with_tax = with_tax
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
+        if self.amount_without_tax is not None:
+            result['amountWithoutTax'] = self.amount_without_tax
         if self.name is not None:
             result['name'] = self.name
         if self.quantity is not None:
             result['quantity'] = self.quantity
         if self.specification is not None:
             result['specification'] = self.specification
         if self.tax_rate is not None:
             result['taxRate'] = self.tax_rate
         if self.unit is not None:
             result['unit'] = self.unit
         if self.unit_price_with_tax is not None:
             result['unitPriceWithTax'] = self.unit_price_with_tax
+        if self.unit_price_without_tax is not None:
+            result['unitPriceWithoutTax'] = self.unit_price_without_tax
+        if self.with_tax is not None:
+            result['withTax'] = self.with_tax
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
+        if m.get('amountWithoutTax') is not None:
+            self.amount_without_tax = m.get('amountWithoutTax')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('quantity') is not None:
             self.quantity = m.get('quantity')
         if m.get('specification') is not None:
             self.specification = m.get('specification')
         if m.get('taxRate') is not None:
             self.tax_rate = m.get('taxRate')
         if m.get('unit') is not None:
             self.unit = m.get('unit')
         if m.get('unitPriceWithTax') is not None:
             self.unit_price_with_tax = m.get('unitPriceWithTax')
+        if m.get('unitPriceWithoutTax') is not None:
+            self.unit_price_without_tax = m.get('unitPriceWithoutTax')
+        if m.get('withTax') is not None:
+            self.with_tax = m.get('withTax')
         return self
 
 
 class QueryReceiptDetailForInvoiceResponseBodyResult(TeaModel):
     def __init__(
         self,
         amount: str = None,
         apply_status: str = None,
+        biz_status: str = None,
         create_time: str = None,
         creator: QueryReceiptDetailForInvoiceResponseBodyResultCreator = None,
         customer: QueryReceiptDetailForInvoiceResponseBodyResultCustomer = None,
         drawer_email: str = None,
         drawer_telephone: str = None,
         invoice_type: str = None,
         model_id: str = None,
@@ -6861,14 +6886,15 @@
         remark: str = None,
         source: str = None,
         status: str = None,
         title: str = None,
     ):
         self.amount = amount
         self.apply_status = apply_status
+        self.biz_status = biz_status
         self.create_time = create_time
         self.creator = creator
         self.customer = customer
         self.drawer_email = drawer_email
         self.drawer_telephone = drawer_telephone
         self.invoice_type = invoice_type
         self.model_id = model_id
@@ -6902,14 +6928,16 @@
             return _map
 
         result = dict()
         if self.amount is not None:
             result['amount'] = self.amount
         if self.apply_status is not None:
             result['applyStatus'] = self.apply_status
+        if self.biz_status is not None:
+            result['bizStatus'] = self.biz_status
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.creator is not None:
             result['creator'] = self.creator.to_map()
         if self.customer is not None:
             result['customer'] = self.customer.to_map()
         if self.drawer_email is not None:
@@ -6952,14 +6980,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('amount') is not None:
             self.amount = m.get('amount')
         if m.get('applyStatus') is not None:
             self.apply_status = m.get('applyStatus')
+        if m.get('bizStatus') is not None:
+            self.biz_status = m.get('bizStatus')
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('creator') is not None:
             temp_model = QueryReceiptDetailForInvoiceResponseBodyResultCreator()
             self.creator = temp_model.from_map(m['creator'])
         if m.get('customer') is not None:
             temp_model = QueryReceiptDetailForInvoiceResponseBodyResultCustomer()
@@ -7110,22 +7140,24 @@
         return self
 
 
 class QueryReceiptForInvoiceRequest(TeaModel):
     def __init__(
         self,
         apply_status_list: List[str] = None,
+        biz_status_list: List[str] = None,
         end_time: int = None,
         page_number: int = None,
         page_size: int = None,
         receipt_status_list: List[str] = None,
         start_time: int = None,
         title: str = None,
     ):
         self.apply_status_list = apply_status_list
+        self.biz_status_list = biz_status_list
         self.end_time = end_time
         self.page_number = page_number
         self.page_size = page_size
         self.receipt_status_list = receipt_status_list
         self.start_time = start_time
         self.title = title
 
@@ -7136,14 +7168,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.apply_status_list is not None:
             result['applyStatusList'] = self.apply_status_list
+        if self.biz_status_list is not None:
+            result['bizStatusList'] = self.biz_status_list
         if self.end_time is not None:
             result['endTime'] = self.end_time
         if self.page_number is not None:
             result['pageNumber'] = self.page_number
         if self.page_size is not None:
             result['pageSize'] = self.page_size
         if self.receipt_status_list is not None:
@@ -7154,14 +7188,16 @@
             result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('applyStatusList') is not None:
             self.apply_status_list = m.get('applyStatusList')
+        if m.get('bizStatusList') is not None:
+            self.biz_status_list = m.get('bizStatusList')
         if m.get('endTime') is not None:
             self.end_time = m.get('endTime')
         if m.get('pageNumber') is not None:
             self.page_number = m.get('pageNumber')
         if m.get('pageSize') is not None:
             self.page_size = m.get('pageSize')
         if m.get('receiptStatusList') is not None:
@@ -7245,78 +7281,97 @@
         return self
 
 
 class QueryReceiptForInvoiceResponseBodyListProductInfoList(TeaModel):
     def __init__(
         self,
         amount_with_tax: str = None,
+        amount_without_tax: str = None,
         name: str = None,
         quantity: str = None,
         specification: str = None,
         tax_rate: str = None,
         unit: str = None,
         unit_price_with_tax: str = None,
+        unit_price_without_tax: str = None,
+        with_tax: bool = None,
     ):
         self.amount_with_tax = amount_with_tax
+        self.amount_without_tax = amount_without_tax
         self.name = name
         self.quantity = quantity
         self.specification = specification
         self.tax_rate = tax_rate
         self.unit = unit
         self.unit_price_with_tax = unit_price_with_tax
+        self.unit_price_without_tax = unit_price_without_tax
+        self.with_tax = with_tax
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
+        if self.amount_without_tax is not None:
+            result['amountWithoutTax'] = self.amount_without_tax
         if self.name is not None:
             result['name'] = self.name
         if self.quantity is not None:
             result['quantity'] = self.quantity
         if self.specification is not None:
             result['specification'] = self.specification
         if self.tax_rate is not None:
             result['taxRate'] = self.tax_rate
         if self.unit is not None:
             result['unit'] = self.unit
         if self.unit_price_with_tax is not None:
             result['unitPriceWithTax'] = self.unit_price_with_tax
+        if self.unit_price_without_tax is not None:
+            result['unitPriceWithoutTax'] = self.unit_price_without_tax
+        if self.with_tax is not None:
+            result['withTax'] = self.with_tax
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
+        if m.get('amountWithoutTax') is not None:
+            self.amount_without_tax = m.get('amountWithoutTax')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('quantity') is not None:
             self.quantity = m.get('quantity')
         if m.get('specification') is not None:
             self.specification = m.get('specification')
         if m.get('taxRate') is not None:
             self.tax_rate = m.get('taxRate')
         if m.get('unit') is not None:
             self.unit = m.get('unit')
         if m.get('unitPriceWithTax') is not None:
             self.unit_price_with_tax = m.get('unitPriceWithTax')
+        if m.get('unitPriceWithoutTax') is not None:
+            self.unit_price_without_tax = m.get('unitPriceWithoutTax')
+        if m.get('withTax') is not None:
+            self.with_tax = m.get('withTax')
         return self
 
 
 class QueryReceiptForInvoiceResponseBodyList(TeaModel):
     def __init__(
         self,
         amount: str = None,
         apply_status: str = None,
+        biz_status: str = None,
         create_time: str = None,
         creator: QueryReceiptForInvoiceResponseBodyListCreator = None,
         customer: QueryReceiptForInvoiceResponseBodyListCustomer = None,
         drawer_email: str = None,
         drawer_telephone: str = None,
         invoice_type: str = None,
         model_id: str = None,
@@ -7332,14 +7387,15 @@
         remark: str = None,
         source: str = None,
         status: str = None,
         title: str = None,
     ):
         self.amount = amount
         self.apply_status = apply_status
+        self.biz_status = biz_status
         self.create_time = create_time
         self.creator = creator
         self.customer = customer
         self.drawer_email = drawer_email
         self.drawer_telephone = drawer_telephone
         self.invoice_type = invoice_type
         self.model_id = model_id
@@ -7373,14 +7429,16 @@
             return _map
 
         result = dict()
         if self.amount is not None:
             result['amount'] = self.amount
         if self.apply_status is not None:
             result['applyStatus'] = self.apply_status
+        if self.biz_status is not None:
+            result['bizStatus'] = self.biz_status
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.creator is not None:
             result['creator'] = self.creator.to_map()
         if self.customer is not None:
             result['customer'] = self.customer.to_map()
         if self.drawer_email is not None:
@@ -7423,14 +7481,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('amount') is not None:
             self.amount = m.get('amount')
         if m.get('applyStatus') is not None:
             self.apply_status = m.get('applyStatus')
+        if m.get('bizStatus') is not None:
+            self.biz_status = m.get('bizStatus')
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('creator') is not None:
             temp_model = QueryReceiptForInvoiceResponseBodyListCreator()
             self.creator = temp_model.from_map(m['creator'])
         if m.get('customer') is not None:
             temp_model = QueryReceiptForInvoiceResponseBodyListCustomer()
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -401,14 +401,418 @@
         conference_id: str,
         request: dingtalkconference__1__0_models.FocusRequest,
     ) -> dingtalkconference__1__0_models.FocusResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkconference__1__0_models.FocusHeaders()
         return await self.focus_with_options_async(conference_id, request, headers, runtime)
 
+    def get_conf_data_by_conference_id_with_options(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDataByConferenceIdRequest,
+        headers: dingtalkconference__1__0_models.GetConfDataByConferenceIdHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetConfDataByConferenceIdResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.real_data):
+            query['realData'] = request.real_data
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetConfDataByConferenceId',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/{conference_id}/infos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetConfDataByConferenceIdResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_conf_data_by_conference_id_with_options_async(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDataByConferenceIdRequest,
+        headers: dingtalkconference__1__0_models.GetConfDataByConferenceIdHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetConfDataByConferenceIdResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.real_data):
+            query['realData'] = request.real_data
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetConfDataByConferenceId',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/{conference_id}/infos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetConfDataByConferenceIdResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_conf_data_by_conference_id(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDataByConferenceIdRequest,
+    ) -> dingtalkconference__1__0_models.GetConfDataByConferenceIdResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetConfDataByConferenceIdHeaders()
+        return self.get_conf_data_by_conference_id_with_options(conference_id, request, headers, runtime)
+
+    async def get_conf_data_by_conference_id_async(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDataByConferenceIdRequest,
+    ) -> dingtalkconference__1__0_models.GetConfDataByConferenceIdResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetConfDataByConferenceIdHeaders()
+        return await self.get_conf_data_by_conference_id_with_options_async(conference_id, request, headers, runtime)
+
+    def get_conf_detail_data_with_options(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDetailDataRequest,
+        headers: dingtalkconference__1__0_models.GetConfDetailDataHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetConfDetailDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.nick):
+            query['nick'] = request.nick
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetConfDetailData',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/{conference_id}/details',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetConfDetailDataResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_conf_detail_data_with_options_async(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDetailDataRequest,
+        headers: dingtalkconference__1__0_models.GetConfDetailDataHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetConfDetailDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.nick):
+            query['nick'] = request.nick
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetConfDetailData',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/{conference_id}/details',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetConfDetailDataResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_conf_detail_data(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDetailDataRequest,
+    ) -> dingtalkconference__1__0_models.GetConfDetailDataResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetConfDetailDataHeaders()
+        return self.get_conf_detail_data_with_options(conference_id, request, headers, runtime)
+
+    async def get_conf_detail_data_async(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetConfDetailDataRequest,
+    ) -> dingtalkconference__1__0_models.GetConfDetailDataResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetConfDetailDataHeaders()
+        return await self.get_conf_detail_data_with_options_async(conference_id, request, headers, runtime)
+
+    def get_history_conf_data_list_with_options(
+        self,
+        request: dingtalkconference__1__0_models.GetHistoryConfDataListRequest,
+        headers: dingtalkconference__1__0_models.GetHistoryConfDataListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetHistoryConfDataListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.creator_nike):
+            query['creatorNike'] = request.creator_nike
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.free_type):
+            query['freeType'] = request.free_type
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.real_data):
+            query['realData'] = request.real_data
+        if not UtilClient.is_unset(request.scene):
+            query['scene'] = request.scene
+        if not UtilClient.is_unset(request.start_time):
+            query['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.title):
+            query['title'] = request.title
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetHistoryConfDataList',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/histories/dataLists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetHistoryConfDataListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_history_conf_data_list_with_options_async(
+        self,
+        request: dingtalkconference__1__0_models.GetHistoryConfDataListRequest,
+        headers: dingtalkconference__1__0_models.GetHistoryConfDataListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetHistoryConfDataListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.creator_nike):
+            query['creatorNike'] = request.creator_nike
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.free_type):
+            query['freeType'] = request.free_type
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.real_data):
+            query['realData'] = request.real_data
+        if not UtilClient.is_unset(request.scene):
+            query['scene'] = request.scene
+        if not UtilClient.is_unset(request.start_time):
+            query['startTime'] = request.start_time
+        if not UtilClient.is_unset(request.title):
+            query['title'] = request.title
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetHistoryConfDataList',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/histories/dataLists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetHistoryConfDataListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_history_conf_data_list(
+        self,
+        request: dingtalkconference__1__0_models.GetHistoryConfDataListRequest,
+    ) -> dingtalkconference__1__0_models.GetHistoryConfDataListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetHistoryConfDataListHeaders()
+        return self.get_history_conf_data_list_with_options(request, headers, runtime)
+
+    async def get_history_conf_data_list_async(
+        self,
+        request: dingtalkconference__1__0_models.GetHistoryConfDataListRequest,
+    ) -> dingtalkconference__1__0_models.GetHistoryConfDataListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetHistoryConfDataListHeaders()
+        return await self.get_history_conf_data_list_with_options_async(request, headers, runtime)
+
+    def get_user_metric_data_with_options(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetUserMetricDataRequest,
+        headers: dingtalkconference__1__0_models.GetUserMetricDataHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetUserMetricDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.begin_time):
+            query['beginTime'] = request.begin_time
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetUserMetricData',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/{conference_id}/metricDatas',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetUserMetricDataResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_user_metric_data_with_options_async(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetUserMetricDataRequest,
+        headers: dingtalkconference__1__0_models.GetUserMetricDataHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.GetUserMetricDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.begin_time):
+            query['beginTime'] = request.begin_time
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetUserMetricData',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/{conference_id}/metricDatas',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.GetUserMetricDataResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_user_metric_data(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetUserMetricDataRequest,
+    ) -> dingtalkconference__1__0_models.GetUserMetricDataResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetUserMetricDataHeaders()
+        return self.get_user_metric_data_with_options(conference_id, request, headers, runtime)
+
+    async def get_user_metric_data_async(
+        self,
+        conference_id: str,
+        request: dingtalkconference__1__0_models.GetUserMetricDataRequest,
+    ) -> dingtalkconference__1__0_models.GetUserMetricDataResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.GetUserMetricDataHeaders()
+        return await self.get_user_metric_data_with_options_async(conference_id, request, headers, runtime)
+
     def invite_users_with_options(
         self,
         conference_id: str,
         request: dingtalkconference__1__0_models.InviteUsersRequest,
         headers: dingtalkconference__1__0_models.InviteUsersHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.InviteUsersResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List, Any
+from typing import Dict, List
 
 
-class CloseVideoConferenceHeaders(TeaModel):
+class GetDeptHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,80 +33,104 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CloseVideoConferenceRequest(TeaModel):
+class GetDeptRequest(TeaModel):
     def __init__(
         self,
-        union_id: str = None,
+        language: str = None,
+        sub_corp_id: str = None,
     ):
-        self.union_id = union_id
+        self.language = language
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.language is not None:
+            result['language'] = self.language
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('language') is not None:
+            self.language = m.get('language')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class CloseVideoConferenceResponseBody(TeaModel):
+class GetDeptResponseBody(TeaModel):
     def __init__(
         self,
-        cause: str = None,
-        code: int = None,
+        department_id: int = None,
+        department_name: str = None,
+        from_union_org: bool = None,
+        order: int = None,
+        parent_department_id: int = None,
     ):
-        self.cause = cause
-        self.code = code
+        self.department_id = department_id
+        self.department_name = department_name
+        self.from_union_org = from_union_org
+        self.order = order
+        self.parent_department_id = parent_department_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.cause is not None:
-            result['cause'] = self.cause
-        if self.code is not None:
-            result['code'] = self.code
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.department_name is not None:
+            result['departmentName'] = self.department_name
+        if self.from_union_org is not None:
+            result['fromUnionOrg'] = self.from_union_org
+        if self.order is not None:
+            result['order'] = self.order
+        if self.parent_department_id is not None:
+            result['parentDepartmentId'] = self.parent_department_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cause') is not None:
-            self.cause = m.get('cause')
-        if m.get('code') is not None:
-            self.code = m.get('code')
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('departmentName') is not None:
+            self.department_name = m.get('departmentName')
+        if m.get('fromUnionOrg') is not None:
+            self.from_union_org = m.get('fromUnionOrg')
+        if m.get('order') is not None:
+            self.order = m.get('order')
+        if m.get('parentDepartmentId') is not None:
+            self.parent_department_id = m.get('parentDepartmentId')
         return self
 
 
-class CloseVideoConferenceResponse(TeaModel):
+class GetDeptResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CloseVideoConferenceResponseBody = None,
+        body: GetDeptResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -132,20 +156,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CloseVideoConferenceResponseBody()
+            temp_model = GetDeptResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CohostsHeaders(TeaModel):
+class GetResidentDeptHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -170,115 +194,98 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CohostsRequestUserList(TeaModel):
+class GetResidentDeptRequest(TeaModel):
     def __init__(
         self,
-        union_id: str = None,
+        sub_corp_id: str = None,
     ):
-        self.union_id = union_id
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
-        return self
-
-
-class CohostsRequest(TeaModel):
-    def __init__(
-        self,
-        action: str = None,
-        user_list: List[CohostsRequestUserList] = None,
-    ):
-        self.action = action
-        self.user_list = user_list
-
-    def validate(self):
-        if self.user_list:
-            for k in self.user_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.action is not None:
-            result['action'] = self.action
-        result['userList'] = []
-        if self.user_list is not None:
-            for k in self.user_list:
-                result['userList'].append(k.to_map() if k else None)
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('action') is not None:
-            self.action = m.get('action')
-        self.user_list = []
-        if m.get('userList') is not None:
-            for k in m.get('userList'):
-                temp_model = CohostsRequestUserList()
-                self.user_list.append(temp_model.from_map(k))
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class CohostsResponseBody(TeaModel):
+class GetResidentDeptResponseBody(TeaModel):
     def __init__(
         self,
-        success: bool = None,
+        contact_type: str = None,
+        department_id: int = None,
+        department_name: str = None,
+        dept_type: str = None,
+        feature: str = None,
     ):
-        self.success = success
+        self.contact_type = contact_type
+        self.department_id = department_id
+        self.department_name = department_name
+        self.dept_type = dept_type
+        self.feature = feature
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.contact_type is not None:
+            result['contactType'] = self.contact_type
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.department_name is not None:
+            result['departmentName'] = self.department_name
+        if self.dept_type is not None:
+            result['deptType'] = self.dept_type
+        if self.feature is not None:
+            result['feature'] = self.feature
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('contactType') is not None:
+            self.contact_type = m.get('contactType')
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('departmentName') is not None:
+            self.department_name = m.get('departmentName')
+        if m.get('deptType') is not None:
+            self.dept_type = m.get('deptType')
+        if m.get('feature') is not None:
+            self.feature = m.get('feature')
         return self
 
 
-class CohostsResponse(TeaModel):
+class GetResidentDeptResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CohostsResponseBody = None,
+        body: GetResidentDeptResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -304,20 +311,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CohostsResponseBody()
+            temp_model = GetResidentDeptResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateVideoConferenceHeaders(TeaModel):
+class GetResidentUserInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -342,122 +349,145 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CreateVideoConferenceRequest(TeaModel):
+class GetResidentUserInfoRequest(TeaModel):
     def __init__(
         self,
-        conf_title: str = None,
-        invite_caller: bool = None,
-        invite_user_ids: List[str] = None,
-        user_id: str = None,
+        sub_corp_id: str = None,
     ):
-        self.conf_title = conf_title
-        self.invite_caller = invite_caller
-        self.invite_user_ids = invite_user_ids
-        self.user_id = user_id
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.conf_title is not None:
-            result['confTitle'] = self.conf_title
-        if self.invite_caller is not None:
-            result['inviteCaller'] = self.invite_caller
-        if self.invite_user_ids is not None:
-            result['inviteUserIds'] = self.invite_user_ids
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('confTitle') is not None:
-            self.conf_title = m.get('confTitle')
-        if m.get('inviteCaller') is not None:
-            self.invite_caller = m.get('inviteCaller')
-        if m.get('inviteUserIds') is not None:
-            self.invite_user_ids = m.get('inviteUserIds')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class CreateVideoConferenceResponseBody(TeaModel):
+class GetResidentUserInfoResponseBodyRoles(TeaModel):
     def __init__(
         self,
-        conference_id: str = None,
-        conference_password: str = None,
-        external_link_url: str = None,
-        host_password: str = None,
-        phone_numbers: List[str] = None,
-        room_code: str = None,
+        role_id: int = None,
+        role_name: str = None,
+        tag_code: str = None,
     ):
-        self.conference_id = conference_id
-        self.conference_password = conference_password
-        self.external_link_url = external_link_url
-        self.host_password = host_password
-        self.phone_numbers = phone_numbers
-        self.room_code = room_code
+        self.role_id = role_id
+        self.role_name = role_name
+        self.tag_code = tag_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.conference_id is not None:
-            result['conferenceId'] = self.conference_id
-        if self.conference_password is not None:
-            result['conferencePassword'] = self.conference_password
-        if self.external_link_url is not None:
-            result['externalLinkUrl'] = self.external_link_url
-        if self.host_password is not None:
-            result['hostPassword'] = self.host_password
-        if self.phone_numbers is not None:
-            result['phoneNumbers'] = self.phone_numbers
-        if self.room_code is not None:
-            result['roomCode'] = self.room_code
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        if self.role_name is not None:
+            result['roleName'] = self.role_name
+        if self.tag_code is not None:
+            result['tagCode'] = self.tag_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('conferenceId') is not None:
-            self.conference_id = m.get('conferenceId')
-        if m.get('conferencePassword') is not None:
-            self.conference_password = m.get('conferencePassword')
-        if m.get('externalLinkUrl') is not None:
-            self.external_link_url = m.get('externalLinkUrl')
-        if m.get('hostPassword') is not None:
-            self.host_password = m.get('hostPassword')
-        if m.get('phoneNumbers') is not None:
-            self.phone_numbers = m.get('phoneNumbers')
-        if m.get('roomCode') is not None:
-            self.room_code = m.get('roomCode')
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        if m.get('roleName') is not None:
+            self.role_name = m.get('roleName')
+        if m.get('tagCode') is not None:
+            self.tag_code = m.get('tagCode')
         return self
 
 
-class CreateVideoConferenceResponse(TeaModel):
+class GetResidentUserInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        feature: str = None,
+        name: str = None,
+        roles: List[GetResidentUserInfoResponseBodyRoles] = None,
+        union_id: str = None,
+        userid: str = None,
+    ):
+        self.feature = feature
+        self.name = name
+        self.roles = roles
+        self.union_id = union_id
+        self.userid = userid
+
+    def validate(self):
+        if self.roles:
+            for k in self.roles:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.feature is not None:
+            result['feature'] = self.feature
+        if self.name is not None:
+            result['name'] = self.name
+        result['roles'] = []
+        if self.roles is not None:
+            for k in self.roles:
+                result['roles'].append(k.to_map() if k else None)
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.userid is not None:
+            result['userid'] = self.userid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('feature') is not None:
+            self.feature = m.get('feature')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        self.roles = []
+        if m.get('roles') is not None:
+            for k in m.get('roles'):
+                temp_model = GetResidentUserInfoResponseBodyRoles()
+                self.roles.append(temp_model.from_map(k))
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userid') is not None:
+            self.userid = m.get('userid')
+        return self
+
+
+class GetResidentUserInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CreateVideoConferenceResponseBody = None,
+        body: GetResidentUserInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -483,20 +513,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CreateVideoConferenceResponseBody()
+            temp_model = GetResidentUserInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class FocusHeaders(TeaModel):
+class GetUserHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -521,258 +551,420 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class FocusRequest(TeaModel):
+class GetUserRequest(TeaModel):
     def __init__(
         self,
-        action: str = None,
-        union_id: str = None,
+        language: str = None,
+        sub_corp_id: str = None,
     ):
-        self.action = action
-        self.union_id = union_id
+        self.language = language
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.action is not None:
-            result['action'] = self.action
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.language is not None:
+            result['language'] = self.language
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('action') is not None:
-            self.action = m.get('action')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('language') is not None:
+            self.language = m.get('language')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class FocusResponseBody(TeaModel):
+class GetUserResponseBodyDepartmentOrderSet(TeaModel):
     def __init__(
         self,
-        success: bool = None,
+        department_id: int = None,
+        order: int = None,
     ):
-        self.success = success
+        self.department_id = department_id
+        self.order = order
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.order is not None:
+            result['order'] = self.order
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('order') is not None:
+            self.order = m.get('order')
         return self
 
 
-class FocusResponse(TeaModel):
+class GetUserResponseBodyLeaderInDepartment(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: FocusResponseBody = None,
+        department_id: int = None,
+        leader: bool = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.department_id = department_id
+        self.leader = leader
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.leader is not None:
+            result['leader'] = self.leader
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = FocusResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('leader') is not None:
+            self.leader = m.get('leader')
         return self
 
 
-class InviteUsersHeaders(TeaModel):
+class GetUserResponseBodyRoleList(TeaModel):
     def __init__(
         self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
+        group_name: str = None,
+        role_id: int = None,
+        role_name: str = None,
     ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+        self.group_name = group_name
+        self.role_id = role_id
+        self.role_name = role_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        if self.group_name is not None:
+            result['groupName'] = self.group_name
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        if self.role_name is not None:
+            result['roleName'] = self.role_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        if m.get('groupName') is not None:
+            self.group_name = m.get('groupName')
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        if m.get('roleName') is not None:
+            self.role_name = m.get('roleName')
         return self
 
 
-class InviteUsersRequestInviteeList(TeaModel):
+class GetUserResponseBodyUnionEmpExtUnionEmpMapList(TeaModel):
     def __init__(
         self,
-        nick: str = None,
-        union_id: str = None,
+        corp_id: str = None,
+        staff_id: str = None,
     ):
-        self.nick = nick
-        self.union_id = union_id
+        self.corp_id = corp_id
+        self.staff_id = staff_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.nick is not None:
-            result['nick'] = self.nick
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.staff_id is not None:
+            result['staffId'] = self.staff_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('nick') is not None:
-            self.nick = m.get('nick')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('staffId') is not None:
+            self.staff_id = m.get('staffId')
         return self
 
 
-class InviteUsersRequest(TeaModel):
+class GetUserResponseBodyUnionEmpExt(TeaModel):
     def __init__(
         self,
-        invitee_list: List[InviteUsersRequestInviteeList] = None,
-        union_id: str = None,
+        corp_id: str = None,
+        staff_id: str = None,
+        union_emp_map_list: List[GetUserResponseBodyUnionEmpExtUnionEmpMapList] = None,
     ):
-        self.invitee_list = invitee_list
-        self.union_id = union_id
+        self.corp_id = corp_id
+        self.staff_id = staff_id
+        self.union_emp_map_list = union_emp_map_list
 
     def validate(self):
-        if self.invitee_list:
-            for k in self.invitee_list:
+        if self.union_emp_map_list:
+            for k in self.union_emp_map_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['inviteeList'] = []
-        if self.invitee_list is not None:
-            for k in self.invitee_list:
-                result['inviteeList'].append(k.to_map() if k else None)
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.staff_id is not None:
+            result['staffId'] = self.staff_id
+        result['unionEmpMapList'] = []
+        if self.union_emp_map_list is not None:
+            for k in self.union_emp_map_list:
+                result['unionEmpMapList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.invitee_list = []
-        if m.get('inviteeList') is not None:
-            for k in m.get('inviteeList'):
-                temp_model = InviteUsersRequestInviteeList()
-                self.invitee_list.append(temp_model.from_map(k))
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('staffId') is not None:
+            self.staff_id = m.get('staffId')
+        self.union_emp_map_list = []
+        if m.get('unionEmpMapList') is not None:
+            for k in m.get('unionEmpMapList'):
+                temp_model = GetUserResponseBodyUnionEmpExtUnionEmpMapList()
+                self.union_emp_map_list.append(temp_model.from_map(k))
         return self
 
 
-class InviteUsersResponseBody(TeaModel):
-    def __init__(
-        self,
-        success: bool = None,
+class GetUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        active: bool = None,
+        admin: bool = None,
+        boss: bool = None,
+        department_id_list: List[int] = None,
+        department_order_set: List[GetUserResponseBodyDepartmentOrderSet] = None,
+        exclusive_account: bool = None,
+        exclusive_account_type: str = None,
+        extension: str = None,
+        hired_date: int = None,
+        job_number: str = None,
+        leader_in_department: List[GetUserResponseBodyLeaderInDepartment] = None,
+        manager_user_id: str = None,
+        name: str = None,
+        real_authed: bool = None,
+        remark: str = None,
+        role_list: List[GetUserResponseBodyRoleList] = None,
+        senior: bool = None,
+        title: str = None,
+        union_emp_ext: GetUserResponseBodyUnionEmpExt = None,
+        union_id: str = None,
+        user_id: str = None,
+        work_place: str = None,
     ):
-        self.success = success
+        self.active = active
+        self.admin = admin
+        self.boss = boss
+        self.department_id_list = department_id_list
+        self.department_order_set = department_order_set
+        self.exclusive_account = exclusive_account
+        self.exclusive_account_type = exclusive_account_type
+        self.extension = extension
+        self.hired_date = hired_date
+        self.job_number = job_number
+        self.leader_in_department = leader_in_department
+        self.manager_user_id = manager_user_id
+        self.name = name
+        self.real_authed = real_authed
+        self.remark = remark
+        self.role_list = role_list
+        self.senior = senior
+        self.title = title
+        self.union_emp_ext = union_emp_ext
+        self.union_id = union_id
+        self.user_id = user_id
+        self.work_place = work_place
 
     def validate(self):
-        pass
+        if self.department_order_set:
+            for k in self.department_order_set:
+                if k:
+                    k.validate()
+        if self.leader_in_department:
+            for k in self.leader_in_department:
+                if k:
+                    k.validate()
+        if self.role_list:
+            for k in self.role_list:
+                if k:
+                    k.validate()
+        if self.union_emp_ext:
+            self.union_emp_ext.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.active is not None:
+            result['active'] = self.active
+        if self.admin is not None:
+            result['admin'] = self.admin
+        if self.boss is not None:
+            result['boss'] = self.boss
+        if self.department_id_list is not None:
+            result['departmentIdList'] = self.department_id_list
+        result['departmentOrderSet'] = []
+        if self.department_order_set is not None:
+            for k in self.department_order_set:
+                result['departmentOrderSet'].append(k.to_map() if k else None)
+        if self.exclusive_account is not None:
+            result['exclusiveAccount'] = self.exclusive_account
+        if self.exclusive_account_type is not None:
+            result['exclusiveAccountType'] = self.exclusive_account_type
+        if self.extension is not None:
+            result['extension'] = self.extension
+        if self.hired_date is not None:
+            result['hiredDate'] = self.hired_date
+        if self.job_number is not None:
+            result['jobNumber'] = self.job_number
+        result['leaderInDepartment'] = []
+        if self.leader_in_department is not None:
+            for k in self.leader_in_department:
+                result['leaderInDepartment'].append(k.to_map() if k else None)
+        if self.manager_user_id is not None:
+            result['managerUserId'] = self.manager_user_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.real_authed is not None:
+            result['realAuthed'] = self.real_authed
+        if self.remark is not None:
+            result['remark'] = self.remark
+        result['roleList'] = []
+        if self.role_list is not None:
+            for k in self.role_list:
+                result['roleList'].append(k.to_map() if k else None)
+        if self.senior is not None:
+            result['senior'] = self.senior
+        if self.title is not None:
+            result['title'] = self.title
+        if self.union_emp_ext is not None:
+            result['unionEmpExt'] = self.union_emp_ext.to_map()
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.work_place is not None:
+            result['workPlace'] = self.work_place
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('active') is not None:
+            self.active = m.get('active')
+        if m.get('admin') is not None:
+            self.admin = m.get('admin')
+        if m.get('boss') is not None:
+            self.boss = m.get('boss')
+        if m.get('departmentIdList') is not None:
+            self.department_id_list = m.get('departmentIdList')
+        self.department_order_set = []
+        if m.get('departmentOrderSet') is not None:
+            for k in m.get('departmentOrderSet'):
+                temp_model = GetUserResponseBodyDepartmentOrderSet()
+                self.department_order_set.append(temp_model.from_map(k))
+        if m.get('exclusiveAccount') is not None:
+            self.exclusive_account = m.get('exclusiveAccount')
+        if m.get('exclusiveAccountType') is not None:
+            self.exclusive_account_type = m.get('exclusiveAccountType')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
+        if m.get('hiredDate') is not None:
+            self.hired_date = m.get('hiredDate')
+        if m.get('jobNumber') is not None:
+            self.job_number = m.get('jobNumber')
+        self.leader_in_department = []
+        if m.get('leaderInDepartment') is not None:
+            for k in m.get('leaderInDepartment'):
+                temp_model = GetUserResponseBodyLeaderInDepartment()
+                self.leader_in_department.append(temp_model.from_map(k))
+        if m.get('managerUserId') is not None:
+            self.manager_user_id = m.get('managerUserId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('realAuthed') is not None:
+            self.real_authed = m.get('realAuthed')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        self.role_list = []
+        if m.get('roleList') is not None:
+            for k in m.get('roleList'):
+                temp_model = GetUserResponseBodyRoleList()
+                self.role_list.append(temp_model.from_map(k))
+        if m.get('senior') is not None:
+            self.senior = m.get('senior')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('unionEmpExt') is not None:
+            temp_model = GetUserResponseBodyUnionEmpExt()
+            self.union_emp_ext = temp_model.from_map(m['unionEmpExt'])
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('workPlace') is not None:
+            self.work_place = m.get('workPlace')
         return self
 
 
-class InviteUsersResponse(TeaModel):
+class GetUserResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: InviteUsersResponseBody = None,
+        body: GetUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -798,20 +990,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = InviteUsersResponseBody()
+            temp_model = GetUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class KickMembersHeaders(TeaModel):
+class GetUserByUnionIdHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -836,121 +1028,92 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class KickMembersRequestUserList(TeaModel):
+class GetUserByUnionIdRequest(TeaModel):
     def __init__(
         self,
-        participant_id: str = None,
+        language: str = None,
+        sub_corp_id: str = None,
         union_id: str = None,
     ):
-        self.participant_id = participant_id
+        self.language = language
+        self.sub_corp_id = sub_corp_id
         self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.participant_id is not None:
-            result['participantId'] = self.participant_id
+        if self.language is not None:
+            result['language'] = self.language
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         if self.union_id is not None:
             result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('participantId') is not None:
-            self.participant_id = m.get('participantId')
+        if m.get('language') is not None:
+            self.language = m.get('language')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
         return self
 
 
-class KickMembersRequest(TeaModel):
+class GetUserByUnionIdResponseBody(TeaModel):
     def __init__(
         self,
-        forbidden_rejoin: bool = None,
-        user_list: List[KickMembersRequestUserList] = None,
-    ):
-        self.forbidden_rejoin = forbidden_rejoin
-        self.user_list = user_list
-
-    def validate(self):
-        if self.user_list:
-            for k in self.user_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.forbidden_rejoin is not None:
-            result['forbiddenRejoin'] = self.forbidden_rejoin
-        result['userList'] = []
-        if self.user_list is not None:
-            for k in self.user_list:
-                result['userList'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('forbiddenRejoin') is not None:
-            self.forbidden_rejoin = m.get('forbiddenRejoin')
-        self.user_list = []
-        if m.get('userList') is not None:
-            for k in m.get('userList'):
-                temp_model = KickMembersRequestUserList()
-                self.user_list.append(temp_model.from_map(k))
-        return self
-
-
-class KickMembersResponseBody(TeaModel):
-    def __init__(
-        self,
-        success: bool = None,
+        contact_type: int = None,
+        user_id: str = None,
     ):
-        self.success = success
+        self.contact_type = contact_type
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.contact_type is not None:
+            result['contactType'] = self.contact_type
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('contactType') is not None:
+            self.contact_type = m.get('contactType')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class KickMembersResponse(TeaModel):
+class GetUserByUnionIdResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: KickMembersResponseBody = None,
+        body: GetUserByUnionIdResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -976,20 +1139,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = KickMembersResponseBody()
+            temp_model = GetUserByUnionIdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class MuteAllHeaders(TeaModel):
+class GetVillageOrgInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1014,80 +1177,59 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class MuteAllRequest(TeaModel):
-    def __init__(
-        self,
-        action: str = None,
-        force_mute: bool = None,
-    ):
-        self.action = action
-        self.force_mute = force_mute
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.action is not None:
-            result['action'] = self.action
-        if self.force_mute is not None:
-            result['forceMute'] = self.force_mute
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('action') is not None:
-            self.action = m.get('action')
-        if m.get('forceMute') is not None:
-            self.force_mute = m.get('forceMute')
-        return self
-
-
-class MuteAllResponseBody(TeaModel):
+class GetVillageOrgInfoResponseBody(TeaModel):
     def __init__(
         self,
-        success: bool = None,
+        region_id: str = None,
+        region_location: str = None,
+        region_type: str = None,
     ):
-        self.success = success
+        self.region_id = region_id
+        self.region_location = region_location
+        self.region_type = region_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.region_location is not None:
+            result['regionLocation'] = self.region_location
+        if self.region_type is not None:
+            result['regionType'] = self.region_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('regionLocation') is not None:
+            self.region_location = m.get('regionLocation')
+        if m.get('regionType') is not None:
+            self.region_type = m.get('regionType')
         return self
 
 
-class MuteAllResponse(TeaModel):
+class GetVillageOrgInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: MuteAllResponseBody = None,
+        body: GetVillageOrgInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1113,20 +1255,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = MuteAllResponseBody()
+            temp_model = GetVillageOrgInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class MuteMembersHeaders(TeaModel):
+class ListDeptSimpleUsersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1151,121 +1293,163 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class MuteMembersRequestUserList(TeaModel):
+class ListDeptSimpleUsersRequest(TeaModel):
     def __init__(
         self,
-        participant_id: str = None,
-        union_id: str = None,
+        contain_access_limit: bool = None,
+        cursor: int = None,
+        language: str = None,
+        order_field: str = None,
+        size: int = None,
+        sub_corp_id: str = None,
     ):
-        self.participant_id = participant_id
-        self.union_id = union_id
+        self.contain_access_limit = contain_access_limit
+        self.cursor = cursor
+        self.language = language
+        self.order_field = order_field
+        self.size = size
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.participant_id is not None:
-            result['participantId'] = self.participant_id
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.contain_access_limit is not None:
+            result['containAccessLimit'] = self.contain_access_limit
+        if self.cursor is not None:
+            result['cursor'] = self.cursor
+        if self.language is not None:
+            result['language'] = self.language
+        if self.order_field is not None:
+            result['orderField'] = self.order_field
+        if self.size is not None:
+            result['size'] = self.size
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('participantId') is not None:
-            self.participant_id = m.get('participantId')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('containAccessLimit') is not None:
+            self.contain_access_limit = m.get('containAccessLimit')
+        if m.get('cursor') is not None:
+            self.cursor = m.get('cursor')
+        if m.get('language') is not None:
+            self.language = m.get('language')
+        if m.get('orderField') is not None:
+            self.order_field = m.get('orderField')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class MuteMembersRequest(TeaModel):
+class ListDeptSimpleUsersResponseBodyUserList(TeaModel):
     def __init__(
         self,
-        action: str = None,
-        user_list: List[MuteMembersRequestUserList] = None,
+        name: str = None,
+        user_id: str = None,
     ):
-        self.action = action
-        self.user_list = user_list
+        self.name = name
+        self.user_id = user_id
 
     def validate(self):
-        if self.user_list:
-            for k in self.user_list:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.action is not None:
-            result['action'] = self.action
-        result['userList'] = []
-        if self.user_list is not None:
-            for k in self.user_list:
-                result['userList'].append(k.to_map() if k else None)
+        if self.name is not None:
+            result['name'] = self.name
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('action') is not None:
-            self.action = m.get('action')
-        self.user_list = []
-        if m.get('userList') is not None:
-            for k in m.get('userList'):
-                temp_model = MuteMembersRequestUserList()
-                self.user_list.append(temp_model.from_map(k))
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class MuteMembersResponseBody(TeaModel):
+class ListDeptSimpleUsersResponseBody(TeaModel):
     def __init__(
         self,
-        success: bool = None,
+        has_more: bool = None,
+        next_cursor: int = None,
+        total_count: int = None,
+        user_list: List[ListDeptSimpleUsersResponseBodyUserList] = None,
     ):
-        self.success = success
+        self.has_more = has_more
+        self.next_cursor = next_cursor
+        self.total_count = total_count
+        self.user_list = user_list
 
     def validate(self):
-        pass
+        if self.user_list:
+            for k in self.user_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        if self.next_cursor is not None:
+            result['nextCursor'] = self.next_cursor
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        result['userList'] = []
+        if self.user_list is not None:
+            for k in self.user_list:
+                result['userList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        if m.get('nextCursor') is not None:
+            self.next_cursor = m.get('nextCursor')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        self.user_list = []
+        if m.get('userList') is not None:
+            for k in m.get('userList'):
+                temp_model = ListDeptSimpleUsersResponseBodyUserList()
+                self.user_list.append(temp_model.from_map(k))
         return self
 
 
-class MuteMembersResponse(TeaModel):
+class ListDeptSimpleUsersResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: MuteMembersResponseBody = None,
+        body: ListDeptSimpleUsersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1291,20 +1475,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = MuteMembersResponseBody()
+            temp_model = ListDeptSimpleUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryCloudRecordTextHeaders(TeaModel):
+class ListDeptUserIdsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1329,299 +1513,74 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryCloudRecordTextRequest(TeaModel):
+class ListDeptUserIdsRequest(TeaModel):
     def __init__(
         self,
-        direction: str = None,
-        max_results: int = None,
-        next_token: int = None,
-        start_time: int = None,
-        union_id: str = None,
+        sub_corp_id: str = None,
     ):
-        self.direction = direction
-        self.max_results = max_results
-        self.next_token = next_token
-        self.start_time = start_time
-        self.union_id = union_id
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.direction is not None:
-            result['direction'] = self.direction
-        if self.max_results is not None:
-            result['maxResults'] = self.max_results
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('direction') is not None:
-            self.direction = m.get('direction')
-        if m.get('maxResults') is not None:
-            self.max_results = m.get('maxResults')
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class QueryCloudRecordTextResponseBodyParagraphListSentenceListWordList(TeaModel):
+class ListDeptUserIdsResponseBody(TeaModel):
     def __init__(
         self,
-        end_time: int = None,
-        start_time: int = None,
-        word: str = None,
-        word_id: str = None,
+        user_id_list: List[str] = None,
     ):
-        self.end_time = end_time
-        self.start_time = start_time
-        self.word = word
-        self.word_id = word_id
+        self.user_id_list = user_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.word is not None:
-            result['word'] = self.word
-        if self.word_id is not None:
-            result['wordId'] = self.word_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('word') is not None:
-            self.word = m.get('word')
-        if m.get('wordId') is not None:
-            self.word_id = m.get('wordId')
-        return self
-
-
-class QueryCloudRecordTextResponseBodyParagraphListSentenceList(TeaModel):
-    def __init__(
-        self,
-        end_time: int = None,
-        sentence: str = None,
-        start_time: int = None,
-        union_id: str = None,
-        word_list: List[QueryCloudRecordTextResponseBodyParagraphListSentenceListWordList] = None,
-    ):
-        self.end_time = end_time
-        self.sentence = sentence
-        self.start_time = start_time
-        self.union_id = union_id
-        self.word_list = word_list
-
-    def validate(self):
-        if self.word_list:
-            for k in self.word_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.sentence is not None:
-            result['sentence'] = self.sentence
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
-        result['wordList'] = []
-        if self.word_list is not None:
-            for k in self.word_list:
-                result['wordList'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('sentence') is not None:
-            self.sentence = m.get('sentence')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
-        self.word_list = []
-        if m.get('wordList') is not None:
-            for k in m.get('wordList'):
-                temp_model = QueryCloudRecordTextResponseBodyParagraphListSentenceListWordList()
-                self.word_list.append(temp_model.from_map(k))
-        return self
-
-
-class QueryCloudRecordTextResponseBodyParagraphList(TeaModel):
-    def __init__(
-        self,
-        end_time: int = None,
-        next_ttoken: int = None,
-        nick_name: str = None,
-        paragraph: str = None,
-        record_id: int = None,
-        sentence_list: List[QueryCloudRecordTextResponseBodyParagraphListSentenceList] = None,
-        start_time: int = None,
-        status: int = None,
-        union_id: str = None,
-    ):
-        self.end_time = end_time
-        self.next_ttoken = next_ttoken
-        self.nick_name = nick_name
-        self.paragraph = paragraph
-        self.record_id = record_id
-        self.sentence_list = sentence_list
-        self.start_time = start_time
-        self.status = status
-        self.union_id = union_id
-
-    def validate(self):
-        if self.sentence_list:
-            for k in self.sentence_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.next_ttoken is not None:
-            result['nextTtoken'] = self.next_ttoken
-        if self.nick_name is not None:
-            result['nickName'] = self.nick_name
-        if self.paragraph is not None:
-            result['paragraph'] = self.paragraph
-        if self.record_id is not None:
-            result['recordId'] = self.record_id
-        result['sentenceList'] = []
-        if self.sentence_list is not None:
-            for k in self.sentence_list:
-                result['sentenceList'].append(k.to_map() if k else None)
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.status is not None:
-            result['status'] = self.status
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.user_id_list is not None:
+            result['userIdList'] = self.user_id_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('nextTtoken') is not None:
-            self.next_ttoken = m.get('nextTtoken')
-        if m.get('nickName') is not None:
-            self.nick_name = m.get('nickName')
-        if m.get('paragraph') is not None:
-            self.paragraph = m.get('paragraph')
-        if m.get('recordId') is not None:
-            self.record_id = m.get('recordId')
-        self.sentence_list = []
-        if m.get('sentenceList') is not None:
-            for k in m.get('sentenceList'):
-                temp_model = QueryCloudRecordTextResponseBodyParagraphListSentenceList()
-                self.sentence_list.append(temp_model.from_map(k))
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('userIdList') is not None:
+            self.user_id_list = m.get('userIdList')
         return self
 
 
-class QueryCloudRecordTextResponseBody(TeaModel):
-    def __init__(
-        self,
-        has_more: bool = None,
-        paragraph_list: List[QueryCloudRecordTextResponseBodyParagraphList] = None,
-    ):
-        self.has_more = has_more
-        self.paragraph_list = paragraph_list
-
-    def validate(self):
-        if self.paragraph_list:
-            for k in self.paragraph_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.has_more is not None:
-            result['hasMore'] = self.has_more
-        result['paragraphList'] = []
-        if self.paragraph_list is not None:
-            for k in self.paragraph_list:
-                result['paragraphList'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('hasMore') is not None:
-            self.has_more = m.get('hasMore')
-        self.paragraph_list = []
-        if m.get('paragraphList') is not None:
-            for k in m.get('paragraphList'):
-                temp_model = QueryCloudRecordTextResponseBodyParagraphList()
-                self.paragraph_list.append(temp_model.from_map(k))
-        return self
-
-
-class QueryCloudRecordTextResponse(TeaModel):
+class ListDeptUserIdsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryCloudRecordTextResponseBody = None,
+        body: ListDeptUserIdsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1647,20 +1606,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryCloudRecordTextResponseBody()
+            temp_model = ListDeptUserIdsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryCloudRecordVideoHeaders(TeaModel):
+class ListDeptUsersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1685,157 +1644,181 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryCloudRecordVideoRequest(TeaModel):
+class ListDeptUsersRequest(TeaModel):
     def __init__(
         self,
-        union_id: str = None,
+        contain_access_limit: bool = None,
+        cursor: int = None,
+        language: str = None,
+        order_field: str = None,
+        size: int = None,
+        sub_corp_id: str = None,
     ):
-        self.union_id = union_id
+        self.contain_access_limit = contain_access_limit
+        self.cursor = cursor
+        self.language = language
+        self.order_field = order_field
+        self.size = size
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.contain_access_limit is not None:
+            result['containAccessLimit'] = self.contain_access_limit
+        if self.cursor is not None:
+            result['cursor'] = self.cursor
+        if self.language is not None:
+            result['language'] = self.language
+        if self.order_field is not None:
+            result['orderField'] = self.order_field
+        if self.size is not None:
+            result['size'] = self.size
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('containAccessLimit') is not None:
+            self.contain_access_limit = m.get('containAccessLimit')
+        if m.get('cursor') is not None:
+            self.cursor = m.get('cursor')
+        if m.get('language') is not None:
+            self.language = m.get('language')
+        if m.get('orderField') is not None:
+            self.order_field = m.get('orderField')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class QueryCloudRecordVideoResponseBodyVideoList(TeaModel):
+class ListDeptUsersResponseBodyUserList(TeaModel):
     def __init__(
         self,
-        duration: int = None,
-        end_time: int = None,
-        file_size: int = None,
-        media_id: str = None,
-        record_id: str = None,
-        record_type: int = None,
-        region_id: str = None,
-        start_time: int = None,
+        active: bool = None,
+        department_list: List[int] = None,
+        job_number: str = None,
+        name: str = None,
         union_id: str = None,
+        user_id: str = None,
     ):
-        self.duration = duration
-        self.end_time = end_time
-        self.file_size = file_size
-        self.media_id = media_id
-        self.record_id = record_id
-        self.record_type = record_type
-        self.region_id = region_id
-        self.start_time = start_time
+        self.active = active
+        self.department_list = department_list
+        self.job_number = job_number
+        self.name = name
         self.union_id = union_id
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.duration is not None:
-            result['duration'] = self.duration
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.file_size is not None:
-            result['fileSize'] = self.file_size
-        if self.media_id is not None:
-            result['mediaId'] = self.media_id
-        if self.record_id is not None:
-            result['recordId'] = self.record_id
-        if self.record_type is not None:
-            result['recordType'] = self.record_type
-        if self.region_id is not None:
-            result['regionId'] = self.region_id
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
+        if self.active is not None:
+            result['active'] = self.active
+        if self.department_list is not None:
+            result['departmentList'] = self.department_list
+        if self.job_number is not None:
+            result['jobNumber'] = self.job_number
+        if self.name is not None:
+            result['name'] = self.name
         if self.union_id is not None:
             result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('duration') is not None:
-            self.duration = m.get('duration')
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('fileSize') is not None:
-            self.file_size = m.get('fileSize')
-        if m.get('mediaId') is not None:
-            self.media_id = m.get('mediaId')
-        if m.get('recordId') is not None:
-            self.record_id = m.get('recordId')
-        if m.get('recordType') is not None:
-            self.record_type = m.get('recordType')
-        if m.get('regionId') is not None:
-            self.region_id = m.get('regionId')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
+        if m.get('active') is not None:
+            self.active = m.get('active')
+        if m.get('departmentList') is not None:
+            self.department_list = m.get('departmentList')
+        if m.get('jobNumber') is not None:
+            self.job_number = m.get('jobNumber')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class QueryCloudRecordVideoResponseBody(TeaModel):
+class ListDeptUsersResponseBody(TeaModel):
     def __init__(
         self,
-        video_list: List[QueryCloudRecordVideoResponseBodyVideoList] = None,
+        has_more: bool = None,
+        next_cursor: int = None,
+        user_list: List[ListDeptUsersResponseBodyUserList] = None,
     ):
-        self.video_list = video_list
+        self.has_more = has_more
+        self.next_cursor = next_cursor
+        self.user_list = user_list
 
     def validate(self):
-        if self.video_list:
-            for k in self.video_list:
+        if self.user_list:
+            for k in self.user_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['videoList'] = []
-        if self.video_list is not None:
-            for k in self.video_list:
-                result['videoList'].append(k.to_map() if k else None)
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        if self.next_cursor is not None:
+            result['nextCursor'] = self.next_cursor
+        result['userList'] = []
+        if self.user_list is not None:
+            for k in self.user_list:
+                result['userList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.video_list = []
-        if m.get('videoList') is not None:
-            for k in m.get('videoList'):
-                temp_model = QueryCloudRecordVideoResponseBodyVideoList()
-                self.video_list.append(temp_model.from_map(k))
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        if m.get('nextCursor') is not None:
+            self.next_cursor = m.get('nextCursor')
+        self.user_list = []
+        if m.get('userList') is not None:
+            for k in m.get('userList'):
+                temp_model = ListDeptUsersResponseBodyUserList()
+                self.user_list.append(temp_model.from_map(k))
         return self
 
 
-class QueryCloudRecordVideoResponse(TeaModel):
+class ListDeptUsersResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryCloudRecordVideoResponseBody = None,
+        body: ListDeptUsersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1861,20 +1844,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryCloudRecordVideoResponseBody()
+            temp_model = ListDeptUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryCloudRecordVideoPlayInfoHeaders(TeaModel):
+class ListParentByDeptHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1899,110 +1882,80 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryCloudRecordVideoPlayInfoRequest(TeaModel):
+class ListParentByDeptRequest(TeaModel):
     def __init__(
         self,
-        media_id: str = None,
-        region_id: str = None,
-        union_id: str = None,
+        department_id: int = None,
+        sub_corp_id: str = None,
     ):
-        self.media_id = media_id
-        self.region_id = region_id
-        self.union_id = union_id
+        self.department_id = department_id
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.media_id is not None:
-            result['mediaId'] = self.media_id
-        if self.region_id is not None:
-            result['regionId'] = self.region_id
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('mediaId') is not None:
-            self.media_id = m.get('mediaId')
-        if m.get('regionId') is not None:
-            self.region_id = m.get('regionId')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class QueryCloudRecordVideoPlayInfoResponseBody(TeaModel):
+class ListParentByDeptResponseBody(TeaModel):
     def __init__(
         self,
-        duration: int = None,
-        file_size: int = None,
-        mp_4file_url: str = None,
-        play_url: str = None,
-        status: int = None,
+        department_id_list: List[int] = None,
     ):
-        self.duration = duration
-        self.file_size = file_size
-        self.mp_4file_url = mp_4file_url
-        self.play_url = play_url
-        self.status = status
+        self.department_id_list = department_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.duration is not None:
-            result['duration'] = self.duration
-        if self.file_size is not None:
-            result['fileSize'] = self.file_size
-        if self.mp_4file_url is not None:
-            result['mp4FileUrl'] = self.mp_4file_url
-        if self.play_url is not None:
-            result['playUrl'] = self.play_url
-        if self.status is not None:
-            result['status'] = self.status
+        if self.department_id_list is not None:
+            result['departmentIdList'] = self.department_id_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('duration') is not None:
-            self.duration = m.get('duration')
-        if m.get('fileSize') is not None:
-            self.file_size = m.get('fileSize')
-        if m.get('mp4FileUrl') is not None:
-            self.mp_4file_url = m.get('mp4FileUrl')
-        if m.get('playUrl') is not None:
-            self.play_url = m.get('playUrl')
-        if m.get('status') is not None:
-            self.status = m.get('status')
+        if m.get('departmentIdList') is not None:
+            self.department_id_list = m.get('departmentIdList')
         return self
 
 
-class QueryCloudRecordVideoPlayInfoResponse(TeaModel):
+class ListParentByDeptResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryCloudRecordVideoPlayInfoResponseBody = None,
+        body: ListParentByDeptResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2028,20 +1981,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryCloudRecordVideoPlayInfoResponseBody()
+            temp_model = ListParentByDeptResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryConferenceInfoHeaders(TeaModel):
+class ListParentByUserHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2066,148 +2019,80 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryConferenceInfoResponseBodyConfInfo(TeaModel):
+class ListParentByUserRequest(TeaModel):
     def __init__(
         self,
-        active_num: int = None,
-        attend_num: int = None,
-        conf_duration: int = None,
-        conference_id: str = None,
-        creator_id: str = None,
-        creator_nick: str = None,
-        end_time: int = None,
-        external_link_url: str = None,
-        invited_num: int = None,
-        room_code: str = None,
-        start_time: int = None,
-        status: int = None,
-        title: str = None,
+        sub_corp_id: str = None,
+        user_id: str = None,
     ):
-        self.active_num = active_num
-        self.attend_num = attend_num
-        self.conf_duration = conf_duration
-        self.conference_id = conference_id
-        self.creator_id = creator_id
-        self.creator_nick = creator_nick
-        self.end_time = end_time
-        self.external_link_url = external_link_url
-        self.invited_num = invited_num
-        self.room_code = room_code
-        self.start_time = start_time
-        self.status = status
-        self.title = title
+        self.sub_corp_id = sub_corp_id
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.active_num is not None:
-            result['activeNum'] = self.active_num
-        if self.attend_num is not None:
-            result['attendNum'] = self.attend_num
-        if self.conf_duration is not None:
-            result['confDuration'] = self.conf_duration
-        if self.conference_id is not None:
-            result['conferenceId'] = self.conference_id
-        if self.creator_id is not None:
-            result['creatorId'] = self.creator_id
-        if self.creator_nick is not None:
-            result['creatorNick'] = self.creator_nick
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.external_link_url is not None:
-            result['externalLinkUrl'] = self.external_link_url
-        if self.invited_num is not None:
-            result['invitedNum'] = self.invited_num
-        if self.room_code is not None:
-            result['roomCode'] = self.room_code
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.status is not None:
-            result['status'] = self.status
-        if self.title is not None:
-            result['title'] = self.title
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('activeNum') is not None:
-            self.active_num = m.get('activeNum')
-        if m.get('attendNum') is not None:
-            self.attend_num = m.get('attendNum')
-        if m.get('confDuration') is not None:
-            self.conf_duration = m.get('confDuration')
-        if m.get('conferenceId') is not None:
-            self.conference_id = m.get('conferenceId')
-        if m.get('creatorId') is not None:
-            self.creator_id = m.get('creatorId')
-        if m.get('creatorNick') is not None:
-            self.creator_nick = m.get('creatorNick')
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('externalLinkUrl') is not None:
-            self.external_link_url = m.get('externalLinkUrl')
-        if m.get('invitedNum') is not None:
-            self.invited_num = m.get('invitedNum')
-        if m.get('roomCode') is not None:
-            self.room_code = m.get('roomCode')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('title') is not None:
-            self.title = m.get('title')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class QueryConferenceInfoResponseBody(TeaModel):
+class ListParentByUserResponseBody(TeaModel):
     def __init__(
         self,
-        conf_info: QueryConferenceInfoResponseBodyConfInfo = None,
+        department_id_list: List[int] = None,
     ):
-        self.conf_info = conf_info
+        self.department_id_list = department_id_list
 
     def validate(self):
-        if self.conf_info:
-            self.conf_info.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.conf_info is not None:
-            result['confInfo'] = self.conf_info.to_map()
+        if self.department_id_list is not None:
+            result['departmentIdList'] = self.department_id_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('confInfo') is not None:
-            temp_model = QueryConferenceInfoResponseBodyConfInfo()
-            self.conf_info = temp_model.from_map(m['confInfo'])
+        if m.get('departmentIdList') is not None:
+            self.department_id_list = m.get('departmentIdList')
         return self
 
 
-class QueryConferenceInfoResponse(TeaModel):
+class ListParentByUserResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryConferenceInfoResponseBody = None,
+        body: ListParentByUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2233,20 +2118,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryConferenceInfoResponseBody()
+            temp_model = ListParentByUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryConferenceInfoBatchHeaders(TeaModel):
+class ListResidentDeptUsersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2271,204 +2156,210 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryConferenceInfoBatchRequest(TeaModel):
+class ListResidentDeptUsersRequest(TeaModel):
     def __init__(
         self,
-        conference_id_list: List[str] = None,
+        cursor: int = None,
+        role: str = None,
+        size: int = None,
+        sub_corp_id: str = None,
     ):
-        self.conference_id_list = conference_id_list
+        self.cursor = cursor
+        self.role = role
+        self.size = size
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.conference_id_list is not None:
-            result['conferenceIdList'] = self.conference_id_list
+        if self.cursor is not None:
+            result['cursor'] = self.cursor
+        if self.role is not None:
+            result['role'] = self.role
+        if self.size is not None:
+            result['size'] = self.size
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('conferenceIdList') is not None:
-            self.conference_id_list = m.get('conferenceIdList')
+        if m.get('cursor') is not None:
+            self.cursor = m.get('cursor')
+        if m.get('role') is not None:
+            self.role = m.get('role')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class QueryConferenceInfoBatchResponseBodyInfosUserList(TeaModel):
+class ListResidentDeptUsersResponseBodyUserListRoles(TeaModel):
     def __init__(
         self,
-        attend_status: int = None,
-        camera_status: int = None,
-        mic_status: int = None,
-        nick: str = None,
-        reject_description: str = None,
-        user_id: str = None,
+        tag_code: str = None,
+        tag_id: int = None,
+        tag_name: str = None,
     ):
-        self.attend_status = attend_status
-        self.camera_status = camera_status
-        self.mic_status = mic_status
-        self.nick = nick
-        self.reject_description = reject_description
-        self.user_id = user_id
+        self.tag_code = tag_code
+        self.tag_id = tag_id
+        self.tag_name = tag_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.attend_status is not None:
-            result['attendStatus'] = self.attend_status
-        if self.camera_status is not None:
-            result['cameraStatus'] = self.camera_status
-        if self.mic_status is not None:
-            result['micStatus'] = self.mic_status
-        if self.nick is not None:
-            result['nick'] = self.nick
-        if self.reject_description is not None:
-            result['rejectDescription'] = self.reject_description
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.tag_code is not None:
+            result['tagCode'] = self.tag_code
+        if self.tag_id is not None:
+            result['tagId'] = self.tag_id
+        if self.tag_name is not None:
+            result['tagName'] = self.tag_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('attendStatus') is not None:
-            self.attend_status = m.get('attendStatus')
-        if m.get('cameraStatus') is not None:
-            self.camera_status = m.get('cameraStatus')
-        if m.get('micStatus') is not None:
-            self.mic_status = m.get('micStatus')
-        if m.get('nick') is not None:
-            self.nick = m.get('nick')
-        if m.get('rejectDescription') is not None:
-            self.reject_description = m.get('rejectDescription')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('tagCode') is not None:
+            self.tag_code = m.get('tagCode')
+        if m.get('tagId') is not None:
+            self.tag_id = m.get('tagId')
+        if m.get('tagName') is not None:
+            self.tag_name = m.get('tagName')
         return self
 
 
-class QueryConferenceInfoBatchResponseBodyInfos(TeaModel):
+class ListResidentDeptUsersResponseBodyUserList(TeaModel):
     def __init__(
         self,
-        conference_id: str = None,
-        media_status: int = None,
-        start_time: int = None,
-        status: int = None,
-        title: str = None,
-        user_list: List[QueryConferenceInfoBatchResponseBodyInfosUserList] = None,
+        feature: str = None,
+        name: str = None,
+        roles: List[ListResidentDeptUsersResponseBodyUserListRoles] = None,
+        union_id: str = None,
+        user_id: str = None,
     ):
-        self.conference_id = conference_id
-        self.media_status = media_status
-        self.start_time = start_time
-        self.status = status
-        self.title = title
-        self.user_list = user_list
+        self.feature = feature
+        self.name = name
+        self.roles = roles
+        self.union_id = union_id
+        self.user_id = user_id
 
     def validate(self):
-        if self.user_list:
-            for k in self.user_list:
+        if self.roles:
+            for k in self.roles:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.conference_id is not None:
-            result['conferenceId'] = self.conference_id
-        if self.media_status is not None:
-            result['mediaStatus'] = self.media_status
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.status is not None:
-            result['status'] = self.status
-        if self.title is not None:
-            result['title'] = self.title
-        result['userList'] = []
-        if self.user_list is not None:
-            for k in self.user_list:
-                result['userList'].append(k.to_map() if k else None)
+        if self.feature is not None:
+            result['feature'] = self.feature
+        if self.name is not None:
+            result['name'] = self.name
+        result['roles'] = []
+        if self.roles is not None:
+            for k in self.roles:
+                result['roles'].append(k.to_map() if k else None)
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('conferenceId') is not None:
-            self.conference_id = m.get('conferenceId')
-        if m.get('mediaStatus') is not None:
-            self.media_status = m.get('mediaStatus')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        self.user_list = []
-        if m.get('userList') is not None:
-            for k in m.get('userList'):
-                temp_model = QueryConferenceInfoBatchResponseBodyInfosUserList()
-                self.user_list.append(temp_model.from_map(k))
+        if m.get('feature') is not None:
+            self.feature = m.get('feature')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        self.roles = []
+        if m.get('roles') is not None:
+            for k in m.get('roles'):
+                temp_model = ListResidentDeptUsersResponseBodyUserListRoles()
+                self.roles.append(temp_model.from_map(k))
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class QueryConferenceInfoBatchResponseBody(TeaModel):
+class ListResidentDeptUsersResponseBody(TeaModel):
     def __init__(
         self,
-        infos: List[QueryConferenceInfoBatchResponseBodyInfos] = None,
+        has_more: bool = None,
+        next_cursor: int = None,
+        user_list: List[ListResidentDeptUsersResponseBodyUserList] = None,
     ):
-        self.infos = infos
+        self.has_more = has_more
+        self.next_cursor = next_cursor
+        self.user_list = user_list
 
     def validate(self):
-        if self.infos:
-            for k in self.infos:
+        if self.user_list:
+            for k in self.user_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['infos'] = []
-        if self.infos is not None:
-            for k in self.infos:
-                result['infos'].append(k.to_map() if k else None)
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        if self.next_cursor is not None:
+            result['nextCursor'] = self.next_cursor
+        result['userList'] = []
+        if self.user_list is not None:
+            for k in self.user_list:
+                result['userList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.infos = []
-        if m.get('infos') is not None:
-            for k in m.get('infos'):
-                temp_model = QueryConferenceInfoBatchResponseBodyInfos()
-                self.infos.append(temp_model.from_map(k))
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        if m.get('nextCursor') is not None:
+            self.next_cursor = m.get('nextCursor')
+        self.user_list = []
+        if m.get('userList') is not None:
+            for k in m.get('userList'):
+                temp_model = ListResidentDeptUsersResponseBodyUserList()
+                self.user_list.append(temp_model.from_map(k))
         return self
 
 
-class QueryConferenceInfoBatchResponse(TeaModel):
+class ListResidentDeptUsersResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryConferenceInfoBatchResponseBody = None,
+        body: ListResidentDeptUsersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2494,20 +2385,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryConferenceInfoBatchResponseBody()
+            temp_model = ListResidentDeptUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryConferenceMembersHeaders(TeaModel):
+class ListResidentSubDeptsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2532,187 +2423,151 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryConferenceMembersRequest(TeaModel):
+class ListResidentSubDeptsRequest(TeaModel):
     def __init__(
         self,
-        max_results: int = None,
-        next_token: str = None,
+        cursor: int = None,
+        size: int = None,
+        sub_corp_id: str = None,
     ):
-        self.max_results = max_results
-        self.next_token = next_token
+        self.cursor = cursor
+        self.size = size
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.max_results is not None:
-            result['maxResults'] = self.max_results
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
+        if self.cursor is not None:
+            result['cursor'] = self.cursor
+        if self.size is not None:
+            result['size'] = self.size
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('maxResults') is not None:
-            self.max_results = m.get('maxResults')
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
+        if m.get('cursor') is not None:
+            self.cursor = m.get('cursor')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class QueryConferenceMembersResponseBodyMemberModels(TeaModel):
+class ListResidentSubDeptsResponseBodyDepartmentList(TeaModel):
     def __init__(
         self,
-        attend_status: int = None,
-        co_host: bool = None,
-        conference_id: str = None,
-        duration: int = None,
-        host: bool = None,
-        join_time: int = None,
-        leave_time: int = None,
-        outer_org_member: bool = None,
-        pstn_join: bool = None,
-        union_id: str = None,
-        user_nick: str = None,
+        department_id: int = None,
+        department_name: str = None,
+        super_department_id: int = None,
     ):
-        self.attend_status = attend_status
-        self.co_host = co_host
-        self.conference_id = conference_id
-        self.duration = duration
-        self.host = host
-        self.join_time = join_time
-        self.leave_time = leave_time
-        self.outer_org_member = outer_org_member
-        self.pstn_join = pstn_join
-        self.union_id = union_id
-        self.user_nick = user_nick
+        self.department_id = department_id
+        self.department_name = department_name
+        self.super_department_id = super_department_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.attend_status is not None:
-            result['attendStatus'] = self.attend_status
-        if self.co_host is not None:
-            result['coHost'] = self.co_host
-        if self.conference_id is not None:
-            result['conferenceId'] = self.conference_id
-        if self.duration is not None:
-            result['duration'] = self.duration
-        if self.host is not None:
-            result['host'] = self.host
-        if self.join_time is not None:
-            result['joinTime'] = self.join_time
-        if self.leave_time is not None:
-            result['leaveTime'] = self.leave_time
-        if self.outer_org_member is not None:
-            result['outerOrgMember'] = self.outer_org_member
-        if self.pstn_join is not None:
-            result['pstnJoin'] = self.pstn_join
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
-        if self.user_nick is not None:
-            result['userNick'] = self.user_nick
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.department_name is not None:
+            result['departmentName'] = self.department_name
+        if self.super_department_id is not None:
+            result['superDepartmentId'] = self.super_department_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('attendStatus') is not None:
-            self.attend_status = m.get('attendStatus')
-        if m.get('coHost') is not None:
-            self.co_host = m.get('coHost')
-        if m.get('conferenceId') is not None:
-            self.conference_id = m.get('conferenceId')
-        if m.get('duration') is not None:
-            self.duration = m.get('duration')
-        if m.get('host') is not None:
-            self.host = m.get('host')
-        if m.get('joinTime') is not None:
-            self.join_time = m.get('joinTime')
-        if m.get('leaveTime') is not None:
-            self.leave_time = m.get('leaveTime')
-        if m.get('outerOrgMember') is not None:
-            self.outer_org_member = m.get('outerOrgMember')
-        if m.get('pstnJoin') is not None:
-            self.pstn_join = m.get('pstnJoin')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
-        if m.get('userNick') is not None:
-            self.user_nick = m.get('userNick')
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('departmentName') is not None:
+            self.department_name = m.get('departmentName')
+        if m.get('superDepartmentId') is not None:
+            self.super_department_id = m.get('superDepartmentId')
         return self
 
 
-class QueryConferenceMembersResponseBody(TeaModel):
+class ListResidentSubDeptsResponseBody(TeaModel):
     def __init__(
         self,
-        member_models: List[QueryConferenceMembersResponseBodyMemberModels] = None,
-        next_token: str = None,
-        total_count: int = None,
+        department_list: List[ListResidentSubDeptsResponseBodyDepartmentList] = None,
+        has_more: bool = None,
+        next_cursor: int = None,
+        total: int = None,
     ):
-        self.member_models = member_models
-        self.next_token = next_token
-        self.total_count = total_count
+        self.department_list = department_list
+        self.has_more = has_more
+        self.next_cursor = next_cursor
+        self.total = total
 
     def validate(self):
-        if self.member_models:
-            for k in self.member_models:
+        if self.department_list:
+            for k in self.department_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['memberModels'] = []
-        if self.member_models is not None:
-            for k in self.member_models:
-                result['memberModels'].append(k.to_map() if k else None)
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
+        result['departmentList'] = []
+        if self.department_list is not None:
+            for k in self.department_list:
+                result['departmentList'].append(k.to_map() if k else None)
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        if self.next_cursor is not None:
+            result['nextCursor'] = self.next_cursor
+        if self.total is not None:
+            result['total'] = self.total
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.member_models = []
-        if m.get('memberModels') is not None:
-            for k in m.get('memberModels'):
-                temp_model = QueryConferenceMembersResponseBodyMemberModels()
-                self.member_models.append(temp_model.from_map(k))
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
+        self.department_list = []
+        if m.get('departmentList') is not None:
+            for k in m.get('departmentList'):
+                temp_model = ListResidentSubDeptsResponseBodyDepartmentList()
+                self.department_list.append(temp_model.from_map(k))
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        if m.get('nextCursor') is not None:
+            self.next_cursor = m.get('nextCursor')
+        if m.get('total') is not None:
+            self.total = m.get('total')
         return self
 
 
-class QueryConferenceMembersResponse(TeaModel):
+class ListResidentSubDeptsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryConferenceMembersResponseBody = None,
+        body: ListResidentSubDeptsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2738,20 +2593,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryConferenceMembersResponseBody()
+            temp_model = ListResidentSubDeptsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryScheduleConferenceInfoHeaders(TeaModel):
+class ListResidentUserInfosHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2776,300 +2631,219 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryScheduleConferenceInfoRequest(TeaModel):
+class ListResidentUserInfosRequest(TeaModel):
     def __init__(
         self,
-        max_results: int = None,
-        next_token: str = None,
+        sub_corp_id: str = None,
+        user_ids: List[str] = None,
     ):
-        self.max_results = max_results
-        self.next_token = next_token
+        self.sub_corp_id = sub_corp_id
+        self.user_ids = user_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.max_results is not None:
-            result['maxResults'] = self.max_results
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
+        if self.user_ids is not None:
+            result['userIds'] = self.user_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('maxResults') is not None:
-            self.max_results = m.get('maxResults')
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
+        if m.get('userIds') is not None:
+            self.user_ids = m.get('userIds')
         return self
 
 
-class QueryScheduleConferenceInfoResponseBodyConferenceList(TeaModel):
+class ListResidentUserInfosShrinkRequest(TeaModel):
     def __init__(
         self,
-        conference_id: str = None,
-        end_time: int = None,
-        room_code: str = None,
-        start_time: int = None,
-        status: int = None,
-        title: str = None,
+        sub_corp_id: str = None,
+        user_ids_shrink: str = None,
     ):
-        self.conference_id = conference_id
-        self.end_time = end_time
-        self.room_code = room_code
-        self.start_time = start_time
-        self.status = status
-        self.title = title
+        self.sub_corp_id = sub_corp_id
+        self.user_ids_shrink = user_ids_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.conference_id is not None:
-            result['conferenceId'] = self.conference_id
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.room_code is not None:
-            result['roomCode'] = self.room_code
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.status is not None:
-            result['status'] = self.status
-        if self.title is not None:
-            result['title'] = self.title
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
+        if self.user_ids_shrink is not None:
+            result['userIds'] = self.user_ids_shrink
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('conferenceId') is not None:
-            self.conference_id = m.get('conferenceId')
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('roomCode') is not None:
-            self.room_code = m.get('roomCode')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('title') is not None:
-            self.title = m.get('title')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
+        if m.get('userIds') is not None:
+            self.user_ids_shrink = m.get('userIds')
         return self
 
 
-class QueryScheduleConferenceInfoResponseBody(TeaModel):
+class ListResidentUserInfosResponseBodyUserListRoles(TeaModel):
     def __init__(
         self,
-        conference_list: List[QueryScheduleConferenceInfoResponseBodyConferenceList] = None,
-        next_token: str = None,
-        total_count: int = None,
+        tag_code: str = None,
+        tag_id: int = None,
+        tag_name: str = None,
     ):
-        self.conference_list = conference_list
-        self.next_token = next_token
-        self.total_count = total_count
-
-    def validate(self):
-        if self.conference_list:
-            for k in self.conference_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['conferenceList'] = []
-        if self.conference_list is not None:
-            for k in self.conference_list:
-                result['conferenceList'].append(k.to_map() if k else None)
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.conference_list = []
-        if m.get('conferenceList') is not None:
-            for k in m.get('conferenceList'):
-                temp_model = QueryScheduleConferenceInfoResponseBodyConferenceList()
-                self.conference_list.append(temp_model.from_map(k))
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
-        return self
-
-
-class QueryScheduleConferenceInfoResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: QueryScheduleConferenceInfoResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = QueryScheduleConferenceInfoResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class StartCloudRecordHeaders(TeaModel):
-    def __init__(
-        self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
-    ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+        self.tag_code = tag_code
+        self.tag_id = tag_id
+        self.tag_name = tag_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        if self.tag_code is not None:
+            result['tagCode'] = self.tag_code
+        if self.tag_id is not None:
+            result['tagId'] = self.tag_id
+        if self.tag_name is not None:
+            result['tagName'] = self.tag_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        if m.get('tagCode') is not None:
+            self.tag_code = m.get('tagCode')
+        if m.get('tagId') is not None:
+            self.tag_id = m.get('tagId')
+        if m.get('tagName') is not None:
+            self.tag_name = m.get('tagName')
         return self
 
 
-class StartCloudRecordRequest(TeaModel):
+class ListResidentUserInfosResponseBodyUserList(TeaModel):
     def __init__(
         self,
-        mode: str = None,
-        small_window_position: str = None,
+        feature: str = None,
+        roles: List[ListResidentUserInfosResponseBodyUserListRoles] = None,
         union_id: str = None,
+        user_id: str = None,
+        user_name: str = None,
     ):
-        self.mode = mode
-        self.small_window_position = small_window_position
+        self.feature = feature
+        self.roles = roles
         self.union_id = union_id
+        self.user_id = user_id
+        self.user_name = user_name
 
     def validate(self):
-        pass
+        if self.roles:
+            for k in self.roles:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.mode is not None:
-            result['mode'] = self.mode
-        if self.small_window_position is not None:
-            result['smallWindowPosition'] = self.small_window_position
+        if self.feature is not None:
+            result['feature'] = self.feature
+        result['roles'] = []
+        if self.roles is not None:
+            for k in self.roles:
+                result['roles'].append(k.to_map() if k else None)
         if self.union_id is not None:
             result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.user_name is not None:
+            result['userName'] = self.user_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('mode') is not None:
-            self.mode = m.get('mode')
-        if m.get('smallWindowPosition') is not None:
-            self.small_window_position = m.get('smallWindowPosition')
+        if m.get('feature') is not None:
+            self.feature = m.get('feature')
+        self.roles = []
+        if m.get('roles') is not None:
+            for k in m.get('roles'):
+                temp_model = ListResidentUserInfosResponseBodyUserListRoles()
+                self.roles.append(temp_model.from_map(k))
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('userName') is not None:
+            self.user_name = m.get('userName')
         return self
 
 
-class StartCloudRecordResponseBody(TeaModel):
+class ListResidentUserInfosResponseBody(TeaModel):
     def __init__(
         self,
-        code: str = None,
+        user_list: List[ListResidentUserInfosResponseBodyUserList] = None,
     ):
-        self.code = code
+        self.user_list = user_list
 
     def validate(self):
-        pass
+        if self.user_list:
+            for k in self.user_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.code is not None:
-            result['code'] = self.code
+        result['userList'] = []
+        if self.user_list is not None:
+            for k in self.user_list:
+                result['userList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('code') is not None:
-            self.code = m.get('code')
+        self.user_list = []
+        if m.get('userList') is not None:
+            for k in m.get('userList'):
+                temp_model = ListResidentUserInfosResponseBodyUserList()
+                self.user_list.append(temp_model.from_map(k))
         return self
 
 
-class StartCloudRecordResponse(TeaModel):
+class ListResidentUserInfosResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: StartCloudRecordResponseBody = None,
+        body: ListResidentUserInfosResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3095,20 +2869,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = StartCloudRecordResponseBody()
+            temp_model = ListResidentUserInfosResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class StartStreamOutHeaders(TeaModel):
+class ListSimpleUsersByRoleHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -3133,110 +2907,157 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class StartStreamOutRequest(TeaModel):
+class ListSimpleUsersByRoleRequest(TeaModel):
     def __init__(
         self,
-        mode: str = None,
-        need_host_join: bool = None,
-        small_window_position: str = None,
-        stream_name: str = None,
-        stream_url_list: List[str] = None,
+        offset: int = None,
+        role_id: int = None,
+        size: int = None,
+        sub_corp_id: str = None,
+    ):
+        self.offset = offset
+        self.role_id = role_id
+        self.size = size
+        self.sub_corp_id = sub_corp_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.offset is not None:
+            result['offset'] = self.offset
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        if self.size is not None:
+            result['size'] = self.size
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('offset') is not None:
+            self.offset = m.get('offset')
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
+        return self
+
+
+class ListSimpleUsersByRoleResponseBodyUserList(TeaModel):
+    def __init__(
+        self,
+        job_number: str = None,
+        name: str = None,
         union_id: str = None,
+        user_id: str = None,
     ):
-        self.mode = mode
-        self.need_host_join = need_host_join
-        self.small_window_position = small_window_position
-        self.stream_name = stream_name
-        self.stream_url_list = stream_url_list
+        self.job_number = job_number
+        self.name = name
         self.union_id = union_id
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.mode is not None:
-            result['mode'] = self.mode
-        if self.need_host_join is not None:
-            result['needHostJoin'] = self.need_host_join
-        if self.small_window_position is not None:
-            result['smallWindowPosition'] = self.small_window_position
-        if self.stream_name is not None:
-            result['streamName'] = self.stream_name
-        if self.stream_url_list is not None:
-            result['streamUrlList'] = self.stream_url_list
+        if self.job_number is not None:
+            result['jobNumber'] = self.job_number
+        if self.name is not None:
+            result['name'] = self.name
         if self.union_id is not None:
             result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('mode') is not None:
-            self.mode = m.get('mode')
-        if m.get('needHostJoin') is not None:
-            self.need_host_join = m.get('needHostJoin')
-        if m.get('smallWindowPosition') is not None:
-            self.small_window_position = m.get('smallWindowPosition')
-        if m.get('streamName') is not None:
-            self.stream_name = m.get('streamName')
-        if m.get('streamUrlList') is not None:
-            self.stream_url_list = m.get('streamUrlList')
+        if m.get('jobNumber') is not None:
+            self.job_number = m.get('jobNumber')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class StartStreamOutResponseBody(TeaModel):
+class ListSimpleUsersByRoleResponseBody(TeaModel):
     def __init__(
         self,
-        fail_stream_map: Dict[str, Any] = None,
-        success_stream_map: Dict[str, Any] = None,
+        has_more: bool = None,
+        next_cursor: int = None,
+        user_list: List[ListSimpleUsersByRoleResponseBodyUserList] = None,
     ):
-        self.fail_stream_map = fail_stream_map
-        self.success_stream_map = success_stream_map
+        self.has_more = has_more
+        self.next_cursor = next_cursor
+        self.user_list = user_list
 
     def validate(self):
-        pass
+        if self.user_list:
+            for k in self.user_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fail_stream_map is not None:
-            result['failStreamMap'] = self.fail_stream_map
-        if self.success_stream_map is not None:
-            result['successStreamMap'] = self.success_stream_map
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        if self.next_cursor is not None:
+            result['nextCursor'] = self.next_cursor
+        result['userList'] = []
+        if self.user_list is not None:
+            for k in self.user_list:
+                result['userList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('failStreamMap') is not None:
-            self.fail_stream_map = m.get('failStreamMap')
-        if m.get('successStreamMap') is not None:
-            self.success_stream_map = m.get('successStreamMap')
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        if m.get('nextCursor') is not None:
+            self.next_cursor = m.get('nextCursor')
+        self.user_list = []
+        if m.get('userList') is not None:
+            for k in m.get('userList'):
+                temp_model = ListSimpleUsersByRoleResponseBodyUserList()
+                self.user_list.append(temp_model.from_map(k))
         return self
 
 
-class StartStreamOutResponse(TeaModel):
+class ListSimpleUsersByRoleResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: StartStreamOutResponseBody = None,
+        body: ListSimpleUsersByRoleResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3262,20 +3083,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = StartStreamOutResponseBody()
+            temp_model = ListSimpleUsersByRoleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class StopCloudRecordHeaders(TeaModel):
+class ListSubCorpsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -3300,74 +3121,157 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class StopCloudRecordRequest(TeaModel):
+class ListSubCorpsRequest(TeaModel):
     def __init__(
         self,
-        union_id: str = None,
+        is_only_direct: bool = None,
+        sub_corp_id: str = None,
+        types: str = None,
     ):
-        self.union_id = union_id
+        self.is_only_direct = is_only_direct
+        self.sub_corp_id = sub_corp_id
+        self.types = types
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.is_only_direct is not None:
+            result['isOnlyDirect'] = self.is_only_direct
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
+        if self.types is not None:
+            result['types'] = self.types
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('isOnlyDirect') is not None:
+            self.is_only_direct = m.get('isOnlyDirect')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
+        if m.get('types') is not None:
+            self.types = m.get('types')
         return self
 
 
-class StopCloudRecordResponseBody(TeaModel):
+class ListSubCorpsResponseBodyCorpList(TeaModel):
     def __init__(
         self,
-        code: str = None,
+        corp_id: str = None,
+        corp_name: str = None,
+        industry: str = None,
+        industry_code: int = None,
+        region_id: str = None,
+        region_location: str = None,
+        region_type: str = None,
     ):
-        self.code = code
+        self.corp_id = corp_id
+        self.corp_name = corp_name
+        self.industry = industry
+        self.industry_code = industry_code
+        self.region_id = region_id
+        self.region_location = region_location
+        self.region_type = region_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.code is not None:
-            result['code'] = self.code
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.corp_name is not None:
+            result['corpName'] = self.corp_name
+        if self.industry is not None:
+            result['industry'] = self.industry
+        if self.industry_code is not None:
+            result['industryCode'] = self.industry_code
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.region_location is not None:
+            result['regionLocation'] = self.region_location
+        if self.region_type is not None:
+            result['regionType'] = self.region_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('corpName') is not None:
+            self.corp_name = m.get('corpName')
+        if m.get('industry') is not None:
+            self.industry = m.get('industry')
+        if m.get('industryCode') is not None:
+            self.industry_code = m.get('industryCode')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('regionLocation') is not None:
+            self.region_location = m.get('regionLocation')
+        if m.get('regionType') is not None:
+            self.region_type = m.get('regionType')
+        return self
+
+
+class ListSubCorpsResponseBody(TeaModel):
+    def __init__(
+        self,
+        corp_list: List[ListSubCorpsResponseBodyCorpList] = None,
+    ):
+        self.corp_list = corp_list
+
+    def validate(self):
+        if self.corp_list:
+            for k in self.corp_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['corpList'] = []
+        if self.corp_list is not None:
+            for k in self.corp_list:
+                result['corpList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('code') is not None:
-            self.code = m.get('code')
+        self.corp_list = []
+        if m.get('corpList') is not None:
+            for k in m.get('corpList'):
+                temp_model = ListSubCorpsResponseBodyCorpList()
+                self.corp_list.append(temp_model.from_map(k))
         return self
 
 
-class StopCloudRecordResponse(TeaModel):
+class ListSubCorpsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: StopCloudRecordResponseBody = None,
+        body: ListSubCorpsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3393,20 +3297,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = StopCloudRecordResponseBody()
+            temp_model = ListSubCorpsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class StopStreamOutHeaders(TeaModel):
+class ListSubDeptHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -3431,196 +3335,121 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class StopStreamOutRequest(TeaModel):
+class ListSubDeptRequest(TeaModel):
     def __init__(
         self,
-        stop_all_stream: bool = None,
-        stream_id: str = None,
-        union_id: str = None,
+        language: str = None,
+        sub_corp_id: str = None,
     ):
-        self.stop_all_stream = stop_all_stream
-        self.stream_id = stream_id
-        self.union_id = union_id
+        self.language = language
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.stop_all_stream is not None:
-            result['stopAllStream'] = self.stop_all_stream
-        if self.stream_id is not None:
-            result['streamId'] = self.stream_id
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.language is not None:
+            result['language'] = self.language
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('stopAllStream') is not None:
-            self.stop_all_stream = m.get('stopAllStream')
-        if m.get('streamId') is not None:
-            self.stream_id = m.get('streamId')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('language') is not None:
+            self.language = m.get('language')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class StopStreamOutResponseBody(TeaModel):
+class ListSubDeptResponseBodyResult(TeaModel):
     def __init__(
         self,
-        code: str = None,
+        department_id: int = None,
+        name: str = None,
     ):
-        self.code = code
+        self.department_id = department_id
+        self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.code is not None:
-            result['code'] = self.code
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.name is not None:
+            result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('code') is not None:
-            self.code = m.get('code')
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         return self
 
 
-class StopStreamOutResponse(TeaModel):
+class ListSubDeptResponseBody(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: StopStreamOutResponseBody = None,
+        result: List[ListSubDeptResponseBodyResult] = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.result = result
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = StopStreamOutResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class UpdateVideoConferenceExtInfoHeaders(TeaModel):
-    def __init__(
-        self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
-    ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
-        return self
-
-
-class UpdateVideoConferenceExtInfoResponseBody(TeaModel):
-    def __init__(
-        self,
-        case: str = None,
-        code: str = None,
-    ):
-        self.case = case
-        self.code = code
-
-    def validate(self):
-        pass
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.case is not None:
-            result['case'] = self.case
-        if self.code is not None:
-            result['code'] = self.code
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('case') is not None:
-            self.case = m.get('case')
-        if m.get('code') is not None:
-            self.code = m.get('code')
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = ListSubDeptResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
         return self
 
 
-class UpdateVideoConferenceExtInfoResponse(TeaModel):
+class ListSubDeptResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: UpdateVideoConferenceExtInfoResponseBody = None,
+        body: ListSubDeptResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3646,20 +3475,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = UpdateVideoConferenceExtInfoResponseBody()
+            temp_model = ListSubDeptResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class UpdateVideoConferenceSettingHeaders(TeaModel):
+class ListSubDeptIdsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -3684,110 +3513,74 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class UpdateVideoConferenceSettingRequest(TeaModel):
+class ListSubDeptIdsRequest(TeaModel):
     def __init__(
         self,
-        allow_unmute_self: bool = None,
-        auto_transfer_host: bool = None,
-        forbidden_share_screen: bool = None,
-        lock_conference: bool = None,
-        mute_all: bool = None,
-        only_internal_employees_join: bool = None,
+        sub_corp_id: str = None,
     ):
-        self.allow_unmute_self = allow_unmute_self
-        self.auto_transfer_host = auto_transfer_host
-        self.forbidden_share_screen = forbidden_share_screen
-        self.lock_conference = lock_conference
-        self.mute_all = mute_all
-        self.only_internal_employees_join = only_internal_employees_join
+        self.sub_corp_id = sub_corp_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.allow_unmute_self is not None:
-            result['allowUnmuteSelf'] = self.allow_unmute_self
-        if self.auto_transfer_host is not None:
-            result['autoTransferHost'] = self.auto_transfer_host
-        if self.forbidden_share_screen is not None:
-            result['forbiddenShareScreen'] = self.forbidden_share_screen
-        if self.lock_conference is not None:
-            result['lockConference'] = self.lock_conference
-        if self.mute_all is not None:
-            result['muteAll'] = self.mute_all
-        if self.only_internal_employees_join is not None:
-            result['onlyInternalEmployeesJoin'] = self.only_internal_employees_join
+        if self.sub_corp_id is not None:
+            result['subCorpId'] = self.sub_corp_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('allowUnmuteSelf') is not None:
-            self.allow_unmute_self = m.get('allowUnmuteSelf')
-        if m.get('autoTransferHost') is not None:
-            self.auto_transfer_host = m.get('autoTransferHost')
-        if m.get('forbiddenShareScreen') is not None:
-            self.forbidden_share_screen = m.get('forbiddenShareScreen')
-        if m.get('lockConference') is not None:
-            self.lock_conference = m.get('lockConference')
-        if m.get('muteAll') is not None:
-            self.mute_all = m.get('muteAll')
-        if m.get('onlyInternalEmployeesJoin') is not None:
-            self.only_internal_employees_join = m.get('onlyInternalEmployeesJoin')
+        if m.get('subCorpId') is not None:
+            self.sub_corp_id = m.get('subCorpId')
         return self
 
 
-class UpdateVideoConferenceSettingResponseBody(TeaModel):
+class ListSubDeptIdsResponseBody(TeaModel):
     def __init__(
         self,
-        case: str = None,
-        code: str = None,
+        department_id_list: List[int] = None,
     ):
-        self.case = case
-        self.code = code
+        self.department_id_list = department_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.case is not None:
-            result['case'] = self.case
-        if self.code is not None:
-            result['code'] = self.code
+        if self.department_id_list is not None:
+            result['departmentIdList'] = self.department_id_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('case') is not None:
-            self.case = m.get('case')
-        if m.get('code') is not None:
-            self.code = m.get('code')
+        if m.get('departmentIdList') is not None:
+            self.department_id_list = m.get('departmentIdList')
         return self
 
 
-class UpdateVideoConferenceSettingResponse(TeaModel):
+class ListSubDeptIdsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: UpdateVideoConferenceSettingResponseBody = None,
+        body: ListSubDeptIdsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3813,12 +3606,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = UpdateVideoConferenceSettingResponseBody()
+            temp_model = ListSubDeptIdsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7839,22 +7839,24 @@
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
         search_field: int = None,
         search_file_type: int = None,
         space_id: str = None,
+        space_ids: List[str] = None,
         summary_length: int = None,
         visit_time_range: SearchRequestDentryRequestVisitTimeRange = None,
     ):
         self.max_results = max_results
         self.next_token = next_token
         self.search_field = search_field
         self.search_file_type = search_file_type
         self.space_id = space_id
+        self.space_ids = space_ids
         self.summary_length = summary_length
         self.visit_time_range = visit_time_range
 
     def validate(self):
         if self.visit_time_range:
             self.visit_time_range.validate()
 
@@ -7870,14 +7872,16 @@
             result['nextToken'] = self.next_token
         if self.search_field is not None:
             result['searchField'] = self.search_field
         if self.search_file_type is not None:
             result['searchFileType'] = self.search_file_type
         if self.space_id is not None:
             result['spaceId'] = self.space_id
+        if self.space_ids is not None:
+            result['spaceIds'] = self.space_ids
         if self.summary_length is not None:
             result['summaryLength'] = self.summary_length
         if self.visit_time_range is not None:
             result['visitTimeRange'] = self.visit_time_range.to_map()
         return result
 
     def from_map(self, m: dict = None):
@@ -7888,14 +7892,16 @@
             self.next_token = m.get('nextToken')
         if m.get('searchField') is not None:
             self.search_field = m.get('searchField')
         if m.get('searchFileType') is not None:
             self.search_file_type = m.get('searchFileType')
         if m.get('spaceId') is not None:
             self.space_id = m.get('spaceId')
+        if m.get('spaceIds') is not None:
+            self.space_ids = m.get('spaceIds')
         if m.get('summaryLength') is not None:
             self.summary_length = m.get('summaryLength')
         if m.get('visitTimeRange') is not None:
             temp_model = SearchRequestDentryRequestVisitTimeRange()
             self.visit_time_range = temp_model.from_map(m['visitTimeRange'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3375,14 +3375,116 @@
         self,
         request: dingtalkedu__1__0_models.DeactivateDeviceRequest,
     ) -> dingtalkedu__1__0_models.DeactivateDeviceResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkedu__1__0_models.DeactivateDeviceHeaders()
         return await self.deactivate_device_with_options_async(request, headers, runtime)
 
+    def deduct_point_with_options(
+        self,
+        request: dingtalkedu__1__0_models.DeductPointRequest,
+        headers: dingtalkedu__1__0_models.DeductPointHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.DeductPointResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.biz_id):
+            body['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.deduct_desc):
+            body['deductDesc'] = request.deduct_desc
+        if not UtilClient.is_unset(request.deduct_detail_url):
+            body['deductDetailUrl'] = request.deduct_detail_url
+        if not UtilClient.is_unset(request.deduct_num):
+            body['deductNum'] = request.deduct_num
+        if not UtilClient.is_unset(request.point_type):
+            body['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeductPoint',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/deduct',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.DeductPointResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def deduct_point_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.DeductPointRequest,
+        headers: dingtalkedu__1__0_models.DeductPointHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.DeductPointResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.biz_id):
+            body['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.deduct_desc):
+            body['deductDesc'] = request.deduct_desc
+        if not UtilClient.is_unset(request.deduct_detail_url):
+            body['deductDetailUrl'] = request.deduct_detail_url
+        if not UtilClient.is_unset(request.deduct_num):
+            body['deductNum'] = request.deduct_num
+        if not UtilClient.is_unset(request.point_type):
+            body['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeductPoint',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/deduct',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.DeductPointResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def deduct_point(
+        self,
+        request: dingtalkedu__1__0_models.DeductPointRequest,
+    ) -> dingtalkedu__1__0_models.DeductPointResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.DeductPointHeaders()
+        return self.deduct_point_with_options(request, headers, runtime)
+
+    async def deduct_point_async(
+        self,
+        request: dingtalkedu__1__0_models.DeductPointRequest,
+    ) -> dingtalkedu__1__0_models.DeductPointResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.DeductPointHeaders()
+        return await self.deduct_point_with_options_async(request, headers, runtime)
+
     def delete_dept_with_options(
         self,
         dept_id: str,
         request: dingtalkedu__1__0_models.DeleteDeptRequest,
         headers: dingtalkedu__1__0_models.DeleteDeptHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkedu__1__0_models.DeleteDeptResponse:
@@ -5179,14 +5281,190 @@
         self,
         request: dingtalkedu__1__0_models.GetOpenCoursesRequest,
     ) -> dingtalkedu__1__0_models.GetOpenCoursesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkedu__1__0_models.GetOpenCoursesHeaders()
         return await self.get_open_courses_with_options_async(request, headers, runtime)
 
+    def get_point_action_record_with_options(
+        self,
+        request: dingtalkedu__1__0_models.GetPointActionRecordRequest,
+        headers: dingtalkedu__1__0_models.GetPointActionRecordHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetPointActionRecordResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.biz_id):
+            query['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.point_type):
+            query['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPointActionRecord',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/actionRecords',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetPointActionRecordResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_point_action_record_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.GetPointActionRecordRequest,
+        headers: dingtalkedu__1__0_models.GetPointActionRecordHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetPointActionRecordResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.biz_id):
+            query['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.point_type):
+            query['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPointActionRecord',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/actionRecords',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetPointActionRecordResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_point_action_record(
+        self,
+        request: dingtalkedu__1__0_models.GetPointActionRecordRequest,
+    ) -> dingtalkedu__1__0_models.GetPointActionRecordResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetPointActionRecordHeaders()
+        return self.get_point_action_record_with_options(request, headers, runtime)
+
+    async def get_point_action_record_async(
+        self,
+        request: dingtalkedu__1__0_models.GetPointActionRecordRequest,
+    ) -> dingtalkedu__1__0_models.GetPointActionRecordResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetPointActionRecordHeaders()
+        return await self.get_point_action_record_with_options_async(request, headers, runtime)
+
+    def get_point_info_with_options(
+        self,
+        request: dingtalkedu__1__0_models.GetPointInfoRequest,
+        headers: dingtalkedu__1__0_models.GetPointInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetPointInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.point_type):
+            query['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPointInfo',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/infos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetPointInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_point_info_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.GetPointInfoRequest,
+        headers: dingtalkedu__1__0_models.GetPointInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetPointInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.point_type):
+            query['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPointInfo',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/infos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetPointInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_point_info(
+        self,
+        request: dingtalkedu__1__0_models.GetPointInfoRequest,
+    ) -> dingtalkedu__1__0_models.GetPointInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetPointInfoHeaders()
+        return self.get_point_info_with_options(request, headers, runtime)
+
+    async def get_point_info_async(
+        self,
+        request: dingtalkedu__1__0_models.GetPointInfoRequest,
+    ) -> dingtalkedu__1__0_models.GetPointInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetPointInfoHeaders()
+        return await self.get_point_info_with_options_async(request, headers, runtime)
+
     def get_remote_class_course_with_options(
         self,
         course_code: str,
         request: dingtalkedu__1__0_models.GetRemoteClassCourseRequest,
         headers: dingtalkedu__1__0_models.GetRemoteClassCourseHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkedu__1__0_models.GetRemoteClassCourseResponse:
@@ -6437,14 +6715,108 @@
         self,
         request: dingtalkedu__1__0_models.PreDialRequest,
     ) -> dingtalkedu__1__0_models.PreDialResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkedu__1__0_models.PreDialHeaders()
         return await self.pre_dial_with_options_async(request, headers, runtime)
 
+    def provide_point_with_options(
+        self,
+        request: dingtalkedu__1__0_models.ProvidePointRequest,
+        headers: dingtalkedu__1__0_models.ProvidePointHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.ProvidePointResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.action_code):
+            body['actionCode'] = request.action_code
+        if not UtilClient.is_unset(request.biz_id):
+            body['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.point_type):
+            body['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ProvidePoint',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/provide',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.ProvidePointResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def provide_point_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.ProvidePointRequest,
+        headers: dingtalkedu__1__0_models.ProvidePointHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.ProvidePointResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.action_code):
+            body['actionCode'] = request.action_code
+        if not UtilClient.is_unset(request.biz_id):
+            body['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.point_type):
+            body['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ProvidePoint',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/points/provide',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.ProvidePointResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def provide_point(
+        self,
+        request: dingtalkedu__1__0_models.ProvidePointRequest,
+    ) -> dingtalkedu__1__0_models.ProvidePointResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.ProvidePointHeaders()
+        return self.provide_point_with_options(request, headers, runtime)
+
+    async def provide_point_async(
+        self,
+        request: dingtalkedu__1__0_models.ProvidePointRequest,
+    ) -> dingtalkedu__1__0_models.ProvidePointResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.ProvidePointHeaders()
+        return await self.provide_point_with_options_async(request, headers, runtime)
+
     def query_all_subjects_from_class_schedule_with_options(
         self,
         tmp_req: dingtalkedu__1__0_models.QueryAllSubjectsFromClassScheduleRequest,
         headers: dingtalkedu__1__0_models.QueryAllSubjectsFromClassScheduleHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkedu__1__0_models.QueryAllSubjectsFromClassScheduleResponse:
         UtilClient.validate_model(tmp_req)
@@ -8977,14 +9349,104 @@
         self,
         request: dingtalkedu__1__0_models.ReportDeviceUseLogRequest,
     ) -> dingtalkedu__1__0_models.ReportDeviceUseLogResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkedu__1__0_models.ReportDeviceUseLogHeaders()
         return await self.report_device_use_log_with_options_async(request, headers, runtime)
 
+    def rollback_deduct_point_with_options(
+        self,
+        request: dingtalkedu__1__0_models.RollbackDeductPointRequest,
+        headers: dingtalkedu__1__0_models.RollbackDeductPointHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.RollbackDeductPointResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.biz_id):
+            body['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.point_type):
+            body['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RollbackDeductPoint',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/deductPoints/rollback',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.RollbackDeductPointResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def rollback_deduct_point_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.RollbackDeductPointRequest,
+        headers: dingtalkedu__1__0_models.RollbackDeductPointHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.RollbackDeductPointResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.biz_id):
+            body['bizId'] = request.biz_id
+        if not UtilClient.is_unset(request.point_type):
+            body['pointType'] = request.point_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RollbackDeductPoint',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/deductPoints/rollback',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.RollbackDeductPointResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def rollback_deduct_point(
+        self,
+        request: dingtalkedu__1__0_models.RollbackDeductPointRequest,
+    ) -> dingtalkedu__1__0_models.RollbackDeductPointResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.RollbackDeductPointHeaders()
+        return self.rollback_deduct_point_with_options(request, headers, runtime)
+
+    async def rollback_deduct_point_async(
+        self,
+        request: dingtalkedu__1__0_models.RollbackDeductPointRequest,
+    ) -> dingtalkedu__1__0_models.RollbackDeductPointResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.RollbackDeductPointHeaders()
+        return await self.rollback_deduct_point_with_options_async(request, headers, runtime)
+
     def search_teachers_with_options(
         self,
         request: dingtalkedu__1__0_models.SearchTeachersRequest,
         headers: dingtalkedu__1__0_models.SearchTeachersHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkedu__1__0_models.SearchTeachersResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7016,14 +7016,175 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeactivateDeviceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeductPointHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class DeductPointRequest(TeaModel):
+    def __init__(
+        self,
+        biz_id: str = None,
+        deduct_desc: str = None,
+        deduct_detail_url: str = None,
+        deduct_num: int = None,
+        point_type: str = None,
+    ):
+        self.biz_id = biz_id
+        self.deduct_desc = deduct_desc
+        self.deduct_detail_url = deduct_detail_url
+        self.deduct_num = deduct_num
+        self.point_type = point_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_id is not None:
+            result['bizId'] = self.biz_id
+        if self.deduct_desc is not None:
+            result['deductDesc'] = self.deduct_desc
+        if self.deduct_detail_url is not None:
+            result['deductDetailUrl'] = self.deduct_detail_url
+        if self.deduct_num is not None:
+            result['deductNum'] = self.deduct_num
+        if self.point_type is not None:
+            result['pointType'] = self.point_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizId') is not None:
+            self.biz_id = m.get('bizId')
+        if m.get('deductDesc') is not None:
+            self.deduct_desc = m.get('deductDesc')
+        if m.get('deductDetailUrl') is not None:
+            self.deduct_detail_url = m.get('deductDetailUrl')
+        if m.get('deductNum') is not None:
+            self.deduct_num = m.get('deductNum')
+        if m.get('pointType') is not None:
+            self.point_type = m.get('pointType')
+        return self
+
+
+class DeductPointResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class DeductPointResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeductPointResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeductPointResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteDeptHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -10192,14 +10353,376 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetOpenCoursesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetPointActionRecordHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetPointActionRecordRequest(TeaModel):
+    def __init__(
+        self,
+        biz_id: str = None,
+        point_type: str = None,
+    ):
+        self.biz_id = biz_id
+        self.point_type = point_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_id is not None:
+            result['bizId'] = self.biz_id
+        if self.point_type is not None:
+            result['pointType'] = self.point_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizId') is not None:
+            self.biz_id = m.get('bizId')
+        if m.get('pointType') is not None:
+            self.point_type = m.get('pointType')
+        return self
+
+
+class GetPointActionRecordResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        action_time: str = None,
+        quantity: int = None,
+        status: str = None,
+    ):
+        self.action_time = action_time
+        self.quantity = quantity
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action_time is not None:
+            result['actionTime'] = self.action_time
+        if self.quantity is not None:
+            result['quantity'] = self.quantity
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('actionTime') is not None:
+            self.action_time = m.get('actionTime')
+        if m.get('quantity') is not None:
+            self.quantity = m.get('quantity')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
+class GetPointActionRecordResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: GetPointActionRecordResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = GetPointActionRecordResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class GetPointActionRecordResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetPointActionRecordResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetPointActionRecordResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetPointInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetPointInfoRequest(TeaModel):
+    def __init__(
+        self,
+        point_type: str = None,
+    ):
+        self.point_type = point_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.point_type is not None:
+            result['pointType'] = self.point_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('pointType') is not None:
+            self.point_type = m.get('pointType')
+        return self
+
+
+class GetPointInfoResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        available_quota: int = None,
+        end_time: str = None,
+        start_time: str = None,
+    ):
+        self.available_quota = available_quota
+        self.end_time = end_time
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.available_quota is not None:
+            result['availableQuota'] = self.available_quota
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('availableQuota') is not None:
+            self.available_quota = m.get('availableQuota')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        return self
+
+
+class GetPointInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: GetPointInfoResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = GetPointInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class GetPointInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetPointInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetPointInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetRemoteClassCourseHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -13279,14 +13802,204 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PreDialResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ProvidePointHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class ProvidePointRequest(TeaModel):
+    def __init__(
+        self,
+        action_code: str = None,
+        biz_id: str = None,
+        point_type: str = None,
+    ):
+        self.action_code = action_code
+        self.biz_id = biz_id
+        self.point_type = point_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action_code is not None:
+            result['actionCode'] = self.action_code
+        if self.biz_id is not None:
+            result['bizId'] = self.biz_id
+        if self.point_type is not None:
+            result['pointType'] = self.point_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('actionCode') is not None:
+            self.action_code = m.get('actionCode')
+        if m.get('bizId') is not None:
+            self.biz_id = m.get('bizId')
+        if m.get('pointType') is not None:
+            self.point_type = m.get('pointType')
+        return self
+
+
+class ProvidePointResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        available_quota: int = None,
+        provide_num: int = None,
+        provide_success: bool = None,
+    ):
+        self.available_quota = available_quota
+        self.provide_num = provide_num
+        self.provide_success = provide_success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.available_quota is not None:
+            result['availableQuota'] = self.available_quota
+        if self.provide_num is not None:
+            result['provideNum'] = self.provide_num
+        if self.provide_success is not None:
+            result['provideSuccess'] = self.provide_success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('availableQuota') is not None:
+            self.available_quota = m.get('availableQuota')
+        if m.get('provideNum') is not None:
+            self.provide_num = m.get('provideNum')
+        if m.get('provideSuccess') is not None:
+            self.provide_success = m.get('provideSuccess')
+        return self
+
+
+class ProvidePointResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: ProvidePointResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = ProvidePointResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class ProvidePointResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ProvidePointResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ProvidePointResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryAllSubjectsFromClassScheduleHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -19768,14 +20481,157 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ReportDeviceUseLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RollbackDeductPointHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class RollbackDeductPointRequest(TeaModel):
+    def __init__(
+        self,
+        biz_id: str = None,
+        point_type: str = None,
+    ):
+        self.biz_id = biz_id
+        self.point_type = point_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_id is not None:
+            result['bizId'] = self.biz_id
+        if self.point_type is not None:
+            result['pointType'] = self.point_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizId') is not None:
+            self.biz_id = m.get('bizId')
+        if m.get('pointType') is not None:
+            self.point_type = m.get('pointType')
+        return self
+
+
+class RollbackDeductPointResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class RollbackDeductPointResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RollbackDeductPointResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RollbackDeductPointResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SearchTeachersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
-from alibabacloud_dingtalk.flashmeeting_1_0 import models as dingtalkflashmeeting__1__0_models
+from alibabacloud_dingtalk.wiki_1_0 import models as dingtalkwiki__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
@@ -25,190 +25,178 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
-    def create_flash_meeting_with_options(
+    def wiki_words_detail_with_options(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-        headers: dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsDetailHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.creator):
-            body['creator'] = request.creator
-        if not UtilClient.is_unset(request.event_id):
-            body['eventId'] = request.event_id
-        if not UtilClient.is_unset(request.title):
-            body['title'] = request.title
+        query = {}
+        if not UtilClient.is_unset(request.word_name):
+            query['wordName'] = request.word_name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            body=OpenApiUtilClient.parse_to_map(body)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CreateFlashMeeting',
-            version='flashmeeting_1.0',
+            action='WikiWordsDetail',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/flashmeeting/meetings',
-            method='POST',
+            pathname=f'/v1.0/wiki/words/details',
+            method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse(),
+            dingtalkwiki__1__0_models.WikiWordsDetailResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def create_flash_meeting_with_options_async(
+    async def wiki_words_detail_with_options_async(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-        headers: dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsDetailHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.creator):
-            body['creator'] = request.creator
-        if not UtilClient.is_unset(request.event_id):
-            body['eventId'] = request.event_id
-        if not UtilClient.is_unset(request.title):
-            body['title'] = request.title
+        query = {}
+        if not UtilClient.is_unset(request.word_name):
+            query['wordName'] = request.word_name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            body=OpenApiUtilClient.parse_to_map(body)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CreateFlashMeeting',
-            version='flashmeeting_1.0',
+            action='WikiWordsDetail',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/flashmeeting/meetings',
-            method='POST',
+            pathname=f'/v1.0/wiki/words/details',
+            method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse(),
+            dingtalkwiki__1__0_models.WikiWordsDetailResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def create_flash_meeting(
+    def wiki_words_detail(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders()
-        return self.create_flash_meeting_with_options(request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsDetailHeaders()
+        return self.wiki_words_detail_with_options(request, headers, runtime)
 
-    async def create_flash_meeting_async(
+    async def wiki_words_detail_async(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsDetailRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsDetailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders()
-        return await self.create_flash_meeting_with_options_async(request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsDetailHeaders()
+        return await self.wiki_words_detail_with_options_async(request, headers, runtime)
 
-    def get_shanhui_by_calendar_with_options(
+    def wiki_words_parse_with_options(
         self,
-        request: dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarRequest,
-        headers: dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsParseHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.event_id):
-            query['eventId'] = request.event_id
-        if not UtilClient.is_unset(request.user_id):
-            query['userId'] = request.user_id
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='GetShanhuiByCalendar',
-            version='flashmeeting_1.0',
+            action='WikiWordsParse',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/flashmeeting/calendars/meeting',
-            method='GET',
+            pathname=f'/v1.0/wiki/words/parse',
+            method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarResponse(),
+            dingtalkwiki__1__0_models.WikiWordsParseResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def get_shanhui_by_calendar_with_options_async(
+    async def wiki_words_parse_with_options_async(
         self,
-        request: dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarRequest,
-        headers: dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarHeaders,
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+        headers: dingtalkwiki__1__0_models.WikiWordsParseHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarResponse:
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.event_id):
-            query['eventId'] = request.event_id
-        if not UtilClient.is_unset(request.user_id):
-            query['userId'] = request.user_id
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            query=OpenApiUtilClient.query(query)
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='GetShanhuiByCalendar',
-            version='flashmeeting_1.0',
+            action='WikiWordsParse',
+            version='wiki_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/flashmeeting/calendars/meeting',
-            method='GET',
+            pathname=f'/v1.0/wiki/words/parse',
+            method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarResponse(),
+            dingtalkwiki__1__0_models.WikiWordsParseResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def get_shanhui_by_calendar(
+    def wiki_words_parse(
         self,
-        request: dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarRequest,
-    ) -> dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarHeaders()
-        return self.get_shanhui_by_calendar_with_options(request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsParseHeaders()
+        return self.wiki_words_parse_with_options(request, headers, runtime)
 
-    async def get_shanhui_by_calendar_async(
+    async def wiki_words_parse_async(
         self,
-        request: dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarRequest,
-    ) -> dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarResponse:
+        request: dingtalkwiki__1__0_models.WikiWordsParseRequest,
+    ) -> dingtalkwiki__1__0_models.WikiWordsParseResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkflashmeeting__1__0_models.GetShanhuiByCalendarHeaders()
-        return await self.get_shanhui_by_calendar_with_options_async(request, headers, runtime)
+        headers = dingtalkwiki__1__0_models.WikiWordsParseHeaders()
+        return await self.wiki_words_parse_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List
+from typing import Dict
 
 
-class CreateFlashMeetingHeaders(TeaModel):
+class CreateGroupBlackboardHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,110 +33,110 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CreateFlashMeetingRequest(TeaModel):
+class CreateGroupBlackboardRequest(TeaModel):
     def __init__(
         self,
-        creator: str = None,
-        event_id: str = None,
-        title: str = None,
+        content: str = None,
+        open_conversation_id: str = None,
+        send_ding: bool = None,
+        sticky: bool = None,
+        unique_id: str = None,
+        user_id: str = None,
     ):
-        self.creator = creator
-        self.event_id = event_id
-        self.title = title
+        self.content = content
+        self.open_conversation_id = open_conversation_id
+        self.send_ding = send_ding
+        self.sticky = sticky
+        self.unique_id = unique_id
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.creator is not None:
-            result['creator'] = self.creator
-        if self.event_id is not None:
-            result['eventId'] = self.event_id
-        if self.title is not None:
-            result['title'] = self.title
+        if self.content is not None:
+            result['content'] = self.content
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.send_ding is not None:
+            result['sendDing'] = self.send_ding
+        if self.sticky is not None:
+            result['sticky'] = self.sticky
+        if self.unique_id is not None:
+            result['uniqueId'] = self.unique_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('creator') is not None:
-            self.creator = m.get('creator')
-        if m.get('eventId') is not None:
-            self.event_id = m.get('eventId')
-        if m.get('title') is not None:
-            self.title = m.get('title')
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('sendDing') is not None:
+            self.send_ding = m.get('sendDing')
+        if m.get('sticky') is not None:
+            self.sticky = m.get('sticky')
+        if m.get('uniqueId') is not None:
+            self.unique_id = m.get('uniqueId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class CreateFlashMeetingResponseBody(TeaModel):
+class CreateGroupBlackboardResponseBody(TeaModel):
     def __init__(
         self,
-        end_time: int = None,
-        flash_meeting_key: str = None,
-        start_time: int = None,
-        title: str = None,
-        url: str = None,
+        data_id: str = None,
+        success: bool = None,
     ):
-        self.end_time = end_time
-        self.flash_meeting_key = flash_meeting_key
-        self.start_time = start_time
-        self.title = title
-        self.url = url
+        self.data_id = data_id
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.flash_meeting_key is not None:
-            result['flashMeetingKey'] = self.flash_meeting_key
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.title is not None:
-            result['title'] = self.title
-        if self.url is not None:
-            result['url'] = self.url
+        if self.data_id is not None:
+            result['dataId'] = self.data_id
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('flashMeetingKey') is not None:
-            self.flash_meeting_key = m.get('flashMeetingKey')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        if m.get('url') is not None:
-            self.url = m.get('url')
+        if m.get('dataId') is not None:
+            self.data_id = m.get('dataId')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class CreateFlashMeetingResponse(TeaModel):
+class CreateGroupBlackboardResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CreateFlashMeetingResponseBody = None,
+        body: CreateGroupBlackboardResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -162,20 +162,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CreateFlashMeetingResponseBody()
+            temp_model = CreateGroupBlackboardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetShanhuiByCalendarHeaders(TeaModel):
+class DeleteGroupBlackboardHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -200,186 +200,92 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetShanhuiByCalendarRequest(TeaModel):
+class DeleteGroupBlackboardRequest(TeaModel):
     def __init__(
         self,
-        event_id: str = None,
+        data_id: str = None,
+        open_conversation_id: str = None,
         user_id: str = None,
     ):
-        self.event_id = event_id
+        self.data_id = data_id
+        self.open_conversation_id = open_conversation_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.event_id is not None:
-            result['eventId'] = self.event_id
+        if self.data_id is not None:
+            result['dataId'] = self.data_id
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('eventId') is not None:
-            self.event_id = m.get('eventId')
+        if m.get('dataId') is not None:
+            self.data_id = m.get('dataId')
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
 
 
-class GetShanhuiByCalendarResponseBodyResultTopics(TeaModel):
-    def __init__(
-        self,
-        doc_key: str = None,
-        title: str = None,
-    ):
-        self.doc_key = doc_key
-        self.title = title
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.doc_key is not None:
-            result['docKey'] = self.doc_key
-        if self.title is not None:
-            result['title'] = self.title
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('docKey') is not None:
-            self.doc_key = m.get('docKey')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        return self
-
-
-class GetShanhuiByCalendarResponseBodyResult(TeaModel):
-    def __init__(
-        self,
-        end_time: int = None,
-        flashmeeting_key: str = None,
-        start_time: int = None,
-        summary_doc_key: str = None,
-        title: str = None,
-        topics: List[GetShanhuiByCalendarResponseBodyResultTopics] = None,
-    ):
-        self.end_time = end_time
-        self.flashmeeting_key = flashmeeting_key
-        self.start_time = start_time
-        self.summary_doc_key = summary_doc_key
-        self.title = title
-        self.topics = topics
-
-    def validate(self):
-        if self.topics:
-            for k in self.topics:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.flashmeeting_key is not None:
-            result['flashmeetingKey'] = self.flashmeeting_key
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.summary_doc_key is not None:
-            result['summaryDocKey'] = self.summary_doc_key
-        if self.title is not None:
-            result['title'] = self.title
-        result['topics'] = []
-        if self.topics is not None:
-            for k in self.topics:
-                result['topics'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('flashmeetingKey') is not None:
-            self.flashmeeting_key = m.get('flashmeetingKey')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('summaryDocKey') is not None:
-            self.summary_doc_key = m.get('summaryDocKey')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        self.topics = []
-        if m.get('topics') is not None:
-            for k in m.get('topics'):
-                temp_model = GetShanhuiByCalendarResponseBodyResultTopics()
-                self.topics.append(temp_model.from_map(k))
-        return self
-
-
-class GetShanhuiByCalendarResponseBody(TeaModel):
+class DeleteGroupBlackboardResponseBody(TeaModel):
     def __init__(
         self,
-        result: GetShanhuiByCalendarResponseBodyResult = None,
+        is_deleted: bool = None,
         success: bool = None,
     ):
-        self.result = result
+        self.is_deleted = is_deleted
         self.success = success
 
     def validate(self):
-        if self.result:
-            self.result.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.result is not None:
-            result['result'] = self.result.to_map()
+        if self.is_deleted is not None:
+            result['isDeleted'] = self.is_deleted
         if self.success is not None:
             result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('result') is not None:
-            temp_model = GetShanhuiByCalendarResponseBodyResult()
-            self.result = temp_model.from_map(m['result'])
+        if m.get('isDeleted') is not None:
+            self.is_deleted = m.get('isDeleted')
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
 
 
-class GetShanhuiByCalendarResponse(TeaModel):
+class DeleteGroupBlackboardResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetShanhuiByCalendarResponseBody = None,
+        body: DeleteGroupBlackboardResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -405,12 +311,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetShanhuiByCalendarResponseBody()
+            temp_model = DeleteGroupBlackboardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict
+from typing import Dict, List
 
 
-class CreateGroupBlackboardHeaders(TeaModel):
+class QueryGoodsListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,259 +33,204 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CreateGroupBlackboardRequest(TeaModel):
+class QueryGoodsListRequest(TeaModel):
     def __init__(
         self,
-        content: str = None,
-        open_conversation_id: str = None,
-        send_ding: bool = None,
-        sticky: bool = None,
-        unique_id: str = None,
-        user_id: str = None,
+        end_time_in_mills: int = None,
+        max_results: int = None,
+        next_token: int = None,
+        start_time_in_mills: int = None,
     ):
-        self.content = content
-        self.open_conversation_id = open_conversation_id
-        self.send_ding = send_ding
-        self.sticky = sticky
-        self.unique_id = unique_id
-        self.user_id = user_id
+        self.end_time_in_mills = end_time_in_mills
+        self.max_results = max_results
+        self.next_token = next_token
+        self.start_time_in_mills = start_time_in_mills
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.content is not None:
-            result['content'] = self.content
-        if self.open_conversation_id is not None:
-            result['openConversationId'] = self.open_conversation_id
-        if self.send_ding is not None:
-            result['sendDing'] = self.send_ding
-        if self.sticky is not None:
-            result['sticky'] = self.sticky
-        if self.unique_id is not None:
-            result['uniqueId'] = self.unique_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.end_time_in_mills is not None:
+            result['endTimeInMills'] = self.end_time_in_mills
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.start_time_in_mills is not None:
+            result['startTimeInMills'] = self.start_time_in_mills
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('content') is not None:
-            self.content = m.get('content')
-        if m.get('openConversationId') is not None:
-            self.open_conversation_id = m.get('openConversationId')
-        if m.get('sendDing') is not None:
-            self.send_ding = m.get('sendDing')
-        if m.get('sticky') is not None:
-            self.sticky = m.get('sticky')
-        if m.get('uniqueId') is not None:
-            self.unique_id = m.get('uniqueId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('endTimeInMills') is not None:
+            self.end_time_in_mills = m.get('endTimeInMills')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('startTimeInMills') is not None:
+            self.start_time_in_mills = m.get('startTimeInMills')
         return self
 
 
-class CreateGroupBlackboardResponseBody(TeaModel):
+class QueryGoodsListResponseBodyResultList(TeaModel):
     def __init__(
         self,
-        data_id: str = None,
-        success: bool = None,
+        goods_name: str = None,
+        goods_no: str = None,
+        instance_id: str = None,
+        product_specs: str = None,
+        unit: str = None,
     ):
-        self.data_id = data_id
-        self.success = success
+        self.goods_name = goods_name
+        self.goods_no = goods_no
+        self.instance_id = instance_id
+        self.product_specs = product_specs
+        self.unit = unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.data_id is not None:
-            result['dataId'] = self.data_id
-        if self.success is not None:
-            result['success'] = self.success
+        if self.goods_name is not None:
+            result['goodsName'] = self.goods_name
+        if self.goods_no is not None:
+            result['goodsNo'] = self.goods_no
+        if self.instance_id is not None:
+            result['instanceId'] = self.instance_id
+        if self.product_specs is not None:
+            result['productSpecs'] = self.product_specs
+        if self.unit is not None:
+            result['unit'] = self.unit
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('dataId') is not None:
-            self.data_id = m.get('dataId')
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('goodsName') is not None:
+            self.goods_name = m.get('goodsName')
+        if m.get('goodsNo') is not None:
+            self.goods_no = m.get('goodsNo')
+        if m.get('instanceId') is not None:
+            self.instance_id = m.get('instanceId')
+        if m.get('productSpecs') is not None:
+            self.product_specs = m.get('productSpecs')
+        if m.get('unit') is not None:
+            self.unit = m.get('unit')
         return self
 
 
-class CreateGroupBlackboardResponse(TeaModel):
+class QueryGoodsListResponseBodyResult(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: CreateGroupBlackboardResponseBody = None,
+        has_more: bool = None,
+        list: List[QueryGoodsListResponseBodyResultList] = None,
+        max_results: int = None,
+        next_token: str = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.has_more = has_more
+        self.list = list
+        self.max_results = max_results
+        self.next_token = next_token
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = CreateGroupBlackboardResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = QueryGoodsListResponseBodyResultList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class DeleteGroupBlackboardHeaders(TeaModel):
+class QueryGoodsListResponseBody(TeaModel):
     def __init__(
         self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
-    ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
-        return self
-
-
-class DeleteGroupBlackboardRequest(TeaModel):
-    def __init__(
-        self,
-        data_id: str = None,
-        open_conversation_id: str = None,
-        user_id: str = None,
-    ):
-        self.data_id = data_id
-        self.open_conversation_id = open_conversation_id
-        self.user_id = user_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data_id is not None:
-            result['dataId'] = self.data_id
-        if self.open_conversation_id is not None:
-            result['openConversationId'] = self.open_conversation_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('dataId') is not None:
-            self.data_id = m.get('dataId')
-        if m.get('openConversationId') is not None:
-            self.open_conversation_id = m.get('openConversationId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        return self
-
-
-class DeleteGroupBlackboardResponseBody(TeaModel):
-    def __init__(
-        self,
-        is_deleted: bool = None,
+        result: QueryGoodsListResponseBodyResult = None,
         success: bool = None,
     ):
-        self.is_deleted = is_deleted
+        self.result = result
         self.success = success
 
     def validate(self):
-        pass
+        if self.result:
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.is_deleted is not None:
-            result['isDeleted'] = self.is_deleted
+        if self.result is not None:
+            result['result'] = self.result.to_map()
         if self.success is not None:
             result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('isDeleted') is not None:
-            self.is_deleted = m.get('isDeleted')
+        if m.get('result') is not None:
+            temp_model = QueryGoodsListResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
 
 
-class DeleteGroupBlackboardResponse(TeaModel):
+class QueryGoodsListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: DeleteGroupBlackboardResponseBody = None,
+        body: QueryGoodsListResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -311,12 +256,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = DeleteGroupBlackboardResponseBody()
+            temp_model = QueryGoodsListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3049,14 +3049,112 @@
         project_id: str,
         request: dingtalkproject__1__0_models.SeachTaskStageRequest,
     ) -> dingtalkproject__1__0_models.SeachTaskStageResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkproject__1__0_models.SeachTaskStageHeaders()
         return await self.seach_task_stage_with_options_async(user_id, project_id, request, headers, runtime)
 
+    def search_all_tasks_by_tql_with_options(
+        self,
+        user_id: str,
+        request: dingtalkproject__1__0_models.SearchAllTasksByTqlRequest,
+        headers: dingtalkproject__1__0_models.SearchAllTasksByTqlHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkproject__1__0_models.SearchAllTasksByTqlResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.tql):
+            query['tql'] = request.tql
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SearchAllTasksByTql',
+            version='project_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/project/users/{user_id}/tql/tasks/search',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkproject__1__0_models.SearchAllTasksByTqlResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def search_all_tasks_by_tql_with_options_async(
+        self,
+        user_id: str,
+        request: dingtalkproject__1__0_models.SearchAllTasksByTqlRequest,
+        headers: dingtalkproject__1__0_models.SearchAllTasksByTqlHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkproject__1__0_models.SearchAllTasksByTqlResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.tql):
+            query['tql'] = request.tql
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SearchAllTasksByTql',
+            version='project_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/project/users/{user_id}/tql/tasks/search',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkproject__1__0_models.SearchAllTasksByTqlResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def search_all_tasks_by_tql(
+        self,
+        user_id: str,
+        request: dingtalkproject__1__0_models.SearchAllTasksByTqlRequest,
+    ) -> dingtalkproject__1__0_models.SearchAllTasksByTqlResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkproject__1__0_models.SearchAllTasksByTqlHeaders()
+        return self.search_all_tasks_by_tql_with_options(user_id, request, headers, runtime)
+
+    async def search_all_tasks_by_tql_async(
+        self,
+        user_id: str,
+        request: dingtalkproject__1__0_models.SearchAllTasksByTqlRequest,
+    ) -> dingtalkproject__1__0_models.SearchAllTasksByTqlResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkproject__1__0_models.SearchAllTasksByTqlHeaders()
+        return await self.search_all_tasks_by_tql_with_options_async(user_id, request, headers, runtime)
+
     def search_oranization_customfield_with_options(
         self,
         user_id: str,
         request: dingtalkproject__1__0_models.SearchOranizationCustomfieldRequest,
         headers: dingtalkproject__1__0_models.SearchOranizationCustomfieldHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.SearchOranizationCustomfieldResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7255,14 +7255,175 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SeachTaskStageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SearchAllTasksByTqlHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SearchAllTasksByTqlRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        tql: str = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.tql = tql
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.tql is not None:
+            result['tql'] = self.tql
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('tql') is not None:
+            self.tql = m.get('tql')
+        return self
+
+
+class SearchAllTasksByTqlResponseBody(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        request_id: str = None,
+        result: List[str] = None,
+        total_size: int = None,
+    ):
+        self.next_token = next_token
+        self.request_id = request_id
+        self.result = result
+        self.total_size = total_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.result is not None:
+            result['result'] = self.result
+        if self.total_size is not None:
+            result['totalSize'] = self.total_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('totalSize') is not None:
+            self.total_size = m.get('totalSize')
+        return self
+
+
+class SearchAllTasksByTqlResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SearchAllTasksByTqlResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SearchAllTasksByTqlResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SearchOranizationCustomfieldHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List
+from typing import Dict, List, Any
 
 
-class GetDeptHeaders(TeaModel):
+class CloseVideoConferenceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,104 +33,80 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetDeptRequest(TeaModel):
+class CloseVideoConferenceRequest(TeaModel):
     def __init__(
         self,
-        language: str = None,
-        sub_corp_id: str = None,
+        union_id: str = None,
     ):
-        self.language = language
-        self.sub_corp_id = sub_corp_id
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.language is not None:
-            result['language'] = self.language
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('language') is not None:
-            self.language = m.get('language')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class GetDeptResponseBody(TeaModel):
+class CloseVideoConferenceResponseBody(TeaModel):
     def __init__(
         self,
-        department_id: int = None,
-        department_name: str = None,
-        from_union_org: bool = None,
-        order: int = None,
-        parent_department_id: int = None,
+        cause: str = None,
+        code: int = None,
     ):
-        self.department_id = department_id
-        self.department_name = department_name
-        self.from_union_org = from_union_org
-        self.order = order
-        self.parent_department_id = parent_department_id
+        self.cause = cause
+        self.code = code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id is not None:
-            result['departmentId'] = self.department_id
-        if self.department_name is not None:
-            result['departmentName'] = self.department_name
-        if self.from_union_org is not None:
-            result['fromUnionOrg'] = self.from_union_org
-        if self.order is not None:
-            result['order'] = self.order
-        if self.parent_department_id is not None:
-            result['parentDepartmentId'] = self.parent_department_id
+        if self.cause is not None:
+            result['cause'] = self.cause
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentId') is not None:
-            self.department_id = m.get('departmentId')
-        if m.get('departmentName') is not None:
-            self.department_name = m.get('departmentName')
-        if m.get('fromUnionOrg') is not None:
-            self.from_union_org = m.get('fromUnionOrg')
-        if m.get('order') is not None:
-            self.order = m.get('order')
-        if m.get('parentDepartmentId') is not None:
-            self.parent_department_id = m.get('parentDepartmentId')
+        if m.get('cause') is not None:
+            self.cause = m.get('cause')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
-class GetDeptResponse(TeaModel):
+class CloseVideoConferenceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetDeptResponseBody = None,
+        body: CloseVideoConferenceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -156,20 +132,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetDeptResponseBody()
+            temp_model = CloseVideoConferenceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetResidentDeptHeaders(TeaModel):
+class CohostsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -194,98 +170,115 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetResidentDeptRequest(TeaModel):
+class CohostsRequestUserList(TeaModel):
     def __init__(
         self,
-        sub_corp_id: str = None,
+        union_id: str = None,
     ):
-        self.sub_corp_id = sub_corp_id
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class GetResidentDeptResponseBody(TeaModel):
+class CohostsRequest(TeaModel):
     def __init__(
         self,
-        contact_type: str = None,
-        department_id: int = None,
-        department_name: str = None,
-        dept_type: str = None,
-        feature: str = None,
+        action: str = None,
+        user_list: List[CohostsRequestUserList] = None,
     ):
-        self.contact_type = contact_type
-        self.department_id = department_id
-        self.department_name = department_name
-        self.dept_type = dept_type
-        self.feature = feature
+        self.action = action
+        self.user_list = user_list
+
+    def validate(self):
+        if self.user_list:
+            for k in self.user_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action is not None:
+            result['action'] = self.action
+        result['userList'] = []
+        if self.user_list is not None:
+            for k in self.user_list:
+                result['userList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        self.user_list = []
+        if m.get('userList') is not None:
+            for k in m.get('userList'):
+                temp_model = CohostsRequestUserList()
+                self.user_list.append(temp_model.from_map(k))
+        return self
+
+
+class CohostsResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.contact_type is not None:
-            result['contactType'] = self.contact_type
-        if self.department_id is not None:
-            result['departmentId'] = self.department_id
-        if self.department_name is not None:
-            result['departmentName'] = self.department_name
-        if self.dept_type is not None:
-            result['deptType'] = self.dept_type
-        if self.feature is not None:
-            result['feature'] = self.feature
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('contactType') is not None:
-            self.contact_type = m.get('contactType')
-        if m.get('departmentId') is not None:
-            self.department_id = m.get('departmentId')
-        if m.get('departmentName') is not None:
-            self.department_name = m.get('departmentName')
-        if m.get('deptType') is not None:
-            self.dept_type = m.get('deptType')
-        if m.get('feature') is not None:
-            self.feature = m.get('feature')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class GetResidentDeptResponse(TeaModel):
+class CohostsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetResidentDeptResponseBody = None,
+        body: CohostsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -311,20 +304,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetResidentDeptResponseBody()
+            temp_model = CohostsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetResidentUserInfoHeaders(TeaModel):
+class CreateVideoConferenceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -349,145 +342,259 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetResidentUserInfoRequest(TeaModel):
+class CreateVideoConferenceRequest(TeaModel):
     def __init__(
         self,
-        sub_corp_id: str = None,
+        conf_title: str = None,
+        invite_caller: bool = None,
+        invite_user_ids: List[str] = None,
+        user_id: str = None,
     ):
-        self.sub_corp_id = sub_corp_id
+        self.conf_title = conf_title
+        self.invite_caller = invite_caller
+        self.invite_user_ids = invite_user_ids
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.conf_title is not None:
+            result['confTitle'] = self.conf_title
+        if self.invite_caller is not None:
+            result['inviteCaller'] = self.invite_caller
+        if self.invite_user_ids is not None:
+            result['inviteUserIds'] = self.invite_user_ids
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('confTitle') is not None:
+            self.conf_title = m.get('confTitle')
+        if m.get('inviteCaller') is not None:
+            self.invite_caller = m.get('inviteCaller')
+        if m.get('inviteUserIds') is not None:
+            self.invite_user_ids = m.get('inviteUserIds')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class CreateVideoConferenceResponseBody(TeaModel):
+    def __init__(
+        self,
+        conference_id: str = None,
+        conference_password: str = None,
+        external_link_url: str = None,
+        host_password: str = None,
+        phone_numbers: List[str] = None,
+        room_code: str = None,
+    ):
+        self.conference_id = conference_id
+        self.conference_password = conference_password
+        self.external_link_url = external_link_url
+        self.host_password = host_password
+        self.phone_numbers = phone_numbers
+        self.room_code = room_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.conference_password is not None:
+            result['conferencePassword'] = self.conference_password
+        if self.external_link_url is not None:
+            result['externalLinkUrl'] = self.external_link_url
+        if self.host_password is not None:
+            result['hostPassword'] = self.host_password
+        if self.phone_numbers is not None:
+            result['phoneNumbers'] = self.phone_numbers
+        if self.room_code is not None:
+            result['roomCode'] = self.room_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('conferencePassword') is not None:
+            self.conference_password = m.get('conferencePassword')
+        if m.get('externalLinkUrl') is not None:
+            self.external_link_url = m.get('externalLinkUrl')
+        if m.get('hostPassword') is not None:
+            self.host_password = m.get('hostPassword')
+        if m.get('phoneNumbers') is not None:
+            self.phone_numbers = m.get('phoneNumbers')
+        if m.get('roomCode') is not None:
+            self.room_code = m.get('roomCode')
+        return self
+
+
+class CreateVideoConferenceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateVideoConferenceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateVideoConferenceResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetResidentUserInfoResponseBodyRoles(TeaModel):
+class FocusHeaders(TeaModel):
     def __init__(
         self,
-        role_id: int = None,
-        role_name: str = None,
-        tag_code: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.role_id = role_id
-        self.role_name = role_name
-        self.tag_code = tag_code
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.role_id is not None:
-            result['roleId'] = self.role_id
-        if self.role_name is not None:
-            result['roleName'] = self.role_name
-        if self.tag_code is not None:
-            result['tagCode'] = self.tag_code
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('roleId') is not None:
-            self.role_id = m.get('roleId')
-        if m.get('roleName') is not None:
-            self.role_name = m.get('roleName')
-        if m.get('tagCode') is not None:
-            self.tag_code = m.get('tagCode')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetResidentUserInfoResponseBody(TeaModel):
+class FocusRequest(TeaModel):
     def __init__(
         self,
-        feature: str = None,
-        name: str = None,
-        roles: List[GetResidentUserInfoResponseBodyRoles] = None,
+        action: str = None,
         union_id: str = None,
-        userid: str = None,
     ):
-        self.feature = feature
-        self.name = name
-        self.roles = roles
+        self.action = action
         self.union_id = union_id
-        self.userid = userid
 
     def validate(self):
-        if self.roles:
-            for k in self.roles:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.feature is not None:
-            result['feature'] = self.feature
-        if self.name is not None:
-            result['name'] = self.name
-        result['roles'] = []
-        if self.roles is not None:
-            for k in self.roles:
-                result['roles'].append(k.to_map() if k else None)
+        if self.action is not None:
+            result['action'] = self.action
         if self.union_id is not None:
             result['unionId'] = self.union_id
-        if self.userid is not None:
-            result['userid'] = self.userid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('feature') is not None:
-            self.feature = m.get('feature')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        self.roles = []
-        if m.get('roles') is not None:
-            for k in m.get('roles'):
-                temp_model = GetResidentUserInfoResponseBodyRoles()
-                self.roles.append(temp_model.from_map(k))
+        if m.get('action') is not None:
+            self.action = m.get('action')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
-        if m.get('userid') is not None:
-            self.userid = m.get('userid')
         return self
 
 
-class GetResidentUserInfoResponse(TeaModel):
+class FocusResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class FocusResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetResidentUserInfoResponseBody = None,
+        body: FocusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -513,20 +620,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetResidentUserInfoResponseBody()
+            temp_model = FocusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetUserHeaders(TeaModel):
+class GetConfDataByConferenceIdHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -551,420 +658,390 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetUserRequest(TeaModel):
+class GetConfDataByConferenceIdRequest(TeaModel):
     def __init__(
         self,
-        language: str = None,
-        sub_corp_id: str = None,
+        real_data: bool = None,
     ):
-        self.language = language
-        self.sub_corp_id = sub_corp_id
+        self.real_data = real_data
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.language is not None:
-            result['language'] = self.language
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.real_data is not None:
+            result['realData'] = self.real_data
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('language') is not None:
-            self.language = m.get('language')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('realData') is not None:
+            self.real_data = m.get('realData')
         return self
 
 
-class GetUserResponseBodyDepartmentOrderSet(TeaModel):
+class GetConfDataByConferenceIdResponseBody(TeaModel):
     def __init__(
         self,
-        department_id: int = None,
-        order: int = None,
+        conference_id: str = None,
+        creator_id: str = None,
+        creator_nick: str = None,
+        dept_name: str = None,
+        end_time: int = None,
+        free_type: str = None,
+        scene: str = None,
+        start_time: int = None,
+        time_length: int = None,
+        title: str = None,
+        user_count: int = None,
     ):
-        self.department_id = department_id
-        self.order = order
+        self.conference_id = conference_id
+        self.creator_id = creator_id
+        self.creator_nick = creator_nick
+        self.dept_name = dept_name
+        self.end_time = end_time
+        self.free_type = free_type
+        self.scene = scene
+        self.start_time = start_time
+        self.time_length = time_length
+        self.title = title
+        self.user_count = user_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id is not None:
-            result['departmentId'] = self.department_id
-        if self.order is not None:
-            result['order'] = self.order
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.creator_id is not None:
+            result['creatorId'] = self.creator_id
+        if self.creator_nick is not None:
+            result['creatorNick'] = self.creator_nick
+        if self.dept_name is not None:
+            result['deptName'] = self.dept_name
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.free_type is not None:
+            result['freeType'] = self.free_type
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.time_length is not None:
+            result['timeLength'] = self.time_length
+        if self.title is not None:
+            result['title'] = self.title
+        if self.user_count is not None:
+            result['userCount'] = self.user_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentId') is not None:
-            self.department_id = m.get('departmentId')
-        if m.get('order') is not None:
-            self.order = m.get('order')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('creatorId') is not None:
+            self.creator_id = m.get('creatorId')
+        if m.get('creatorNick') is not None:
+            self.creator_nick = m.get('creatorNick')
+        if m.get('deptName') is not None:
+            self.dept_name = m.get('deptName')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('freeType') is not None:
+            self.free_type = m.get('freeType')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('timeLength') is not None:
+            self.time_length = m.get('timeLength')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('userCount') is not None:
+            self.user_count = m.get('userCount')
         return self
 
 
-class GetUserResponseBodyLeaderInDepartment(TeaModel):
+class GetConfDataByConferenceIdResponse(TeaModel):
     def __init__(
         self,
-        department_id: int = None,
-        leader: bool = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetConfDataByConferenceIdResponseBody = None,
     ):
-        self.department_id = department_id
-        self.leader = leader
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
 
     def validate(self):
-        pass
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id is not None:
-            result['departmentId'] = self.department_id
-        if self.leader is not None:
-            result['leader'] = self.leader
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentId') is not None:
-            self.department_id = m.get('departmentId')
-        if m.get('leader') is not None:
-            self.leader = m.get('leader')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetConfDataByConferenceIdResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetUserResponseBodyRoleList(TeaModel):
+class GetConfDetailDataHeaders(TeaModel):
     def __init__(
         self,
-        group_name: str = None,
-        role_id: int = None,
-        role_name: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.group_name = group_name
-        self.role_id = role_id
-        self.role_name = role_name
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.group_name is not None:
-            result['groupName'] = self.group_name
-        if self.role_id is not None:
-            result['roleId'] = self.role_id
-        if self.role_name is not None:
-            result['roleName'] = self.role_name
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('groupName') is not None:
-            self.group_name = m.get('groupName')
-        if m.get('roleId') is not None:
-            self.role_id = m.get('roleId')
-        if m.get('roleName') is not None:
-            self.role_name = m.get('roleName')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetUserResponseBodyUnionEmpExtUnionEmpMapList(TeaModel):
+class GetConfDetailDataRequest(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        staff_id: str = None,
+        max_results: int = None,
+        next_token: str = None,
+        nick: str = None,
     ):
-        self.corp_id = corp_id
-        self.staff_id = staff_id
+        self.max_results = max_results
+        self.next_token = next_token
+        self.nick = nick
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.staff_id is not None:
-            result['staffId'] = self.staff_id
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.nick is not None:
+            result['nick'] = self.nick
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('staffId') is not None:
-            self.staff_id = m.get('staffId')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('nick') is not None:
+            self.nick = m.get('nick')
         return self
 
 
-class GetUserResponseBodyUnionEmpExt(TeaModel):
+class GetConfDetailDataResponseBodyList(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        staff_id: str = None,
-        union_emp_map_list: List[GetUserResponseBodyUnionEmpExtUnionEmpMapList] = None,
+        belong_org: str = None,
+        conference_id: str = None,
+        device_type: str = None,
+        duration: int = None,
+        join_time: int = None,
+        leave_time: int = None,
+        network_quality: str = None,
+        nick: str = None,
+        role: str = None,
+        session_id: str = None,
+        status: str = None,
+        union_id: str = None,
+        version: str = None,
     ):
-        self.corp_id = corp_id
-        self.staff_id = staff_id
-        self.union_emp_map_list = union_emp_map_list
+        self.belong_org = belong_org
+        self.conference_id = conference_id
+        self.device_type = device_type
+        self.duration = duration
+        self.join_time = join_time
+        self.leave_time = leave_time
+        self.network_quality = network_quality
+        self.nick = nick
+        self.role = role
+        self.session_id = session_id
+        self.status = status
+        self.union_id = union_id
+        self.version = version
 
     def validate(self):
-        if self.union_emp_map_list:
-            for k in self.union_emp_map_list:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.staff_id is not None:
-            result['staffId'] = self.staff_id
-        result['unionEmpMapList'] = []
-        if self.union_emp_map_list is not None:
-            for k in self.union_emp_map_list:
-                result['unionEmpMapList'].append(k.to_map() if k else None)
+        if self.belong_org is not None:
+            result['belongOrg'] = self.belong_org
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.device_type is not None:
+            result['deviceType'] = self.device_type
+        if self.duration is not None:
+            result['duration'] = self.duration
+        if self.join_time is not None:
+            result['joinTime'] = self.join_time
+        if self.leave_time is not None:
+            result['leaveTime'] = self.leave_time
+        if self.network_quality is not None:
+            result['networkQuality'] = self.network_quality
+        if self.nick is not None:
+            result['nick'] = self.nick
+        if self.role is not None:
+            result['role'] = self.role
+        if self.session_id is not None:
+            result['sessionId'] = self.session_id
+        if self.status is not None:
+            result['status'] = self.status
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.version is not None:
+            result['version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('staffId') is not None:
-            self.staff_id = m.get('staffId')
-        self.union_emp_map_list = []
-        if m.get('unionEmpMapList') is not None:
-            for k in m.get('unionEmpMapList'):
-                temp_model = GetUserResponseBodyUnionEmpExtUnionEmpMapList()
-                self.union_emp_map_list.append(temp_model.from_map(k))
+        if m.get('belongOrg') is not None:
+            self.belong_org = m.get('belongOrg')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('deviceType') is not None:
+            self.device_type = m.get('deviceType')
+        if m.get('duration') is not None:
+            self.duration = m.get('duration')
+        if m.get('joinTime') is not None:
+            self.join_time = m.get('joinTime')
+        if m.get('leaveTime') is not None:
+            self.leave_time = m.get('leaveTime')
+        if m.get('networkQuality') is not None:
+            self.network_quality = m.get('networkQuality')
+        if m.get('nick') is not None:
+            self.nick = m.get('nick')
+        if m.get('role') is not None:
+            self.role = m.get('role')
+        if m.get('sessionId') is not None:
+            self.session_id = m.get('sessionId')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('version') is not None:
+            self.version = m.get('version')
         return self
 
 
-class GetUserResponseBody(TeaModel):
-    def __init__(
-        self,
-        active: bool = None,
-        admin: bool = None,
-        boss: bool = None,
-        department_id_list: List[int] = None,
-        department_order_set: List[GetUserResponseBodyDepartmentOrderSet] = None,
-        exclusive_account: bool = None,
-        exclusive_account_type: str = None,
-        extension: str = None,
-        hired_date: int = None,
-        job_number: str = None,
-        leader_in_department: List[GetUserResponseBodyLeaderInDepartment] = None,
-        manager_user_id: str = None,
-        name: str = None,
-        real_authed: bool = None,
-        remark: str = None,
-        role_list: List[GetUserResponseBodyRoleList] = None,
-        senior: bool = None,
-        title: str = None,
-        union_emp_ext: GetUserResponseBodyUnionEmpExt = None,
-        union_id: str = None,
-        user_id: str = None,
-        work_place: str = None,
+class GetConfDetailDataResponseBody(TeaModel):
+    def __init__(
+        self,
+        list: List[GetConfDetailDataResponseBodyList] = None,
+        next_token: str = None,
     ):
-        self.active = active
-        self.admin = admin
-        self.boss = boss
-        self.department_id_list = department_id_list
-        self.department_order_set = department_order_set
-        self.exclusive_account = exclusive_account
-        self.exclusive_account_type = exclusive_account_type
-        self.extension = extension
-        self.hired_date = hired_date
-        self.job_number = job_number
-        self.leader_in_department = leader_in_department
-        self.manager_user_id = manager_user_id
-        self.name = name
-        self.real_authed = real_authed
-        self.remark = remark
-        self.role_list = role_list
-        self.senior = senior
-        self.title = title
-        self.union_emp_ext = union_emp_ext
-        self.union_id = union_id
-        self.user_id = user_id
-        self.work_place = work_place
+        self.list = list
+        self.next_token = next_token
 
     def validate(self):
-        if self.department_order_set:
-            for k in self.department_order_set:
-                if k:
-                    k.validate()
-        if self.leader_in_department:
-            for k in self.leader_in_department:
+        if self.list:
+            for k in self.list:
                 if k:
                     k.validate()
-        if self.role_list:
-            for k in self.role_list:
-                if k:
-                    k.validate()
-        if self.union_emp_ext:
-            self.union_emp_ext.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.active is not None:
-            result['active'] = self.active
-        if self.admin is not None:
-            result['admin'] = self.admin
-        if self.boss is not None:
-            result['boss'] = self.boss
-        if self.department_id_list is not None:
-            result['departmentIdList'] = self.department_id_list
-        result['departmentOrderSet'] = []
-        if self.department_order_set is not None:
-            for k in self.department_order_set:
-                result['departmentOrderSet'].append(k.to_map() if k else None)
-        if self.exclusive_account is not None:
-            result['exclusiveAccount'] = self.exclusive_account
-        if self.exclusive_account_type is not None:
-            result['exclusiveAccountType'] = self.exclusive_account_type
-        if self.extension is not None:
-            result['extension'] = self.extension
-        if self.hired_date is not None:
-            result['hiredDate'] = self.hired_date
-        if self.job_number is not None:
-            result['jobNumber'] = self.job_number
-        result['leaderInDepartment'] = []
-        if self.leader_in_department is not None:
-            for k in self.leader_in_department:
-                result['leaderInDepartment'].append(k.to_map() if k else None)
-        if self.manager_user_id is not None:
-            result['managerUserId'] = self.manager_user_id
-        if self.name is not None:
-            result['name'] = self.name
-        if self.real_authed is not None:
-            result['realAuthed'] = self.real_authed
-        if self.remark is not None:
-            result['remark'] = self.remark
-        result['roleList'] = []
-        if self.role_list is not None:
-            for k in self.role_list:
-                result['roleList'].append(k.to_map() if k else None)
-        if self.senior is not None:
-            result['senior'] = self.senior
-        if self.title is not None:
-            result['title'] = self.title
-        if self.union_emp_ext is not None:
-            result['unionEmpExt'] = self.union_emp_ext.to_map()
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        if self.work_place is not None:
-            result['workPlace'] = self.work_place
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('active') is not None:
-            self.active = m.get('active')
-        if m.get('admin') is not None:
-            self.admin = m.get('admin')
-        if m.get('boss') is not None:
-            self.boss = m.get('boss')
-        if m.get('departmentIdList') is not None:
-            self.department_id_list = m.get('departmentIdList')
-        self.department_order_set = []
-        if m.get('departmentOrderSet') is not None:
-            for k in m.get('departmentOrderSet'):
-                temp_model = GetUserResponseBodyDepartmentOrderSet()
-                self.department_order_set.append(temp_model.from_map(k))
-        if m.get('exclusiveAccount') is not None:
-            self.exclusive_account = m.get('exclusiveAccount')
-        if m.get('exclusiveAccountType') is not None:
-            self.exclusive_account_type = m.get('exclusiveAccountType')
-        if m.get('extension') is not None:
-            self.extension = m.get('extension')
-        if m.get('hiredDate') is not None:
-            self.hired_date = m.get('hiredDate')
-        if m.get('jobNumber') is not None:
-            self.job_number = m.get('jobNumber')
-        self.leader_in_department = []
-        if m.get('leaderInDepartment') is not None:
-            for k in m.get('leaderInDepartment'):
-                temp_model = GetUserResponseBodyLeaderInDepartment()
-                self.leader_in_department.append(temp_model.from_map(k))
-        if m.get('managerUserId') is not None:
-            self.manager_user_id = m.get('managerUserId')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('realAuthed') is not None:
-            self.real_authed = m.get('realAuthed')
-        if m.get('remark') is not None:
-            self.remark = m.get('remark')
-        self.role_list = []
-        if m.get('roleList') is not None:
-            for k in m.get('roleList'):
-                temp_model = GetUserResponseBodyRoleList()
-                self.role_list.append(temp_model.from_map(k))
-        if m.get('senior') is not None:
-            self.senior = m.get('senior')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        if m.get('unionEmpExt') is not None:
-            temp_model = GetUserResponseBodyUnionEmpExt()
-            self.union_emp_ext = temp_model.from_map(m['unionEmpExt'])
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        if m.get('workPlace') is not None:
-            self.work_place = m.get('workPlace')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = GetConfDetailDataResponseBodyList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class GetUserResponse(TeaModel):
+class GetConfDetailDataResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetUserResponseBody = None,
+        body: GetConfDetailDataResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -990,20 +1067,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetUserResponseBody()
+            temp_model = GetConfDetailDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetUserByUnionIdHeaders(TeaModel):
+class GetHistoryConfDataListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1028,92 +1105,223 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetUserByUnionIdRequest(TeaModel):
+class GetHistoryConfDataListRequest(TeaModel):
     def __init__(
         self,
-        language: str = None,
-        sub_corp_id: str = None,
-        union_id: str = None,
+        creator_nike: str = None,
+        end_time: int = None,
+        free_type: str = None,
+        max_results: int = None,
+        next_token: str = None,
+        real_data: bool = None,
+        scene: str = None,
+        start_time: int = None,
+        title: str = None,
     ):
-        self.language = language
-        self.sub_corp_id = sub_corp_id
-        self.union_id = union_id
+        self.creator_nike = creator_nike
+        self.end_time = end_time
+        self.free_type = free_type
+        self.max_results = max_results
+        self.next_token = next_token
+        self.real_data = real_data
+        self.scene = scene
+        self.start_time = start_time
+        self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.language is not None:
-            result['language'] = self.language
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.creator_nike is not None:
+            result['creatorNike'] = self.creator_nike
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.free_type is not None:
+            result['freeType'] = self.free_type
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.real_data is not None:
+            result['realData'] = self.real_data
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.title is not None:
+            result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('language') is not None:
-            self.language = m.get('language')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('creatorNike') is not None:
+            self.creator_nike = m.get('creatorNike')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('freeType') is not None:
+            self.free_type = m.get('freeType')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('realData') is not None:
+            self.real_data = m.get('realData')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('title') is not None:
+            self.title = m.get('title')
         return self
 
 
-class GetUserByUnionIdResponseBody(TeaModel):
+class GetHistoryConfDataListResponseBodyList(TeaModel):
     def __init__(
         self,
-        contact_type: int = None,
-        user_id: str = None,
+        conference_id: str = None,
+        creator_id: str = None,
+        creator_nick: str = None,
+        dept_name: str = None,
+        end_time: int = None,
+        free_type: str = None,
+        scene: str = None,
+        start_time: int = None,
+        time_length: int = None,
+        title: str = None,
+        user_count: int = None,
     ):
-        self.contact_type = contact_type
-        self.user_id = user_id
+        self.conference_id = conference_id
+        self.creator_id = creator_id
+        self.creator_nick = creator_nick
+        self.dept_name = dept_name
+        self.end_time = end_time
+        self.free_type = free_type
+        self.scene = scene
+        self.start_time = start_time
+        self.time_length = time_length
+        self.title = title
+        self.user_count = user_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.contact_type is not None:
-            result['contactType'] = self.contact_type
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.creator_id is not None:
+            result['creatorId'] = self.creator_id
+        if self.creator_nick is not None:
+            result['creatorNick'] = self.creator_nick
+        if self.dept_name is not None:
+            result['deptName'] = self.dept_name
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.free_type is not None:
+            result['freeType'] = self.free_type
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.time_length is not None:
+            result['timeLength'] = self.time_length
+        if self.title is not None:
+            result['title'] = self.title
+        if self.user_count is not None:
+            result['userCount'] = self.user_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('contactType') is not None:
-            self.contact_type = m.get('contactType')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('creatorId') is not None:
+            self.creator_id = m.get('creatorId')
+        if m.get('creatorNick') is not None:
+            self.creator_nick = m.get('creatorNick')
+        if m.get('deptName') is not None:
+            self.dept_name = m.get('deptName')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('freeType') is not None:
+            self.free_type = m.get('freeType')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('timeLength') is not None:
+            self.time_length = m.get('timeLength')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('userCount') is not None:
+            self.user_count = m.get('userCount')
         return self
 
 
-class GetUserByUnionIdResponse(TeaModel):
+class GetHistoryConfDataListResponseBody(TeaModel):
+    def __init__(
+        self,
+        list: List[GetHistoryConfDataListResponseBodyList] = None,
+        next_token: str = None,
+    ):
+        self.list = list
+        self.next_token = next_token
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = GetHistoryConfDataListResponseBodyList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        return self
+
+
+class GetHistoryConfDataListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetUserByUnionIdResponseBody = None,
+        body: GetHistoryConfDataListResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1139,20 +1347,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetUserByUnionIdResponseBody()
+            temp_model = GetHistoryConfDataListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetVillageOrgInfoHeaders(TeaModel):
+class GetUserMetricDataHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1177,59 +1385,241 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class GetVillageOrgInfoResponseBody(TeaModel):
+class GetUserMetricDataRequest(TeaModel):
     def __init__(
         self,
-        region_id: str = None,
-        region_location: str = None,
-        region_type: str = None,
+        begin_time: int = None,
+        end_time: int = None,
+        union_id: str = None,
     ):
-        self.region_id = region_id
-        self.region_location = region_location
-        self.region_type = region_type
+        self.begin_time = begin_time
+        self.end_time = end_time
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.region_id is not None:
-            result['regionId'] = self.region_id
-        if self.region_location is not None:
-            result['regionLocation'] = self.region_location
-        if self.region_type is not None:
-            result['regionType'] = self.region_type
+        if self.begin_time is not None:
+            result['beginTime'] = self.begin_time
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('regionId') is not None:
-            self.region_id = m.get('regionId')
-        if m.get('regionLocation') is not None:
-            self.region_location = m.get('regionLocation')
-        if m.get('regionType') is not None:
-            self.region_type = m.get('regionType')
+        if m.get('beginTime') is not None:
+            self.begin_time = m.get('beginTime')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class GetUserMetricDataResponseBodyMetricDataList(TeaModel):
+    def __init__(
+        self,
+        audio_play_level: str = None,
+        audio_rec_level: str = None,
+        audio_recv_bit_rate: str = None,
+        audio_send_bit_rate: str = None,
+        camera_recv_bit_rate: str = None,
+        camera_recv_frame: str = None,
+        camera_recv_resolution_actual: str = None,
+        camera_send_bit_rate: str = None,
+        camera_send_frame: str = None,
+        camera_send_resolution_actual: str = None,
+        lost_rate: str = None,
+        recv_bit_rate: str = None,
+        round_trip_time: str = None,
+        screen_recv_bit_rate: str = None,
+        screen_recv_frame: str = None,
+        screen_recv_resolution_actual: str = None,
+        screen_send_bit_rate: str = None,
+        screen_send_frame: str = None,
+        screen_send_resolution_actual: str = None,
+        send_bit_rate: str = None,
+        timestamp: int = None,
+    ):
+        self.audio_play_level = audio_play_level
+        self.audio_rec_level = audio_rec_level
+        self.audio_recv_bit_rate = audio_recv_bit_rate
+        self.audio_send_bit_rate = audio_send_bit_rate
+        self.camera_recv_bit_rate = camera_recv_bit_rate
+        self.camera_recv_frame = camera_recv_frame
+        self.camera_recv_resolution_actual = camera_recv_resolution_actual
+        self.camera_send_bit_rate = camera_send_bit_rate
+        self.camera_send_frame = camera_send_frame
+        self.camera_send_resolution_actual = camera_send_resolution_actual
+        self.lost_rate = lost_rate
+        self.recv_bit_rate = recv_bit_rate
+        self.round_trip_time = round_trip_time
+        self.screen_recv_bit_rate = screen_recv_bit_rate
+        self.screen_recv_frame = screen_recv_frame
+        self.screen_recv_resolution_actual = screen_recv_resolution_actual
+        self.screen_send_bit_rate = screen_send_bit_rate
+        self.screen_send_frame = screen_send_frame
+        self.screen_send_resolution_actual = screen_send_resolution_actual
+        self.send_bit_rate = send_bit_rate
+        self.timestamp = timestamp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audio_play_level is not None:
+            result['audioPlayLevel'] = self.audio_play_level
+        if self.audio_rec_level is not None:
+            result['audioRecLevel'] = self.audio_rec_level
+        if self.audio_recv_bit_rate is not None:
+            result['audioRecvBitRate'] = self.audio_recv_bit_rate
+        if self.audio_send_bit_rate is not None:
+            result['audioSendBitRate'] = self.audio_send_bit_rate
+        if self.camera_recv_bit_rate is not None:
+            result['cameraRecvBitRate'] = self.camera_recv_bit_rate
+        if self.camera_recv_frame is not None:
+            result['cameraRecvFrame'] = self.camera_recv_frame
+        if self.camera_recv_resolution_actual is not None:
+            result['cameraRecvResolutionActual'] = self.camera_recv_resolution_actual
+        if self.camera_send_bit_rate is not None:
+            result['cameraSendBitRate'] = self.camera_send_bit_rate
+        if self.camera_send_frame is not None:
+            result['cameraSendFrame'] = self.camera_send_frame
+        if self.camera_send_resolution_actual is not None:
+            result['cameraSendResolutionActual'] = self.camera_send_resolution_actual
+        if self.lost_rate is not None:
+            result['lostRate'] = self.lost_rate
+        if self.recv_bit_rate is not None:
+            result['recvBitRate'] = self.recv_bit_rate
+        if self.round_trip_time is not None:
+            result['roundTripTime'] = self.round_trip_time
+        if self.screen_recv_bit_rate is not None:
+            result['screenRecvBitRate'] = self.screen_recv_bit_rate
+        if self.screen_recv_frame is not None:
+            result['screenRecvFrame'] = self.screen_recv_frame
+        if self.screen_recv_resolution_actual is not None:
+            result['screenRecvResolutionActual'] = self.screen_recv_resolution_actual
+        if self.screen_send_bit_rate is not None:
+            result['screenSendBitRate'] = self.screen_send_bit_rate
+        if self.screen_send_frame is not None:
+            result['screenSendFrame'] = self.screen_send_frame
+        if self.screen_send_resolution_actual is not None:
+            result['screenSendResolutionActual'] = self.screen_send_resolution_actual
+        if self.send_bit_rate is not None:
+            result['sendBitRate'] = self.send_bit_rate
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('audioPlayLevel') is not None:
+            self.audio_play_level = m.get('audioPlayLevel')
+        if m.get('audioRecLevel') is not None:
+            self.audio_rec_level = m.get('audioRecLevel')
+        if m.get('audioRecvBitRate') is not None:
+            self.audio_recv_bit_rate = m.get('audioRecvBitRate')
+        if m.get('audioSendBitRate') is not None:
+            self.audio_send_bit_rate = m.get('audioSendBitRate')
+        if m.get('cameraRecvBitRate') is not None:
+            self.camera_recv_bit_rate = m.get('cameraRecvBitRate')
+        if m.get('cameraRecvFrame') is not None:
+            self.camera_recv_frame = m.get('cameraRecvFrame')
+        if m.get('cameraRecvResolutionActual') is not None:
+            self.camera_recv_resolution_actual = m.get('cameraRecvResolutionActual')
+        if m.get('cameraSendBitRate') is not None:
+            self.camera_send_bit_rate = m.get('cameraSendBitRate')
+        if m.get('cameraSendFrame') is not None:
+            self.camera_send_frame = m.get('cameraSendFrame')
+        if m.get('cameraSendResolutionActual') is not None:
+            self.camera_send_resolution_actual = m.get('cameraSendResolutionActual')
+        if m.get('lostRate') is not None:
+            self.lost_rate = m.get('lostRate')
+        if m.get('recvBitRate') is not None:
+            self.recv_bit_rate = m.get('recvBitRate')
+        if m.get('roundTripTime') is not None:
+            self.round_trip_time = m.get('roundTripTime')
+        if m.get('screenRecvBitRate') is not None:
+            self.screen_recv_bit_rate = m.get('screenRecvBitRate')
+        if m.get('screenRecvFrame') is not None:
+            self.screen_recv_frame = m.get('screenRecvFrame')
+        if m.get('screenRecvResolutionActual') is not None:
+            self.screen_recv_resolution_actual = m.get('screenRecvResolutionActual')
+        if m.get('screenSendBitRate') is not None:
+            self.screen_send_bit_rate = m.get('screenSendBitRate')
+        if m.get('screenSendFrame') is not None:
+            self.screen_send_frame = m.get('screenSendFrame')
+        if m.get('screenSendResolutionActual') is not None:
+            self.screen_send_resolution_actual = m.get('screenSendResolutionActual')
+        if m.get('sendBitRate') is not None:
+            self.send_bit_rate = m.get('sendBitRate')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        return self
+
+
+class GetUserMetricDataResponseBody(TeaModel):
+    def __init__(
+        self,
+        metric_data_list: List[GetUserMetricDataResponseBodyMetricDataList] = None,
+    ):
+        self.metric_data_list = metric_data_list
+
+    def validate(self):
+        if self.metric_data_list:
+            for k in self.metric_data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['metricDataList'] = []
+        if self.metric_data_list is not None:
+            for k in self.metric_data_list:
+                result['metricDataList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.metric_data_list = []
+        if m.get('metricDataList') is not None:
+            for k in m.get('metricDataList'):
+                temp_model = GetUserMetricDataResponseBodyMetricDataList()
+                self.metric_data_list.append(temp_model.from_map(k))
         return self
 
 
-class GetVillageOrgInfoResponse(TeaModel):
+class GetUserMetricDataResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetVillageOrgInfoResponseBody = None,
+        body: GetUserMetricDataResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1255,20 +1645,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetVillageOrgInfoResponseBody()
+            temp_model = GetUserMetricDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListDeptSimpleUsersHeaders(TeaModel):
+class InviteUsersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1293,163 +1683,299 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListDeptSimpleUsersRequest(TeaModel):
+class InviteUsersRequestInviteeList(TeaModel):
     def __init__(
         self,
-        contain_access_limit: bool = None,
-        cursor: int = None,
-        language: str = None,
-        order_field: str = None,
-        size: int = None,
-        sub_corp_id: str = None,
+        nick: str = None,
+        union_id: str = None,
     ):
-        self.contain_access_limit = contain_access_limit
-        self.cursor = cursor
-        self.language = language
-        self.order_field = order_field
-        self.size = size
-        self.sub_corp_id = sub_corp_id
+        self.nick = nick
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.contain_access_limit is not None:
-            result['containAccessLimit'] = self.contain_access_limit
-        if self.cursor is not None:
-            result['cursor'] = self.cursor
-        if self.language is not None:
-            result['language'] = self.language
-        if self.order_field is not None:
-            result['orderField'] = self.order_field
-        if self.size is not None:
-            result['size'] = self.size
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.nick is not None:
+            result['nick'] = self.nick
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('containAccessLimit') is not None:
-            self.contain_access_limit = m.get('containAccessLimit')
-        if m.get('cursor') is not None:
-            self.cursor = m.get('cursor')
-        if m.get('language') is not None:
-            self.language = m.get('language')
-        if m.get('orderField') is not None:
-            self.order_field = m.get('orderField')
-        if m.get('size') is not None:
-            self.size = m.get('size')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('nick') is not None:
+            self.nick = m.get('nick')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class ListDeptSimpleUsersResponseBodyUserList(TeaModel):
+class InviteUsersRequest(TeaModel):
     def __init__(
         self,
-        name: str = None,
-        user_id: str = None,
+        invitee_list: List[InviteUsersRequestInviteeList] = None,
+        union_id: str = None,
     ):
-        self.name = name
-        self.user_id = user_id
+        self.invitee_list = invitee_list
+        self.union_id = union_id
+
+    def validate(self):
+        if self.invitee_list:
+            for k in self.invitee_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['inviteeList'] = []
+        if self.invitee_list is not None:
+            for k in self.invitee_list:
+                result['inviteeList'].append(k.to_map() if k else None)
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.invitee_list = []
+        if m.get('inviteeList') is not None:
+            for k in m.get('inviteeList'):
+                temp_model = InviteUsersRequestInviteeList()
+                self.invitee_list.append(temp_model.from_map(k))
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class InviteUsersResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.name is not None:
-            result['name'] = self.name
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class ListDeptSimpleUsersResponseBody(TeaModel):
+class InviteUsersResponse(TeaModel):
     def __init__(
         self,
-        has_more: bool = None,
-        next_cursor: int = None,
-        total_count: int = None,
-        user_list: List[ListDeptSimpleUsersResponseBodyUserList] = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: InviteUsersResponseBody = None,
     ):
-        self.has_more = has_more
-        self.next_cursor = next_cursor
-        self.total_count = total_count
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = InviteUsersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class KickMembersHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class KickMembersRequestUserList(TeaModel):
+    def __init__(
+        self,
+        participant_id: str = None,
+        union_id: str = None,
+    ):
+        self.participant_id = participant_id
+        self.union_id = union_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.participant_id is not None:
+            result['participantId'] = self.participant_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('participantId') is not None:
+            self.participant_id = m.get('participantId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class KickMembersRequest(TeaModel):
+    def __init__(
+        self,
+        forbidden_rejoin: bool = None,
+        user_list: List[KickMembersRequestUserList] = None,
+    ):
+        self.forbidden_rejoin = forbidden_rejoin
         self.user_list = user_list
 
     def validate(self):
         if self.user_list:
             for k in self.user_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.has_more is not None:
-            result['hasMore'] = self.has_more
-        if self.next_cursor is not None:
-            result['nextCursor'] = self.next_cursor
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
+        if self.forbidden_rejoin is not None:
+            result['forbiddenRejoin'] = self.forbidden_rejoin
         result['userList'] = []
         if self.user_list is not None:
             for k in self.user_list:
                 result['userList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('hasMore') is not None:
-            self.has_more = m.get('hasMore')
-        if m.get('nextCursor') is not None:
-            self.next_cursor = m.get('nextCursor')
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
+        if m.get('forbiddenRejoin') is not None:
+            self.forbidden_rejoin = m.get('forbiddenRejoin')
         self.user_list = []
         if m.get('userList') is not None:
             for k in m.get('userList'):
-                temp_model = ListDeptSimpleUsersResponseBodyUserList()
+                temp_model = KickMembersRequestUserList()
                 self.user_list.append(temp_model.from_map(k))
         return self
 
 
-class ListDeptSimpleUsersResponse(TeaModel):
+class KickMembersResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class KickMembersResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListDeptSimpleUsersResponseBody = None,
+        body: KickMembersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1475,20 +2001,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListDeptSimpleUsersResponseBody()
+            temp_model = KickMembersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListDeptUserIdsHeaders(TeaModel):
+class MuteAllHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1513,74 +2039,80 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListDeptUserIdsRequest(TeaModel):
+class MuteAllRequest(TeaModel):
     def __init__(
         self,
-        sub_corp_id: str = None,
+        action: str = None,
+        force_mute: bool = None,
     ):
-        self.sub_corp_id = sub_corp_id
+        self.action = action
+        self.force_mute = force_mute
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.action is not None:
+            result['action'] = self.action
+        if self.force_mute is not None:
+            result['forceMute'] = self.force_mute
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        if m.get('forceMute') is not None:
+            self.force_mute = m.get('forceMute')
         return self
 
 
-class ListDeptUserIdsResponseBody(TeaModel):
+class MuteAllResponseBody(TeaModel):
     def __init__(
         self,
-        user_id_list: List[str] = None,
+        success: bool = None,
     ):
-        self.user_id_list = user_id_list
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.user_id_list is not None:
-            result['userIdList'] = self.user_id_list
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('userIdList') is not None:
-            self.user_id_list = m.get('userIdList')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class ListDeptUserIdsResponse(TeaModel):
+class MuteAllResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListDeptUserIdsResponseBody = None,
+        body: MuteAllResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1606,20 +2138,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListDeptUserIdsResponseBody()
+            temp_model = MuteAllResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListDeptUsersHeaders(TeaModel):
+class MuteMembersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1644,181 +2176,477 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListDeptUsersRequest(TeaModel):
+class MuteMembersRequestUserList(TeaModel):
+    def __init__(
+        self,
+        participant_id: str = None,
+        union_id: str = None,
+    ):
+        self.participant_id = participant_id
+        self.union_id = union_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.participant_id is not None:
+            result['participantId'] = self.participant_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('participantId') is not None:
+            self.participant_id = m.get('participantId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class MuteMembersRequest(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        user_list: List[MuteMembersRequestUserList] = None,
+    ):
+        self.action = action
+        self.user_list = user_list
+
+    def validate(self):
+        if self.user_list:
+            for k in self.user_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action is not None:
+            result['action'] = self.action
+        result['userList'] = []
+        if self.user_list is not None:
+            for k in self.user_list:
+                result['userList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        self.user_list = []
+        if m.get('userList') is not None:
+            for k in m.get('userList'):
+                temp_model = MuteMembersRequestUserList()
+                self.user_list.append(temp_model.from_map(k))
+        return self
+
+
+class MuteMembersResponseBody(TeaModel):
     def __init__(
         self,
-        contain_access_limit: bool = None,
-        cursor: int = None,
-        language: str = None,
-        order_field: str = None,
-        size: int = None,
-        sub_corp_id: str = None,
+        success: bool = None,
     ):
-        self.contain_access_limit = contain_access_limit
-        self.cursor = cursor
-        self.language = language
-        self.order_field = order_field
-        self.size = size
-        self.sub_corp_id = sub_corp_id
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.contain_access_limit is not None:
-            result['containAccessLimit'] = self.contain_access_limit
-        if self.cursor is not None:
-            result['cursor'] = self.cursor
-        if self.language is not None:
-            result['language'] = self.language
-        if self.order_field is not None:
-            result['orderField'] = self.order_field
-        if self.size is not None:
-            result['size'] = self.size
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('containAccessLimit') is not None:
-            self.contain_access_limit = m.get('containAccessLimit')
-        if m.get('cursor') is not None:
-            self.cursor = m.get('cursor')
-        if m.get('language') is not None:
-            self.language = m.get('language')
-        if m.get('orderField') is not None:
-            self.order_field = m.get('orderField')
-        if m.get('size') is not None:
-            self.size = m.get('size')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class ListDeptUsersResponseBodyUserList(TeaModel):
+class MuteMembersResponse(TeaModel):
     def __init__(
         self,
-        active: bool = None,
-        department_list: List[int] = None,
-        job_number: str = None,
-        name: str = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: MuteMembersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = MuteMembersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class QueryCloudRecordTextHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryCloudRecordTextRequest(TeaModel):
+    def __init__(
+        self,
+        direction: str = None,
+        max_results: int = None,
+        next_token: int = None,
+        start_time: int = None,
         union_id: str = None,
-        user_id: str = None,
     ):
-        self.active = active
-        self.department_list = department_list
-        self.job_number = job_number
-        self.name = name
+        self.direction = direction
+        self.max_results = max_results
+        self.next_token = next_token
+        self.start_time = start_time
         self.union_id = union_id
-        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.active is not None:
-            result['active'] = self.active
-        if self.department_list is not None:
-            result['departmentList'] = self.department_list
-        if self.job_number is not None:
-            result['jobNumber'] = self.job_number
-        if self.name is not None:
-            result['name'] = self.name
+        if self.direction is not None:
+            result['direction'] = self.direction
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
         if self.union_id is not None:
             result['unionId'] = self.union_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('active') is not None:
-            self.active = m.get('active')
-        if m.get('departmentList') is not None:
-            self.department_list = m.get('departmentList')
-        if m.get('jobNumber') is not None:
-            self.job_number = m.get('jobNumber')
-        if m.get('name') is not None:
-            self.name = m.get('name')
+        if m.get('direction') is not None:
+            self.direction = m.get('direction')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class QueryCloudRecordTextResponseBodyParagraphListSentenceListWordList(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        start_time: int = None,
+        word: str = None,
+        word_id: str = None,
+    ):
+        self.end_time = end_time
+        self.start_time = start_time
+        self.word = word
+        self.word_id = word_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.word is not None:
+            result['word'] = self.word
+        if self.word_id is not None:
+            result['wordId'] = self.word_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('word') is not None:
+            self.word = m.get('word')
+        if m.get('wordId') is not None:
+            self.word_id = m.get('wordId')
+        return self
+
+
+class QueryCloudRecordTextResponseBodyParagraphListSentenceList(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        sentence: str = None,
+        start_time: int = None,
+        union_id: str = None,
+        word_list: List[QueryCloudRecordTextResponseBodyParagraphListSentenceListWordList] = None,
+    ):
+        self.end_time = end_time
+        self.sentence = sentence
+        self.start_time = start_time
+        self.union_id = union_id
+        self.word_list = word_list
+
+    def validate(self):
+        if self.word_list:
+            for k in self.word_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.sentence is not None:
+            result['sentence'] = self.sentence
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        result['wordList'] = []
+        if self.word_list is not None:
+            for k in self.word_list:
+                result['wordList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('sentence') is not None:
+            self.sentence = m.get('sentence')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        self.word_list = []
+        if m.get('wordList') is not None:
+            for k in m.get('wordList'):
+                temp_model = QueryCloudRecordTextResponseBodyParagraphListSentenceListWordList()
+                self.word_list.append(temp_model.from_map(k))
+        return self
+
+
+class QueryCloudRecordTextResponseBodyParagraphList(TeaModel):
+    def __init__(
+        self,
+        end_time: int = None,
+        next_ttoken: int = None,
+        nick_name: str = None,
+        paragraph: str = None,
+        record_id: int = None,
+        sentence_list: List[QueryCloudRecordTextResponseBodyParagraphListSentenceList] = None,
+        start_time: int = None,
+        status: int = None,
+        union_id: str = None,
+    ):
+        self.end_time = end_time
+        self.next_ttoken = next_ttoken
+        self.nick_name = nick_name
+        self.paragraph = paragraph
+        self.record_id = record_id
+        self.sentence_list = sentence_list
+        self.start_time = start_time
+        self.status = status
+        self.union_id = union_id
+
+    def validate(self):
+        if self.sentence_list:
+            for k in self.sentence_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.next_ttoken is not None:
+            result['nextTtoken'] = self.next_ttoken
+        if self.nick_name is not None:
+            result['nickName'] = self.nick_name
+        if self.paragraph is not None:
+            result['paragraph'] = self.paragraph
+        if self.record_id is not None:
+            result['recordId'] = self.record_id
+        result['sentenceList'] = []
+        if self.sentence_list is not None:
+            for k in self.sentence_list:
+                result['sentenceList'].append(k.to_map() if k else None)
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.status is not None:
+            result['status'] = self.status
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('nextTtoken') is not None:
+            self.next_ttoken = m.get('nextTtoken')
+        if m.get('nickName') is not None:
+            self.nick_name = m.get('nickName')
+        if m.get('paragraph') is not None:
+            self.paragraph = m.get('paragraph')
+        if m.get('recordId') is not None:
+            self.record_id = m.get('recordId')
+        self.sentence_list = []
+        if m.get('sentenceList') is not None:
+            for k in m.get('sentenceList'):
+                temp_model = QueryCloudRecordTextResponseBodyParagraphListSentenceList()
+                self.sentence_list.append(temp_model.from_map(k))
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('status') is not None:
+            self.status = m.get('status')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
         return self
 
 
-class ListDeptUsersResponseBody(TeaModel):
+class QueryCloudRecordTextResponseBody(TeaModel):
     def __init__(
         self,
         has_more: bool = None,
-        next_cursor: int = None,
-        user_list: List[ListDeptUsersResponseBodyUserList] = None,
+        paragraph_list: List[QueryCloudRecordTextResponseBodyParagraphList] = None,
     ):
         self.has_more = has_more
-        self.next_cursor = next_cursor
-        self.user_list = user_list
+        self.paragraph_list = paragraph_list
 
     def validate(self):
-        if self.user_list:
-            for k in self.user_list:
+        if self.paragraph_list:
+            for k in self.paragraph_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.has_more is not None:
             result['hasMore'] = self.has_more
-        if self.next_cursor is not None:
-            result['nextCursor'] = self.next_cursor
-        result['userList'] = []
-        if self.user_list is not None:
-            for k in self.user_list:
-                result['userList'].append(k.to_map() if k else None)
+        result['paragraphList'] = []
+        if self.paragraph_list is not None:
+            for k in self.paragraph_list:
+                result['paragraphList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('hasMore') is not None:
             self.has_more = m.get('hasMore')
-        if m.get('nextCursor') is not None:
-            self.next_cursor = m.get('nextCursor')
-        self.user_list = []
-        if m.get('userList') is not None:
-            for k in m.get('userList'):
-                temp_model = ListDeptUsersResponseBodyUserList()
-                self.user_list.append(temp_model.from_map(k))
+        self.paragraph_list = []
+        if m.get('paragraphList') is not None:
+            for k in m.get('paragraphList'):
+                temp_model = QueryCloudRecordTextResponseBodyParagraphList()
+                self.paragraph_list.append(temp_model.from_map(k))
         return self
 
 
-class ListDeptUsersResponse(TeaModel):
+class QueryCloudRecordTextResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListDeptUsersResponseBody = None,
+        body: QueryCloudRecordTextResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1844,20 +2672,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListDeptUsersResponseBody()
+            temp_model = QueryCloudRecordTextResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListParentByDeptHeaders(TeaModel):
+class QueryCloudRecordVideoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -1882,80 +2710,157 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListParentByDeptRequest(TeaModel):
+class QueryCloudRecordVideoRequest(TeaModel):
     def __init__(
         self,
-        department_id: int = None,
-        sub_corp_id: str = None,
+        union_id: str = None,
     ):
-        self.department_id = department_id
-        self.sub_corp_id = sub_corp_id
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id is not None:
-            result['departmentId'] = self.department_id
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentId') is not None:
-            self.department_id = m.get('departmentId')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class ListParentByDeptResponseBody(TeaModel):
+class QueryCloudRecordVideoResponseBodyVideoList(TeaModel):
     def __init__(
         self,
-        department_id_list: List[int] = None,
+        duration: int = None,
+        end_time: int = None,
+        file_size: int = None,
+        media_id: str = None,
+        record_id: str = None,
+        record_type: int = None,
+        region_id: str = None,
+        start_time: int = None,
+        union_id: str = None,
     ):
-        self.department_id_list = department_id_list
+        self.duration = duration
+        self.end_time = end_time
+        self.file_size = file_size
+        self.media_id = media_id
+        self.record_id = record_id
+        self.record_type = record_type
+        self.region_id = region_id
+        self.start_time = start_time
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id_list is not None:
-            result['departmentIdList'] = self.department_id_list
+        if self.duration is not None:
+            result['duration'] = self.duration
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.file_size is not None:
+            result['fileSize'] = self.file_size
+        if self.media_id is not None:
+            result['mediaId'] = self.media_id
+        if self.record_id is not None:
+            result['recordId'] = self.record_id
+        if self.record_type is not None:
+            result['recordType'] = self.record_type
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentIdList') is not None:
-            self.department_id_list = m.get('departmentIdList')
+        if m.get('duration') is not None:
+            self.duration = m.get('duration')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('fileSize') is not None:
+            self.file_size = m.get('fileSize')
+        if m.get('mediaId') is not None:
+            self.media_id = m.get('mediaId')
+        if m.get('recordId') is not None:
+            self.record_id = m.get('recordId')
+        if m.get('recordType') is not None:
+            self.record_type = m.get('recordType')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class ListParentByDeptResponse(TeaModel):
+class QueryCloudRecordVideoResponseBody(TeaModel):
+    def __init__(
+        self,
+        video_list: List[QueryCloudRecordVideoResponseBodyVideoList] = None,
+    ):
+        self.video_list = video_list
+
+    def validate(self):
+        if self.video_list:
+            for k in self.video_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['videoList'] = []
+        if self.video_list is not None:
+            for k in self.video_list:
+                result['videoList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.video_list = []
+        if m.get('videoList') is not None:
+            for k in m.get('videoList'):
+                temp_model = QueryCloudRecordVideoResponseBodyVideoList()
+                self.video_list.append(temp_model.from_map(k))
+        return self
+
+
+class QueryCloudRecordVideoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListParentByDeptResponseBody = None,
+        body: QueryCloudRecordVideoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -1981,20 +2886,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListParentByDeptResponseBody()
+            temp_model = QueryCloudRecordVideoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListParentByUserHeaders(TeaModel):
+class QueryCloudRecordVideoPlayInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2019,80 +2924,110 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListParentByUserRequest(TeaModel):
+class QueryCloudRecordVideoPlayInfoRequest(TeaModel):
     def __init__(
         self,
-        sub_corp_id: str = None,
-        user_id: str = None,
+        media_id: str = None,
+        region_id: str = None,
+        union_id: str = None,
     ):
-        self.sub_corp_id = sub_corp_id
-        self.user_id = user_id
+        self.media_id = media_id
+        self.region_id = region_id
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.media_id is not None:
+            result['mediaId'] = self.media_id
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('mediaId') is not None:
+            self.media_id = m.get('mediaId')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class ListParentByUserResponseBody(TeaModel):
+class QueryCloudRecordVideoPlayInfoResponseBody(TeaModel):
     def __init__(
         self,
-        department_id_list: List[int] = None,
+        duration: int = None,
+        file_size: int = None,
+        mp_4file_url: str = None,
+        play_url: str = None,
+        status: int = None,
     ):
-        self.department_id_list = department_id_list
+        self.duration = duration
+        self.file_size = file_size
+        self.mp_4file_url = mp_4file_url
+        self.play_url = play_url
+        self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id_list is not None:
-            result['departmentIdList'] = self.department_id_list
+        if self.duration is not None:
+            result['duration'] = self.duration
+        if self.file_size is not None:
+            result['fileSize'] = self.file_size
+        if self.mp_4file_url is not None:
+            result['mp4FileUrl'] = self.mp_4file_url
+        if self.play_url is not None:
+            result['playUrl'] = self.play_url
+        if self.status is not None:
+            result['status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentIdList') is not None:
-            self.department_id_list = m.get('departmentIdList')
+        if m.get('duration') is not None:
+            self.duration = m.get('duration')
+        if m.get('fileSize') is not None:
+            self.file_size = m.get('fileSize')
+        if m.get('mp4FileUrl') is not None:
+            self.mp_4file_url = m.get('mp4FileUrl')
+        if m.get('playUrl') is not None:
+            self.play_url = m.get('playUrl')
+        if m.get('status') is not None:
+            self.status = m.get('status')
         return self
 
 
-class ListParentByUserResponse(TeaModel):
+class QueryCloudRecordVideoPlayInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListParentByUserResponseBody = None,
+        body: QueryCloudRecordVideoPlayInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2118,20 +3053,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListParentByUserResponseBody()
+            temp_model = QueryCloudRecordVideoPlayInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListResidentDeptUsersHeaders(TeaModel):
+class QueryConferenceInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2156,210 +3091,409 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListResidentDeptUsersRequest(TeaModel):
+class QueryConferenceInfoResponseBodyConfInfo(TeaModel):
     def __init__(
         self,
-        cursor: int = None,
-        role: str = None,
-        size: int = None,
-        sub_corp_id: str = None,
+        active_num: int = None,
+        attend_num: int = None,
+        conf_duration: int = None,
+        conference_id: str = None,
+        creator_id: str = None,
+        creator_nick: str = None,
+        end_time: int = None,
+        external_link_url: str = None,
+        invited_num: int = None,
+        room_code: str = None,
+        start_time: int = None,
+        status: int = None,
+        title: str = None,
     ):
-        self.cursor = cursor
-        self.role = role
-        self.size = size
-        self.sub_corp_id = sub_corp_id
+        self.active_num = active_num
+        self.attend_num = attend_num
+        self.conf_duration = conf_duration
+        self.conference_id = conference_id
+        self.creator_id = creator_id
+        self.creator_nick = creator_nick
+        self.end_time = end_time
+        self.external_link_url = external_link_url
+        self.invited_num = invited_num
+        self.room_code = room_code
+        self.start_time = start_time
+        self.status = status
+        self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.cursor is not None:
-            result['cursor'] = self.cursor
-        if self.role is not None:
-            result['role'] = self.role
-        if self.size is not None:
-            result['size'] = self.size
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.active_num is not None:
+            result['activeNum'] = self.active_num
+        if self.attend_num is not None:
+            result['attendNum'] = self.attend_num
+        if self.conf_duration is not None:
+            result['confDuration'] = self.conf_duration
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.creator_id is not None:
+            result['creatorId'] = self.creator_id
+        if self.creator_nick is not None:
+            result['creatorNick'] = self.creator_nick
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.external_link_url is not None:
+            result['externalLinkUrl'] = self.external_link_url
+        if self.invited_num is not None:
+            result['invitedNum'] = self.invited_num
+        if self.room_code is not None:
+            result['roomCode'] = self.room_code
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.status is not None:
+            result['status'] = self.status
+        if self.title is not None:
+            result['title'] = self.title
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cursor') is not None:
-            self.cursor = m.get('cursor')
-        if m.get('role') is not None:
-            self.role = m.get('role')
-        if m.get('size') is not None:
-            self.size = m.get('size')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('activeNum') is not None:
+            self.active_num = m.get('activeNum')
+        if m.get('attendNum') is not None:
+            self.attend_num = m.get('attendNum')
+        if m.get('confDuration') is not None:
+            self.conf_duration = m.get('confDuration')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('creatorId') is not None:
+            self.creator_id = m.get('creatorId')
+        if m.get('creatorNick') is not None:
+            self.creator_nick = m.get('creatorNick')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('externalLinkUrl') is not None:
+            self.external_link_url = m.get('externalLinkUrl')
+        if m.get('invitedNum') is not None:
+            self.invited_num = m.get('invitedNum')
+        if m.get('roomCode') is not None:
+            self.room_code = m.get('roomCode')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class QueryConferenceInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        conf_info: QueryConferenceInfoResponseBodyConfInfo = None,
+    ):
+        self.conf_info = conf_info
+
+    def validate(self):
+        if self.conf_info:
+            self.conf_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conf_info is not None:
+            result['confInfo'] = self.conf_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('confInfo') is not None:
+            temp_model = QueryConferenceInfoResponseBodyConfInfo()
+            self.conf_info = temp_model.from_map(m['confInfo'])
+        return self
+
+
+class QueryConferenceInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryConferenceInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryConferenceInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListResidentDeptUsersResponseBodyUserListRoles(TeaModel):
+class QueryConferenceInfoBatchHeaders(TeaModel):
     def __init__(
         self,
-        tag_code: str = None,
-        tag_id: int = None,
-        tag_name: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.tag_code = tag_code
-        self.tag_id = tag_id
-        self.tag_name = tag_name
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.tag_code is not None:
-            result['tagCode'] = self.tag_code
-        if self.tag_id is not None:
-            result['tagId'] = self.tag_id
-        if self.tag_name is not None:
-            result['tagName'] = self.tag_name
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('tagCode') is not None:
-            self.tag_code = m.get('tagCode')
-        if m.get('tagId') is not None:
-            self.tag_id = m.get('tagId')
-        if m.get('tagName') is not None:
-            self.tag_name = m.get('tagName')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListResidentDeptUsersResponseBodyUserList(TeaModel):
+class QueryConferenceInfoBatchRequest(TeaModel):
     def __init__(
         self,
-        feature: str = None,
-        name: str = None,
-        roles: List[ListResidentDeptUsersResponseBodyUserListRoles] = None,
-        union_id: str = None,
+        conference_id_list: List[str] = None,
+    ):
+        self.conference_id_list = conference_id_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conference_id_list is not None:
+            result['conferenceIdList'] = self.conference_id_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('conferenceIdList') is not None:
+            self.conference_id_list = m.get('conferenceIdList')
+        return self
+
+
+class QueryConferenceInfoBatchResponseBodyInfosUserList(TeaModel):
+    def __init__(
+        self,
+        attend_status: int = None,
+        camera_status: int = None,
+        mic_status: int = None,
+        nick: str = None,
+        reject_description: str = None,
         user_id: str = None,
     ):
-        self.feature = feature
-        self.name = name
-        self.roles = roles
-        self.union_id = union_id
+        self.attend_status = attend_status
+        self.camera_status = camera_status
+        self.mic_status = mic_status
+        self.nick = nick
+        self.reject_description = reject_description
         self.user_id = user_id
 
     def validate(self):
-        if self.roles:
-            for k in self.roles:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.feature is not None:
-            result['feature'] = self.feature
-        if self.name is not None:
-            result['name'] = self.name
-        result['roles'] = []
-        if self.roles is not None:
-            for k in self.roles:
-                result['roles'].append(k.to_map() if k else None)
-        if self.union_id is not None:
-            result['unionId'] = self.union_id
+        if self.attend_status is not None:
+            result['attendStatus'] = self.attend_status
+        if self.camera_status is not None:
+            result['cameraStatus'] = self.camera_status
+        if self.mic_status is not None:
+            result['micStatus'] = self.mic_status
+        if self.nick is not None:
+            result['nick'] = self.nick
+        if self.reject_description is not None:
+            result['rejectDescription'] = self.reject_description
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('feature') is not None:
-            self.feature = m.get('feature')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        self.roles = []
-        if m.get('roles') is not None:
-            for k in m.get('roles'):
-                temp_model = ListResidentDeptUsersResponseBodyUserListRoles()
-                self.roles.append(temp_model.from_map(k))
-        if m.get('unionId') is not None:
-            self.union_id = m.get('unionId')
+        if m.get('attendStatus') is not None:
+            self.attend_status = m.get('attendStatus')
+        if m.get('cameraStatus') is not None:
+            self.camera_status = m.get('cameraStatus')
+        if m.get('micStatus') is not None:
+            self.mic_status = m.get('micStatus')
+        if m.get('nick') is not None:
+            self.nick = m.get('nick')
+        if m.get('rejectDescription') is not None:
+            self.reject_description = m.get('rejectDescription')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
 
 
-class ListResidentDeptUsersResponseBody(TeaModel):
+class QueryConferenceInfoBatchResponseBodyInfos(TeaModel):
     def __init__(
         self,
-        has_more: bool = None,
-        next_cursor: int = None,
-        user_list: List[ListResidentDeptUsersResponseBodyUserList] = None,
+        conference_id: str = None,
+        media_status: int = None,
+        start_time: int = None,
+        status: int = None,
+        title: str = None,
+        user_list: List[QueryConferenceInfoBatchResponseBodyInfosUserList] = None,
     ):
-        self.has_more = has_more
-        self.next_cursor = next_cursor
+        self.conference_id = conference_id
+        self.media_status = media_status
+        self.start_time = start_time
+        self.status = status
+        self.title = title
         self.user_list = user_list
 
     def validate(self):
         if self.user_list:
             for k in self.user_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.has_more is not None:
-            result['hasMore'] = self.has_more
-        if self.next_cursor is not None:
-            result['nextCursor'] = self.next_cursor
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.media_status is not None:
+            result['mediaStatus'] = self.media_status
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.status is not None:
+            result['status'] = self.status
+        if self.title is not None:
+            result['title'] = self.title
         result['userList'] = []
         if self.user_list is not None:
             for k in self.user_list:
                 result['userList'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('hasMore') is not None:
-            self.has_more = m.get('hasMore')
-        if m.get('nextCursor') is not None:
-            self.next_cursor = m.get('nextCursor')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('mediaStatus') is not None:
+            self.media_status = m.get('mediaStatus')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('title') is not None:
+            self.title = m.get('title')
         self.user_list = []
         if m.get('userList') is not None:
             for k in m.get('userList'):
-                temp_model = ListResidentDeptUsersResponseBodyUserList()
+                temp_model = QueryConferenceInfoBatchResponseBodyInfosUserList()
                 self.user_list.append(temp_model.from_map(k))
         return self
 
 
-class ListResidentDeptUsersResponse(TeaModel):
+class QueryConferenceInfoBatchResponseBody(TeaModel):
+    def __init__(
+        self,
+        infos: List[QueryConferenceInfoBatchResponseBodyInfos] = None,
+    ):
+        self.infos = infos
+
+    def validate(self):
+        if self.infos:
+            for k in self.infos:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['infos'] = []
+        if self.infos is not None:
+            for k in self.infos:
+                result['infos'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.infos = []
+        if m.get('infos') is not None:
+            for k in m.get('infos'):
+                temp_model = QueryConferenceInfoBatchResponseBodyInfos()
+                self.infos.append(temp_model.from_map(k))
+        return self
+
+
+class QueryConferenceInfoBatchResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListResidentDeptUsersResponseBody = None,
+        body: QueryConferenceInfoBatchResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2385,20 +3519,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListResidentDeptUsersResponseBody()
+            temp_model = QueryConferenceInfoBatchResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListResidentSubDeptsHeaders(TeaModel):
+class QueryConferenceMembersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2423,151 +3557,187 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListResidentSubDeptsRequest(TeaModel):
+class QueryConferenceMembersRequest(TeaModel):
     def __init__(
         self,
-        cursor: int = None,
-        size: int = None,
-        sub_corp_id: str = None,
+        max_results: int = None,
+        next_token: str = None,
     ):
-        self.cursor = cursor
-        self.size = size
-        self.sub_corp_id = sub_corp_id
+        self.max_results = max_results
+        self.next_token = next_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.cursor is not None:
-            result['cursor'] = self.cursor
-        if self.size is not None:
-            result['size'] = self.size
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cursor') is not None:
-            self.cursor = m.get('cursor')
-        if m.get('size') is not None:
-            self.size = m.get('size')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class ListResidentSubDeptsResponseBodyDepartmentList(TeaModel):
+class QueryConferenceMembersResponseBodyMemberModels(TeaModel):
     def __init__(
         self,
-        department_id: int = None,
-        department_name: str = None,
-        super_department_id: int = None,
+        attend_status: int = None,
+        co_host: bool = None,
+        conference_id: str = None,
+        duration: int = None,
+        host: bool = None,
+        join_time: int = None,
+        leave_time: int = None,
+        outer_org_member: bool = None,
+        pstn_join: bool = None,
+        union_id: str = None,
+        user_nick: str = None,
     ):
-        self.department_id = department_id
-        self.department_name = department_name
-        self.super_department_id = super_department_id
+        self.attend_status = attend_status
+        self.co_host = co_host
+        self.conference_id = conference_id
+        self.duration = duration
+        self.host = host
+        self.join_time = join_time
+        self.leave_time = leave_time
+        self.outer_org_member = outer_org_member
+        self.pstn_join = pstn_join
+        self.union_id = union_id
+        self.user_nick = user_nick
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id is not None:
-            result['departmentId'] = self.department_id
-        if self.department_name is not None:
-            result['departmentName'] = self.department_name
-        if self.super_department_id is not None:
-            result['superDepartmentId'] = self.super_department_id
+        if self.attend_status is not None:
+            result['attendStatus'] = self.attend_status
+        if self.co_host is not None:
+            result['coHost'] = self.co_host
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.duration is not None:
+            result['duration'] = self.duration
+        if self.host is not None:
+            result['host'] = self.host
+        if self.join_time is not None:
+            result['joinTime'] = self.join_time
+        if self.leave_time is not None:
+            result['leaveTime'] = self.leave_time
+        if self.outer_org_member is not None:
+            result['outerOrgMember'] = self.outer_org_member
+        if self.pstn_join is not None:
+            result['pstnJoin'] = self.pstn_join
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_nick is not None:
+            result['userNick'] = self.user_nick
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentId') is not None:
-            self.department_id = m.get('departmentId')
-        if m.get('departmentName') is not None:
-            self.department_name = m.get('departmentName')
-        if m.get('superDepartmentId') is not None:
-            self.super_department_id = m.get('superDepartmentId')
+        if m.get('attendStatus') is not None:
+            self.attend_status = m.get('attendStatus')
+        if m.get('coHost') is not None:
+            self.co_host = m.get('coHost')
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('duration') is not None:
+            self.duration = m.get('duration')
+        if m.get('host') is not None:
+            self.host = m.get('host')
+        if m.get('joinTime') is not None:
+            self.join_time = m.get('joinTime')
+        if m.get('leaveTime') is not None:
+            self.leave_time = m.get('leaveTime')
+        if m.get('outerOrgMember') is not None:
+            self.outer_org_member = m.get('outerOrgMember')
+        if m.get('pstnJoin') is not None:
+            self.pstn_join = m.get('pstnJoin')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userNick') is not None:
+            self.user_nick = m.get('userNick')
         return self
 
 
-class ListResidentSubDeptsResponseBody(TeaModel):
+class QueryConferenceMembersResponseBody(TeaModel):
     def __init__(
         self,
-        department_list: List[ListResidentSubDeptsResponseBodyDepartmentList] = None,
-        has_more: bool = None,
-        next_cursor: int = None,
-        total: int = None,
+        member_models: List[QueryConferenceMembersResponseBodyMemberModels] = None,
+        next_token: str = None,
+        total_count: int = None,
     ):
-        self.department_list = department_list
-        self.has_more = has_more
-        self.next_cursor = next_cursor
-        self.total = total
+        self.member_models = member_models
+        self.next_token = next_token
+        self.total_count = total_count
 
     def validate(self):
-        if self.department_list:
-            for k in self.department_list:
+        if self.member_models:
+            for k in self.member_models:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['departmentList'] = []
-        if self.department_list is not None:
-            for k in self.department_list:
-                result['departmentList'].append(k.to_map() if k else None)
-        if self.has_more is not None:
-            result['hasMore'] = self.has_more
-        if self.next_cursor is not None:
-            result['nextCursor'] = self.next_cursor
-        if self.total is not None:
-            result['total'] = self.total
+        result['memberModels'] = []
+        if self.member_models is not None:
+            for k in self.member_models:
+                result['memberModels'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.department_list = []
-        if m.get('departmentList') is not None:
-            for k in m.get('departmentList'):
-                temp_model = ListResidentSubDeptsResponseBodyDepartmentList()
-                self.department_list.append(temp_model.from_map(k))
-        if m.get('hasMore') is not None:
-            self.has_more = m.get('hasMore')
-        if m.get('nextCursor') is not None:
-            self.next_cursor = m.get('nextCursor')
-        if m.get('total') is not None:
-            self.total = m.get('total')
+        self.member_models = []
+        if m.get('memberModels') is not None:
+            for k in m.get('memberModels'):
+                temp_model = QueryConferenceMembersResponseBodyMemberModels()
+                self.member_models.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
         return self
 
 
-class ListResidentSubDeptsResponse(TeaModel):
+class QueryConferenceMembersResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListResidentSubDeptsResponseBody = None,
+        body: QueryConferenceMembersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2593,20 +3763,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListResidentSubDeptsResponseBody()
+            temp_model = QueryConferenceMembersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListResidentUserInfosHeaders(TeaModel):
+class QueryScheduleConferenceInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2631,219 +3801,300 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListResidentUserInfosRequest(TeaModel):
+class QueryScheduleConferenceInfoRequest(TeaModel):
     def __init__(
         self,
-        sub_corp_id: str = None,
-        user_ids: List[str] = None,
+        max_results: int = None,
+        next_token: str = None,
     ):
-        self.sub_corp_id = sub_corp_id
-        self.user_ids = user_ids
+        self.max_results = max_results
+        self.next_token = next_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
-        if self.user_ids is not None:
-            result['userIds'] = self.user_ids
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
-        if m.get('userIds') is not None:
-            self.user_ids = m.get('userIds')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class ListResidentUserInfosShrinkRequest(TeaModel):
+class QueryScheduleConferenceInfoResponseBodyConferenceList(TeaModel):
     def __init__(
         self,
-        sub_corp_id: str = None,
-        user_ids_shrink: str = None,
+        conference_id: str = None,
+        end_time: int = None,
+        room_code: str = None,
+        start_time: int = None,
+        status: int = None,
+        title: str = None,
     ):
-        self.sub_corp_id = sub_corp_id
-        self.user_ids_shrink = user_ids_shrink
+        self.conference_id = conference_id
+        self.end_time = end_time
+        self.room_code = room_code
+        self.start_time = start_time
+        self.status = status
+        self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
-        if self.user_ids_shrink is not None:
-            result['userIds'] = self.user_ids_shrink
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.room_code is not None:
+            result['roomCode'] = self.room_code
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.status is not None:
+            result['status'] = self.status
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('roomCode') is not None:
+            self.room_code = m.get('roomCode')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class QueryScheduleConferenceInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        conference_list: List[QueryScheduleConferenceInfoResponseBodyConferenceList] = None,
+        next_token: str = None,
+        total_count: int = None,
+    ):
+        self.conference_list = conference_list
+        self.next_token = next_token
+        self.total_count = total_count
+
+    def validate(self):
+        if self.conference_list:
+            for k in self.conference_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['conferenceList'] = []
+        if self.conference_list is not None:
+            for k in self.conference_list:
+                result['conferenceList'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.conference_list = []
+        if m.get('conferenceList') is not None:
+            for k in m.get('conferenceList'):
+                temp_model = QueryScheduleConferenceInfoResponseBodyConferenceList()
+                self.conference_list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class QueryScheduleConferenceInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryScheduleConferenceInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
-        if m.get('userIds') is not None:
-            self.user_ids_shrink = m.get('userIds')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryScheduleConferenceInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListResidentUserInfosResponseBodyUserListRoles(TeaModel):
+class StartCloudRecordHeaders(TeaModel):
     def __init__(
         self,
-        tag_code: str = None,
-        tag_id: int = None,
-        tag_name: str = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
     ):
-        self.tag_code = tag_code
-        self.tag_id = tag_id
-        self.tag_name = tag_name
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.tag_code is not None:
-            result['tagCode'] = self.tag_code
-        if self.tag_id is not None:
-            result['tagId'] = self.tag_id
-        if self.tag_name is not None:
-            result['tagName'] = self.tag_name
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('tagCode') is not None:
-            self.tag_code = m.get('tagCode')
-        if m.get('tagId') is not None:
-            self.tag_id = m.get('tagId')
-        if m.get('tagName') is not None:
-            self.tag_name = m.get('tagName')
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListResidentUserInfosResponseBodyUserList(TeaModel):
+class StartCloudRecordRequest(TeaModel):
     def __init__(
         self,
-        feature: str = None,
-        roles: List[ListResidentUserInfosResponseBodyUserListRoles] = None,
+        mode: str = None,
+        small_window_position: str = None,
         union_id: str = None,
-        user_id: str = None,
-        user_name: str = None,
     ):
-        self.feature = feature
-        self.roles = roles
+        self.mode = mode
+        self.small_window_position = small_window_position
         self.union_id = union_id
-        self.user_id = user_id
-        self.user_name = user_name
 
     def validate(self):
-        if self.roles:
-            for k in self.roles:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.feature is not None:
-            result['feature'] = self.feature
-        result['roles'] = []
-        if self.roles is not None:
-            for k in self.roles:
-                result['roles'].append(k.to_map() if k else None)
+        if self.mode is not None:
+            result['mode'] = self.mode
+        if self.small_window_position is not None:
+            result['smallWindowPosition'] = self.small_window_position
         if self.union_id is not None:
             result['unionId'] = self.union_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        if self.user_name is not None:
-            result['userName'] = self.user_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('feature') is not None:
-            self.feature = m.get('feature')
-        self.roles = []
-        if m.get('roles') is not None:
-            for k in m.get('roles'):
-                temp_model = ListResidentUserInfosResponseBodyUserListRoles()
-                self.roles.append(temp_model.from_map(k))
+        if m.get('mode') is not None:
+            self.mode = m.get('mode')
+        if m.get('smallWindowPosition') is not None:
+            self.small_window_position = m.get('smallWindowPosition')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        if m.get('userName') is not None:
-            self.user_name = m.get('userName')
         return self
 
 
-class ListResidentUserInfosResponseBody(TeaModel):
+class StartCloudRecordResponseBody(TeaModel):
     def __init__(
         self,
-        user_list: List[ListResidentUserInfosResponseBodyUserList] = None,
+        code: str = None,
     ):
-        self.user_list = user_list
+        self.code = code
 
     def validate(self):
-        if self.user_list:
-            for k in self.user_list:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['userList'] = []
-        if self.user_list is not None:
-            for k in self.user_list:
-                result['userList'].append(k.to_map() if k else None)
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.user_list = []
-        if m.get('userList') is not None:
-            for k in m.get('userList'):
-                temp_model = ListResidentUserInfosResponseBodyUserList()
-                self.user_list.append(temp_model.from_map(k))
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
-class ListResidentUserInfosResponse(TeaModel):
+class StartCloudRecordResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListResidentUserInfosResponseBody = None,
+        body: StartCloudRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -2869,20 +4120,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListResidentUserInfosResponseBody()
+            temp_model = StartCloudRecordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListSimpleUsersByRoleHeaders(TeaModel):
+class StartStreamOutHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -2907,157 +4158,110 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListSimpleUsersByRoleRequest(TeaModel):
+class StartStreamOutRequest(TeaModel):
     def __init__(
         self,
-        offset: int = None,
-        role_id: int = None,
-        size: int = None,
-        sub_corp_id: str = None,
-    ):
-        self.offset = offset
-        self.role_id = role_id
-        self.size = size
-        self.sub_corp_id = sub_corp_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.offset is not None:
-            result['offset'] = self.offset
-        if self.role_id is not None:
-            result['roleId'] = self.role_id
-        if self.size is not None:
-            result['size'] = self.size
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('offset') is not None:
-            self.offset = m.get('offset')
-        if m.get('roleId') is not None:
-            self.role_id = m.get('roleId')
-        if m.get('size') is not None:
-            self.size = m.get('size')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
-        return self
-
-
-class ListSimpleUsersByRoleResponseBodyUserList(TeaModel):
-    def __init__(
-        self,
-        job_number: str = None,
-        name: str = None,
+        mode: str = None,
+        need_host_join: bool = None,
+        small_window_position: str = None,
+        stream_name: str = None,
+        stream_url_list: List[str] = None,
         union_id: str = None,
-        user_id: str = None,
     ):
-        self.job_number = job_number
-        self.name = name
+        self.mode = mode
+        self.need_host_join = need_host_join
+        self.small_window_position = small_window_position
+        self.stream_name = stream_name
+        self.stream_url_list = stream_url_list
         self.union_id = union_id
-        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.job_number is not None:
-            result['jobNumber'] = self.job_number
-        if self.name is not None:
-            result['name'] = self.name
+        if self.mode is not None:
+            result['mode'] = self.mode
+        if self.need_host_join is not None:
+            result['needHostJoin'] = self.need_host_join
+        if self.small_window_position is not None:
+            result['smallWindowPosition'] = self.small_window_position
+        if self.stream_name is not None:
+            result['streamName'] = self.stream_name
+        if self.stream_url_list is not None:
+            result['streamUrlList'] = self.stream_url_list
         if self.union_id is not None:
             result['unionId'] = self.union_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('jobNumber') is not None:
-            self.job_number = m.get('jobNumber')
-        if m.get('name') is not None:
-            self.name = m.get('name')
+        if m.get('mode') is not None:
+            self.mode = m.get('mode')
+        if m.get('needHostJoin') is not None:
+            self.need_host_join = m.get('needHostJoin')
+        if m.get('smallWindowPosition') is not None:
+            self.small_window_position = m.get('smallWindowPosition')
+        if m.get('streamName') is not None:
+            self.stream_name = m.get('streamName')
+        if m.get('streamUrlList') is not None:
+            self.stream_url_list = m.get('streamUrlList')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
         return self
 
 
-class ListSimpleUsersByRoleResponseBody(TeaModel):
+class StartStreamOutResponseBody(TeaModel):
     def __init__(
         self,
-        has_more: bool = None,
-        next_cursor: int = None,
-        user_list: List[ListSimpleUsersByRoleResponseBodyUserList] = None,
+        fail_stream_map: Dict[str, Any] = None,
+        success_stream_map: Dict[str, Any] = None,
     ):
-        self.has_more = has_more
-        self.next_cursor = next_cursor
-        self.user_list = user_list
+        self.fail_stream_map = fail_stream_map
+        self.success_stream_map = success_stream_map
 
     def validate(self):
-        if self.user_list:
-            for k in self.user_list:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.has_more is not None:
-            result['hasMore'] = self.has_more
-        if self.next_cursor is not None:
-            result['nextCursor'] = self.next_cursor
-        result['userList'] = []
-        if self.user_list is not None:
-            for k in self.user_list:
-                result['userList'].append(k.to_map() if k else None)
+        if self.fail_stream_map is not None:
+            result['failStreamMap'] = self.fail_stream_map
+        if self.success_stream_map is not None:
+            result['successStreamMap'] = self.success_stream_map
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('hasMore') is not None:
-            self.has_more = m.get('hasMore')
-        if m.get('nextCursor') is not None:
-            self.next_cursor = m.get('nextCursor')
-        self.user_list = []
-        if m.get('userList') is not None:
-            for k in m.get('userList'):
-                temp_model = ListSimpleUsersByRoleResponseBodyUserList()
-                self.user_list.append(temp_model.from_map(k))
+        if m.get('failStreamMap') is not None:
+            self.fail_stream_map = m.get('failStreamMap')
+        if m.get('successStreamMap') is not None:
+            self.success_stream_map = m.get('successStreamMap')
         return self
 
 
-class ListSimpleUsersByRoleResponse(TeaModel):
+class StartStreamOutResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListSimpleUsersByRoleResponseBody = None,
+        body: StartStreamOutResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3083,20 +4287,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListSimpleUsersByRoleResponseBody()
+            temp_model = StartStreamOutResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListSubCorpsHeaders(TeaModel):
+class StopCloudRecordHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -3121,157 +4325,74 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListSubCorpsRequest(TeaModel):
+class StopCloudRecordRequest(TeaModel):
     def __init__(
         self,
-        is_only_direct: bool = None,
-        sub_corp_id: str = None,
-        types: str = None,
+        union_id: str = None,
     ):
-        self.is_only_direct = is_only_direct
-        self.sub_corp_id = sub_corp_id
-        self.types = types
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.is_only_direct is not None:
-            result['isOnlyDirect'] = self.is_only_direct
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
-        if self.types is not None:
-            result['types'] = self.types
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('isOnlyDirect') is not None:
-            self.is_only_direct = m.get('isOnlyDirect')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
-        if m.get('types') is not None:
-            self.types = m.get('types')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class ListSubCorpsResponseBodyCorpList(TeaModel):
+class StopCloudRecordResponseBody(TeaModel):
     def __init__(
         self,
-        corp_id: str = None,
-        corp_name: str = None,
-        industry: str = None,
-        industry_code: int = None,
-        region_id: str = None,
-        region_location: str = None,
-        region_type: str = None,
+        code: str = None,
     ):
-        self.corp_id = corp_id
-        self.corp_name = corp_name
-        self.industry = industry
-        self.industry_code = industry_code
-        self.region_id = region_id
-        self.region_location = region_location
-        self.region_type = region_type
+        self.code = code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.corp_id is not None:
-            result['corpId'] = self.corp_id
-        if self.corp_name is not None:
-            result['corpName'] = self.corp_name
-        if self.industry is not None:
-            result['industry'] = self.industry
-        if self.industry_code is not None:
-            result['industryCode'] = self.industry_code
-        if self.region_id is not None:
-            result['regionId'] = self.region_id
-        if self.region_location is not None:
-            result['regionLocation'] = self.region_location
-        if self.region_type is not None:
-            result['regionType'] = self.region_type
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('corpId') is not None:
-            self.corp_id = m.get('corpId')
-        if m.get('corpName') is not None:
-            self.corp_name = m.get('corpName')
-        if m.get('industry') is not None:
-            self.industry = m.get('industry')
-        if m.get('industryCode') is not None:
-            self.industry_code = m.get('industryCode')
-        if m.get('regionId') is not None:
-            self.region_id = m.get('regionId')
-        if m.get('regionLocation') is not None:
-            self.region_location = m.get('regionLocation')
-        if m.get('regionType') is not None:
-            self.region_type = m.get('regionType')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
-class ListSubCorpsResponseBody(TeaModel):
-    def __init__(
-        self,
-        corp_list: List[ListSubCorpsResponseBodyCorpList] = None,
-    ):
-        self.corp_list = corp_list
-
-    def validate(self):
-        if self.corp_list:
-            for k in self.corp_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['corpList'] = []
-        if self.corp_list is not None:
-            for k in self.corp_list:
-                result['corpList'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.corp_list = []
-        if m.get('corpList') is not None:
-            for k in m.get('corpList'):
-                temp_model = ListSubCorpsResponseBodyCorpList()
-                self.corp_list.append(temp_model.from_map(k))
-        return self
-
-
-class ListSubCorpsResponse(TeaModel):
+class StopCloudRecordResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListSubCorpsResponseBody = None,
+        body: StopCloudRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3297,20 +4418,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListSubCorpsResponseBody()
+            temp_model = StopCloudRecordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListSubDeptHeaders(TeaModel):
+class StopStreamOutHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -3335,121 +4456,196 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListSubDeptRequest(TeaModel):
+class StopStreamOutRequest(TeaModel):
     def __init__(
         self,
-        language: str = None,
-        sub_corp_id: str = None,
+        stop_all_stream: bool = None,
+        stream_id: str = None,
+        union_id: str = None,
     ):
-        self.language = language
-        self.sub_corp_id = sub_corp_id
+        self.stop_all_stream = stop_all_stream
+        self.stream_id = stream_id
+        self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.language is not None:
-            result['language'] = self.language
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.stop_all_stream is not None:
+            result['stopAllStream'] = self.stop_all_stream
+        if self.stream_id is not None:
+            result['streamId'] = self.stream_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('language') is not None:
-            self.language = m.get('language')
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('stopAllStream') is not None:
+            self.stop_all_stream = m.get('stopAllStream')
+        if m.get('streamId') is not None:
+            self.stream_id = m.get('streamId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
         return self
 
 
-class ListSubDeptResponseBodyResult(TeaModel):
+class StopStreamOutResponseBody(TeaModel):
     def __init__(
         self,
-        department_id: int = None,
-        name: str = None,
+        code: str = None,
     ):
-        self.department_id = department_id
-        self.name = name
+        self.code = code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id is not None:
-            result['departmentId'] = self.department_id
-        if self.name is not None:
-            result['name'] = self.name
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentId') is not None:
-            self.department_id = m.get('departmentId')
-        if m.get('name') is not None:
-            self.name = m.get('name')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
-class ListSubDeptResponseBody(TeaModel):
+class StopStreamOutResponse(TeaModel):
     def __init__(
         self,
-        result: List[ListSubDeptResponseBodyResult] = None,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: StopStreamOutResponseBody = None,
     ):
-        self.result = result
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
 
     def validate(self):
-        if self.result:
-            for k in self.result:
-                if k:
-                    k.validate()
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = StopStreamOutResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateVideoConferenceExtInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UpdateVideoConferenceExtInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        case: str = None,
+        code: str = None,
+    ):
+        self.case = case
+        self.code = code
+
+    def validate(self):
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['result'] = []
-        if self.result is not None:
-            for k in self.result:
-                result['result'].append(k.to_map() if k else None)
+        if self.case is not None:
+            result['case'] = self.case
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.result = []
-        if m.get('result') is not None:
-            for k in m.get('result'):
-                temp_model = ListSubDeptResponseBodyResult()
-                self.result.append(temp_model.from_map(k))
+        if m.get('case') is not None:
+            self.case = m.get('case')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
-class ListSubDeptResponse(TeaModel):
+class UpdateVideoConferenceExtInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListSubDeptResponseBody = None,
+        body: UpdateVideoConferenceExtInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3475,20 +4671,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListSubDeptResponseBody()
+            temp_model = UpdateVideoConferenceExtInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListSubDeptIdsHeaders(TeaModel):
+class UpdateVideoConferenceSettingHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -3513,74 +4709,110 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class ListSubDeptIdsRequest(TeaModel):
+class UpdateVideoConferenceSettingRequest(TeaModel):
     def __init__(
         self,
-        sub_corp_id: str = None,
+        allow_unmute_self: bool = None,
+        auto_transfer_host: bool = None,
+        forbidden_share_screen: bool = None,
+        lock_conference: bool = None,
+        mute_all: bool = None,
+        only_internal_employees_join: bool = None,
     ):
-        self.sub_corp_id = sub_corp_id
+        self.allow_unmute_self = allow_unmute_self
+        self.auto_transfer_host = auto_transfer_host
+        self.forbidden_share_screen = forbidden_share_screen
+        self.lock_conference = lock_conference
+        self.mute_all = mute_all
+        self.only_internal_employees_join = only_internal_employees_join
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.sub_corp_id is not None:
-            result['subCorpId'] = self.sub_corp_id
+        if self.allow_unmute_self is not None:
+            result['allowUnmuteSelf'] = self.allow_unmute_self
+        if self.auto_transfer_host is not None:
+            result['autoTransferHost'] = self.auto_transfer_host
+        if self.forbidden_share_screen is not None:
+            result['forbiddenShareScreen'] = self.forbidden_share_screen
+        if self.lock_conference is not None:
+            result['lockConference'] = self.lock_conference
+        if self.mute_all is not None:
+            result['muteAll'] = self.mute_all
+        if self.only_internal_employees_join is not None:
+            result['onlyInternalEmployeesJoin'] = self.only_internal_employees_join
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('subCorpId') is not None:
-            self.sub_corp_id = m.get('subCorpId')
+        if m.get('allowUnmuteSelf') is not None:
+            self.allow_unmute_self = m.get('allowUnmuteSelf')
+        if m.get('autoTransferHost') is not None:
+            self.auto_transfer_host = m.get('autoTransferHost')
+        if m.get('forbiddenShareScreen') is not None:
+            self.forbidden_share_screen = m.get('forbiddenShareScreen')
+        if m.get('lockConference') is not None:
+            self.lock_conference = m.get('lockConference')
+        if m.get('muteAll') is not None:
+            self.mute_all = m.get('muteAll')
+        if m.get('onlyInternalEmployeesJoin') is not None:
+            self.only_internal_employees_join = m.get('onlyInternalEmployeesJoin')
         return self
 
 
-class ListSubDeptIdsResponseBody(TeaModel):
+class UpdateVideoConferenceSettingResponseBody(TeaModel):
     def __init__(
         self,
-        department_id_list: List[int] = None,
+        case: str = None,
+        code: str = None,
     ):
-        self.department_id_list = department_id_list
+        self.case = case
+        self.code = code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_id_list is not None:
-            result['departmentIdList'] = self.department_id_list
+        if self.case is not None:
+            result['case'] = self.case
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentIdList') is not None:
-            self.department_id_list = m.get('departmentIdList')
+        if m.get('case') is not None:
+            self.case = m.get('case')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
-class ListSubDeptIdsResponse(TeaModel):
+class UpdateVideoConferenceSettingResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListSubDeptIdsResponseBody = None,
+        body: UpdateVideoConferenceSettingResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -3606,12 +4838,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListSubDeptIdsResponseBody()
+            temp_model = UpdateVideoConferenceSettingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.20
+Version: 2.0.21
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.20/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.21/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,17 @@
 alibabacloud_dingtalk/customer_service_1_0/models.py
 alibabacloud_dingtalk/datacenter_1_0/__init__.py
 alibabacloud_dingtalk/datacenter_1_0/client.py
 alibabacloud_dingtalk/datacenter_1_0/models.py
 alibabacloud_dingtalk/devicemng_1_0/__init__.py
 alibabacloud_dingtalk/devicemng_1_0/client.py
 alibabacloud_dingtalk/devicemng_1_0/models.py
+alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+alibabacloud_dingtalk/ding_phone_1_0/client.py
+alibabacloud_dingtalk/ding_phone_1_0/models.py
 alibabacloud_dingtalk/dingmi_1_0/__init__.py
 alibabacloud_dingtalk/dingmi_1_0/client.py
 alibabacloud_dingtalk/dingmi_1_0/models.py
 alibabacloud_dingtalk/diot_1_0/__init__.py
 alibabacloud_dingtalk/diot_1_0/client.py
 alibabacloud_dingtalk/diot_1_0/models.py
 alibabacloud_dingtalk/doc_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.20/setup.py` & `alibabacloud_dingtalk-2.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 13/06/2023
+Created on 16/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

