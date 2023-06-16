# Comparing `tmp/kingsoftcloud-sdk-python-1.0.3.tar.gz` & `tmp/kingsoftcloud-sdk-python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.0.3.tar", last modified: Wed Mar 29 08:36:55 2023, max compression
+gzip compressed data, was "kingsoftcloud-sdk-python-1.1.0.tar", last modified: Fri Jun 16 08:20:55 2023, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.0.3.tar` & `kingsoftcloud-sdk-python-1.1.0.tar`

### file list

```diff
@@ -1,113 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.058120 kingsoftcloud-sdk-python-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-29 08:36:55.058120 kingsoftcloud-sdk-python-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.046120 kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-29 08:36:55.000000 kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-03-29 08:36:55.000000 kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:36:55.000000 kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-29 08:36:55.000000 kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-29 08:36:55.000000 kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.046120 kingsoftcloud-sdk-python-1.0.3/ksyun/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.046120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.046120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20211209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20211209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20211209/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20211209/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.050120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   118595 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.054120 kingsoftcloud-sdk-python-1.0.3/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.058120 kingsoftcloud-sdk-python-1.0.3/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.058120 kingsoftcloud-sdk-python-1.0.3/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:55.058120 kingsoftcloud-sdk-python-1.0.3/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/ksyun/common/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-29 08:36:55.058120 kingsoftcloud-sdk-python-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-29 08:36:40.000000 kingsoftcloud-sdk-python-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 08:20:55.000000 kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.881421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47258 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57434 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.885421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122915 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.889421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/slb/v20171210/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.893421 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68705 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73360 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/ksyun/common/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 08:20:55.897421 kingsoftcloud-sdk-python-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-16 08:20:44.000000 kingsoftcloud-sdk-python-1.1.0/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.0.3/LICENSE` & `kingsoftcloud-sdk-python-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.0.3
+Version: 1.1.0
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.0.3/README.rst` & `kingsoftcloud-sdk-python-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.0.3
+Version: 1.1.0
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.0.3/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud-sdk-python-1.1.0/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -20,18 +20,30 @@
 ksyun/client/bill_union/__init__.py
 ksyun/client/bill_union/v20200101/__init__.py
 ksyun/client/bill_union/v20200101/client.py
 ksyun/client/bill_union/v20200101/models.py
 ksyun/client/bill_union/v20211209/__init__.py
 ksyun/client/bill_union/v20211209/client.py
 ksyun/client/bill_union/v20211209/models.py
+ksyun/client/bws/__init__.py
+ksyun/client/bws/v20160304/__init__.py
+ksyun/client/bws/v20160304/client.py
+ksyun/client/bws/v20160304/models.py
 ksyun/client/ebs/__init__.py
 ksyun/client/ebs/v20160304/__init__.py
 ksyun/client/ebs/v20160304/client.py
 ksyun/client/ebs/v20160304/models.py
+ksyun/client/eip/__init__.py
+ksyun/client/eip/v20160304/__init__.py
+ksyun/client/eip/v20160304/client.py
+ksyun/client/eip/v20160304/models.py
+ksyun/client/epc/__init__.py
+ksyun/client/epc/v20151101/__init__.py
+ksyun/client/epc/v20151101/client.py
+ksyun/client/epc/v20151101/models.py
 ksyun/client/iam/__init__.py
 ksyun/client/iam/v20151101/__init__.py
 ksyun/client/iam/v20151101/client.py
 ksyun/client/iam/v20151101/models.py
 ksyun/client/kad/__init__.py
 ksyun/client/kad/v20161122/__init__.py
 ksyun/client/kad/v20161122/client.py
@@ -40,18 +52,33 @@
 ksyun/client/kead/v20200101/__init__.py
 ksyun/client/kead/v20200101/client.py
 ksyun/client/kead/v20200101/models.py
 ksyun/client/kec/__init__.py
 ksyun/client/kec/v20160304/__init__.py
 ksyun/client/kec/v20160304/client.py
 ksyun/client/kec/v20160304/models.py
+ksyun/client/mongodb/__init__.py
+ksyun/client/mongodb/v20170101/__init__.py
+ksyun/client/mongodb/v20170101/client.py
+ksyun/client/mongodb/v20170101/models.py
 ksyun/client/resourcemanager/__init__.py
 ksyun/client/resourcemanager/v20210320/__init__.py
 ksyun/client/resourcemanager/v20210320/client.py
 ksyun/client/resourcemanager/v20210320/models.py
