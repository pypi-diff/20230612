# Comparing `tmp/lamindb_setup-0.47.4.tar.gz` & `tmp/lamindb_setup-0.47.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.47.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.47.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.47.4.tar` & `lamindb_setup-0.47.5.tar`

### file list

```diff
@@ -1,91 +1,85 @@
--rw-r--r--   0        0        0     4010 2023-06-05 07:30:18.302219 lamindb_setup-0.47.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-06-01 15:58:18.274054 lamindb_setup-0.47.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-06-01 15:58:18.274134 lamindb_setup-0.47.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-06-01 15:58:18.274221 lamindb_setup-0.47.4/.gitignore
--rw-r--r--   0        0        0      100 2023-06-01 15:58:18.274299 lamindb_setup-0.47.4/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-05 07:30:18.302425 lamindb_setup-0.47.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-06-01 15:58:18.274545 lamindb_setup-0.47.4/LICENSE
--rw-r--r--   0        0        0      318 2023-06-05 07:30:18.302530 lamindb_setup-0.47.4/README.md
--rw-r--r--   0        0        0    54030 2023-06-10 19:43:58.322358 lamindb_setup-0.47.4/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-05 07:30:18.302966 lamindb_setup-0.47.4/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-05 07:30:18.303105 lamindb_setup-0.47.4/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 15:58:18.275949 lamindb_setup-0.47.4/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 16:09:22.842055 lamindb_setup-0.47.4/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 13:53:23.373767 lamindb_setup-0.47.4/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4362 2023-06-08 13:53:23.373956 lamindb_setup-0.47.4/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-08 13:53:23.374226 lamindb_setup-0.47.4/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     3293 2023-06-10 10:42:49.132865 lamindb_setup-0.47.4/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 18:13:52.871462 lamindb_setup-0.47.4/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 18:13:52.872258 lamindb_setup-0.47.4/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 13:53:23.374760 lamindb_setup-0.47.4/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 13:53:23.374929 lamindb_setup-0.47.4/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 13:53:23.375035 lamindb_setup-0.47.4/docs/reference.md
--rw-r--r--   0        0        0      365 2023-06-01 15:58:18.277034 lamindb_setup-0.47.4/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:57:01.647274 lamindb_setup-0.47.4/lamin-project.yaml
--rw-r--r--   0        0        0     2715 2023-06-10 19:43:44.432746 lamindb_setup-0.47.4/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-07 20:38:59.482711 lamindb_setup-0.47.4/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:41.044617 lamindb_setup-0.47.4/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      661 2023-06-09 20:32:18.168808 lamindb_setup-0.47.4/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 16:09:22.843059 lamindb_setup-0.47.4/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-05 07:30:18.304343 lamindb_setup-0.47.4/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-01 15:58:18.277912 lamindb_setup-0.47.4/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6835 2023-06-10 18:56:23.117926 lamindb_setup-0.47.4/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     5411 2023-06-09 20:04:14.225151 lamindb_setup-0.47.4/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      322 2023-06-05 07:30:18.304745 lamindb_setup-0.47.4/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:25:55.266155 lamindb_setup-0.47.4/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-05 07:30:18.304849 lamindb_setup-0.47.4/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-05 07:30:18.305060 lamindb_setup-0.47.4/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1891 2023-06-07 20:38:59.483389 lamindb_setup-0.47.4/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-01 15:58:18.279311 lamindb_setup-0.47.4/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 15:58:18.279395 lamindb_setup-0.47.4/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 15:58:18.279466 lamindb_setup-0.47.4/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-05 07:30:18.305347 lamindb_setup-0.47.4/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-05 07:30:18.305424 lamindb_setup-0.47.4/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-01 15:58:18.279648 lamindb_setup-0.47.4/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5385 2023-06-07 16:33:24.023221 lamindb_setup-0.47.4/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 15:58:18.279932 lamindb_setup-0.47.4/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     2905 2023-06-08 18:13:52.872904 lamindb_setup-0.47.4/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 15:58:18.280089 lamindb_setup-0.47.4/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     9315 2023-06-08 18:13:52.873426 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 15:58:18.280386 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 15:58:18.280470 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-05 07:30:18.305825 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 15:58:18.280631 lamindb_setup-0.47.4/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2224 2023-06-10 19:43:06.748471 lamindb_setup-0.47.4/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:41.044990 lamindb_setup-0.47.4/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5057 2023-06-05 07:30:18.306219 lamindb_setup-0.47.4/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2670 2023-06-08 18:13:52.874452 lamindb_setup-0.47.4/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0     2811 2023-06-05 11:32:22.995643 lamindb_setup-0.47.4/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-06-05 11:32:22.995738 lamindb_setup-0.47.4/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-06-05 11:32:22.995812 lamindb_setup-0.47.4/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-06-05 11:32:22.995890 lamindb_setup-0.47.4/lnschema-core/.gitignore
--rw-r--r--   0        0        0        0 2023-06-05 11:32:22.995916 lamindb_setup-0.47.4/lnschema-core/.gitmodules
--rw-r--r--   0        0        0     1836 2023-06-05 11:32:22.996008 lamindb_setup-0.47.4/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-06-05 11:32:22.996105 lamindb_setup-0.47.4/lnschema-core/LICENSE
--rw-r--r--   0        0        0      364 2023-06-05 11:32:22.996173 lamindb_setup-0.47.4/lnschema-core/README.md
--rw-r--r--   0        0        0    25740 2023-06-05 11:32:22.996389 lamindb_setup-0.47.4/lnschema-core/docs/changelog.md
--rw-r--r--   0        0        0     1485 2023-06-05 11:32:22.996551 lamindb_setup-0.47.4/lnschema-core/docs/guide/core-schema.ipynb
--rw-r--r--   0        0        0       52 2023-06-05 11:32:22.996748 lamindb_setup-0.47.4/lnschema-core/docs/guide/index.md
--rw-r--r--   0        0        0      112 2023-06-05 11:32:22.996845 lamindb_setup-0.47.4/lnschema-core/docs/index.md
--rw-r--r--   0        0        0      202 2023-06-05 11:32:22.996914 lamindb_setup-0.47.4/lnschema-core/lamin-project.yaml
--rw-r--r--   0        0        0      592 2023-06-05 11:32:22.997066 lamindb_setup-0.47.4/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1515 2023-06-05 11:32:22.997223 lamindb_setup-0.47.4/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0      756 2023-06-05 11:32:22.997329 lamindb_setup-0.47.4/lnschema-core/lnschema_core/_types.py
--rw-r--r--   0        0        0      349 2023-06-05 11:32:22.997395 lamindb_setup-0.47.4/lnschema-core/lnschema_core/_users.py
--rw-r--r--   0        0        0     2810 2023-06-05 11:32:22.997546 lamindb_setup-0.47.4/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11504 2023-06-05 11:32:22.997705 lamindb_setup-0.47.4/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-05 11:32:22.997742 lamindb_setup-0.47.4/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    24760 2023-06-05 11:32:22.997959 lamindb_setup-0.47.4/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      180 2023-06-05 11:32:22.998145 lamindb_setup-0.47.4/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0     1299 2023-06-05 11:32:22.998461 lamindb_setup-0.47.4/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-05 11:32:22.998642 lamindb_setup-0.47.4/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      475 2023-06-05 11:32:22.998792 lamindb_setup-0.47.4/lnschema-core/tests/test_notebooks.py
--rw-r--r--   0        0        0     1911 2023-06-07 16:33:24.024562 lamindb_setup-0.47.4/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-10 19:26:14.501478 lamindb_setup-0.47.4/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-05 07:30:18.308956 lamindb_setup-0.47.4/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 15:58:18.282108 lamindb_setup-0.47.4/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 15:58:18.282187 lamindb_setup-0.47.4/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 13:53:23.375191 lamindb_setup-0.47.4/tests/test_login.py
--rw-r--r--   0        0        0      243 2023-06-01 15:58:18.282270 lamindb_setup-0.47.4/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 13:53:23.375328 lamindb_setup-0.47.4/tests/test_signup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.4/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.5/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.5/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.5/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.5/README.md
+-rw-r--r--   0        0        0    54372 2023-06-12 16:17:32.140039 lamindb_setup-0.47.5/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.5/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.5/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.5/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.5/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.5/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.5/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.5/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.5/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.5/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.5/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.5/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.5/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.5/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.5/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.5/lamin-project.yaml
+-rw-r--r--   0        0        0     2715 2023-06-12 16:17:24.241651 lamindb_setup-0.47.5/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.5/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.5/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.5/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.5/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.5/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.5/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6835 2023-06-11 19:14:24.008674 lamindb_setup-0.47.5/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.5/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.47.5/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.5/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.5/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.5/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.5/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.5/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.5/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.5/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.5/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.5/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.5/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.5/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.5/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     7711 2023-06-12 16:16:41.585610 lamindb_setup-0.47.5/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.5/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     9331 2023-06-11 19:14:24.009365 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.5/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2224 2023-06-11 19:14:24.009694 lamindb_setup-0.47.5/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.5/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.47.5/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2670 2023-06-08 17:51:53.349359 lamindb_setup-0.47.5/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      815 2023-06-12 10:24:01.838397 lamindb_setup-0.47.5/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.5/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.5/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.5/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.5/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    27017 2023-06-12 10:24:01.838867 lamindb_setup-0.47.5/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.5/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.5/lnschema-core/README.md
+-rw-r--r--   0        0        0      608 2023-06-12 10:24:01.839439 lamindb_setup-0.47.5/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.5/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.5/lnschema-core/lnschema_core/_queryset.py
+-rw-r--r--   0        0        0     2952 2023-06-12 10:24:01.840105 lamindb_setup-0.47.5/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    15423 2023-06-12 16:08:55.620766 lamindb_setup-0.47.5/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.5/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    22202 2023-06-12 10:24:01.840552 lamindb_setup-0.47.5/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.5/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.5/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      184 2023-06-12 10:24:01.840993 lamindb_setup-0.47.5/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.5/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.5/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-11 19:14:24.010612 lamindb_setup-0.47.5/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.5/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.5/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.47.5/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.5/tests/test_login.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.5/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.5/tests/test_signup.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.5/PKG-INFO
```

