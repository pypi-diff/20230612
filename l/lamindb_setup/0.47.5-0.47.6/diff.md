# Comparing `tmp/lamindb_setup-0.47.5.tar.gz` & `tmp/lamindb_setup-0.47.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.47.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.47.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.47.5.tar` & `lamindb_setup-0.47.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.5/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.5/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.5/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.5/README.md
--rw-r--r--   0        0        0    54372 2023-06-12 16:17:32.140039 lamindb_setup-0.47.5/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.5/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.5/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.5/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.5/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.5/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.5/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.5/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.5/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.5/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.5/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.5/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.5/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.5/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.5/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.5/lamin-project.yaml
--rw-r--r--   0        0        0     2715 2023-06-12 16:17:24.241651 lamindb_setup-0.47.5/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.5/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.5/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.5/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.5/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.5/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.5/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6835 2023-06-11 19:14:24.008674 lamindb_setup-0.47.5/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.5/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.47.5/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.5/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.5/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.5/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.5/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.5/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.5/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.5/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.5/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.5/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.5/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.5/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.5/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     7711 2023-06-12 16:16:41.585610 lamindb_setup-0.47.5/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.5/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     9331 2023-06-11 19:14:24.009365 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2224 2023-06-11 19:14:24.009694 lamindb_setup-0.47.5/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.5/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.47.5/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2670 2023-06-08 17:51:53.349359 lamindb_setup-0.47.5/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      815 2023-06-12 10:24:01.838397 lamindb_setup-0.47.5/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.5/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.5/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.5/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.5/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    27017 2023-06-12 10:24:01.838867 lamindb_setup-0.47.5/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.5/lnschema-core/LICENSE
--rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.5/lnschema-core/README.md
--rw-r--r--   0        0        0      608 2023-06-12 10:24:01.839439 lamindb_setup-0.47.5/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.5/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.5/lnschema-core/lnschema_core/_queryset.py
--rw-r--r--   0        0        0     2952 2023-06-12 10:24:01.840105 lamindb_setup-0.47.5/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    15423 2023-06-12 16:08:55.620766 lamindb_setup-0.47.5/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.5/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    22202 2023-06-12 10:24:01.840552 lamindb_setup-0.47.5/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.5/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.5/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      184 2023-06-12 10:24:01.840993 lamindb_setup-0.47.5/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.5/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.5/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-11 19:14:24.010612 lamindb_setup-0.47.5/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.5/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.5/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.47.5/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.5/tests/test_login.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.5/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.5/tests/test_signup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.5/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.6/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.6/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.6/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.6/README.md
+-rw-r--r--   0        0        0    54530 2023-06-12 20:35:01.136062 lamindb_setup-0.47.6/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.6/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.6/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.6/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.6/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.6/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.6/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.6/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.6/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.6/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.6/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.6/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.6/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.6/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.6/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.6/lamin-project.yaml
+-rw-r--r--   0        0        0     2715 2023-06-12 20:34:39.904011 lamindb_setup-0.47.6/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.6/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.6/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.6/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.6/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.6/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.6/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6835 2023-06-11 19:14:24.008674 lamindb_setup-0.47.6/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.6/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.47.6/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.6/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.6/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.6/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.6/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.6/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.6/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.6/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.6/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.6/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.6/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.6/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.6/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     9986 2023-06-12 20:33:20.803923 lamindb_setup-0.47.6/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.6/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     9331 2023-06-11 19:14:24.009365 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2370 2023-06-12 19:19:26.360494 lamindb_setup-0.47.6/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.6/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.47.6/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2670 2023-06-08 17:51:53.349359 lamindb_setup-0.47.6/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      815 2023-06-12 10:24:01.838397 lamindb_setup-0.47.6/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.6/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.6/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.6/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.6/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    27342 2023-06-12 19:29:46.148924 lamindb_setup-0.47.6/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.6/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.6/lnschema-core/README.md
+-rw-r--r--   0        0        0      608 2023-06-12 19:29:46.149107 lamindb_setup-0.47.6/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.6/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.6/lnschema-core/lnschema_core/_queryset.py
+-rw-r--r--   0        0        0     1644 2023-06-12 19:29:46.149255 lamindb_setup-0.47.6/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    12754 2023-06-12 19:29:46.149559 lamindb_setup-0.47.6/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.6/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    20627 2023-06-12 19:29:46.149767 lamindb_setup-0.47.6/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.6/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.6/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      184 2023-06-12 10:24:01.840993 lamindb_setup-0.47.6/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.6/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.6/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-11 19:14:24.010612 lamindb_setup-0.47.6/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.6/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.6/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.47.6/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.6/tests/test_login.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.6/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.6/tests/test_signup.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.6/PKG-INFO
```

### Comparing `lamindb_setup-0.47.5/.github/workflows/build.yml` & `lamindb_setup-0.47.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/.gitignore` & `lamindb_setup-0.47.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/.pre-commit-config.yaml` & `lamindb_setup-0.47.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/LICENSE` & `lamindb_setup-0.47.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/changelog.md` & `lamindb_setup-0.47.6/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Different migr strategy | [417](https://github.com/laminlabs/lamindb-setup/pull/417) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.6
 🍱 Added migration script from legacy instances | [416](https://github.com/laminlabs/lamindb-setup/pull/416) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.5
 🔥 Adapt locker to lock entire lamindb session | [415](https://github.com/laminlabs/lamindb-setup/pull/415) | [Koncopd](https://github.com/Koncopd) | 2023-06-11 |
 🚑 Only delete bionty sources when bionty is installed | [414](https://github.com/laminlabs/lamindb-setup/pull/414) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.4
 🚚 Rename source_key to source | [413](https://github.com/laminlabs/lamindb-setup/pull/413) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.3
 ⬆️ Rename bionty variables | [412](https://github.com/laminlabs/lamindb-setup/pull/412) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.2
 🚑 Removed `LAMINDB_INSTANCE_LOADED` env variable | [411](https://github.com/laminlabs/lamindb-setup/pull/411) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 | 0.47.1
 ⬆️ Adapt to bionty naming in 0.18.0 | [410](https://github.com/laminlabs/lamindb-setup/pull/410) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 |
```

### Comparing `lamindb_setup-0.47.5/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.47.6/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.47.6/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.47.6/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.47.6/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.47.6/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.47.6/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.47.6/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/docs/guide/setup-user.md` & `lamindb_setup-0.47.6/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/__init__.py` & `lamindb_setup-0.47.6/lamindb_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.47.5"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.47.6"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.47.5/lamindb_setup/__main__.py` & `lamindb_setup-0.47.6/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.47.6/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_close.py` & `lamindb_setup-0.47.6/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_delete.py` & `lamindb_setup-0.47.6/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_docstrings.py` & `lamindb_setup-0.47.6/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_init_instance.py` & `lamindb_setup-0.47.6/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_load_instance.py` & `lamindb_setup-0.47.6/lamindb_setup/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_notebook.py` & `lamindb_setup-0.47.6/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_register_instance.py` & `lamindb_setup-0.47.6/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_schema.py` & `lamindb_setup-0.47.6/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_set.py` & `lamindb_setup-0.47.6/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_settings.py` & `lamindb_setup-0.47.6/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_setup_user.py` & `lamindb_setup-0.47.6/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.47.6/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_django.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_django.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import builtins
 import os
-from pathlib import Path
-from typing import Dict
 
 from lamin_logger import logger
 
 from ._settings_instance import InstanceSettings
 
 IS_RUN_FROM_IPYTHON = getattr(builtins, "__IPYTHON__", False)
 IS_SETUP = False
@@ -19,32 +17,14 @@
     connection.prepare_database()
     executor = MigrationExecutor(connection)
     targets = executor.loader.graph.leaf_nodes()
     planned_migrations = [mig[0] for mig in executor.migration_plan(targets)]
     return planned_migrations
 
 
-def replace_content(filename: Path, mapped_content: Dict[str, str]) -> None:
-    with open(filename) as f:
-        content = f.read()
-    with open(filename, "w") as f:
-        for key, value in mapped_content.items():
-            content = content.replace(key, value)
-        f.write(content)
-
-
-def update_lnschema_core_migration(backward=False):
-    import lnschema_core
-
-    mapper = {"MANAGED = True": "MANAGED = False"}
-    if backward:
-        mapper = {"MANAGED = False": "MANAGED = True"}
-    replace_content(lnschema_core.__file__, mapper)
-
-
 def check_is_legacy_instance_and_fix(isettings) -> bool:
     import sqlalchemy as sa
 
     engine = sa.create_engine(isettings.db)
 
     # this checks whether its a legacy instance before lamindb 0.41.0
     try:
@@ -74,29 +54,44 @@
     if not user_table_exists and not django_table_exists:
         return False
     # the django table is there, it's a django instance
     if django_table_exists:
         return False
     # otherwise, it's a legacy instance: it has the user table but not the django table
 
+    datetime_str = "datetime" if isettings.dialect == "sqlite" else "timestamp"
+
     # now let's proceed
     stmts = [
-        "alter table lnschema_core_run add column run_at datetime",
+        f"alter table lnschema_core_run add column run_at {datetime_str}",
         "drop index if exists ix_core_run_transform_v",
         "drop index if exists ix_lnschema_core_run_transform_version",
+        "drop index if exists ix_lnschema_core_file_transform_version",
         "alter table lnschema_core_run drop column transform_version",
+        "alter table lnschema_core_file drop column transform_version",
         "alter table lnschema_core_project add column external_id varchar(40)",
         "alter table lnschema_core_transform rename column name to short_name",
         "alter table lnschema_core_transform rename column title to name",
         "alter table lnschema_core_runinput add column id bigint",
         "update lnschema_core_transform set name = short_name where name is null",
         "alter table lnschema_core_transform add column stem_id varchar(12)",
         "update lnschema_core_transform set stem_id = id",
         "alter table lnschema_core_features rename to lnschema_core_featureset",
-        "alter table lnschema_core_featureset add column updated_at datetime",
+        f"alter table lnschema_core_featureset add column updated_at {datetime_str}",
+        # now rename
+        "alter table lnschema_core_user rename to lnschema_core_legacy_user",
+        "alter table lnschema_core_storage rename to lnschema_core_legacy_storage",
+        "alter table lnschema_core_project rename to lnschema_core_legacy_project",
+        "alter table lnschema_core_transform rename to lnschema_core_legacy_transform",
+        "alter table lnschema_core_run rename to lnschema_core_legacy_run",
+        "alter table lnschema_core_featureset rename to"
+        " lnschema_core_legacy_featureset",
+        "alter table lnschema_core_folder rename to lnschema_core_legacy_folder",
+        "alter table lnschema_core_file rename to lnschema_core_legacy_file",
+        "alter table lnschema_core_runinput rename to lnschema_core_legacy_runinput",
     ]
     if "bionty" in isettings.schema:
         # fmt: off
         stmts += [
             "alter table lnschema_bionty_species rename to lnschema_bionty_legacy_species",  # noqa
             "alter table lnschema_bionty_gene rename to lnschema_bionty_legacy_gene",  # noqa
             "alter table lnschema_bionty_protein rename to lnschema_bionty_legacy_protein",  # noqa
@@ -112,27 +107,66 @@
         # fmt: on
     with engine.connect() as conn:
         for stmt in stmts:
             try:
                 conn.execute(sa.text(stmt))
             except Exception as e:
                 logger.warning(f"Failed to execute: {stmt} because of {e}")
-
-    update_lnschema_core_migration()
+    logger.success("Created legacy migration preparations")
     return True
 
 
+def insert_legacy_data(isettings: InstanceSettings):
+    import sqlalchemy as sa
+
+    stmts = []
+    if isettings.dialect != "sqlite":
+        # problem is this list is still incomplete, we'd need it for all columns
+        stmts = [
+            "alter table lnschema_core_user alter column created_at drop not null",  # noqa
+            "alter table lnschema_core_transform alter column created_at drop not null",  # noqa
+            "alter table lnschema_core_run alter column created_by_id drop not null",  # noqa
+            "alter table lnschema_core_file alter column updated_at drop not null",  # noqa
+        ]
+
+    engine = sa.create_engine(isettings.db)
+    stmts = [
+        "insert into lnschema_core_user select * from lnschema_core_legacy_user",
+        "insert into lnschema_core_storage select * from lnschema_core_legacy_storage",
+        "insert into lnschema_core_project select * from lnschema_core_legacy_project",
+        "insert into lnschema_core_transform select * from"
+        " lnschema_core_legacy_transform",
+        "insert into lnschema_core_run select * from lnschema_core_legacy_run",
+        "insert into lnschema_core_featureset select * from"
+        " lnschema_core_legacy_featureset",
+        "insert into lnschema_core_folder select * from lnschema_core_legacy_folder",
+        "insert into lnschema_core_file select * from lnschema_core_legacy_file",
+        "insert into lnschema_core_runinput select * from"
+        " lnschema_core_legacy_runinput",
+    ]
+    with engine.connect() as conn:
+        for stmt in stmts:
+            try:
+                conn.execute(sa.text(stmt))
+            except Exception as e:
+                logger.warning(f"Failed to execute: {stmt} because of {e}")
+
+
 def setup_django(
     isettings: InstanceSettings,
     deploy_migrations: bool = False,
     create_migrations: bool = False,
     init: bool = False,
 ):
     if IS_RUN_FROM_IPYTHON:
         os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
+
+    if deploy_migrations:
+        check_legacy = check_is_legacy_instance_and_fix(isettings)
+
     import dj_database_url
     import django
     from django.conf import settings
     from django.core.management import call_command
 
     default_db = dj_database_url.config(
         default=isettings.db,
@@ -159,32 +193,32 @@
             call_command("makemigrations")
             return None
 
         planned_migrations = get_migrations_to_sync()
         if len(planned_migrations) > 0:
             if deploy_migrations:
                 verbosity = 0 if init else 2
-                check = check_is_legacy_instance_and_fix(isettings)
                 call_command("migrate", verbosity=verbosity)
-                if check:
-                    update_lnschema_core_migration(backward=True)
+                if check_legacy:
+                    insert_legacy_data(isettings)
                 if not init:
                     # only update if called from lamin migrate deploy
                     # if called from load_schema(..., init=True)
                     # no need to update the remote sqlite
                     isettings._update_cloud_sqlite_file()
             else:
                 logger.warning(
                     "\n\nYour database is not up to date with your installed"
                     " schemas!\n\nIt misses the following"
                     f" migrations:\n{planned_migrations}\n\nIf you are an admin and"
                     " know what you're doing, deploy the migration:\nlamin migrate"
                     " deploy\n\nOtherwise, please install previouses release of the"
                     " above-mentioned schemas\n\nIn case you haven't yet migrated to"
                     " Django, please upgrade to lamindb 0.41.2 before deploying this"
-                    " migration\n"
+                    " migration - you'll need a manual step then, please reach out to"
+                    " Lamin\n"
                 )
         else:
             if deploy_migrations:
                 logger.info("Database already up-to-date with migrations!")
         global IS_SETUP
         IS_SETUP = True
```

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,23 @@
         from bionty.dev._handle_sources import (
             LAMINDB_SOURCES,
             parse_currently_used_sources,
         )
         from bionty.dev._io import write_yaml
         from lnschema_bionty.models import BiontySource
 
-        active_records = BiontySource.objects.filter(currently_used=True).all().values()
+        try:  # this is only to deal with legacy instances
+            active_records = (
+                BiontySource.objects.filter(currently_used=True).all().values()
+            )
 
-        write_yaml(parse_currently_used_sources(active_records), LAMINDB_SOURCES)
-        logger.hint("Configured default bionty sources from BiontySource table")
+            write_yaml(parse_currently_used_sources(active_records), LAMINDB_SOURCES)
+            logger.hint("Configured default bionty sources from BiontySource table")
+        except Exception:
+            pass
 
 
 def delete_bionty_sources_yaml():
     """Delete LAMINDB_SOURCES_PATH in bionty."""
     try:
         from bionty.dev._handle_sources import LAMINDB_SOURCES
```

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lamindb_setup/dev/upath.py` & `lamindb_setup-0.47.6/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.47.6/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.6/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/.gitignore` & `lamindb_setup-0.47.6/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.47.6/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.47.6/lnschema-core/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🍱 Add migration process for legacy SA instances | [199](https://github.com/laminlabs/lnschema-core/pull/199) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.35.5
+♻️ Less customized IDs | [198](https://github.com/laminlabs/lnschema-core/pull/198) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 |
 ♻️ Move logic to lamindb | [197](https://github.com/laminlabs/lnschema-core/pull/197) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 |
 ✨ Delete storage in File.delete | [196](https://github.com/laminlabs/lnschema-core/pull/196) | [Koncopd](https://github.com/Koncopd) | 2023-06-12 |
 🚚 Rename Featureset to FeatureSet | [194](https://github.com/laminlabs/lnschema-core/pull/194) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.35.4
 ♻️ Move save logic here | [193](https://github.com/laminlabs/lnschema-core/pull/193) | [falexwolf](https://github.com/falexwolf) | 2023-06-10 | 0.35.3
 🔥 Remove unnecessary files | [192](https://github.com/laminlabs/lnschema-core/pull/192) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 | 0.35.2
 👷 Simplify CI & remove docs | [191](https://github.com/laminlabs/lnschema-core/pull/191) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 |
 🚸 Check for required fields | [190](https://github.com/laminlabs/lnschema-core/pull/190) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 | 0.35.1
```

### Comparing `lamindb_setup-0.47.5/lnschema-core/LICENSE` & `lamindb_setup-0.47.6/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.47.6/lnschema-core/lnschema_core/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Data objects & lineage (`yvzi`)."""
 _schema_id = "yvzi"
 _name = "core"
-__version__ = "0.35.4"
+__version__ = "0.35.5"
 
 # can directly import from lamindb_setup going forward
 from lamindb_setup._check_instance_setup import (
     check_instance_setup as _check_instance_setup,
 )
 
 _INSTANCE_SETUP = _check_instance_setup()
```

### Comparing `lamindb_setup-0.47.5/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.47.6/lnschema-core/lnschema_core/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/lnschema_core/_queryset.py` & `lamindb_setup-0.47.6/lnschema-core/lnschema_core/_queryset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.47.6/lnschema-core/lnschema_core/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Dict, Iterable, NamedTuple, Optional, Union, overload  # noqa
 
 from django.db import models
 from django.db.models import PROTECT, Manager
 from lamin_logger import colors, logger
 from upath import UPath
 
-from . import ids
 from ._lookup import lookup as _lookup
 from ._queryset import QuerySet
+from .ids import base62, base62_8, base62_12, base62_20
 from .types import DataLike, PathLike, TransformType
 from .users import current_user_id
 
 is_run_from_ipython = getattr(builtins, "__IPYTHON__", False)
 TRANSFORM_TYPE_DEFAULT = TransformType.notebook if is_run_from_ipython else TransformType.pipeline
 
 
@@ -109,61 +109,51 @@
     """Storage locations, typically cloud storage buckets.
 
     A file can be stored in S3 and GCP buckets or local storage locations.
 
     This ORM tracks these locations along with metadata.
     """
 
-    id = models.CharField(max_length=8, default=ids.storage, db_index=True, primary_key=True)
+    id = models.CharField(max_length=8, default=base62_8, db_index=True, primary_key=True)
     """Universal id, valid across DB instances."""
     root = models.CharField(max_length=255, db_index=True, default=None)
     """Path to the root of the storage location (an s3 path, a local path, etc.)."""
     type = models.CharField(max_length=30, db_index=True)
     """Local vs. s3 vs. gcp etc."""
     region = models.CharField(max_length=63, db_index=True, null=True, default=None)
     """Cloud storage region, if applicable."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
-    created_by = models.ForeignKey(
-        User,
-        PROTECT,
-        default=current_user_id,
-        related_name="created_storages",
-    )
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_storages")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
 
 
 class Project(BaseORM):
     """Projects."""
 
-    id = models.CharField(max_length=8, default=ids.project, primary_key=True)
+    id = models.CharField(max_length=8, default=base62_8, primary_key=True)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, unique=True, default=None)
     """Project name or title."""
-    external_id = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    external_id = models.CharField(max_length=40, db_index=True, null=True, default=None)
     """External id (such as from a project management tool)."""
     folders = models.ManyToManyField("Folder", related_name="projects")
     """Project folders."""
     files = models.ManyToManyField("File", related_name="projects")
     """Project files."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
-    created_by = models.ForeignKey(
-        User,
-        PROTECT,
-        default=current_user_id,
-        related_name="created_projects",
-    )
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_projects")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
 
 
 class Transform(BaseORM):
@@ -182,67 +172,57 @@
     """Universal id, composed of stem_id and version suffix."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Transform name or title, a pipeline name, notebook title, etc..
     """
     short_name = models.CharField(max_length=30, db_index=True, null=True, default=None)
     """A short name.
     """
-    stem_id = models.CharField(max_length=12, default=ids.transform, db_index=True)
+    stem_id = models.CharField(max_length=12, default=base62_12, db_index=True)
     """Stem of id, identifying transform up to version."""
     version = models.CharField(max_length=10, default="0", db_index=True)
     """Version, defaults to `"0"`.
 
     Use this to label different versions of the same pipeline, notebook, etc.
 
     Consider using `semantic versioning <https://semver.org>`__
     with `Python versioning <https://peps.python.org/pep-0440/>`__.
     """
-    type = models.CharField(
-        max_length=20,
-        choices=TransformType.choices(),
-        db_index=True,
-        default=TRANSFORM_TYPE_DEFAULT,
-    )
+    type = models.CharField(max_length=20, choices=TransformType.choices(), db_index=True, default=TRANSFORM_TYPE_DEFAULT)
     """Transform type.
 
     Defaults to `notebook` if run from ipython and to `pipeline` if run from python.
 
     If run from the app, it defaults to `app`.
     """
     reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Reference for the transform, e.g., a URL.
     """
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
-    created_by = models.ForeignKey(
-        User,
-        PROTECT,
-        default=current_user_id,
-        related_name="created_transforms",
-    )
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_transforms")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
         unique_together = (("stem_id", "version"),)
 
     def __init__(self, *args, **kwargs):
         if len(args) > 0:  # initialize with all fields from db as args
             super().__init__(*args, **kwargs)
             return None
         else:  # user-facing calling signature
             # set default ids
             if "id" not in kwargs and "stem_id" not in kwargs:
-                kwargs["id"] = ids.base62(n_char=14)
+                kwargs["id"] = base62(14)
                 kwargs["stem_id"] = kwargs["id"][:12]
             elif "stem_id" in kwargs:
                 assert isinstance(kwargs["stem_id"], str) and len(kwargs["stem_id"]) == 12
-                kwargs["id"] = kwargs["stem_id"] + ids.base62(n_char=2)
+                kwargs["id"] = kwargs["stem_id"] + base62(2)
             elif "id" in kwargs:
                 assert isinstance(kwargs["id"], str) and len(kwargs["id"]) == 14
                 kwargs["stem_id"] = kwargs["id"][:12]
             super().__init__(**kwargs)
 
 
 class Run(BaseORM):
@@ -255,15 +235,15 @@
       given `Run` can output multiple `files`: `run.outputs`.
     - References to inputs are stored in the `RunInput` ORM, a many-to-many link
       ORM between `File` and `Run`. Any `file` might serve as an input for
       multiple `runs`: `file.input_of`. Similarly, any `run` might have many
       `files` as inputs: `run.inputs`.
     """
 
-    id = models.CharField(max_length=20, default=ids.run, primary_key=True)
+    id = models.CharField(max_length=20, default=base62_20, primary_key=True)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Name or title of run."""
     external_id = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """External id (such as from a workflow tool)."""
     transform = models.ForeignKey(Transform, PROTECT, related_name="runs")
     """The transform :class:`~lamindb.Transform` that is being run."""
@@ -312,20 +292,15 @@
     """A feature entity type."""
     files = models.ManyToManyField("File", related_name="featuresets")
     """Files linked to the featureset."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
-    created_by = models.ForeignKey(
-        User,
-        PROTECT,
-        default=current_user_id,
-        related_name="created_featuresets",
-    )
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_featuresets")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
 
     @classmethod
     def from_iterable(
@@ -359,15 +334,15 @@
         super().save(*args, **kwargs)
         for key, records in self._relationships.items():
             [r.save() for r in records]
             getattr(self, key).set(records)
 
 
 class Folder(BaseORM):
-    id = models.CharField(max_length=20, default=ids.folder, primary_key=True)
+    id = models.CharField(max_length=20, primary_key=True)
     """A universal random id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, default=None)
     """Name or title of folder."""
     # below is one of the few cases with null=True, default=None
     key = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Storage key of folder."""
     storage = models.ForeignKey(Storage, PROTECT, related_name="folders", null=True)
@@ -401,69 +376,39 @@
         limit_to_directories: bool = False,
         length_limit: int = 1000,
     ) -> None:
         """Print a visual tree structure."""
         from lamindb._folder import tree
 
         return tree(
-            dir_path=self.path(),
+            self,
             level=level,
             limit_to_directories=limit_to_directories,
             length_limit=length_limit,
         )
 
-    def __init__(self, *args, **kwargs):  # type: ignore
-        if len(args) > 1 and isinstance(args[0], str) and len(args[0]) == 20:  # initialize with all fields from db as args
-            super().__init__(*args, **kwargs)
-            return None
-        else:  # user-facing calling signature
-            if len(args) != 1 and "files" not in kwargs:
-                raise ValueError("Either provide path as arg or provide files as kwarg!")
-            if len(args) == 1:
-                path: Optional[Union[Path, UPath, str]] = args[0]
-            else:
-                path = None
-            name: Optional[str] = kwargs.pop("name") if "name" in kwargs else None
-            key: Optional[str] = kwargs.pop("key") if "key" in kwargs else None
-            files: Optional[str] = kwargs.pop("files") if "files" in kwargs else None
-            if len(kwargs) != 0:
-                raise ValueError(f"These kwargs are not permitted: {kwargs}")
-
-        from lamindb._folder import get_folder_kwargs_from_data
-
-        if path is not None:
-            kwargs, privates = get_folder_kwargs_from_data(
-                path=path,
-                name=name,
-                key=key,
-            )
-            files = kwargs.pop("files")
-        else:
-            kwargs = dict(name=name)
-        kwargs["id"] = ids.folder()
-        super().__init__(**kwargs)
-        if path is not None:
-            self._local_filepath = privates["local_filepath"]
-            self._cloud_filepath = privates["cloud_filepath"]
-            self._files = files
+    def __init__(self, *args, **kwargs):
+        from lamindb._folder import init_folder
+
+        init_folder(self, *args, **kwargs)
 
     def save(self, *args, **kwargs) -> None:
         """Save the folder."""
         # only has attr _files if freshly initialized
         if hasattr(self, "_files"):
             for file in self._files:
                 file.save()
         super().save(*args, **kwargs)
         if hasattr(self, "_files"):
             self.files.set(self._files)
 
 
 class File(BaseORM):
     id = models.CharField(max_length=20, primary_key=True)
-    """A universal random id, valid across DB instances."""
+    """A universal random id (20-char base62), valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """A universal random id, valid across DB instances."""
     suffix = models.CharField(max_length=30, db_index=True, null=True, default=None)
     """File suffix.
 
     This is a file extension if the `file` is stored in a file format.
     It's `None` if the storage format doesn't have a canonical extension.
@@ -581,7 +526,8 @@
 
 class RunInput(BaseORM):
     run = models.ForeignKey("Run", on_delete=models.CASCADE)
     file = models.ForeignKey("File", on_delete=models.CASCADE)
 
     class Meta:
         managed = True
+        unique_together = ("run", "file")
```

### Comparing `lamindb_setup-0.47.5/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.47.6/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/lnschema-core/pyproject.toml` & `lamindb_setup-0.47.6/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/noxfile.py` & `lamindb_setup-0.47.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/pyproject.toml` & `lamindb_setup-0.47.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/tests/test_bionty.py` & `lamindb_setup-0.47.6/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/tests/test_init_instance.py` & `lamindb_setup-0.47.6/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/tests/test_load_instance.py` & `lamindb_setup-0.47.6/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.5/PKG-INFO` & `lamindb_setup-0.47.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.47.5
+Version: 0.47.6
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.10
 Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
```

