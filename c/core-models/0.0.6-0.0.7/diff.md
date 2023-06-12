# Comparing `tmp/core_models-0.0.6.tar.gz` & `tmp/core_models-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_models-0.0.6.tar", last modified: Tue May 30 07:33:15 2023, max compression
+gzip compressed data, was "core_models-0.0.7.tar", last modified: Mon Jun 12 00:07:41 2023, max compression
```

## Comparing `core_models-0.0.6.tar` & `core_models-0.0.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.225239 core_models-0.0.6/
--rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.0.6/LICENSE
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-30 07:33:15.224995 core_models-0.0.6/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.0.6/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.211621 core_models-0.0.6/core_models/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.0.6/core_models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.0.6/core_models/api_response.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.214136 core_models-0.0.6/core_models/app/
--rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.0.6/core_models/app/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     9351 2023-05-22 22:44:46.000000 core_models-0.0.6/core_models/app/admin.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.0.6/core_models/app/apps.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.0.6/core_models/app/context_processors.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.214807 core_models-0.0.6/core_models/app/managers/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.0.6/core_models/app/managers/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2844 2023-05-01 17:47:00.000000 core_models-0.0.6/core_models/app/managers/notification_manager.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.218076 core_models-0.0.6/core_models/app/migrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.0.6/core_models/app/migrations/0001_initial.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.0.6/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.0.6/core_models/app/migrations/0003_alter_user_onboarding_stage.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.0.6/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.0.6/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.0.6/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.0.6/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.0.6/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.0.6/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.0.6/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.0.6/core_models/app/migrations/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.222520 core_models-0.0.6/core_models/app/models/
--rw-r--r--   0 macbookpro   (501) staff       (20)      365 2023-04-28 12:03:37.000000 core_models-0.0.6/core_models/app/models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.0.6/core_models/app/models/bank_account.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.0.6/core_models/app/models/base.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2215 2023-05-29 15:03:18.000000 core_models-0.0.6/core_models/app/models/company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.0.6/core_models/app/models/configuration.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.0.6/core_models/app/models/contract.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.0.6/core_models/app/models/currency.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3288 2023-05-29 08:01:56.000000 core_models-0.0.6/core_models/app/models/invoice.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.0.6/core_models/app/models/notification.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.0.6/core_models/app/models/transaction.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.0.6/core_models/app/models/user.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.223396 core_models-0.0.6/core_models/app/templates/
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.224427 core_models-0.0.6/core_models/app/templates/core_models/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.0.6/core_models/app/templates/core_models/mail-base.html
--rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.0.6/core_models/app/templates/core_models/mail-base.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.0.6/core_models/app/templates/invoice.html
--rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.0.6/core_models/app/templates/reset.html
--rw-r--r--   0 macbookpro   (501) staff       (20)     3022 2023-05-11 22:07:09.000000 core_models-0.0.6/core_models/base_views.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2691 2023-05-29 08:22:45.000000 core_models-0.0.6/core_models/constants.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.0.6/core_models/settings.example.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     7485 2023-05-29 08:46:47.000000 core_models-0.0.6/core_models/settings.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.0.6/core_models/utils.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-30 07:33:15.212808 core_models-0.0.6/core_models.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-30 07:33:15.000000 core_models-0.0.6/core_models.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     1979 2023-05-30 07:33:15.000000 core_models-0.0.6/core_models.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-05-30 07:33:15.000000 core_models-0.0.6/core_models.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      176 2023-05-30 07:33:15.000000 core_models-0.0.6/core_models.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-05-30 07:33:15.000000 core_models-0.0.6/core_models.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.0.6/pyproject.toml
--rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-05-30 07:33:15.225304 core_models-0.0.6/setup.cfg
--rw-r--r--   0 macbookpro   (501) staff       (20)     1213 2023-05-30 07:32:41.000000 core_models-0.0.6/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.891526 core_models-0.0.7/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.0.7/LICENSE
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-06-12 00:07:41.891289 core_models-0.0.7/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.0.7/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.878723 core_models-0.0.7/core_models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.0.7/core_models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.0.7/core_models/api_response.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.880928 core_models-0.0.7/core_models/app/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.0.7/core_models/app/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     9351 2023-05-22 22:44:46.000000 core_models-0.0.7/core_models/app/admin.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.0.7/core_models/app/apps.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.0.7/core_models/app/context_processors.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.881493 core_models-0.0.7/core_models/app/managers/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.0.7/core_models/app/managers/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6142 2023-06-11 23:14:32.000000 core_models-0.0.7/core_models/app/managers/notification_manager.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.884167 core_models-0.0.7/core_models/app/migrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.0.7/core_models/app/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.0.7/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.0.7/core_models/app/migrations/0003_alter_user_onboarding_stage.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.0.7/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.0.7/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.0.7/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.0.7/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.0.7/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.0.7/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.0.7/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.0.7/core_models/app/migrations/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.889079 core_models-0.0.7/core_models/app/models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      365 2023-04-28 12:03:37.000000 core_models-0.0.7/core_models/app/models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.0.7/core_models/app/models/bank_account.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.0.7/core_models/app/models/base.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2215 2023-05-29 15:03:18.000000 core_models-0.0.7/core_models/app/models/company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.0.7/core_models/app/models/configuration.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.0.7/core_models/app/models/contract.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.0.7/core_models/app/models/currency.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3649 2023-06-11 23:15:25.000000 core_models-0.0.7/core_models/app/models/invoice.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.0.7/core_models/app/models/notification.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.0.7/core_models/app/models/transaction.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.0.7/core_models/app/models/user.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.889945 core_models-0.0.7/core_models/app/templates/
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.890826 core_models-0.0.7/core_models/app/templates/core_models/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.0.7/core_models/app/templates/core_models/mail-base.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.0.7/core_models/app/templates/core_models/mail-base.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.0.7/core_models/app/templates/invoice.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.0.7/core_models/app/templates/reset.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3057 2023-06-11 23:29:40.000000 core_models-0.0.7/core_models/base_views.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3324 2023-06-11 21:08:48.000000 core_models-0.0.7/core_models/constants.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.0.7/core_models/settings.example.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     7516 2023-06-11 00:16:44.000000 core_models-0.0.7/core_models/settings.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.0.7/core_models/utils.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-12 00:07:41.879692 core_models-0.0.7/core_models.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-06-12 00:07:41.000000 core_models-0.0.7/core_models.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1979 2023-06-12 00:07:41.000000 core_models-0.0.7/core_models.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-06-12 00:07:41.000000 core_models-0.0.7/core_models.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      195 2023-06-12 00:07:41.000000 core_models-0.0.7/core_models.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-06-12 00:07:41.000000 core_models-0.0.7/core_models.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.0.7/pyproject.toml
+-rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-06-12 00:07:41.891586 core_models-0.0.7/setup.cfg
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1257 2023-06-11 22:40:18.000000 core_models-0.0.7/setup.py
```

### Comparing `core_models-0.0.6/LICENSE` & `core_models-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/README.md` & `core_models-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/api_response.py` & `core_models-0.0.7/core_models/api_response.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/admin.py` & `core_models-0.0.7/core_models/app/admin.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0001_initial.py` & `core_models-0.0.7/core_models/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py` & `core_models-0.0.7/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py` & `core_models-0.0.7/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py` & `core_models-0.0.7/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py` & `core_models-0.0.7/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py` & `core_models-0.0.7/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py` & `core_models-0.0.7/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py` & `core_models-0.0.7/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py` & `core_models-0.0.7/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/models/base.py` & `core_models-0.0.7/core_models/app/models/base.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/models/company.py` & `core_models-0.0.7/core_models/app/models/company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/models/configuration.py` & `core_models-0.0.7/core_models/app/models/configuration.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/models/contract.py` & `core_models-0.0.7/core_models/app/models/contract.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/models/currency.py` & `core_models-0.0.7/core_models/app/models/currency.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/models/invoice.py` & `core_models-0.0.7/core_models/app/models/invoice.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from django.contrib.postgres.search import SearchVectorField
 from django.db import models
 from django.utils import timezone
