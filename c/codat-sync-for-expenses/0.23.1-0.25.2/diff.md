# Comparing `tmp/codat-sync-for-expenses-0.23.1.tar.gz` & `tmp/codat-sync-for-expenses-0.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.23.1.tar", last modified: Tue Jun  6 20:52:35 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.25.2.tar", last modified: Mon Jun 12 10:23:16 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.23.1.tar` & `codat-sync-for-expenses-0.25.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2573 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.369539 codat-sync-for-expenses-0.23.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4844 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2586 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5135 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1266 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1768 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5695 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5368 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/integrationtype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2722 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8485 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:16.011978 codat-sync-for-expenses-0.25.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-12 10:23:16.007978 codat-sync-for-expenses-0.25.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:23:16.011978 codat-sync-for-expenses-0.25.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.987977 codat-sync-for-expenses-0.25.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.991977 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 10:23:15.000000 codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.995977 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4934 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5225 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2555 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.995977 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:15.999977 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1028 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1158 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:16.007978 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3073 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5366 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4833 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/integrationtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      573 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8665 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4818 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:23:16.007978 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-12 10:22:59.000000 codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.23.1/PKG-INFO` & `codat-sync-for-expenses-0.25.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.23.1
+Version: 0.25.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -45,45 +45,45 @@
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### [configuration](docs/configuration/README.md)
+### [configuration](docs/sdks/configuration/README.md)
 