+ksyun/client/sks/__init__.py
+ksyun/client/sks/v20151101/__init__.py
+ksyun/client/sks/v20151101/client.py
+ksyun/client/sks/v20151101/models.py
+ksyun/client/slb/__init__.py
+ksyun/client/slb/v20160304/__init__.py
+ksyun/client/slb/v20160304/client.py
+ksyun/client/slb/v20160304/models.py
+ksyun/client/slb/v20171210/__init__.py
+ksyun/client/slb/v20171210/client.py
+ksyun/client/slb/v20171210/models.py
 ksyun/client/sts/__init__.py
 ksyun/client/sts/v20151101/__init__.py
 ksyun/client/sts/v20151101/client.py
 ksyun/client/sts/v20151101/models.py
 ksyun/client/tagv2/__init__.py
 ksyun/client/tagv2/v20200901/__init__.py
 ksyun/client/tagv2/v20200901/client.py
@@ -59,14 +86,18 @@
 ksyun/client/trade/__init__.py
 ksyun/client/trade/v20200114/__init__.py
 ksyun/client/trade/v20200114/client.py
 ksyun/client/trade/v20200114/models.py
 ksyun/client/trade/v20200831/__init__.py
 ksyun/client/trade/v20200831/client.py
 ksyun/client/trade/v20200831/models.py
+ksyun/client/vpc/__init__.py
+ksyun/client/vpc/v20160304/__init__.py
+ksyun/client/vpc/v20160304/client.py
+ksyun/client/vpc/v20160304/models.py
 ksyun/common/__init__.py
 ksyun/common/abstract_client.py
 ksyun/common/abstract_model.py
 ksyun/common/common_client.py
 ksyun/common/credential.py
 ksyun/common/sign.py
 ksyun/common/exception/__init__.py
```

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/__init__.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.0.3'
+__version__ = '1.1.0'
```

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20211209/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/bill_union/v20211209/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/bill_union/v20211209/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/iam/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2097,45 +2097,22 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
-    def DescribeInstanceKmr(self, request):
-        """DescribeInstanceKmr
-        :param request: Request instance for DescribeInstanceKmr.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeInstanceKmrRequest`
-        """
-        try:
-            params = request._serialize()
-            body = self.call("DescribeInstanceKmr", params)
-            response = json.loads(body)
-            if "Error" not in response:
-                return body
-            else:
-                code = response["Error"]["Code"]
-                message = response["Error"]["Message"]
-                req_id = response["RequestId"]
-                raise KsyunSDKException(code, message, req_id)
-        except Exception as e:
-            if isinstance(e, KsyunSDKException):
-                raise
-            else:
-                raise KsyunSDKException(e.message, e.message)
-
-
-    def ValidatedDiskEncrypt(self, request):
-        """ValidatedDiskEncrypt
-        :param request: Request instance for ValidatedDiskEncrypt.
-        :type request: :class:`ksyun.client.kec.v20160304.models.ValidatedDiskEncryptRequest`
+    def PreMigrateInstance(self, request):
+        """创建预迁移
+        :param request: Request instance for PreMigrateInstance.
+        :type request: :class:`ksyun.client.kec.v20160304.models.PreMigrateInstanceRequest`
         """
         try:
             params = request._serialize()
-            body = self.call("ValidatedDiskEncrypt", params)
+            body = self.call("PreMigrateInstance", params)
             response = json.loads(body)
             if "Error" not in response:
                 return body
             else:
                 code = response["Error"]["Code"]
                 message = response["Error"]["Message"]
                 req_id = response["RequestId"]
@@ -2143,22 +2120,22 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
-    def DistributeKmsPermission(self, request):
-        """DistributeKmsPermission
-        :param request: Request instance for DistributeKmsPermission.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DistributeKmsPermissionRequest`
+    def CancelPreMigrateInstance(self, request):
+        """取消预迁移
+        :param request: Request instance for CancelPreMigrateInstance.
+        :type request: :class:`ksyun.client.kec.v20160304.models.CancelPreMigrateInstanceRequest`
         """
         try:
             params = request._serialize()
-            body = self.call("DistributeKmsPermission", params)
+            body = self.call("CancelPreMigrateInstance", params)
             response = json.loads(body)
             if "Error" not in response:
                 return body
             else:
                 code = response["Error"]["Code"]
                 message = response["Error"]["Message"]
                 req_id = response["RequestId"]
@@ -2166,22 +2143,22 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
-    def DescribeEntrySnapshots(self, request):
-        """DescribeEntrySnapshots
-        :param request: Request instance for DescribeEntrySnapshots.
-        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeEntrySnapshotsRequest`
+    def DescribeInstanceKmr(self, request):
+        """DescribeInstanceKmr
+        :param request: Request instance for DescribeInstanceKmr.
+        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeInstanceKmrRequest`
         """
         try:
             params = request._serialize()