+from model_utils import FieldTracker
+
 from core_models import constants
-from core_models.app.models import User, Currency
+from core_models.app.models import User, Currency, Notification
 from .base import BaseModelAbstract
+from .. import NotificationManager
 
 
 class Invoice(BaseModelAbstract, models.Model):
     seller = models.ForeignKey(User, models.SET_NULL, null=True, blank=True, related_name='sent_invoices')
     buyer = models.ForeignKey(User, models.SET_NULL, null=True, blank=True, related_name='received_invoices')
     financier = models.ForeignKey(User, models.SET_NULL, null=True, blank=True, related_name='funded_invoices')
     currency = models.ForeignKey(Currency, models.SET_NULL, null=True, blank=True)
@@ -28,25 +32,30 @@
     interest = models.DecimalField(decimal_places=2, max_digits=30)
     liquify_fee = models.DecimalField(decimal_places=2, max_digits=30, default=0)
     buyer_amount = models.DecimalField(decimal_places=2, max_digits=30, default=0)
     seller_amount = models.DecimalField(decimal_places=2, max_digits=30, default=0)
     financier_amount = models.DecimalField(decimal_places=2, max_digits=30, default=0)
     metadata = models.JSONField(null=True, blank=True)
 
+    tracker = FieldTracker(fields=['status'])
+
     def save(self, keep_deleted=False, **kwargs):
         if not self.reference:
             now = timezone.now()
             self.reference = f"LQIN{now.strftime('%Y%m%d%H%M%S')}"
         if self.base_rate and self.seller_risk_percentage and self.buyer_risk_percentage:
             self.interest_rate = sum([self.base_rate, self.seller_risk_percentage, self.buyer_risk_percentage])
             self.interest = round(self.total * self.interest_rate, 2)
             self.buyer_amount = self.total
             self.financier_amount = self.total - self.interest
             self.seller_amount = self.financier_amount - self.liquify_fee
