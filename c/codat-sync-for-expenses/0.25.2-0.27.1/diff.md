# Comparing `tmp/codat-sync-for-expenses-0.25.2.tar.gz` & `tmp/codat-sync-for-expenses-0.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.25.2.tar", last modified: Mon Jun 12 10:23:16 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.27.1.tar", last modified: Fri Jun 16 11:14:27 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.25.2.tar` & `codat-sync-for-expenses-0.27.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:16.011978 codat-sync-for-expenses-0.25.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-12 10:23:16.007978 codat-sync-for-expenses-0.25.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:23:16.011978 codat-sync-for-expenses-0.25.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.987977 codat-sync-for-expenses-0.25.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.991977 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.995977 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4934 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5225 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2555 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.995977 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.999977 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:16.007978 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3073 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5366 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4833 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/integrationtype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      573 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8665 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4818 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:16.007978 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.982173 codat-sync-for-expenses-0.27.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.982173 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 11:14:27.000000 codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.986173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4840 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5131 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.986173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.986173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3073 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5366 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4833 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/integrationtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      573 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8477 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4724 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:14:27.990173 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-16 11:14:18.000000 codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.25.2/PKG-INFO` & `codat-sync-for-expenses-0.27.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.25.2
+Version: 0.27.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.25.2/README.md` & `codat-sync-for-expenses-0.27.1/README.md`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/setup.py` & `codat-sync-for-expenses-0.27.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.25.2",
+    version="0.27.1",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.25.2
+Version: 0.27.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.27.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -70,17 +68,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('POST', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('POST', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/expenses.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('POST', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -73,17 +71,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('POST', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/mapping_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/schema.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdk.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdkconfiguration.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sdkconfiguration.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = 'prealpha'
-    sdk_version: str = '0.25.2'
-    gen_version: str = '2.39.2'
+    sdk_version: str = '0.27.1'
+    gen_version: str = '2.41.1'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,17 +27,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('POST', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/sync_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -67,17 +65,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -110,17 +106,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -153,17 +147,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/transaction_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
@@ -68,17 +66,15 @@
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
-            retry_config = utils.RetryConfig('backoff', True)
-            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
-            
+            retry_config = utils.RetryConfig('backoff', utils.BackoffStrategy(500, 60000, 1.5, 3600000), True)
 
         def do_request():
             return client.request('GET', url, params=query_params, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/retries.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 
 class RetryConfig:
     strategy: str
     backoff: BackoffStrategy
     retry_connection_errors: bool
 
-    def __init__(self, strategy: str, retry_connection_errors: bool):
+    def __init__(self, strategy: str, backoff: BackoffStrategy, retry_connection_errors: bool):
         self.strategy = strategy
+        self.backoff = backoff
         self.retry_connection_errors = retry_connection_errors
 
 
 class Retries:
     config: RetryConfig
     status_codes: list[str]
```

### Comparing `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.27.1/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