### Comparing `lamindb_setup-0.47.4/.github/workflows/build.yml` & `lamindb_setup-0.47.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/.gitignore` & `lamindb_setup-0.47.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/.pre-commit-config.yaml` & `lamindb_setup-0.47.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/LICENSE` & `lamindb_setup-0.47.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/changelog.md` & `lamindb_setup-0.47.5/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🍱 Added migration script from legacy instances | [416](https://github.com/laminlabs/lamindb-setup/pull/416) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.5
+🔥 Adapt locker to lock entire lamindb session | [415](https://github.com/laminlabs/lamindb-setup/pull/415) | [Koncopd](https://github.com/Koncopd) | 2023-06-11 |
 🚑 Only delete bionty sources when bionty is installed | [414](https://github.com/laminlabs/lamindb-setup/pull/414) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.4
 🚚 Rename source_key to source | [413](https://github.com/laminlabs/lamindb-setup/pull/413) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.3
 ⬆️ Rename bionty variables | [412](https://github.com/laminlabs/lamindb-setup/pull/412) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.2
 🚑 Removed `LAMINDB_INSTANCE_LOADED` env variable | [411](https://github.com/laminlabs/lamindb-setup/pull/411) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 | 0.47.1
 ⬆️ Adapt to bionty naming in 0.18.0 | [410](https://github.com/laminlabs/lamindb-setup/pull/410) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 |
 🚸 Warn about migrations | [409](https://github.com/laminlabs/lamindb-setup/pull/409) | [falexwolf](https://github.com/falexwolf) | 2023-06-08 | 0.47.0
 📝 Refactor guide | [408](https://github.com/laminlabs/lamindb-setup/pull/408) | [falexwolf](https://github.com/falexwolf) | 2023-06-08 |
```

### Comparing `lamindb_setup-0.47.4/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.47.5/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.47.5/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.47.5/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.47.5/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.47.5/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.47.5/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.47.5/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/docs/guide/setup-user.md` & `lamindb_setup-0.47.5/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/__init__.py` & `lamindb_setup-0.47.5/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.47.4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.47.5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.47.4/lamindb_setup/__main__.py` & `lamindb_setup-0.47.5/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.47.5/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_close.py` & `lamindb_setup-0.47.5/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_delete.py` & `lamindb_setup-0.47.5/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_docstrings.py` & `lamindb_setup-0.47.5/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_init_instance.py` & `lamindb_setup-0.47.5/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_load_instance.py` & `lamindb_setup-0.47.5/lamindb_setup/_load_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,19 @@
         else:
             logger.warning(
                 "Instance metadata exists, but DB might have been corrupted or deleted."
                 " Re-initializing the DB."
             )
             return "instance-not-reachable"
 
+    # at this point the lock should be already initialized
+    if not isettings._cloud_sqlite_locker.has_lock:
+        locked_by = isettings._cloud_sqlite_locker._locked_by
+        raise RuntimeError(f"Can't load the instance, it is locked by {locked_by}.")
+
     # need to set up Django here because we query the storage table
     setup_django(isettings)
     if storage is not None and isettings.dialect == "sqlite":
         update_root_field_in_default_storage(isettings)
     load_from_isettings(isettings)
     return None
```

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_notebook.py` & `lamindb_setup-0.47.5/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_register_instance.py` & `lamindb_setup-0.47.5/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_schema.py` & `lamindb_setup-0.47.5/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_set.py` & `lamindb_setup-0.47.5/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_settings.py` & `lamindb_setup-0.47.5/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_setup_user.py` & `lamindb_setup-0.47.5/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.47.5/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,44 +3,46 @@
 from typing import Optional, Union
 
 import fsspec
 from dateutil.parser import isoparse  # type: ignore
 from lamin_logger import logger
 
 from ._settings_instance import InstanceSettings
-from .upath import UPath
-from .upath import infer_filesystem as _infer_filesystem
+from .upath import UPath, infer_filesystem
 
-EXPIRATION_TIME = 1800  # 30 min
+EXPIRATION_TIME = 3600  # 60 min
 
-MAX_MSG_COUNTER = 1000  # print the msg after this number of iterations
+MAX_MSG_COUNTER = 100  # print the msg after this number of iterations
 
 
 class empty_locker:
+    has_lock = True
+
     @classmethod
     def lock(cls):
         pass
 
     @classmethod
     def unlock(cls):
         pass
 
 
 class Locker:
-    def __init__(self, user_id: str, storage_root: Union[UPath, Path]):
-        logger.debug(f"Init cloud sqlite locker: {user_id}, {storage_root}.")
+    def __init__(self, user_id: str, storage_root: Union[UPath, Path], name: str):
+        logger.debug(f"Init cloud sqlite locker: {user_id}, {storage_root}, {name}.")
 
         self._counter = 0
 
         self.user = user_id
+        self.name = name
 
         self.root = storage_root
-        self.fs, _ = _infer_filesystem(storage_root)
+        self.fs, _ = infer_filesystem(storage_root)
 
-        exclusion_path = storage_root / "exclusion"
+        exclusion_path = storage_root / f"exclusion/{name}"
         self.mapper = fsspec.FSMap(str(exclusion_path), self.fs, create=True)
 
         priorities_path = str(exclusion_path / "priorities")
         if self.fs.exists(priorities_path):
             self.users = self.mapper["priorities"].decode().split("*")
 
             if self.user not in self.users:
@@ -69,17 +71,22 @@
                 user_path = str(exclusion_path / user_endpoint)
                 if not self.fs.exists(user_path):
                     continue
                 if self.mapper[user_endpoint] == b"0":
                     continue
                 period = (datetime.now() - self.modified(user_path)).total_seconds()
                 if period > EXPIRATION_TIME:
+                    logger.info(
+                        f"The lock of the user {user} seems to be stale, clearing"
+                        f" {endpoint}."
+                    )
                     self.mapper[user_endpoint] = b"0"
 
-        self._locked = False
+        self._has_lock = None
+        self._locked_by = None
 
     def modified(self, path):
         if "gcs" not in self.fs.protocol:
             mtime = self.fs.modified(path)
         else:
             stat = self.fs.stat(path)
             if "updated" in stat:
@@ -91,82 +98,95 @@
         # assume in utc if the time zone is not specified
         if mtime.tzinfo is None:
             mtime = mtime.replace(tzinfo=timezone.utc)
         return mtime.astimezone().replace(tzinfo=None)
 
     def _msg_on_counter(self, user):
         if self._counter == MAX_MSG_COUNTER:
-            logger.info(
-                f"Another user ({user}) is doing a write operation to the database, "
-                "please wait or stop the code execution."
-            )
+            logger.info(f"Competing for the lock with the user {user}.")
 
         if self._counter <= MAX_MSG_COUNTER:
             self._counter += 1
 
     def _lock_unsafe(self):
-        if self._locked:
+        if self._has_lock:
             return None
 
+        self._has_lock = True
+        self._locked_by = self.user
+
         self.users = self.mapper["priorities"].decode().split("*")
 
         self.mapper[f"entering/{self.user}"] = b"1"
 
         numbers = [int(self.mapper[f"numbers/{user}"]) for user in self.users]
         number = 1 + max(numbers)
         self.mapper[f"numbers/{self.user}"] = str(number).encode()
 
         self.mapper[f"entering/{self.user}"] = b"0"
 
         for i, user in enumerate(self.users):
             if i == self.priority:
                 continue
 
-            while int(self.mapper[f"entering/{user}"]):
-                self._msg_on_counter(user)
-            while True:
-                c_number = int(self.mapper[f"numbers/{user}"])
-                if c_number == 0:
-                    break
-                if number < c_number:
-                    break
-                if number == c_number and self.priority < i:
-                    break
+            while self.mapper[f"entering/{user}"] == b"1":
                 self._msg_on_counter(user)
 
-        self._locked = True
+            c_number = int(self.mapper[f"numbers/{user}"])
+
+            if c_number == 0:
+                continue
+
+            if (number > c_number) or (number == c_number and self.priority > i):
+                self._has_lock = False
+                self._locked_by = user
+                self.mapper[f"numbers/{self.user}"] = b"0"
+                logger.info(f"The instance is already locked by the user {user}.")
+                return None
 
     def lock(self):
         try:
             self._lock_unsafe()
         except BaseException as e:
             self.unlock()
+            self._clear()
             raise e
 
     def unlock(self):
         self.mapper[f"numbers/{self.user}"] = b"0"
-
-        self._locked = False
+        self._has_lock = None
+        self._locked_by = None
         self._counter = 0
 
     def _clear(self):
-        self.unlock()
         self.mapper[f"entering/{self.user}"] = b"0"
 
+    @property
+    def has_lock(self):
+        if self._has_lock is None:
+            logger.info("The lock has not been initialized, trying to obtain the lock.")
+            self.lock()
+
+        return self._has_lock
+
 
 _locker: Optional[Locker] = None
 
 
 def get_locker(isettings: InstanceSettings) -> Locker:
     from .._settings import settings
 
+    global _locker
+
     user_id = settings.user.id
     storage_root = isettings.storage.root
+    instance_name = isettings.name
 
-    global _locker
-
-    if _locker is None:
-        _locker = Locker(user_id, storage_root)
-    elif user_id != _locker.user or storage_root is not _locker.root:
-        _locker = Locker(user_id, storage_root)
+    if (
+        _locker is None
+        or _locker.user != user_id
+        or _locker.root is not storage_root
+        or _locker.name != instance_name
+    ):
+        _locker = Locker(user_id, storage_root, instance_name)
 
     return _locker
```

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,18 +160,18 @@
         # as it's not relevant to the user
         """Is this a cloud instance with sqlite db."""
         return self.dialect == "sqlite" and self.storage.is_cloud
 
     @property
     def _cloud_sqlite_locker(self):
         # avoid circular import
-        from ._cloud_sqlite_locker import empty_locker
+        from ._cloud_sqlite_locker import empty_locker, get_locker
 
         if self._is_cloud_sqlite:
-            return empty_locker
+            return get_locker(self)
         else:
             return empty_locker
 
     @property
     def storage(self) -> StorageSettings:
         """Low-level access to storage location."""
         return self._storage
```

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lamindb_setup/dev/upath.py` & `lamindb_setup-0.47.5/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.5/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files 22% similar despite different names*

```diff
@@ -16,10 +16,10 @@
   latest-changes:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: docker://tiangolo/latest-changes:0.0.3
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
-          latest_changes_file: docs/changelog.md
+          latest_changes_file: CHANGELOG.md
           latest_changes_header: '--- \| --- \| --- \| --- \| ---\n'
           template_file: ./.github/workflows/latest-changes.jinja2
```

### Comparing `lamindb_setup-0.47.4/lnschema-core/.gitignore` & `lamindb_setup-0.47.5/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.47.5/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lnschema-core/LICENSE` & `lamindb_setup-0.47.5/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/lnschema-core/docs/changelog.md` & `lamindb_setup-0.47.5/lnschema-core/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🎨 Adapted featureset | [185](https://github.com/laminlabs/lnschema-core/pull/185) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-05 |
+♻️ Move logic to lamindb | [197](https://github.com/laminlabs/lnschema-core/pull/197) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 |
+✨ Delete storage in File.delete | [196](https://github.com/laminlabs/lnschema-core/pull/196) | [Koncopd](https://github.com/Koncopd) | 2023-06-12 |
+🚚 Rename Featureset to FeatureSet | [194](https://github.com/laminlabs/lnschema-core/pull/194) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.35.4
+♻️ Move save logic here | [193](https://github.com/laminlabs/lnschema-core/pull/193) | [falexwolf](https://github.com/falexwolf) | 2023-06-10 | 0.35.3
+🔥 Remove unnecessary files | [192](https://github.com/laminlabs/lnschema-core/pull/192) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 | 0.35.2
+👷 Simplify CI & remove docs | [191](https://github.com/laminlabs/lnschema-core/pull/191) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 |
+🚸 Check for required fields | [190](https://github.com/laminlabs/lnschema-core/pull/190) | [falexwolf](https://github.com/falexwolf) | 2023-06-09 | 0.35.1
+🚸 Add select method to `BaseORM` | [189](https://github.com/laminlabs/lnschema-core/pull/189) | [falexwolf](https://github.com/falexwolf) | 2023-06-08 | 0.35.0
+🎨 Auto fetch related names for Featureset | [188](https://github.com/laminlabs/lnschema-core/pull/188) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-08 |
+🏗️ Re-architect transform id | [186](https://github.com/laminlabs/lnschema-core/pull/186) | [falexwolf](https://github.com/falexwolf) | 2023-06-06 | 0.35a7
+🎨 Adapted featureset | [185](https://github.com/laminlabs/lnschema-core/pull/185) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-05 | 0.35a6
 ♻️ Polish schema | [184](https://github.com/laminlabs/lnschema-core/pull/184) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 |
 🚸 Improve QuerySet | [182](https://github.com/laminlabs/lnschema-core/pull/182) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 |
-:fire: Delete SQLAlchemy related content | [181](https://github.com/laminlabs/lnschema-core/pull/181) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
-:fire: Remove unncessary files | [180](https://github.com/laminlabs/lnschema-core/pull/180) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 | 0.35a4
+🔥 Delete SQLAlchemy related content | [181](https://github.com/laminlabs/lnschema-core/pull/181) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 ♻️ Absorb `DjangoORM.create()` in `DjangoORM.__init__()` | [178](https://github.com/laminlabs/lnschema-core/pull/178) | [falexwolf](https://github.com/falexwolf) | 2023-06-03 |
-➖ Remove nbproject from code | [179](https://github.com/laminlabs/lnschema-core/pull/179) | [Koncopd](https://github.com/Koncopd) | 2023-06-03 |
 🏗️ Enable Django backend | [177](https://github.com/laminlabs/lnschema-core/pull/177) | [falexwolf](https://github.com/falexwolf) | 2023-06-02 | 0.35a3
-🚚 Rename lndb to lamindb-setup | [176](https://github.com/laminlabs/lnschema-core/pull/176) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.35a2
+🚚 Rename `lndb` to `lamindb-setup` | [176](https://github.com/laminlabs/lnschema-core/pull/176) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.35a2
 🏗️ Add Django backend | [175](https://github.com/laminlabs/lnschema-core/pull/175) | [falexwolf](https://github.com/falexwolf) | 2023-05-31 | 0.35a1
 👷 Refactor CI | [174](https://github.com/laminlabs/lnschema-core/pull/174) | [falexwolf](https://github.com/falexwolf) | 2023-05-30 |
 🏗️ Remove SQL-level schema modules | [172](https://github.com/laminlabs/lnschema-core/pull/172) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.34.0
 🏗️ Introduce Django skeleton | [171](https://github.com/laminlabs/lnschema-core/pull/171) | [falexwolf](https://github.com/falexwolf) | 2023-05-24 |
 ♻️ Refactor types | [170](https://github.com/laminlabs/lnschema-core/pull/170) | [falexwolf](https://github.com/falexwolf) | 2023-05-23 |
 ♻️ Refactor `BaseORM` | [169](https://github.com/laminlabs/lnschema-core/pull/169) | [falexwolf](https://github.com/falexwolf) | 2023-05-17 | 0.33.8
 🚸 Add `lazy="joined"` to some cheap joins | [168](https://github.com/laminlabs/lnschema-core/pull/168) | [falexwolf](https://github.com/falexwolf) | 2023-05-16 | 0.33.7
```

### Comparing `lamindb_setup-0.47.4/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.47.5/lnschema-core/lnschema_core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Data objects & lineage (`yvzi`)."""
 _schema_id = "yvzi"
 _name = "core"
-__version__ = "0.35a4"
+__version__ = "0.35.4"
 
-import lamindb_setup as _lamindb_setup
+# can directly import from lamindb_setup going forward
 from lamindb_setup._check_instance_setup import (
     check_instance_setup as _check_instance_setup,
 )
 
 _INSTANCE_SETUP = _check_instance_setup()
 
 if _INSTANCE_SETUP:
     from . import ids, types
     from .models import (  # type: ignore
         BaseORM,
-        Featureset,
+        FeatureSet,
         File,
         Folder,
         Project,
         Run,
         RunInput,
         Storage,
         Transform,
         User,
     )
 
-    Features = Featureset  # backward compat
+    Features = FeatureSet  # backward compat
```

### Comparing `lamindb_setup-0.47.4/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.47.5/lnschema-core/lnschema_core/_lookup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from typing import Iterable, Optional
 
 from django.db import models
 
 
 def lookup(orm: models.Model, field: Optional[str] = None):
     """Lookup rows by field."""
+    model_field_names = [i.name for i in orm._meta.fields]
     if field is None:
         # by default use the name field
-        if "name" in orm.__fields__:
+        if "name" in model_field_names:
             field = "name"
         else:
-            non_ids = [i for i in orm.__fields__.keys() if "id" not in i]
+            non_ids = [i for i in model_field_names if "id" not in i]
             if len(non_ids) > 0:
                 # the first field isn't named with id
                 field = non_ids[0]
             else:
                 # the first field
-                field = next(iter(orm.__fields__.keys()))
+                field = model_field_names[0]
     values = set(orm.objects.values_list(field, flat=True))
     for value in [None, ""]:
         if value in values:
             values.remove(value)
     keys = to_lookup_keys(values, padding=orm.__name__)
     nt = namedtuple_from_dict(d=dict(zip(keys, values)), name=orm.__name__)
     return nt
```

### Comparing `lamindb_setup-0.47.4/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.47.5/lnschema-core/lnschema_core/ids.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,22 @@
 def base62(n_char: int) -> str:
     """Like nanoid without hyphen and underscore."""
     alphabet = string.digits + string.ascii_letters.swapcase()
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
     return id
 
 
+class Base62:
+    def __init__(self, n_char: int):
+        self.n_char = n_char
+
+    def __call__(self):
+        return base62(self.n_char)
+
+
 def base26(n_char: int):
     """ASCII lowercase."""
     alphabet = string.ascii_lowercase
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
     return id
```

### Comparing `lamindb_setup-0.47.4/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.47.5/lnschema-core/lnschema_core/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,180 +1,170 @@
 import builtins
-from pathlib import Path, PurePosixPath
-from typing import Dict, Iterable, List, NamedTuple, Optional, Union
+import traceback
+from pathlib import Path
+from typing import Dict, Iterable, NamedTuple, Optional, Union, overload  # noqa
 
-import pandas as pd
 from django.db import models
-from lamin_logger import logger
+from django.db.models import PROTECT, Manager
+from lamin_logger import colors, logger
 from upath import UPath
 
 from . import ids
 from ._lookup import lookup as _lookup
-from ._users import current_user_id
+from ._queryset import QuerySet
 from .types import DataLike, PathLike, TransformType
+from .users import current_user_id
 
 is_run_from_ipython = getattr(builtins, "__IPYTHON__", False)
 TRANSFORM_TYPE_DEFAULT = TransformType.notebook if is_run_from_ipython else TransformType.pipeline
 
 
-class NoResultFound(Exception):
-    pass
+def validate_required_fields(orm, kwargs):
+    required_fields = {k.name for k in orm._meta.fields if not k.null and k.default is None}
+    required_fields_not_passed = {k: None for k in required_fields if k not in kwargs}
+    kwargs.update(required_fields_not_passed)
+    missing_fields = [k for k, v in kwargs.items() if v is None and k in required_fields]
+    if missing_fields:
+        raise TypeError(f"{missing_fields} are required.")
 
 
-class MultipleResultsFound(Exception):
-    pass
-
-
-class LaminQuerySet(models.QuerySet):
-    """Extension of Django QuerySet.
-
-    This brings some of the SQLAlchemy/SQLModel/SQL-inspired calls.
+# todo, make a CreatedUpdated Mixin, but need to figure out docs
+class BaseORM(models.Model):
+    """Base data model.
 
-    As LaminDB was based on SQLAlchemy/SQLModel in the beginning, and might
-    support it again in the future, these calls will be supported longtime.
+    Is essentially equal to the Django Model base class, but adds the following
+    methods.
     """
 
-    def df(self):
-        columns = [field.name for field in self.model._meta.fields]
-        df = pd.DataFrame(self.values(), columns=columns)
-        if "id" in df.columns:
-            df = df.set_index("id")
-        return df
-
-    def list(self) -> List:
-        return list(self)
-
-    def first(self):
-        if len(self) == 0:
-            return None
-        return self[0]
-
-    def one(self):
-        if len(self) == 0:
-            raise NoResultFound
-        elif len(self) > 1:
-            raise MultipleResultsFound
-        else:
-            return self[0]
-
-    def one_or_none(self):
-        if len(self) == 0:
-            return None
-        elif len(self) == 1:
-            return self[0]
-        else:
-            raise MultipleResultsFound
+    def __repr__(self) -> str:
+        fields = [field.name for field in self._meta.fields if not isinstance(field, models.ForeignKey)]
+        fields += [f"{field.name}_id" for field in self._meta.fields if isinstance(field, models.ForeignKey)]
+        fields_str = ", ".join([f"{k}={getattr(self, k)}" for k in fields if hasattr(self, k)])
+        return f"{self.__class__.__name__}({fields_str})"
 
+    def __str__(self) -> str:
+        return self.__repr__()
 
-# todo, make a CreatedUpdated Mixin, but need to figure out docs
-class BaseORM(models.Model):
-    def __repr__(self) -> str:
-        fields = ", ".join([f"{k.name}={getattr(self, k.name)}" for k in self._meta.fields if hasattr(self, k.name)])
-        return f"{self.__class__.__name__}({fields})"
+    def __init__(self, *args, **kwargs):
+        if not args:  # object is loaded from DB
+            validate_required_fields(self, kwargs)
+        super().__init__(*args, **kwargs)
 
     @classmethod
     def lookup(cls, field: Optional[str] = None) -> NamedTuple:
+        """Lookup object for auto-completing field values."""
         return _lookup(cls, field)
 
-    def __str__(self) -> str:
-        return self.__repr__()
+    @classmethod
+    def select(cls, **expressions) -> Union[QuerySet, Manager]:
+        """Query the ORM."""
+        from lamindb._select import select
+
+        return select(cls, **expressions)
 
     class Meta:
         abstract = True
 
 
-class RunInput(BaseORM):
-    run = models.ForeignKey("Run", on_delete=models.CASCADE)
-    file = models.ForeignKey("File", on_delete=models.CASCADE)
-
-    class Meta:
-        managed = True
+# A note on required fields at the ORM level
+#
+# As Django does most of its validation on the Form-level, it doesn't offer functionality
+# for validating the integrity of an ORM object upon instantation (similar to pydantic)
+#
+# For required fields, we define them as commonly done on the SQL level together
+# with a validator in BaseORM (validate_required_fields)
+#
+# This goes against the Django convention, but goes with the SQLModel convention
+# (Optional fields can be null on the SQL level, non-optional fields cannot)
+#
+# Due to Django's convention where CharField has pre-configured (null=False, default=""), marking
+# a required field necessitates passing `default=None`. Without the validator it would trigger
+# an error at the SQL-level, with it, it triggers it at instantiation
 
 
 class User(BaseORM):
     """User accounts.
 
     All data in this table is synched from the cloud user account to ensure a
-    globally unique user identity.
+    universal user identity, valid across DB instances, email & handle changes.
     """
 
-    id = models.CharField(max_length=8, primary_key=True)
+    id = models.CharField(max_length=8, primary_key=True, default=None)
     """Universal id, valid across DB instances."""
-    handle = models.CharField(max_length=30, unique=True, db_index=True)
+    handle = models.CharField(max_length=30, unique=True, db_index=True, default=None)
     """Universal handle, valid across DB instances."""
-    email = models.CharField(max_length=255, unique=True, db_index=True)
+    email = models.CharField(max_length=255, unique=True, db_index=True, default=None)
     """Latest email address."""
     name = models.CharField(max_length=255, db_index=True)
     """Name."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
 
     class Meta:
         managed = True
 
 
 class Storage(BaseORM):
-    """Storage locations, typically cloud buckets.
+    """Storage locations, typically cloud storage buckets.
 
-    A file or run-associated file can be stored in any desired S3,
-    GCP bucket or local storage location.
+    A file can be stored in S3 and GCP buckets or local storage locations.
 
-    This table tracks these locations along with metadata.
+    This ORM tracks these locations along with metadata.
     """
 
     id = models.CharField(max_length=8, default=ids.storage, db_index=True, primary_key=True)
     """Universal id, valid across DB instances."""
-    root = models.CharField(max_length=255, db_index=True)
-    """Path to the root of the storage location: an s3 path, a local path, etc."""
-    type = models.CharField(max_length=63, db_index=True)
+    root = models.CharField(max_length=255, db_index=True, default=None)
+    """Path to the root of the storage location (an s3 path, a local path, etc.)."""
+    type = models.CharField(max_length=30, db_index=True)
     """Local vs. s3 vs. gcp etc."""
-    region = models.CharField(max_length=63, db_index=True, null=True)
+    region = models.CharField(max_length=63, db_index=True, null=True, default=None)
     """Cloud storage region, if applicable."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
-        models.DO_NOTHING,
+        PROTECT,
         default=current_user_id,
         related_name="created_storages",
     )
-    """Creator of record."""
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
 
 
 class Project(BaseORM):
     """Projects."""
 
     id = models.CharField(max_length=8, default=ids.project, primary_key=True)
     """Universal id, valid across DB instances."""
-    name = models.CharField(max_length=255, db_index=True, unique=True)
+    name = models.CharField(max_length=255, db_index=True, unique=True, default=None)
     """Project name or title."""
-    external_id = models.CharField(max_length=255, db_index=True)
+    external_id = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """External id (such as from a project management tool)."""
     folders = models.ManyToManyField("Folder", related_name="projects")
     """Project folders."""
     files = models.ManyToManyField("File", related_name="projects")
     """Project files."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
-        models.DO_NOTHING,
+        PROTECT,
         default=current_user_id,
         related_name="created_projects",
     )
-    """Creator of record."""
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
 
 
 class Transform(BaseORM):
     """Data transformations.
@@ -184,152 +174,159 @@
     A pipeline is versioned software that transforms data.
     This can be anything from typical workflow tools (Nextflow, Snakemake,
     Prefect, Apache Airflow, etc.) to simple (versioned) scripts.
 
     Creating a file is a transform, too.
     """
 
+    id = models.CharField(max_length=14, db_index=True, primary_key=True, default=None)
+    """Universal id, composed of stem_id and version suffix."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """A name for the transform, a pipeline name, or a file name of a notebook or script.
+    """Transform name or title, a pipeline name, notebook title, etc..
     """
-    title = models.TextField(db_index=True, null=True, default=None)
-    """An additional title, like a notebook title.
+    short_name = models.CharField(max_length=30, db_index=True, null=True, default=None)
+    """A short name.
     """
-    uid = models.CharField(max_length=12, default=ids.transform, db_index=True)
-    """Universal id, valid across DB instances."""
-    version = models.CharField(max_length=10, default=None, db_index=True, null=True)
-    """Version identifier, defaults to `"0"`.
+    stem_id = models.CharField(max_length=12, default=ids.transform, db_index=True)
+    """Stem of id, identifying transform up to version."""
+    version = models.CharField(max_length=10, default="0", db_index=True)
+    """Version, defaults to `"0"`.
 
-    Use this to label different versions of the same transform.
+    Use this to label different versions of the same pipeline, notebook, etc.
 
     Consider using `semantic versioning <https://semver.org>`__
     with `Python versioning <https://peps.python.org/pep-0440/>`__.
     """
     type = models.CharField(
         max_length=20,
         choices=TransformType.choices(),
         db_index=True,
         default=TRANSFORM_TYPE_DEFAULT,
     )
     """Transform type.
 
-    Defaults to `notebook` if run from IPython, from a script to `pipeline`.
+    Defaults to `notebook` if run from ipython and to `pipeline` if run from python.
 
     If run from the app, it defaults to `app`.
     """
     reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Reference for the transform, e.g., a URL.
     """
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
-        models.DO_NOTHING,
+        PROTECT,
         default=current_user_id,
         related_name="created_transforms",
     )
-    """Creator of record."""
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
-        unique_together = (("uid", "version"),)
+        unique_together = (("stem_id", "version"),)
+
+    def __init__(self, *args, **kwargs):
+        if len(args) > 0:  # initialize with all fields from db as args
+            super().__init__(*args, **kwargs)
+            return None
+        else:  # user-facing calling signature
+            # set default ids
+            if "id" not in kwargs and "stem_id" not in kwargs:
+                kwargs["id"] = ids.base62(n_char=14)
+                kwargs["stem_id"] = kwargs["id"][:12]
+            elif "stem_id" in kwargs:
+                assert isinstance(kwargs["stem_id"], str) and len(kwargs["stem_id"]) == 12
+                kwargs["id"] = kwargs["stem_id"] + ids.base62(n_char=2)
+            elif "id" in kwargs:
+                assert isinstance(kwargs["id"], str) and len(kwargs["id"]) == 14
+                kwargs["stem_id"] = kwargs["id"][:12]
+            super().__init__(**kwargs)
 
 
 class Run(BaseORM):
-    """Runs of data transforms.
+    """Runs of data transformations.
 
-    A `run` is any transform of a `file`.
+    Typically, a run has inputs and outputs:
 
-    Args:
-        id: Optional[str] = None
-        name: Optional[str] = None
-        load_latest: bool = False - Load latest run for given notebook or pipeline.
-        transform: Optional[Transform] = None
-        inputs: List[File] = None
-        outputs: List[File] = None
-
-    It typically has inputs and outputs:
-
-    - References to outputs are stored in the `file` table in the
-      `run_id` column as a foreign key the `run`
-      table. This is possible as every given `file` has a unique data run:
-      the `run` that produced the `file`. However, note that a given
-      `run` may output several `files`.
-    - References to inputs are stored in the `run_in` table, a
-      many-to-many link table between the `file` and `run` tables. Any
-      `file` might serve as an input for many `runs`. Similarly, any
-      `run` might have many `files` as inputs.
+    - References to outputs are stored in the `File` ORM in the `run` field.
+      This is possible as every given file has a unique run that created it. Any
+      given `Run` can output multiple `files`: `run.outputs`.
+    - References to inputs are stored in the `RunInput` ORM, a many-to-many link
+      ORM between `File` and `Run`. Any `file` might serve as an input for
+      multiple `runs`: `file.input_of`. Similarly, any `run` might have many
+      `files` as inputs: `run.inputs`.
     """
 
     id = models.CharField(max_length=20, default=ids.run, primary_key=True)
     """Universal id, valid across DB instances."""
-    name = models.CharField(max_length=255, db_index=True)
+    name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Name or title of run."""
-    external_id = models.CharField(max_length=255, db_index=True)
+    external_id = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """External id (such as from a workflow tool)."""
-    transform = models.ForeignKey(Transform, models.DO_NOTHING, related_name="runs")
+    transform = models.ForeignKey(Transform, PROTECT, related_name="runs")
     """The transform :class:`~lamindb.Transform` that is being run."""
-    inputs = models.ManyToManyField("File", through=RunInput, related_name="input_of")
+    inputs = models.ManyToManyField("File", through="RunInput", related_name="input_of")
     """The input files for the run."""
     # outputs on File
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
-    updated_at = models.DateTimeField(auto_now=True, db_index=True)
-    """Time of last update to record."""
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_runs")
-    """Creator of record."""
+    run_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of run execution."""
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_runs")
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
 
 
-class Featureset(BaseORM):
+class FeatureSet(BaseORM):
     """Feature sets.
 
     A feature set is represented by the hash of the set of primary keys and the feature type.
 
-    The current supported feature types are lnschema_bionty.Gene,
-    lnschema_bionty.Protein & lnschema_bionty.CellMarker.
+    The current supported feature types are `lnschema_bionty.Gene`,
+    `lnschema_bionty.Protein`, and `lnschema_bionty.CellMarker`.
 
     Guides:
 
     - :doc:`/biology/scrna`
     - :doc:`/biology/flow`
 
     Examples:
 
     >>> import lnschema_bionty as bt
     >>> reference = bt.Gene(species="mouse")
-    >>> features = ln.Features(adata, reference=reference)
-    >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq", features=features)
+    >>> features = ln.Features.from_iterable(adata.var["ensemble_id"], Gene.ensembl_gene_id)
+    >>> features.save()
+    >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq")
+    >>> file.save()
+    >>> file.featuresets.add(featureset)
 
-    Args:
-        data: [Path, str, pd.DataFrame, ad.AnnData] - DataFrame or AnnData to parse.
-        reference: Any = None - Reference for mapping features.
     """
 
-    id = models.CharField(max_length=64, primary_key=True)
-    """A universal id, valid across DB instances: a hash of the linked set of features."""
+    id = models.CharField(max_length=64, primary_key=True, default=None)
+    """A universal id, valid across DB instances, a hash of the linked set of features."""
     type = models.CharField(max_length=64)
     """A feature entity type."""
     files = models.ManyToManyField("File", related_name="featuresets")
     """Files linked to the featureset."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(
         User,
-        models.DO_NOTHING,
+        PROTECT,
         default=current_user_id,
         related_name="created_featuresets",
     )
-    """Creator of record."""
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
 
     @classmethod
     def from_iterable(
         cls,
@@ -344,60 +341,62 @@
             iterable=iterable,
             field=field,
             species=species,
         )
         return features
 
     def __init__(self, *args, **kwargs):  # type: ignore
+        related_names = [i.related_name for i in self.__class__._meta.related_objects]
+
         relationships: Dict = {}
-        if "genes" in kwargs:
-            relationships["genes"] = kwargs.pop("genes")
-        if "proteins" in kwargs:
-            relationships["proteins"] = kwargs.pop("proteins")
-        if "cell_markers" in kwargs:
-            relationships["cell_markers"] = kwargs.pop("cell_markers")
+        for related_name in related_names:
+            if related_name in kwargs:
+                relationships[related_name] = kwargs.pop(related_name)
         self._relationships = relationships
 
         super().__init__(*args, **kwargs)
 
     def save(self, *args, **kwargs):
         super().save(*args, **kwargs)
         for key, records in self._relationships.items():
             [r.save() for r in records]
             getattr(self, key).set(records)
 
 
 class Folder(BaseORM):
     id = models.CharField(max_length=20, default=ids.folder, primary_key=True)
     """A universal random id, valid across DB instances."""
-    name = models.CharField(max_length=255, db_index=True)
-    """Name or title of the folder."""
-    key = models.CharField(max_length=255, null=True, default=None, db_index=True)
-    """Storage key of the folder."""
-    storage = models.ForeignKey(Storage, models.DO_NOTHING, related_name="folders", null=True)
-    """Storage location of the folder."""
+    name = models.CharField(max_length=255, db_index=True, default=None)
+    """Name or title of folder."""
+    # below is one of the few cases with null=True, default=None
+    key = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    """Storage key of folder."""
+    storage = models.ForeignKey(Storage, PROTECT, related_name="folders", null=True)
+    """:class:`~lamindb.Storage` location of folder, see `.path()` for full path."""
     files = models.ManyToManyField("File", related_name="folders")
-    """Files in folder."""
+    """:class:`~lamindb.File` records in folder."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_folders")
-    """Creator of record."""
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_folders")
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     @property
     def __name__(cls) -> str:
         return "Folder"
 
     def path(self) -> Union[Path, UPath]:
         """Path on storage."""
+        from lamindb._file_access import filepath_from_file_or_folder
+
         return filepath_from_file_or_folder(self)
 
     def tree(
         self,
         level: int = -1,
         limit_to_directories: bool = False,
         length_limit: int = 1000,
@@ -423,15 +422,15 @@
                 path: Optional[Union[Path, UPath, str]] = args[0]
             else:
                 path = None
             name: Optional[str] = kwargs.pop("name") if "name" in kwargs else None
             key: Optional[str] = kwargs.pop("key") if "key" in kwargs else None
             files: Optional[str] = kwargs.pop("files") if "files" in kwargs else None
             if len(kwargs) != 0:
-                raise ValueError(f"This kwargs are not permitted: {kwargs}")
+                raise ValueError(f"These kwargs are not permitted: {kwargs}")
 
         from lamindb._folder import get_folder_kwargs_from_data
 
         if path is not None:
             kwargs, privates = get_folder_kwargs_from_data(
                 path=path,
                 name=name,
@@ -443,14 +442,24 @@
         kwargs["id"] = ids.folder()
         super().__init__(**kwargs)
         if path is not None:
             self._local_filepath = privates["local_filepath"]
             self._cloud_filepath = privates["cloud_filepath"]
             self._files = files
 
+    def save(self, *args, **kwargs) -> None:
+        """Save the folder."""
+        # only has attr _files if freshly initialized
+        if hasattr(self, "_files"):
+            for file in self._files:
+                file.save()
+        super().save(*args, **kwargs)
+        if hasattr(self, "_files"):
+            self.files.set(self._files)
+
 
 class File(BaseORM):
     id = models.CharField(max_length=20, primary_key=True)
     """A universal random id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """A universal random id, valid across DB instances."""
     suffix = models.CharField(max_length=30, db_index=True, null=True, default=None)
@@ -462,205 +471,117 @@
     size = models.BigIntegerField(null=True, db_index=True)
     """Size in bytes.
 
     Examples: 1KB is 1e3 bytes, 1MB is 1e6, 1GB is 1e9, 1TB is 1e12 etc.
     """
     hash = models.CharField(max_length=86, db_index=True, null=True, default=None)
     """Hash of file content. 86 base64 chars allow to store 64 bytes, 512 bits."""
+    # below is one of the few cases with null=True, default=None
     key = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Storage key, the relative path within the storage location."""
-    run = models.ForeignKey(Run, models.DO_NOTHING, related_name="outputs", null=True)
+    run = models.ForeignKey(Run, PROTECT, related_name="outputs", null=True)
     """:class:`~lamindb.Run` that created the `file`."""
-    transform = models.ForeignKey(Transform, models.DO_NOTHING, related_name="files", null=True)
+    transform = models.ForeignKey(Transform, PROTECT, related_name="files", null=True)
     """:class:`~lamindb.Transform` whose run created the `file`."""
-    storage: "Storage" = models.ForeignKey(Storage, models.DO_NOTHING, related_name="files")
+    storage: "Storage" = models.ForeignKey(Storage, PROTECT, related_name="files")
     """:class:`~lamindb.Storage` location of `file`, see `.path()` for full path."""
     # folders from Folders.files
     # features from Features.files
     # input_of from Run.inputs
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_files")
-    """Creator of record."""
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_files")
+    """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     def path(self) -> Union[Path, UPath]:
         """Path on storage."""
+        from lamindb._file_access import filepath_from_file_or_folder
+
         return filepath_from_file_or_folder(self)
 
     # likely needs an arg `key`
     def replace(
         self,
         data: Union[PathLike, DataLike],
         run: Optional[Run] = None,
         format: Optional[str] = None,
     ) -> None:
         """Replace file content."""
-        from lamindb._file import get_file_kwargs_from_data
+        from lamindb._file import replace_file
 
-        if isinstance(data, (Path, str)):
-            name_to_pass = None
-        else:
-            name_to_pass = self.name
+        replace_file(self, data, run, format)
 
-        kwargs, privates = get_file_kwargs_from_data(
-            data=data,
-            name=name_to_pass,
-            run=run,
-            format=format,
-        )
-
-        if kwargs["name"] != self.name:
-            logger.warning(f"Your new filename '{kwargs['name']}' does not match the previous filename '{self.name}': to update the name, set file.name = '{kwargs['name']}'")
-
-        if self.key is not None:
-            key_path = PurePosixPath(self.key)
-            if isinstance(data, (Path, str)):
-                new_name = kwargs["name"]  # use the name from the data filepath
-            else:
-                # do not change the key stem to file.name
-                new_name = key_path.stem  # use the stem of the key for in-memory data
-            if PurePosixPath(new_name).suffixes == []:
-                new_name = f"{new_name}{kwargs['suffix']}"
-            if key_path.name != new_name:
-                self._clear_storagekey = self.key
-                self.key = str(key_path.with_name(new_name))
-                logger.warning(f"Replacing the file will also replace the key from '{key_path}' to '{self.key}', and delete '{key_path}' upon `ln.add`")
-        else:
-            self.key = kwargs["key"]
-            old_storage = f"{self.id}{self.suffix}"
-            new_storage = self.key if self.key is not None else f"{self.id}{kwargs['suffix']}"
-            if old_storage != new_storage:
-                self._clear_storagekey = old_storage
-
-        self.suffix = kwargs["suffix"]
-        self.size = kwargs["size"]
-        self.hash = kwargs["hash"]
-        self.run = kwargs["run"]
-        self._local_filepath = privates["local_filepath"]
-        self._cloud_filepath = privates["cloud_filepath"]
-        self._memory_rep = privates["memory_rep"]
-        self._to_store = not privates["check_path_in_storage"]  # no need to upload if new file is already in storage
+    @overload
+    def __init__(
+        data: Union[PathLike, DataLike],
+        key: Optional[str] = None,
+        name: Optional[str] = None,
+        run: Optional[Run] = None,
+    ):
+        ...
 
-    @property
-    def __name__(cls) -> str:
-        return "File"
+    @overload
+    def __init__(
+        *args,
+        **kwargs,
+    ):
+        ...
 
     def __init__(  # type: ignore
         self,
         *args,
         **kwargs,
     ):
-        if len(args) > 1 and isinstance(args[0], str) and len(args[0]) == 20:  # initialize with all fields from db as args
-            super().__init__(*args, **kwargs)
-            return None
-        else:  # user facing calling signature
-            if len(args) > 1:
-                raise ValueError("Only one non-keyword arg allowed")
-            if len(args) == 0:
-                data: Union[PathLike, DataLike] = kwargs["data"]
-            else:
-                data: Union[PathLike, DataLike] = args[0]
-            key: Optional[str] = kwargs["key"] if "key" in kwargs else None
-            name: Optional[str] = kwargs["name"] if "name" in kwargs else None
-            run: Optional[Run] = kwargs["run"] if "run" in kwargs else None
-            format = kwargs["format"] if "format" in kwargs else None
-
-        def log_hint(*, check_path_in_storage: bool, key: str, id: str, suffix: str) -> None:
-            hint = ""
-            if check_path_in_storage:
-                hint += "file in storage ✓"
-            else:
-                hint += "file will be copied to storage upon `ln.add()`"
-            if key is None:
-                hint += f" using storage key = {id}{suffix}"
-            else:
-                hint += f" using storage key = {key}"
-            logger.hint(hint)
-
-        from lamindb._file import get_file_kwargs_from_data
-
-        kwargs, privates = get_file_kwargs_from_data(
-            data=data,
-            name=name,
-            key=key,
-            run=run,
-            format=format,
-        )
-        kwargs["id"] = ids.file()
-        log_hint(
-            check_path_in_storage=privates["check_path_in_storage"],
-            key=kwargs["key"],
-            id=kwargs["id"],
-            suffix=kwargs["suffix"],
-        )
+        from lamindb._file import init_file
 
-        # transform cannot be directly passed, just via run
-        # it's directly stored in the file table to avoid another join
-        # mediate by the run table
-        if kwargs["run"] is not None:
-            if kwargs["run"].transform_id is not None:
-                kwargs["transform_id"] = kwargs["run"].transform_id
-            else:
-                # accessing the relationship should always be possible if
-                # the above if clause was false as then, we should have a fresh
-                # Transform object that is not queried from the DB
-                assert kwargs["run"].transform is not None
-                kwargs["transform"] = kwargs["run"].transform
+        init_file(self, *args, **kwargs)
 
-        super().__init__(**kwargs)
-        if data is not None:
-            self._local_filepath = privates["local_filepath"]
-            self._cloud_filepath = privates["cloud_filepath"]
-            self._memory_rep = privates["memory_rep"]
-            self._to_store = not privates["check_path_in_storage"]
+    def save(self, *args, **kwargs) -> None:
+        """Save the file to database & storage."""
+        self._save_skip_storage(*args, **kwargs)
+        from lamindb._save import check_and_attempt_clearing, check_and_attempt_upload
+
+        exception = check_and_attempt_upload(self)
+        if exception is not None:
+            self._delete_skip_storage()
+            raise RuntimeError(exception)
+        exception = check_and_attempt_clearing(self)
+        if exception is not None:
+            raise RuntimeError(exception)
 
-    def save(self, *args, **kwargs):
+    def _save_skip_storage(self, *args, **kwargs) -> None:
         if self.transform is not None:
             self.transform.save()
         if self.run is not None:
             self.run.save()
         super().save(*args, **kwargs)
 
+    def delete(self, *args, **kwargs) -> None:
+        from lamindb._file_access import storage_key_from_file
+        from lamindb.dev.storage import delete_storage
+
+        storage_key = storage_key_from_file(self)
+
+        self._delete_skip_storage(*args, **kwargs)
+
+        try:
+            delete_storage(storage_key)
+            logger.success(f"Deleted {colors.yellow(f'object {storage_key}')} from storage.")
+        except Exception:
+            traceback.print_exc()
 
-# add type annotations back asap when re-organizing the module
-def storage_key_from_file(file: File):
-    if file.key is None:
-        return f"{file.id}{file.suffix}"
-    else:
-        return file.key
-
-
-# add type annotations back asap when re-organizing the module
-def filepath_from_file_or_folder(file_or_folder: Union[File, Folder]):
-    from lamindb_setup import settings
-    from lamindb_setup.dev import StorageSettings
-
-    # using __name__ for type check to avoid need of
-    # dynamically importing the type
-    if file_or_folder.__name__ == "File":
-        storage_key = storage_key_from_file(file_or_folder)
-    else:
-        storage_key = file_or_folder.key
-        if storage_key is None:
-            raise ValueError("Only real folders have a path!")
-    if file_or_folder.storage_id == settings.storage.id:
-        path = settings.storage.key_to_filepath(storage_key)
-    else:
-        logger.warning(
-            "file.path() is slow for files outside the currently configured storage"
-            " location\nconsider joining for the set of files you're interested in:"
-            " ln.select(ln.File, ln.Storage)the path is storage.root / file.key if"
-            " file.key is not None\notherwise storage.root / (file.id + file.suffix)"
-        )
-        import lamindb as ln
+    def _delete_skip_storage(self, *args, **kwargs) -> None:
+        super().delete(*args, **kwargs)
+
+
+class RunInput(BaseORM):
+    run = models.ForeignKey("Run", on_delete=models.CASCADE)
+    file = models.ForeignKey("File", on_delete=models.CASCADE)
 
-        storage = ln.select(ln.Storage, id=file_or_folder.storage_id).one()
-        # find a better way than passing None to instance_settings in the future!
-        storage_settings = StorageSettings(storage.root, instance_settings=None)
-        path = storage_settings.key_to_filepath(storage_key)
-    return path
+    class Meta:
+        managed = True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lamindb_setup-0.47.4/lnschema-core/pyproject.toml` & `lamindb_setup-0.47.5/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/noxfile.py` & `lamindb_setup-0.47.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/pyproject.toml` & `lamindb_setup-0.47.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/tests/test_bionty.py` & `lamindb_setup-0.47.5/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/tests/test_init_instance.py` & `lamindb_setup-0.47.5/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/tests/test_load_instance.py` & `lamindb_setup-0.47.5/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.4/PKG-INFO` & `lamindb_setup-0.47.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.47.4
+Version: 0.47.5
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.10
 Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
```