+        status_changed = self.tracker.has_changed('status') or not self.id
         super(Invoice, self).save(keep_deleted, **kwargs)
+        if status_changed:
+            NotificationManager.save_invoice_notification(self)
 
     def __unicode__(self):
         return self.reference
 
 
 class InvoiceItem(BaseModelAbstract, models.Model):
     invoice = models.ForeignKey(Invoice, models.CASCADE, related_name="items")
```

### Comparing `core_models-0.0.6/core_models/app/models/transaction.py` & `core_models-0.0.7/core_models/app/models/transaction.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/models/user.py` & `core_models-0.0.7/core_models/app/models/user.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/templates/core_models/mail-base.html` & `core_models-0.0.7/core_models/app/templates/core_models/mail-base.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/templates/core_models/mail-base.txt` & `core_models-0.0.7/core_models/app/templates/core_models/mail-base.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/templates/invoice.html` & `core_models-0.0.7/core_models/app/templates/invoice.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/app/templates/reset.html` & `core_models-0.0.7/core_models/app/templates/reset.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/base_views.py` & `core_models-0.0.7/core_models/base_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-import asyncio
-
 from django.http import Http404
-from django.utils.decorators import classonlymethod
 
 from core_models.api_response import SuccessApiResponse, \
     ServerErrorApiResponse, FailureApiResponse
 from core_models.utils import log_exception
 from rest_framework.exceptions import NotFound, ValidationError
 from rest_framework.generics import ListAPIView, CreateAPIView, UpdateAPIView
 
 
 class BaseListAPIView(ListAPIView):
+
+    def extra_data(self) -> dict:
+        return {}
+
     def list(self, request, *args, **kwargs):
         try:
             response = super(BaseListAPIView, self).list(
                 request, *args, **kwargs)
+            data = {**response.data, **self.extra_data()}
             return SuccessApiResponse(
                 "success",
-                response.data
+                data
             )
         except NotFound:
             return FailureApiResponse("Page not found")
         except Exception as ex:
             log_exception(type(self).__name__, ex)
         return ServerErrorApiResponse()
```

### Comparing `core_models-0.0.6/core_models/constants.py` & `core_models-0.0.7/core_models/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,26 +23,28 @@
 COMPLETED_INVOICE_STATUS = "C"
 CLOSED_INVOICE_STATUS = "X"
 FUNDED_INVOICE_STATUS = "F"
 REJECTED_INVOICE_STATUS = "R"
 WITHDRAWN_INVOICE_STATUS = "W"
 AMEND_INVOICE_STATUS = "A"
 AWAITING_PAYMENT_INVOICE_STATUS = "AP"
+OVERDUE_INVOICE_STATUS = "O"
 
 INVOICE_STATUSES = (
     (DRAFT_INVOICE_STATUS, "Draft"),
     (NEW_INVOICE_STATUS, "New"),
     (VALIDATED_INVOICE_STATUS, "Validated"),
     (COMPLETED_INVOICE_STATUS, "Repaid"),
     (CLOSED_INVOICE_STATUS, "Closed"),
     (FUNDED_INVOICE_STATUS, "Funded"),
     (REJECTED_INVOICE_STATUS, "Rejected"),
     (WITHDRAWN_INVOICE_STATUS, "Withdrawn"),
     (AMEND_INVOICE_STATUS, "For Amendment"),
     (AWAITING_PAYMENT_INVOICE_STATUS, "Awaiting Payment"),
+    (OVERDUE_INVOICE_STATUS, "Overdue"),
 )
 
 FAILED_TXN_STATUS = "F"
 SUCCESS_TXN_STATUS = "S"
 PENDING_TXN_STATUS = "P"
 REVERSED_TXN_STATUS = "R"
 