-* [get_company_configuration](docs/configuration/README.md#get_company_configuration) - Get company configuration
-* [save_company_configuration](docs/configuration/README.md#save_company_configuration) - Set company configuration
+* [get_company_configuration](docs/sdks/configuration/README.md#get_company_configuration) - Get company configuration
+* [save_company_configuration](docs/sdks/configuration/README.md#save_company_configuration) - Set company configuration
 
-### [connections](docs/connections/README.md)
+### [connections](docs/sdks/connections/README.md)
 
-* [create_partner_expense_connection](docs/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
+* [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
 
-### [expenses](docs/expenses/README.md)
+### [expenses](docs/sdks/expenses/README.md)
 
-* [create_expense_dataset](docs/expenses/README.md#create_expense_dataset) - Create expense-transactions
-* [upload_attachment](docs/expenses/README.md#upload_attachment) - Upload attachment
+* [create_expense_dataset](docs/sdks/expenses/README.md#create_expense_dataset) - Create expense-transactions
+* [upload_attachment](docs/sdks/expenses/README.md#upload_attachment) - Upload attachment
 
-### [mapping_options](docs/mappingoptions/README.md)
+### [mapping_options](docs/sdks/mappingoptions/README.md)
 
-* [get_mapping_options](docs/mappingoptions/README.md#get_mapping_options) - Mapping options
+* [get_mapping_options](docs/sdks/mappingoptions/README.md#get_mapping_options) - Mapping options
 
-### [sync](docs/sync/README.md)
+### [sync](docs/sdks/sync/README.md)
 
-* [intiate_sync](docs/sync/README.md#intiate_sync) - Initiate sync
+* [intiate_sync](docs/sdks/sync/README.md#intiate_sync) - Initiate sync
 
-### [sync_status](docs/syncstatus/README.md)
+### [sync_status](docs/sdks/syncstatus/README.md)
 
-* [get_last_successful_sync](docs/syncstatus/README.md#get_last_successful_sync) - Last successful sync
-* [get_latest_sync](docs/syncstatus/README.md#get_latest_sync) - Latest sync status
-* [get_sync_by_id](docs/syncstatus/README.md#get_sync_by_id) - Get Sync status
-* [list_syncs](docs/syncstatus/README.md#list_syncs) - List sync statuses
+* [get_last_successful_sync](docs/sdks/syncstatus/README.md#get_last_successful_sync) - Last successful sync
+* [get_latest_sync](docs/sdks/syncstatus/README.md#get_latest_sync) - Latest sync status
+* [get_sync_by_id](docs/sdks/syncstatus/README.md#get_sync_by_id) - Get Sync status
+* [list_syncs](docs/sdks/syncstatus/README.md#list_syncs) - List sync statuses
 
-### [transaction_status](docs/transactionstatus/README.md)
+### [transaction_status](docs/sdks/transactionstatus/README.md)
 
-* [get_sync_transaction](docs/transactionstatus/README.md#get_sync_transaction) - Get Sync Transaction
-* [list_sync_transactions](docs/transactionstatus/README.md#list_sync_transactions) - Get Sync transactions
+* [get_sync_transaction](docs/sdks/transactionstatus/README.md#get_sync_transaction) - Get Sync Transaction
+* [list_sync_transactions](docs/sdks/transactionstatus/README.md#list_sync_transactions) - Get Sync transactions
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-sync-for-expenses-0.23.1/README.md` & `codat-sync-for-expenses-0.25.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -33,43 +33,43 @@
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### [configuration](docs/configuration/README.md)
+### [configuration](docs/sdks/configuration/README.md)
 
-* [get_company_configuration](docs/configuration/README.md#get_company_configuration) - Get company configuration
-* [save_company_configuration](docs/configuration/README.md#save_company_configuration) - Set company configuration
+* [get_company_configuration](docs/sdks/configuration/README.md#get_company_configuration) - Get company configuration
+* [save_company_configuration](docs/sdks/configuration/README.md#save_company_configuration) - Set company configuration
 
-### [connections](docs/connections/README.md)
+### [connections](docs/sdks/connections/README.md)
 
-* [create_partner_expense_connection](docs/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
+* [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
 
-### [expenses](docs/expenses/README.md)
+### [expenses](docs/sdks/expenses/README.md)
 
-* [create_expense_dataset](docs/expenses/README.md#create_expense_dataset) - Create expense-transactions
-* [upload_attachment](docs/expenses/README.md#upload_attachment) - Upload attachment
+* [create_expense_dataset](docs/sdks/expenses/README.md#create_expense_dataset) - Create expense-transactions
+* [upload_attachment](docs/sdks/expenses/README.md#upload_attachment) - Upload attachment
 
-### [mapping_options](docs/mappingoptions/README.md)
+### [mapping_options](docs/sdks/mappingoptions/README.md)
 
-* [get_mapping_options](docs/mappingoptions/README.md#get_mapping_options) - Mapping options
+* [get_mapping_options](docs/sdks/mappingoptions/README.md#get_mapping_options) - Mapping options
 
-### [sync](docs/sync/README.md)
+### [sync](docs/sdks/sync/README.md)
 
-* [intiate_sync](docs/sync/README.md#intiate_sync) - Initiate sync
+* [intiate_sync](docs/sdks/sync/README.md#intiate_sync) - Initiate sync
 
-### [sync_status](docs/syncstatus/README.md)
+### [sync_status](docs/sdks/syncstatus/README.md)
 
-* [get_last_successful_sync](docs/syncstatus/README.md#get_last_successful_sync) - Last successful sync
-* [get_latest_sync](docs/syncstatus/README.md#get_latest_sync) - Latest sync status
-* [get_sync_by_id](docs/syncstatus/README.md#get_sync_by_id) - Get Sync status
-* [list_syncs](docs/syncstatus/README.md#list_syncs) - List sync statuses
+* [get_last_successful_sync](docs/sdks/syncstatus/README.md#get_last_successful_sync) - Last successful sync
+* [get_latest_sync](docs/sdks/syncstatus/README.md#get_latest_sync) - Latest sync status
+* [get_sync_by_id](docs/sdks/syncstatus/README.md#get_sync_by_id) - Get Sync status
+* [list_syncs](docs/sdks/syncstatus/README.md#list_syncs) - List sync statuses
 
-### [transaction_status](docs/transactionstatus/README.md)
+### [transaction_status](docs/sdks/transactionstatus/README.md)
 
-* [get_sync_transaction](docs/transactionstatus/README.md#get_sync_transaction) - Get Sync Transaction
-* [list_sync_transactions](docs/transactionstatus/README.md#list_sync_transactions) - Get Sync transactions
+* [get_sync_transaction](docs/sdks/transactionstatus/README.md#get_sync_transaction) - Get Sync Transaction
+* [list_sync_transactions](docs/sdks/transactionstatus/README.md#list_sync_transactions) - Get Sync transactions
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-sync-for-expenses-0.23.1/setup.py` & `codat-sync-for-expenses-0.25.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.23.1",
+    version="0.25.2",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.23.1
+Version: 0.25.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -45,45 +45,45 @@
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### [configuration](docs/configuration/README.md)
+### [configuration](docs/sdks/configuration/README.md)
 
-* [get_company_configuration](docs/configuration/README.md#get_company_configuration) - Get company configuration
-* [save_company_configuration](docs/configuration/README.md#save_company_configuration) - Set company configuration
+* [get_company_configuration](docs/sdks/configuration/README.md#get_company_configuration) - Get company configuration
+* [save_company_configuration](docs/sdks/configuration/README.md#save_company_configuration) - Set company configuration
 
-### [connections](docs/connections/README.md)
+### [connections](docs/sdks/connections/README.md)
 
-* [create_partner_expense_connection](docs/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
+* [create_partner_expense_connection](docs/sdks/connections/README.md#create_partner_expense_connection) - Create Partner Expense connection
 
-### [expenses](docs/expenses/README.md)
+### [expenses](docs/sdks/expenses/README.md)
 
-* [create_expense_dataset](docs/expenses/README.md#create_expense_dataset) - Create expense-transactions
-* [upload_attachment](docs/expenses/README.md#upload_attachment) - Upload attachment
+* [create_expense_dataset](docs/sdks/expenses/README.md#create_expense_dataset) - Create expense-transactions
+* [upload_attachment](docs/sdks/expenses/README.md#upload_attachment) - Upload attachment
 
-### [mapping_options](docs/mappingoptions/README.md)
+### [mapping_options](docs/sdks/mappingoptions/README.md)
 
-* [get_mapping_options](docs/mappingoptions/README.md#get_mapping_options) - Mapping options
+* [get_mapping_options](docs/sdks/mappingoptions/README.md#get_mapping_options) - Mapping options
 
-### [sync](docs/sync/README.md)
+### [sync](docs/sdks/sync/README.md)
 
-* [intiate_sync](docs/sync/README.md#intiate_sync) - Initiate sync
+* [intiate_sync](docs/sdks/sync/README.md#intiate_sync) - Initiate sync
 
-### [sync_status](docs/syncstatus/README.md)
+### [sync_status](docs/sdks/syncstatus/README.md)
 
-* [get_last_successful_sync](docs/syncstatus/README.md#get_last_successful_sync) - Last successful sync
-* [get_latest_sync](docs/syncstatus/README.md#get_latest_sync) - Latest sync status
-* [get_sync_by_id](docs/syncstatus/README.md#get_sync_by_id) - Get Sync status
-* [list_syncs](docs/syncstatus/README.md#list_syncs) - List sync statuses
+* [get_last_successful_sync](docs/sdks/syncstatus/README.md#get_last_successful_sync) - Last successful sync
+* [get_latest_sync](docs/sdks/syncstatus/README.md#get_latest_sync) - Latest sync status
+* [get_sync_by_id](docs/sdks/syncstatus/README.md#get_sync_by_id) - Get Sync status
+* [list_syncs](docs/sdks/syncstatus/README.md#list_syncs) - List sync statuses
 
-### [transaction_status](docs/transactionstatus/README.md)
+### [transaction_status](docs/sdks/transactionstatus/README.md)
 
-* [get_sync_transaction](docs/transactionstatus/README.md#get_sync_transaction) - Get Sync Transaction
-* [list_sync_transactions](docs/transactionstatus/README.md#list_sync_transactions) - Get Sync transactions
+* [get_sync_transaction](docs/sdks/transactionstatus/README.md#get_sync_transaction) - Get Sync Transaction
+* [list_sync_transactions](docs/sdks/transactionstatus/README.md#list_sync_transactions) - Get Sync transactions
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.25.2/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Gets a companies expense sync configuration
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
@@ -64,15 +64,15 @@
         
         url = utils.generate_url(operations.SaveCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "company_configuration", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Creates a Partner Expense data connection
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.CreatePartnerExpenseConnectionRequest, base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/expenses.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         
         url = utils.generate_url(operations.CreateExpenseDatasetRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_expense_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
@@ -67,15 +67,15 @@
         
         url = utils.generate_url(operations.UploadAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/mapping_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Gets the expense mapping options for a companies accounting software
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 import requests as requests_http
 from ..shared import createexpenserequest as shared_createexpenserequest
 from ..shared import createexpenseresponse as shared_createexpenseresponse
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class CreateExpenseDatasetRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     create_expense_request: Optional[shared_createexpenserequest.CreateExpenseRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
+
+
+
 @dataclasses.dataclass
 class CreateExpenseDatasetResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     create_expense_response: Optional[shared_createexpenseresponse.CreateExpenseResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""The request made is not valid."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import dataconnection as shared_dataconnection
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class CreatePartnerExpenseConnectionRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
 class CreatePartnerExpenseConnectionResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     data_connection: Optional[shared_dataconnection.DataConnection] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""The request made is not valid."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 import dataclasses
 import requests as requests_http
 from ..shared import companyconfiguration as shared_companyconfiguration
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
-class GetCompanyConfigurationRequest:
-    
+class SaveCompanyConfigurationRequest:
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+    company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
+
+
+
 @dataclasses.dataclass
-class GetCompanyConfigurationResponse:
-    
+class SaveCompanyConfigurationResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
-    r"""Your API request was not properly authorized."""
-    
+    r"""The request made is not valid."""
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import companysyncstatus as shared_companysyncstatus
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class GetLastSuccessfulSyncRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
 class GetLastSuccessfulSyncResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""Your API request was not properly authorized."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import companysyncstatus as shared_companysyncstatus
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class GetLatestSyncRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
 class GetLatestSyncResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""Your API request was not properly authorized."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import mappingoptions as shared_mappingoptions
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class GetMappingOptionsRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
 class GetMappingOptionsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     mapping_options: Optional[shared_mappingoptions.MappingOptions] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""Your API request was not properly authorized."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 import dataclasses
 import requests as requests_http
 from ..shared import companysyncstatus as shared_companysyncstatus
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class GetSyncByIDRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a sync."""
     
 
+
+
+
 @dataclasses.dataclass
 class GetSyncByIDResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""Your API request was not properly authorized."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 import dataclasses
 import requests as requests_http
 from ..shared import schema as shared_schema
 from ..shared import transactionmetadata as shared_transactionmetadata
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class GetSyncTransactionRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a sync."""
     transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transactionId', 'style': 'simple', 'explode': False }})
     r"""The unique identifier for your SMB's transaction."""
     
 
+
+
+
 @dataclasses.dataclass
 class GetSyncTransactionResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""Your API request was not properly authorized."""
     transaction_metadata: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None)
     r"""Success"""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 import requests as requests_http
 from ..shared import codaterrormessage as shared_codaterrormessage
 from ..shared import postsync as shared_postsync
 from ..shared import syncinitiated as shared_syncinitiated
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class IntiateSyncRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     post_sync: Optional[shared_postsync.PostSync] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
+
+
+
 @dataclasses.dataclass
 class IntiateSyncResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     codat_error_message: Optional[shared_codaterrormessage.CodatErrorMessage] = dataclasses.field(default=None)
     r"""If model is incorrect"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     sync_initiated: Optional[shared_syncinitiated.SyncInitiated] = dataclasses.field(default=None)
     r"""Returns the newly created SyncId"""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 import dataclasses
 import requests as requests_http
 from ..shared import schema as shared_schema
 from ..shared import transactionmetadatalist as shared_transactionmetadatalist
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class ListSyncTransactionsRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a sync."""
     page: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
     
 
+
+
+
 @dataclasses.dataclass
 class ListSyncTransactionsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""Your API request was not properly authorized."""
     transaction_metadata_list: Optional[shared_transactionmetadatalist.TransactionMetadataList] = dataclasses.field(default=None)
     r"""Success"""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import companysyncstatus as shared_companysyncstatus
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class ListSyncsRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
+
+
+
 @dataclasses.dataclass
 class ListSyncsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_sync_statuses: Optional[list[shared_companysyncstatus.CompanySyncStatus]] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""Your API request was not properly authorized."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import companyconfiguration as shared_companyconfiguration
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
-class SaveCompanyConfigurationRequest:
-    
+class GetCompanyConfigurationRequest:
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
+
+
+
 @dataclasses.dataclass
-class SaveCompanyConfigurationResponse:
-    
+class GetCompanyConfigurationResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
-    r"""The request made is not valid."""
-    
+    r"""Your API request was not properly authorized."""
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,41 @@
 import dataclasses
 import requests as requests_http
 from ..shared import attachment as shared_attachment
 from ..shared import schema as shared_schema
 from typing import Optional
 
 
+
 @dataclasses.dataclass
 class UploadAttachmentRequestBody:
-    
     content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})
     request_body: str = dataclasses.field(metadata={'multipart_form': { 'field_name': 'requestBody' }})
     
 
+
+
+
 @dataclasses.dataclass
 class UploadAttachmentRequest:
-    
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
     r"""Unique identifier for a sync."""
     transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transactionId', 'style': 'simple', 'explode': False }})
     r"""The unique identifier for your SMB's transaction."""
     request_body: Optional[UploadAttachmentRequestBody] = dataclasses.field(default=None, metadata={'multipart_form': { 'file': True }, 'request': { 'media_type': 'multipart/form-data' }})
     
 
+
+
+
 @dataclasses.dataclass
 class UploadAttachmentResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     attachment: Optional[shared_attachment.Attachment] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
     r"""The request made is not valid."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     TRANSFER_IN = 'TransferIn'
     TRANSFER_OUT = 'TransferOut'
     ADJUSTMENT_IN = 'AdjustmentIn'
     ADJUSTMENT_OUT = 'AdjustmentOut'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class AccountMappingInfo:
-    
     account_type: Optional[AccountMappingInfoAccountType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
     r"""Type of the account."""
     currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
     r"""Currency of the account."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of account."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Name of the account as it appears in the companies accounting software."""
     valid_transaction_types: Optional[list[AccountMappingInfoValidTransactionTypes]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
     r"""Supported transaction types for the account."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class Attachment:
     r"""OK"""
-    
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
     r"""Unique ID of company in Codat"""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of attachment"""
     transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of transaction"""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class BankAccount:
-    
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""The id of the account from which purchases are made"""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,62 +4,71 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CodatErrorMessageValidationErrors:
-    
     item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
     validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
     
 
+
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CodatErrorMessageValidationInternals:
-    
     item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
     validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
     
 
+
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CodatErrorMessageValidationWarnings:
-    
     item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
     validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
     
 
+
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CodatErrorMessageValidation:
-    
     errors: Optional[list[CodatErrorMessageValidationErrors]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
     has_errors: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasErrors'), 'exclude': lambda f: f is None }})
     has_internals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasInternals'), 'exclude': lambda f: f is None }})
     has_warnings: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasWarnings'), 'exclude': lambda f: f is None }})
     internals: Optional[list[CodatErrorMessageValidationInternals]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('internals'), 'exclude': lambda f: f is None }})
     warnings: Optional[list[CodatErrorMessageValidationWarnings]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warnings'), 'exclude': lambda f: f is None }})
     
 
+
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CodatErrorMessage:
     r"""If model is incorrect"""
-    
     can_be_retried: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('canBeRetried'), 'exclude': lambda f: f is None }})
     correlation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('correlationId'), 'exclude': lambda f: f is None }})
     detailed_error_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailedErrorCode'), 'exclude': lambda f: f is None }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     inner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inner'), 'exclude': lambda f: f is None }})
     service: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service'), 'exclude': lambda f: f is None }})
     status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
     validation: Optional[CodatErrorMessageValidation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from ..shared import customer as shared_customer
 from ..shared import supplier as shared_supplier
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CompanyConfiguration:
     r"""Success"""
-    
     bank_account: shared_bankaccount.BankAccount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccount') }})
     customer: shared_customer.Customer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})
     supplier: shared_supplier.Supplier = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplier') }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CompanySyncStatus:
     r"""Success"""
-    
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
     r"""Unique identifier for your SMB in Codat."""
     data_pushed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataPushed'), 'exclude': lambda f: f is None }})
     r"""Boolean of whether the sync resulted in data being pushed."""
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
     r"""Error message of the sync."""
     sync_exception_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncExceptionMessage'), 'exclude': lambda f: f is None }})
@@ -43,8 +43,9 @@
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from ..shared import expensetransaction as shared_expensetransaction
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CreateExpenseRequest:
-    
     items: Optional[list[shared_expensetransaction.ExpenseTransaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items'), 'exclude': lambda f: f is None }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class CreateExpenseResponse:
     r"""OK"""
-    
     dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetId'), 'exclude': lambda f: f is None }})
     r"""Unique id of dataset created"""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class Customer:
-    
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""id of the customer for all income related activities to be associated to."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     BANKING = 'Banking'
     COMMERCE = 'Commerce'
     OTHER = 'Other'
     UNKNOWN = 'Unknown'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class DataConnection:
     r"""A connection represents the link between a `company` and a source of data."""
-    
     created: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created') }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -78,8 +78,9 @@
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class DataConnectionError:
-    
     errored_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('erroredOnUtc'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -31,8 +31,9 @@
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
     status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
     status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     TRANSFER_IN = 'TransferIn'
     TRANSFER_OUT = 'TransferOut'
     ADJUSTMENT_IN = 'AdjustmentIn'
     ADJUSTMENT_OUT = 'AdjustmentOut'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ExpenseTransaction:
-    
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
     r"""Currency the transaction was recorded in."""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     r"""Your unique identifier for the transaction."""
     issue_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issueDate') }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
@@ -78,8 +78,9 @@
     """
     lines: Optional[list[shared_expensetransactionline.ExpenseTransactionLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
     r"""Array of transaction lines."""
     merchant_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('merchantName'), 'exclude': lambda f: f is None }})
     r"""Name of the merchant where the purchase took place"""
     notes: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     r"""Any private, company notes about the transaction."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from ..shared import recordref as shared_recordref
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class ExpenseTransactionLine:
-    
     account_ref: shared_recordref.RecordRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef') }})
     net_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('netAmount') }})
     r"""Amount of the line, exclusive of tax."""
     tax_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount') }})
     r"""Amount of tax for the line."""
     tax_rate_ref: Optional[shared_recordref.RecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})
     tracking_refs: Optional[list[shared_recordref.RecordRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingRefs'), 'exclude': lambda f: f is None }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,12 +4,14 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class HalLink:
+class RecordRef:
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""identifier of linked reference from mapping options."""
     
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
-    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from ..shared import trackingcategorymappinginfo as shared_trackingcategorymappinginfo
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class MappingOptions:
     r"""Success"""
-    
     accounts: Optional[list[shared_accountmappinginfo.AccountMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
     r"""Array of available accounts for mapping."""
     expense_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expenseProvider'), 'exclude': lambda f: f is None }})
     r"""Name of the expense integration."""
     tax_rates: Optional[list[shared_taxratemappinginfo.TaxRateMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
     r"""Array of available tax rates for mapping."""
     tracking_categories: Optional[list[shared_trackingcategorymappinginfo.TrackingCategoryMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingCategories'), 'exclude': lambda f: f is None }})
     r"""Array of available tracking categories for mapping."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,12 +4,13 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class PostSync:
-    
     dataset_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetIds'), 'exclude': lambda f: f is None }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class RecordRef:
-    
+class Supplier:
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""identifier of linked reference from mapping options."""
-    
+    r"""id of the supplier for all purchases to be associated to"""
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/schema.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class Schema:
     r"""Your API request was not properly authorized."""
-    
     can_be_retried: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('canBeRetried'), 'exclude': lambda f: f is None }})
     correlation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('correlationId'), 'exclude': lambda f: f is None }})
     detailed_error_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailedErrorCode'), 'exclude': lambda f: f is None }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     service: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service'), 'exclude': lambda f: f is None }})
     status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
-class Supplier:
+class SyncInitiated:
+    r"""Returns the newly created SyncId"""
+    sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncId'), 'exclude': lambda f: f is None }})
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""id of the supplier for all purchases to be associated to"""
-    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     TRANSFER_IN = 'TransferIn'
     TRANSFER_OUT = 'TransferOut'
     ADJUSTMENT_IN = 'AdjustmentIn'
     ADJUSTMENT_OUT = 'AdjustmentOut'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TaxRateMappingInfo:
-    
     code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
     r"""Code for the tax rate from the accounting platform."""
     effective_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('effectiveTaxRate'), 'exclude': lambda f: f is None }})
     r"""Effective tax rate."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of tax rate."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Name of the tax rate in the accounting platform."""
     total_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalTaxRate'), 'exclude': lambda f: f is None }})
     r"""Total (not compounded) sum of the components of a tax rate."""
     valid_transaction_types: Optional[list[TaxRateMappingInfoValidTransactionTypes]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
     r"""Supported transaction types for the account."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import dataclasses
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TrackingCategoryMappingInfo:
-    
     has_children: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasChildren'), 'exclude': lambda f: f is None }})
     r"""Boolean of whether the tracking category has child categories."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the tracking category."""
     modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
@@ -36,8 +36,9 @@
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Name of the tracking category as it appears in the accounting software."""
     parent_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentId'), 'exclude': lambda f: f is None }})
     r"""ID of the parent tracking category"""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from ..shared import transactionstatus as shared_transactionstatus
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TransactionMetadata:
-    
     integration_type: Optional[shared_integrationtype.IntegrationType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationType'), 'exclude': lambda f: f is None }})
     r"""Type of transaction that has been processed e.g. Expense or Bank Feed."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
     r"""Metadata such as validation errors or the resulting record created in the accounting software."""
     status: Optional[shared_transactionstatus.TransactionStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""Status of the transaction."""
     transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
     r"""Your unique idenfier of the transaction."""
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 from ..shared import transactionmetadata as shared_transactionmetadata
 from codatsyncexpenses import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TransactionMetadataListLinks:
-    
     current: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
     self_: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
     next: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
+
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
+
 @dataclasses.dataclass
 class TransactionMetadataList:
     r"""Success"""
-    
     links: TransactionMetadataListLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
     page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
     results: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
-    
+    
+
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdk.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sdkconfiguration.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sdkconfiguration.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 @dataclass
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
-    sdk_version: str = '0.23.1'
-    gen_version: str = '2.35.9'
+    openapi_doc_version: str = 'prealpha'
+    sdk_version: str = '0.25.2'
+    gen_version: str = '2.39.2'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         
         url = utils.generate_url(operations.IntiateSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "post_sync", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/sync_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Gets the status of the last successfull sync
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetLastSuccessfulSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/lastSuccessful/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
@@ -61,15 +61,15 @@
         Gets the latest sync status
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetLatestSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/latest/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
@@ -104,15 +104,15 @@
         Get the sync status for a specified sync
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetSyncByIDRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
@@ -147,15 +147,15 @@
         Gets a list of sync statuses
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.ListSyncsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/list/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/transaction_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Gets the status of a transaction for a sync
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
@@ -62,15 +62,15 @@
         """
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListSyncTransactionsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
         client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.25.2/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