-            body = self.call("DescribeEntrySnapshots", params)
+            body = self.call("DescribeInstanceKmr", params)
             response = json.loads(body)
             if "Error" not in response:
                 return body
             else:
                 code = response["Error"]["Code"]
                 message = response["Error"]["Message"]
                 req_id = response["RequestId"]
```

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/kec/v20160304/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,18 @@
         :param InstanceId: 待返回描述信息的实例ID列表，N的范围为1-100
 标准UUID格式，形如`^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$`
         :type PathPrefix: Filter
         :param ProjectId: 待返回实例信息的项目ID列表，N的范围为1-100
 
         :type PathPrefix: Filter
         :param Filter: 待返回实例信息的项目ID列表，N的范围为1-100
-支持如下过滤器名称<br>instance-id 实例ID<br>subnet-id 子网ID<br>vpc-id vpc ID<br>instance-name 实例名称<br>instance-type 实例类型<br>private-ip-address 内网IP<br>image-id 镜像ID<br>charge-type 计费模式（Monthly（包年包月）、Daily（按量付费（按日月结））、HourlyInstantSettlement（按量付费）、Spot（竞价型实例））<br>ProjectId.N 所属项目<br>network-interface.subnet-id 网络接口关联的子网ID<br>network-interface.network-interface-id 网卡的ID<br>network-interface.group-id 网络接口关联的安全组ID<br>instance-state.name [实例状态](https://docs.ksyun.com/documents/836)<br>availability-zone-name [可用区（AvailabilityZone）](https://docs.ksyun.com/documents/67)
+支持如下过滤器名称<br>instance-id 实例ID<br>subnet-id 子网ID<br>vpc-id vpc ID<br>instance-name 实例名称<br>instance-type 实例类型<br>private-ip-address 内网IP<br>image-id 镜像ID<br>charge-type 计费模式（1（包年包月）、5（按量付费（按日月结））、87（按量付费）、810（竞价型实例））2（按小时计费）, 
+
+84（PostPaidByHour)
+<br>ProjectId.N 所属项目<br>network-interface.subnet-id 网络接口关联的子网ID<br>network-interface.network-interface-id 网卡的ID<br>network-interface.group-id 网络接口关联的安全组ID<br>instance-state.name [实例状态](https://docs.ksyun.com/documents/836)<br>availability-zone-name [可用区（AvailabilityZone）](https://docs.ksyun.com/documents/67)
         :type PathPrefix: Filter
         :param Sort: 筛选器
 支持如下筛选器名称：<br>InstanceName –主机名称<br>CreationDate –创建时间<br>PrivateIpAddress - 主机内网IP（主网卡）
         :type PathPrefix: String
         :param Search: 搜索条件，模糊匹配
 支持字段：实例名（InstanceName）、主网卡私有IP地址（PrivateIpAddress）
         :type PathPrefix: String
@@ -93,14 +96,20 @@
         :type PathPrefix: String
         :param ProjectId: 实例所属项目ID
         :type PathPrefix: Int
         :param DataDisk: 数据盘是否随实例释放
         :type PathPrefix: Filter
         :param NetworkInterface: 辅网卡
         :type PathPrefix: Filter
+        :param Userdata: 用户自定义数据
+        :type PathPrefix: String
+        :param SystemDisk.DiskType: 系统盘类型
+        :type PathPrefix: String
+        :param SystemDisk.DiskSize: 系统盘大小
+        :type PathPrefix: Int
         """
         self.ImageId = None
         self.DedicatedHostId = None
         self.InstanceConfigure.VCPU = None
         self.InstanceConfigure.MemoryGb = None
         self.InstanceType = None
         self.DataDiskGb = None
@@ -113,14 +122,17 @@
         self.SecurityGroupId = None
         self.PrivateIpAddress = None
         self.InstanceName = None
         self.InstanceNameSuffix = None
         self.ProjectId = None
         self.DataDisk = None
         self.NetworkInterface = None
+        self.Userdata = None
+        self.SystemDisk.DiskType = None
+        self.SystemDisk.DiskSize = None
 
     def _deserialize(self, params):
         if params.get("ImageId"):
             self.ImageId = params.get("ImageId")
         if params.get("DedicatedHostId"):
             self.DedicatedHostId = params.get("DedicatedHostId")
         if params.get("InstanceConfigure.VCPU"):
@@ -153,14 +165,20 @@
             self.InstanceNameSuffix = params.get("InstanceNameSuffix")
         if params.get("ProjectId"):
             self.ProjectId = params.get("ProjectId")
         if params.get("DataDisk"):
             self.DataDisk = params.get("DataDisk")
         if params.get("NetworkInterface"):
             self.NetworkInterface = params.get("NetworkInterface")
+        if params.get("Userdata"):
+            self.Userdata = params.get("Userdata")
+        if params.get("SystemDisk.DiskType"):
+            self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
+        if params.get("SystemDisk.DiskSize"):
+            self.SystemDisk.DiskSize = params.get("SystemDisk.DiskSize")
 
 
 class StartInstancesRequest(AbstractModel):
     """StartInstances请求参数结构体
     """
 
     def __init__(self):
@@ -283,34 +301,40 @@
         :type PathPrefix: String
         :param DataDiskGb: 数据卷容量，单位GB，数据卷只能扩容或者保持不变，且不能低于[实例套餐类型定义](https://docs.ksyun.com/documents/705)的最小值。
 
         :type PathPrefix: Int
         :param CrossInstanceMigrate: 当前操作是否为变更实例套餐类型，若当前操作变更实例类型必须指定为true。（变更过程中必须保持云服务器关机状态；变更完成后启动云服务器生效；涉及本地盘类型的机型变更需加白名单）
 true/false
         :type PathPrefix: Boolean
-        :param SystemDisk.DiskType: 目标套餐系统盘类型（当本地盘机型变更为云盘机型时才需填写此参数）
+        :param SystemDisk.DiskType: 不能给默认值，不传默认按价格体系配置systemDisk属性中第一个创建
         :type PathPrefix: String
         :param DataDisk: 目标套餐数据盘类型（当本地盘机型变更为云盘机型时才需填写此参数，此参数仅对源本地数据盘生效）
 
         :type PathPrefix: Filter
         :param StopInstance: 是否对运行中的实例选择关机：是-true，否-false(默认)
         :type PathPrefix: Boolean
         :param AutoRestart: 变更实例类型后是否自动重启: 是-true，否-false(默认)
         :type PathPrefix: Boolean
+        :param SystemDisk.DiskSize: 系统盘大小，最大值500，最小值0
+        :type PathPrefix: Int
+        :param SystemDisk.ResizeType: 扩容 offline 离线扩容| online 在线扩容
+        :type PathPrefix: String
         """
         self.InstanceId = None
         self.InstanceType = None
         self.InstanceConfigure.VCPU = None
         self.InstanceConfigure.MemoryGb = None
         self.DataDiskGb = None
         self.CrossInstanceMigrate = None
         self.SystemDisk.DiskType = None
         self.DataDisk = None
         self.StopInstance = None
         self.AutoRestart = None
+        self.SystemDisk.DiskSize = None
+        self.SystemDisk.ResizeType = None
 
     def _deserialize(self, params):
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
         if params.get("InstanceType"):
             self.InstanceType = params.get("InstanceType")
         if params.get("InstanceConfigure.VCPU"):
@@ -325,14 +349,18 @@
             self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
         if params.get("DataDisk"):
             self.DataDisk = params.get("DataDisk")
         if params.get("StopInstance"):
             self.StopInstance = params.get("StopInstance")
         if params.get("AutoRestart"):
             self.AutoRestart = params.get("AutoRestart")
+        if params.get("SystemDisk.DiskSize"):
+            self.SystemDisk.DiskSize = params.get("SystemDisk.DiskSize")
+        if params.get("SystemDisk.ResizeType"):
+            self.SystemDisk.ResizeType = params.get("SystemDisk.ResizeType")
 
 
 class TerminateInstancesRequest(AbstractModel):
     """TerminateInstances请求参数结构体
     """
 
     def __init__(self):
@@ -416,46 +444,56 @@
         r"""更换或者重新安装实例操作系统
         :param InstanceId: 待更换或者重新安装操作系统的实例ID
 标准UUID格式，形如`^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$`
         :type PathPrefix: String
         :param ImageId: 待更换的镜像ID；如果缺省，表明无需改变镜像，只需重新安装实例的操作系统。
 标准UUID格式，形如`^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$`
         :type PathPrefix: String
-        :param SystemDisk: 云主机系统盘配置参数。若不指定该参数，则按照系统默认值进行分配。通用型N2、N3主机支持更换操作系统时指定系统盘大小。
+        :param SystemDisk.DiskSize: 云主机系统盘配置参数。若不指定该参数，则按照系统默认值进行分配。通用型N2、N3主机支持更换操作系统时指定系统盘大小。
 [SystemDisk](https://docs.ksyun.com/documents/5866)
-        :type PathPrefix: String
+        :type PathPrefix: Int
         :param InstancePassword: 实例开机密码
 最短8字符，最长32字符，必须包含大小写英文字符和数字，支持其他可见字符
         :type PathPrefix: String
         :param KeyId: 密钥ID
         :type PathPrefix: Filter
         :param KeepImageLogin: 保留镜像设置登录。该参数只对使用自定义镜像有效。当该值填写为true，默认InstancePassword参数无效。该参数与InstancePassword必须填写一个。
 true/false,默认false
         :type PathPrefix: Boolean
+        :param SystemDisk.DiskType: 不能给默认值，不传默认按价格体系配置systemDisk属性中第一个创建
+        :type PathPrefix: String
+        :param SystemDisk.ResizeType: 扩容 offline 离线扩容| online 在线扩容
+        :type PathPrefix: String
         """
         self.InstanceId = None
         self.ImageId = None
-        self.SystemDisk = None
+        self.SystemDisk.DiskSize = None
         self.InstancePassword = None
         self.KeyId = None
         self.KeepImageLogin = None
+        self.SystemDisk.DiskType = None
+        self.SystemDisk.ResizeType = None
 
     def _deserialize(self, params):
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
         if params.get("ImageId"):
             self.ImageId = params.get("ImageId")
-        if params.get("SystemDisk"):
-            self.SystemDisk = params.get("SystemDisk")
+        if params.get("SystemDisk.DiskSize"):
+            self.SystemDisk.DiskSize = params.get("SystemDisk.DiskSize")
         if params.get("InstancePassword"):
             self.InstancePassword = params.get("InstancePassword")
         if params.get("KeyId"):
             self.KeyId = params.get("KeyId")
         if params.get("KeepImageLogin"):
             self.KeepImageLogin = params.get("KeepImageLogin")
+        if params.get("SystemDisk.DiskType"):
+            self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
+        if params.get("SystemDisk.ResizeType"):
+            self.SystemDisk.ResizeType = params.get("SystemDisk.ResizeType")
 
 
 class CreateImageRequest(AbstractModel):
     """CreateImage请求参数结构体
     """
 
     def __init__(self):
@@ -731,15 +769,15 @@
 class DeleteLocalVolumeSnapshotRequest(AbstractModel):
     """DeleteLocalVolumeSnapshot请求参数结构体
     """
 
     def __init__(self):
         r"""删除本地盘快照
         :param LocalVolumeSnapshotId: 快照Id，支持批量删除，格式为LocalVolumeSnapshotId.N=XXX，N=1,2,3…100。
-        :type PathPrefix: Array
+        :type PathPrefix: Filter
         """
         self.LocalVolumeSnapshotId = None
 
     def _deserialize(self, params):
         if params.get("LocalVolumeSnapshotId"):
             self.LocalVolumeSnapshotId = params.get("LocalVolumeSnapshotId")
 
@@ -1024,17 +1062,16 @@
         :type PathPrefix: Boolean
         :param KeyId: 密钥对 
  
         :type PathPrefix: Filter
         :param DataDisk: 云盘数据盘类型 
  
         :type PathPrefix: Filter
-        :param SystemDisk: 系统盘类型 
- Local_SSD：本地SSD硬盘；SSD2.0：SSD云硬盘2.0；SATA2.0：普通云硬盘2.0；SSD3.0：SSD云硬盘3.0
-        :type PathPrefix: Filter
+        :param SystemDisk.DiskSize: 系统盘大小，最小值为0，最大值为500
+        :type PathPrefix: String
         :param AddressBandWidth: 弹性IP的带宽 
  
         :type PathPrefix: Int
         :param BandWidthShareId: 弹性IP指定的共享带宽ID 
  
         :type PathPrefix: String
         :param LineId: 弹性IP的链路类型的ID 
@@ -1054,35 +1091,41 @@
         :type PathPrefix: String
         :param InstanceNameTimeSuffix:  实例名称时间戳后缀，true/false 
  
         :type PathPrefix: Boolean
         :param Tag:  启动配置创建的ECS实例的标签键 
  支持1-128个字符，仅支持中英文字符、数字及±=._/@:
         :type PathPrefix: Filter
+        :param SystemDisk.DiskType: 不能给默认值，不传默认按价格体系配置systemDisk属性中第一个创建
+        :type PathPrefix: String
+        :param SystemDisk.ResizeType: 扩容 offline 离线扩容| online 在线扩容
+        :type PathPrefix: String
         """
         self.ScalingConfigurationName = None
         self.ImageId = None
         self.Password = None
         self.InstanceType = None
         self.ChargeType = None
         self.DataDiskGb = None
         self.ProjectId = None
         self.KeepImageLogin = None
         self.KeyId = None
         self.DataDisk = None
-        self.SystemDisk = None
+        self.SystemDisk.DiskSize = None
         self.AddressBandWidth = None
         self.BandWidthShareId = None
         self.LineId = None
         self.AddressProjectId = None
         self.InstanceName = None
         self.InstanceNameSuffix = None
         self.UserData = None
         self.InstanceNameTimeSuffix = None
         self.Tag = None
+        self.SystemDisk.DiskType = None
+        self.SystemDisk.ResizeType = None
 
     def _deserialize(self, params):
         if params.get("ScalingConfigurationName"):
             self.ScalingConfigurationName = params.get("ScalingConfigurationName")
         if params.get("ImageId"):
             self.ImageId = params.get("ImageId")
         if params.get("Password"):
@@ -1097,16 +1140,16 @@
             self.ProjectId = params.get("ProjectId")
         if params.get("KeepImageLogin"):
             self.KeepImageLogin = params.get("KeepImageLogin")
         if params.get("KeyId"):
             self.KeyId = params.get("KeyId")
         if params.get("DataDisk"):
             self.DataDisk = params.get("DataDisk")
-        if params.get("SystemDisk"):
-            self.SystemDisk = params.get("SystemDisk")
+        if params.get("SystemDisk.DiskSize"):
+            self.SystemDisk.DiskSize = params.get("SystemDisk.DiskSize")
         if params.get("AddressBandWidth"):
             self.AddressBandWidth = params.get("AddressBandWidth")
         if params.get("BandWidthShareId"):
             self.BandWidthShareId = params.get("BandWidthShareId")
         if params.get("LineId"):
             self.LineId = params.get("LineId")
         if params.get("AddressProjectId"):
@@ -1117,14 +1160,18 @@
             self.InstanceNameSuffix = params.get("InstanceNameSuffix")
         if params.get("UserData"):
             self.UserData = params.get("UserData")
         if params.get("InstanceNameTimeSuffix"):
             self.InstanceNameTimeSuffix = params.get("InstanceNameTimeSuffix")
         if params.get("Tag"):
             self.Tag = params.get("Tag")
+        if params.get("SystemDisk.DiskType"):
+            self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
+        if params.get("SystemDisk.ResizeType"):
+            self.SystemDisk.ResizeType = params.get("SystemDisk.ResizeType")
 
 
 class DeleteScalingConfigurationRequest(AbstractModel):
     """DeleteScalingConfiguration请求参数结构体
     """
 
     def __init__(self):
@@ -2351,15 +2398,15 @@
         r"""创建实例启动模版
         :param ImageId: 镜像ID
 标准UUID格式，形如`^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$`
         :type PathPrefix: String
         :param InstanceType: 实例套餐类型，如果调用时未指定实例套餐类型，默认值为I1.1A
 [实例套餐类型有效值](https://docs.ksyun.com/documents/40858) <br>具体套餐信息参考[实例套餐类型定义](https://docs.ksyun.com/documents/705)
         :type PathPrefix: String
-        :param SystemDisk: 云主机系统盘配置参数。若不指定该参数，则按照系统默认值进行分配。通用型N2、N3主机支持更换操作系统时指定系统盘大小。
+        :param SystemDisk.DiskSize: 系统盘内存大小，最小值为0，最大值为500
         :type PathPrefix: String
         :param DataDiskGb: 数据卷容量，单位GB，容量限制依据[实例套餐类型定义](https://docs.ksyun.com/documents/705)变化，如果调用时未指定，则为相应实例套餐类型最小值。InstanceType为通用型主机时，此参数不生效。
         :type PathPrefix: Int
         :param SubnetId: VPC环境下的子网ID，绑定到主网卡。
 标准UUID格式，形如`^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$`
         :type PathPrefix: String
         :param DataDisk: 数据盘（云盘）的类型，数据盘n的类型，n 的取值范围为 [1, 8]。只支持I2、I2联网增强、N1、N2、N3、S3和I3。DataDisk.n.Type与DataDisk.n.Size必须都填写才有效。
@@ -2405,18 +2452,22 @@
         :param AddressPurchaseTime: 弹性IP的购买时长，只有购买包年包月弹性IP时不可缺省。
         :type PathPrefix: Int
         :param AddressProjectId: 弹性IP项目的ID
         :type PathPrefix: String
         :param ModelName: 实例启动模版名称，不允许重复
 ModelTest001
         :type PathPrefix: String
+        :param SystemDisk.DiskType: 不能给默认值，不传默认按价格体系配置systemDisk属性中第一个创建
+        :type PathPrefix: String
+        :param SystemDisk.ResizeType: 扩容 offline 离线扩容| online 在线扩容
+        :type PathPrefix: String
         """
         self.ImageId = None
         self.InstanceType = None
-        self.SystemDisk = None
+        self.SystemDisk.DiskSize = None
         self.DataDiskGb = None
         self.SubnetId = None
         self.DataDisk = None
         self.KeepImageLogin = None
         self.KeyId = None
         self.ChargeType = None
         self.PurchaseTime = None
@@ -2429,22 +2480,24 @@
         self.DataGuardId = None
         self.AddressBandWidth = None
         self.LineId = None
         self.AddressChargeType = None
         self.AddressPurchaseTime = None
         self.AddressProjectId = None
         self.ModelName = None
+        self.SystemDisk.DiskType = None
+        self.SystemDisk.ResizeType = None
 
     def _deserialize(self, params):
         if params.get("ImageId"):
             self.ImageId = params.get("ImageId")
         if params.get("InstanceType"):
             self.InstanceType = params.get("InstanceType")
-        if params.get("SystemDisk"):
-            self.SystemDisk = params.get("SystemDisk")
+        if params.get("SystemDisk.DiskSize"):
+            self.SystemDisk.DiskSize = params.get("SystemDisk.DiskSize")
         if params.get("DataDiskGb"):
             self.DataDiskGb = params.get("DataDiskGb")
         if params.get("SubnetId"):
             self.SubnetId = params.get("SubnetId")
         if params.get("DataDisk"):
             self.DataDisk = params.get("DataDisk")
         if params.get("KeepImageLogin"):
@@ -2477,14 +2530,18 @@
             self.AddressChargeType = params.get("AddressChargeType")
         if params.get("AddressPurchaseTime"):
             self.AddressPurchaseTime = params.get("AddressPurchaseTime")
         if params.get("AddressProjectId"):
             self.AddressProjectId = params.get("AddressProjectId")
         if params.get("ModelName"):
             self.ModelName = params.get("ModelName")
+        if params.get("SystemDisk.DiskType"):
+            self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
+        if params.get("SystemDisk.ResizeType"):
+            self.SystemDisk.ResizeType = params.get("SystemDisk.ResizeType")
 
 
 class TerminateModelsRequest(AbstractModel):
     """TerminateModels请求参数结构体
     """
 
     def __init__(self):
@@ -2707,17 +2764,17 @@
         :type PathPrefix: Boolean
         :param KeyId: 密钥对 
  
         :type PathPrefix: Filter
         :param DataDisk: 云盘数据盘类型 
  
         :type PathPrefix: Filter
-        :param SystemDisk: 系统盘类型 
+        :param SystemDisk.DiskSize: 系统盘大小，最小值为0，最大值为500
  
-        :type PathPrefix: Filter
+        :type PathPrefix: Int
         :param AddressBandWidth: 弹性IP的带宽 
  
         :type PathPrefix: Int
         :param BandWidthShareId: 弹性IP指定的共享带宽ID 
  
         :type PathPrefix: String
         :param LineId: 弹性IP的链路类型的ID 
@@ -2743,39 +2800,45 @@
         :type PathPrefix: Filter
         :param LoginSetAfter: 
         :type PathPrefix: Boolean
         :param IpBindAfter: 
         :type PathPrefix: Boolean
         :param InstanceNameRandom: 实例名称随机生成
         :type PathPrefix: Boolean
+        :param SystemDisk.DiskType: 不能给默认值，不传默认按价格体系配置systemDisk属性中第一个创建
+        :type PathPrefix: String
+        :param SystemDisk.ResizeType: 扩容 offline 离线扩容| online 在线扩容
+        :type PathPrefix: String
         """
         self.ScalingConfigurationId = None
         self.ScalingConfigurationName = None
         self.ImageId = None
         self.Password = None
         self.InstanceType = None
         self.ChargeType = None
         self.DataDiskGb = None
         self.ProjectId = None
         self.KeepImageLogin = None
         self.KeyId = None
         self.DataDisk = None
-        self.SystemDisk = None
+        self.SystemDisk.DiskSize = None
         self.AddressBandWidth = None
         self.BandWidthShareId = None
         self.LineId = None
         self.AddressProjectId = None
         self.InstanceName = None
         self.InstanceNameSuffix = None
         self.UserData = None
         self.InstanceNameTimeSuffix = None
         self.Tag = None
         self.LoginSetAfter = None
         self.IpBindAfter = None
         self.InstanceNameRandom = None
+        self.SystemDisk.DiskType = None
+        self.SystemDisk.ResizeType = None
 
     def _deserialize(self, params):
         if params.get("ScalingConfigurationId"):
             self.ScalingConfigurationId = params.get("ScalingConfigurationId")
         if params.get("ScalingConfigurationName"):
             self.ScalingConfigurationName = params.get("ScalingConfigurationName")
         if params.get("ImageId"):
@@ -2792,16 +2855,16 @@
             self.ProjectId = params.get("ProjectId")
         if params.get("KeepImageLogin"):
             self.KeepImageLogin = params.get("KeepImageLogin")
         if params.get("KeyId"):
             self.KeyId = params.get("KeyId")
         if params.get("DataDisk"):
             self.DataDisk = params.get("DataDisk")
-        if params.get("SystemDisk"):
-            self.SystemDisk = params.get("SystemDisk")
+        if params.get("SystemDisk.DiskSize"):
+            self.SystemDisk.DiskSize = params.get("SystemDisk.DiskSize")
         if params.get("AddressBandWidth"):
             self.AddressBandWidth = params.get("AddressBandWidth")
         if params.get("BandWidthShareId"):
             self.BandWidthShareId = params.get("BandWidthShareId")
         if params.get("LineId"):
             self.LineId = params.get("LineId")
         if params.get("AddressProjectId"):
@@ -2818,14 +2881,18 @@
             self.Tag = params.get("Tag")
         if params.get("LoginSetAfter"):
             self.LoginSetAfter = params.get("LoginSetAfter")
         if params.get("IpBindAfter"):
             self.IpBindAfter = params.get("IpBindAfter")
         if params.get("InstanceNameRandom"):
             self.InstanceNameRandom = params.get("InstanceNameRandom")
+        if params.get("SystemDisk.DiskType"):
+            self.SystemDisk.DiskType = params.get("SystemDisk.DiskType")
+        if params.get("SystemDisk.ResizeType"):
+            self.SystemDisk.ResizeType = params.get("SystemDisk.ResizeType")
 
 
 class DescribeSpotPriceHistoryRequest(AbstractModel):
     """DescribeSpotPriceHistory请求参数结构体
     """
 
     def __init__(self):
@@ -2994,60 +3061,71 @@
         self.InstanceId = None
 
     def _deserialize(self, params):
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
 
 
-class DescribeInstanceKmrRequest(AbstractModel):
-    """DescribeInstanceKmr请求参数结构体
+class PreMigrateInstanceRequest(AbstractModel):
+    """PreMigrateInstance请求参数结构体
     """
 
     def __init__(self):
-        r"""DescribeInstanceKmr
-        """
-
-    def _deserialize(self, params):
-        return
-
+        r"""创建预迁移
+        :param InstanceId: 实例id
+        :type PathPrefix: String
+        :param InstanceType: 目标实例类型
+        :type PathPrefix: String
+        :param SystemDiskType: 云盘系统盘的类型。
 
-class ValidatedDiskEncryptRequest(AbstractModel):
-    """ValidatedDiskEncrypt请求参数结构体
-    """
+有效值：SSD3.0，EHDD
+        :type PathPrefix: String
+        :param DataDiskType: 云盘数据盘的类型。
 
-    def __init__(self):
-        r"""ValidatedDiskEncrypt
-        :param AccountId: 用户id
+有效值：SSD3.0，EHDD
         :type PathPrefix: String
         """
-        self.AccountId = None
+        self.InstanceId = None
+        self.InstanceType = None
+        self.SystemDiskType = None
+        self.DataDiskType = None
 
     def _deserialize(self, params):
-        if params.get("AccountId"):
-            self.AccountId = params.get("AccountId")
+        if params.get("InstanceId"):
+            self.InstanceId = params.get("InstanceId")
+        if params.get("InstanceType"):
+            self.InstanceType = params.get("InstanceType")
+        if params.get("SystemDiskType"):
+            self.SystemDiskType = params.get("SystemDiskType")
+        if params.get("DataDiskType"):
+            self.DataDiskType = params.get("DataDiskType")
 
 
-class DistributeKmsPermissionRequest(AbstractModel):
-    """DistributeKmsPermission请求参数结构体
+class CancelPreMigrateInstanceRequest(AbstractModel):
+    """CancelPreMigrateInstance请求参数结构体
     """
 
     def __init__(self):
-        r"""DistributeKmsPermission
+        r"""取消预迁移
+        :param InstanceId: 实例id
+        :type PathPrefix: String
         """
+        self.InstanceId = None
 
     def _deserialize(self, params):
-        return
+        if params.get("InstanceId"):
+            self.InstanceId = params.get("InstanceId")
 
 
-class DescribeEntrySnapshotsRequest(AbstractModel):
-    """DescribeEntrySnapshots请求参数结构体
+class DescribeInstanceKmrRequest(AbstractModel):
+    """DescribeInstanceKmr请求参数结构体
     """
 
     def __init__(self):
-        r"""DescribeEntrySnapshots
+        r"""DescribeInstanceKmr
         """
 
     def _deserialize(self, params):
         return
 
 
 class DescribeMinFlavorCountRequest(AbstractModel):
```

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/abstract_client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/abstract_model.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/common_client.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/credential.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/exception/__init__.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/http/request.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/profile/client_profile.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/profile/http_profile.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/ksyun/common/sign.py` & `kingsoftcloud-sdk-python-1.1.0/ksyun/common/sign.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.0.3/setup.py` & `kingsoftcloud-sdk-python-1.1.0/setup.py`

 * *Files identical despite different names*