@@ -78,19 +80,32 @@
 DASHBOARD_CONTRACT_ACCEPTANCE = "D"
 CONTRACT_ACCEPTANCE_CHANNELS = (
     (PHONE_CONTRACT_ACCEPTANCE, "Phone"),
     (MAIL_CONTRACT_ACCEPTANCE, "Mail"),
     (DASHBOARD_CONTRACT_ACCEPTANCE, "Dashboard"),
 )
 
+NEW_INVOICE_NOTIF_TYPE = 'NI'
+INVOICE_WITHDRAWN_NOTIF_TYPE = 'IW'
 INVOICE_REPAID_NOTIF_TYPE = 'IR'
 INVOICE_FUNDED_NOTIF_TYPE = 'IF'
+INVOICE_AWAITING_PAYMENT_NOTIF_TYPE = 'IA'
 INVOICE_VALIDATED_NOTIF_TYPE = 'IV'
+INVOICE_OVERDUE_NOTIF_TYPE = 'IO'
+INVOICE_REJECTED_NOTIF_TYPE = 'IX'
+AMEND_INVOICE_NOTIF_TYPE = 'MI'
 CONTRACT_CONFIRMED_NOTIF_TYPE = 'CC'
 MODIFY_CONTRACT_NOTIF_TYPE = 'CM'
+NEW_CONTRACT_NOTIF_TYPE = 'NC'
 NOTIFICATION_TYPES = (
+    (NEW_INVOICE_NOTIF_TYPE, 'New Invoice'),
+    (INVOICE_WITHDRAWN_NOTIF_TYPE, 'Invoice Withdrawn'),
     (INVOICE_REPAID_NOTIF_TYPE, 'Invoice Repaid'),
     (INVOICE_FUNDED_NOTIF_TYPE, 'Invoice Funded'),
+    (INVOICE_OVERDUE_NOTIF_TYPE, 'Invoice Overdue'),
+    (AMEND_INVOICE_NOTIF_TYPE, 'Amend Invoice'),
+    (INVOICE_AWAITING_PAYMENT_NOTIF_TYPE, 'Invoice Awaiting Payment'),
     (INVOICE_VALIDATED_NOTIF_TYPE, 'Invoice Validated'),
     (CONTRACT_CONFIRMED_NOTIF_TYPE, 'Contract Confirmed'),
     (MODIFY_CONTRACT_NOTIF_TYPE, 'Modify Contract'),
+    (NEW_CONTRACT_NOTIF_TYPE, 'New Contract'),
 )
```

### Comparing `core_models-0.0.6/core_models/settings.example.py` & `core_models-0.0.7/core_models/settings.example.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models/settings.py` & `core_models-0.0.7/core_models/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 CORE_APPS = [
     'storages',
     'cities_light',
     'django_slack',
     'core_models',
     'core_models.app',
+    'django.contrib.postgres',
 ]
 
 
 def db(key):
     return os.getenv(key)
```

### Comparing `core_models-0.0.6/core_models/utils.py` & `core_models-0.0.7/core_models/utils.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/core_models.egg-info/SOURCES.txt` & `core_models-0.0.7/core_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.0.6/setup.py` & `core_models-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Liquify core package'
 LONG_DESCRIPTION = 'Package that holds all models and core ' \
                    'functions/classes of Liquify project'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
@@ -15,15 +15,16 @@
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     package_data={'': ['app/templates/core_models/*']},
     include_package_data=True,
     install_requires=["django", "python-dotenv", "django-safedelete", "redis", 'django-environ',
                       "onesignal-sdk", "django-cities-light", 'daphne', 'psycopg2-binary',
-                      "django-slack", "uvicorn", "django-storages", "boto3", 'dj-database-url'],
+                      "django-slack", "uvicorn", "django-storages", "boto3", 'dj-database-url',
+                      'django-model-utils'],
     # add any
     # additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'liquify'],
     classifiers=[
         "Programming Language :: Python :: 3",
```

